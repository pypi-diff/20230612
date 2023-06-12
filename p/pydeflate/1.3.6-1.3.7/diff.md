# Comparing `tmp/pydeflate-1.3.6.tar.gz` & `tmp/pydeflate-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeflate-1.3.6.tar", max compression
+gzip compressed data, was "pydeflate-1.3.7.tar", max compression
```

## Comparing `pydeflate-1.3.6.tar` & `pydeflate-1.3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1070 2023-05-23 15:39:27.024478 pydeflate-1.3.6/LICENSE
--rw-r--r--   0        0        0     8999 2023-05-23 15:39:27.024478 pydeflate-1.3.6/README.md
--rw-r--r--   0        0        0       25 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/.pydeflate_data/README.md
--rw-r--r--   0        0        0      775 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/deflate/__init__.py
--rw-r--r--   0        0        0    11850 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/deflate/deflate.py
--rw-r--r--   0        0        0     2684 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/deflate/deflator.py
--rw-r--r--   0        0        0        0 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/__init__.py
--rw-r--r--   0        0        0     2285 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/deflate_data.py
--rw-r--r--   0        0        0    12091 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/exchange_data.py
--rw-r--r--   0        0        0     2693 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/imf_data.py
--rw-r--r--   0        0        0     6177 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/oecd_data.py
--rw-r--r--   0        0        0     2103 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/get_data/wb_data.py
--rw-r--r--   0        0        0      894 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/pydeflate_config.py
--rw-r--r--   0        0        0      133 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/settings/emu.json
--rw-r--r--   0        0        0      911 2023-05-23 15:39:27.024478 pydeflate-1.3.6/pydeflate/settings/oecd_codes.json
--rw-r--r--   0        0        0       47 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pydeflate/tools/__init__.py
--rw-r--r--   0        0        0     5465 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pydeflate/tools/exchange.py
--rw-r--r--   0        0        0     2110 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pydeflate/tools/update_data.py
--rw-r--r--   0        0        0     1573 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pydeflate/utils.py
--rw-r--r--   0        0        0     1059 2023-05-23 15:39:27.028478 pydeflate-1.3.6/pyproject.toml
--rw-r--r--   0        0        0    10048 1970-01-01 00:00:00.000000 pydeflate-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-12 15:04:13.184837 pydeflate-1.3.7/LICENSE
+-rw-r--r--   0        0        0     8999 2023-06-12 15:04:13.184837 pydeflate-1.3.7/README.md
+-rw-r--r--   0        0        0       25 2023-06-12 15:04:13.184837 pydeflate-1.3.7/pydeflate/.pydeflate_data/README.md
+-rw-r--r--   0        0        0      817 2023-06-12 15:04:13.184837 pydeflate-1.3.7/pydeflate/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 15:04:13.184837 pydeflate-1.3.7/pydeflate/deflate/__init__.py
+-rw-r--r--   0        0        0    11850 2023-06-12 15:04:13.184837 pydeflate-1.3.7/pydeflate/deflate/deflate.py
+-rw-r--r--   0        0        0     2684 2023-06-12 15:04:13.184837 pydeflate-1.3.7/pydeflate/deflate/deflator.py
+-rw-r--r--   0        0        0        0 2023-06-12 15:04:13.184837 pydeflate-1.3.7/pydeflate/get_data/__init__.py
+-rw-r--r--   0        0        0     2285 2023-06-12 15:04:13.184837 pydeflate-1.3.7/pydeflate/get_data/deflate_data.py
+-rw-r--r--   0        0        0    12091 2023-06-12 15:04:13.184837 pydeflate-1.3.7/pydeflate/get_data/exchange_data.py
+-rw-r--r--   0        0        0     2693 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/get_data/imf_data.py
+-rw-r--r--   0        0        0     7535 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/get_data/oecd_data.py
+-rw-r--r--   0        0        0     2103 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/get_data/wb_data.py
+-rw-r--r--   0        0        0      894 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/pydeflate_config.py
+-rw-r--r--   0        0        0      133 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/settings/emu.json
+-rw-r--r--   0        0        0      911 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/settings/oecd_codes.json
+-rw-r--r--   0        0        0       47 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/tools/__init__.py
+-rw-r--r--   0        0        0     5465 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/tools/exchange.py
+-rw-r--r--   0        0        0     2110 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/tools/update_data.py
+-rw-r--r--   0        0        0     1573 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pydeflate/utils.py
+-rw-r--r--   0        0        0     1059 2023-06-12 15:04:13.188837 pydeflate-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0    10048 1970-01-01 00:00:00.000000 pydeflate-1.3.7/PKG-INFO
```

### Comparing `pydeflate-1.3.6/LICENSE` & `pydeflate-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/README.md` & `pydeflate-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/__init__.py` & `pydeflate-1.3.7/pydeflate/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = """Jorge Rivera"""
-__version__ = "1.3.6"
+__version__ = "1.3.7"
 
 from pydeflate.deflate.deflate import deflate
 from pydeflate.tools.exchange import exchange
 from pydeflate.tools.update_data import update_all_data, warn_updates
 from pydeflate.get_data.oecd_data import update_dac1
 from pydeflate import get_data
 
@@ -20,8 +20,15 @@
     set_bblocks_data_path(PYDEFLATE_PATHS.data)
 
 
 # check that data is fresh enough
 warn_updates()
 
 
