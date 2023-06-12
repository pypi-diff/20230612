# Comparing `tmp/csv_scavenger-1.0.4.tar.gz` & `tmp/csv_scavenger-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_scavenger-1.0.4.tar", max compression
+gzip compressed data, was "csv_scavenger-1.0.5.tar", max compression
```

## Comparing `csv_scavenger-1.0.4.tar` & `csv_scavenger-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4026 2023-06-01 15:42:11.946420 csv_scavenger-1.0.4/csv-scavenger/scavenger.py
--rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.4/LICENSE
--rw-r--r--   0        0        0      542 2023-06-01 15:52:14.476265 csv_scavenger-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      663 2023-05-31 18:15:01.226065 csv_scavenger-1.0.4/README.md
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 csv_scavenger-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4134 2023-06-12 18:51:23.045257 csv_scavenger-1.0.5/csv-scavenger/scavenger.py
+-rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.5/LICENSE
+-rw-r--r--   0        0        0      542 2023-06-12 18:54:46.838597 csv_scavenger-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      663 2023-05-31 18:15:01.226065 csv_scavenger-1.0.5/README.md
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 csv_scavenger-1.0.5/PKG-INFO
```

### Comparing `csv_scavenger-1.0.4/csv-scavenger/scavenger.py` & `csv_scavenger-1.0.5/csv-scavenger/scavenger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import pandas as pd
 from collections import Counter
 from tssplit import tssplit  # type: ignore
-from typing import Optional
 
 
 def _determine_format(lines: list[str]) -> tuple[str, int]:
     formats: list[tuple[str, int]] = []
-    step = len(lines) // 100 if len(lines) > 100 else 1
-    for i, line in enumerate(lines):
-        if i % step == 0:
-            for delim in [";", ",", " ", "\t", "\n", "\r", "\r\n"]:
-                num_of_columns = len(
-                    tssplit(line.strip(), quote='"', delimiter=delim, escape="")  # type: ignore
-                )
-                if num_of_columns > 1:
-                    formats.append((delim, num_of_columns))
+    delimiters = [";", ",", " ", "\t", "\n", "\r", "\r\n"]
+    step = max(1, len(lines) // 100)
+    for i in range(0, len(lines), step):
+        line = lines[i]
+        for delim in delimiters:
+            num_of_columns = len(
+                tssplit(line.strip(), quote='"', delimiter=delim, escape="")  # type: ignore
+            )
+            if num_of_columns > 1:
+                formats.append((delim, num_of_columns))
     counter = Counter(formats)
     try:
         csv_format: tuple[str, int] = counter.most_common(1)[0][0]
     except IndexError:
         raise IndexError(
             "No delimiter found. Currently supported delimiters are the comma, ;, \\t, \\n, \\r, \\r\\n, and whitespace."
         )
     return csv_format
 
 
 def _determine_header_start_last(
     csv_format: tuple[str, int], lines: list[str]
-) -> tuple[Optional[int], Optional[int], Optional[int]]:
+) -> tuple[int | str, int | str, int | str]:
     header_line = "undefined"
     last_line = "undefined"
     first_line = "undefined"
 
     for i, line in enumerate(lines):
         num_of_columns = len(
             tssplit(line.strip(), quote='"', delimiter=csv_format[0], escape="")  # type: ignore
@@ -71,21 +71,25 @@
         raise FileNotFoundError(f"File {file_path} not found.")
 
     csv_format = _determine_format(lines)
 
     header_row, data_start_row, data_end_row = _determine_header_start_last(
         csv_format, lines
     )
-    if (
-        header_row == "undefined"
-        or data_start_row == "undefined"
-        or data_end_row == "undefined"
-    ):
+    if header_row == "undefined":
         raise ValueError("Could not determine header and data rows.")
 
+    try:
+        assert isinstance(data_start_row, int)
+        assert isinstance(data_end_row, int)
+    except AssertionError:
+        raise AssertionError(
+            "Could not determine header and data rows. Please check your CSV file."
+        )
+
     if header_row == "none":
         data = pd.read_csv(  # type: ignore
             file_path,
             sep=csv_format[0],
             skiprows=data_start_row - 1,
             nrows=data_end_row - data_start_row,
             engine="python",
```

### Comparing `csv_scavenger-1.0.4/LICENSE` & `csv_scavenger-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.4/pyproject.toml` & `csv_scavenger-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "csv-scavenger"
-version = "1.0.4"
+version = "1.0.5"
 description = "CSV reader and parser with automatic detection of delimiter and start/end of data."
 authors = ["Gustave Coulombe <magikgus@gmail.com>"]
 readme = "README.md"
 packages = [{include = "scavenger.py", from = "csv-scavenger"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `csv_scavenger-1.0.4/README.md` & `csv_scavenger-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.4/PKG-INFO` & `csv_scavenger-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-scavenger
-Version: 1.0.4
+Version: 1.0.5
 Summary: CSV reader and parser with automatic detection of delimiter and start/end of data.
 Author: Gustave Coulombe
 Author-email: magikgus@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