-__all__ = ["deflate", "exchange", "update_all_data", "set_pydeflate_path", "get_data"]
+__all__ = [
+    "deflate",
+    "exchange",
+    "update_all_data",
+    "set_pydeflate_path",
+    "get_data",
+    "update_dac1",
+]
```

### Comparing `pydeflate-1.3.6/pydeflate/deflate/deflate.py` & `pydeflate-1.3.7/pydeflate/deflate/deflate.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/deflate/deflator.py` & `pydeflate-1.3.7/pydeflate/deflate/deflator.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/get_data/deflate_data.py` & `pydeflate-1.3.7/pydeflate/get_data/deflate_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/get_data/exchange_data.py` & `pydeflate-1.3.7/pydeflate/get_data/exchange_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/get_data/imf_data.py` & `pydeflate-1.3.7/pydeflate/get_data/imf_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/get_data/oecd_data.py` & `pydeflate-1.3.7/pydeflate/get_data/oecd_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import csv
 import io
 import warnings
 import zipfile as zf
 from dataclasses import dataclass
 
 import pandas as pd
 import requests
@@ -15,35 +16,79 @@
 
 warnings.simplefilter("ignore", Warning, lineno=1013)
 
 _BASE_URL: str = "https://stats.oecd.org/DownloadFiles.aspx?DatasetCode="
 _TABLE1_URL: str = f"{_BASE_URL}TABLE1"
 
 
+def _raw2df(csv_file: csv, sep: str, encoding: str) -> pd.DataFrame:
+    """Convert a raw csv to a DataFrame. Check the result if requested"""
+
+    try:
+        _ = pd.read_csv(
+            csv_file, sep=sep, dtype="str", encoding=encoding, low_memory=False
+        )
+    except UnicodeError:
+        raise pd.errors.ParserError
+
+    unnamed_cols = [c for c in _.columns if "unnamed" in c]
+
+    if len(unnamed_cols) > 3:
+        raise pd.errors.ParserError
+
+    if len(_.columns) < 3:
+        raise pd.errors.ParserError
+
+    return _
+
+
+def _extract_df(request_content, file_name: str, separator: str) -> pd.DataFrame:
+    import copy
+
+    for encoding in ["utf_16", "ISO-8859-1"]:
+        try:
+            rc = copy.deepcopy(request_content)
+
+            # Read the zipfile
+            _ = io.BytesIO(rc)
+            raw_csv = zf.ZipFile(_).open(file_name)
+
+            # convert to a dataframe
+            return _raw2df(csv_file=raw_csv, sep=separator, encoding=encoding)
+        except pd.errors.ParserError:
+            logger.debug(f"{encoding} not valid")
+
+    raise pd.errors.ParserError
+
+
 def _read_zip_content(request_content: bytes, file_name: str) -> pd.DataFrame:
     """Read the contents of a zip file
 
     Args:
         request_content: the content of the request
         file_name: the name of the file to read.
 
     Returns:
         A pandas dataframe with the contents of the file
 
     """
-    # Read the zipfile
-    _ = io.BytesIO(request_content)
-    zip_file = zf.ZipFile(_).open(file_name)
-
-    # Try two alternative separators to read the CSV file
     try:
-        return pd.read_csv(zip_file, sep=",", encoding="ISO-8859-1", low_memory=False)
+        return _extract_df(
+            request_content=request_content, separator=",", file_name=file_name
+        )
 
     except UnicodeDecodeError:
-        return pd.read_csv(zip_file, sep="|", encoding="ISO-8859-1", low_memory=False)
+        return _extract_df(
+            request_content=request_content, separator="|", file_name=file_name
+        )
+
+    except pd.errors.ParserError:
+        return _extract_df(
+            request_content=request_content, separator="|", file_name=file_name
+        )
 
 
 def _download_bulk_file(url: str) -> bytes:
     """Get zipfile bytes from the webpage
 
     Args:
         url: the url to download the file from
@@ -90,17 +135,25 @@
         "(aid == 11010 & flow == 1160 & year >=2018)"
     )
 
     # Clean the data
     data = (
         df.filter(cols, axis=1)
         .rename(columns=cols)
-        .astype({"year": "Int32"})
+        .astype(
+            {
+                "year": "Int32",
+                "aid": "Int32",
+                "flow": "Int32",
+                "value": float,
+                "donor_code": "Int32",
+            }
+        )
         .query(query)
-        .filter(["donor_code", "type", "year", "value"])
+        .filter(["donor_code", "type", "year", "value"], axis=1)
         .pivot(index=["donor_code", "year"], columns=["type"], values="value")
         .reset_index()
         .assign(
             exchange=lambda d: round(d.N / d.A, 5),
             deflator=lambda d: round(100 * d.A / d.D, 6),  # implied deflator
             iso_code=lambda d: d.donor_code.map(oecd_codes()),
             year=lambda d: pd.to_datetime(d.year, format="%Y"),
```

### Comparing `pydeflate-1.3.6/pydeflate/get_data/wb_data.py` & `pydeflate-1.3.7/pydeflate/get_data/wb_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/pydeflate_config.py` & `pydeflate-1.3.7/pydeflate/pydeflate_config.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/settings/oecd_codes.json` & `pydeflate-1.3.7/pydeflate/settings/oecd_codes.json`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/tools/exchange.py` & `pydeflate-1.3.7/pydeflate/tools/exchange.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/tools/update_data.py` & `pydeflate-1.3.7/pydeflate/tools/update_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pydeflate/utils.py` & `pydeflate-1.3.7/pydeflate/utils.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.6/pyproject.toml` & `pydeflate-1.3.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydeflate"
-version = "1.3.6"
+version = "1.3.7"
 description = "Package to convert current prices figures to constant prices and vice versa"
 authors = ["Jorge Rivera <jorge.rivera@one.org>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: End Users/Desktop',
```

### Comparing `pydeflate-1.3.6/PKG-INFO` & `pydeflate-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeflate
-Version: 1.3.6
+Version: 1.3.7
 Summary: Package to convert current prices figures to constant prices and vice versa
 License: MIT
 Author: Jorge Rivera
 Author-email: jorge.rivera@one.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

