# Comparing `tmp/oda_data-1.0.1.tar.gz` & `tmp/oda_data-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_data-1.0.1.tar", max compression
+gzip compressed data, was "oda_data-1.0.2.tar", max compression
```

## Comparing `oda_data-1.0.1.tar` & `oda_data-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1069 2023-04-13 16:13:58.602182 oda_data-1.0.1/LICENSE
--rw-r--r--   0        0        0     5055 2023-04-13 16:13:58.602182 oda_data-1.0.1/README.md
--rw-r--r--   0        0        0      157 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/.raw_data/README.md
--rw-r--r--   0        0        0      184 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/README.md
--rw-r--r--   0        0        0     1190 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/__init__.py
--rw-r--r--   0        0        0      782 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/classes/README.md
--rw-r--r--   0        0        0        0 2023-04-13 16:13:58.602182 oda_data-1.0.1/oda_data/classes/__init__.py
--rw-r--r--   0        0        0    22978 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/classes/oda_data.py
--rw-r--r--   0        0        0      360 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/classes/representations.py
--rw-r--r--   0        0        0      476 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/clean_data/README.md
--rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/clean_data/__init__.py
--rw-r--r--   0        0        0     5283 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/clean_data/common.py
--rw-r--r--   0        0        0      844 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/config.py
--rw-r--r--   0        0        0     3189 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/README.md
--rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/__init__.py
--rw-r--r--   0        0        0     5761 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/common.py
--rw-r--r--   0        0        0     2030 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/crs.py
--rw-r--r--   0        0        0      840 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/dac1.py
--rw-r--r--   0        0        0      847 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/dac2a.py
--rw-r--r--   0        0        0      889 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/get_data/multisystem.py
--rw-r--r--   0        0        0      119 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/README.md
--rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/__init__.py
--rw-r--r--   0        0        0     1512 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/linked_indicators.py
--rw-r--r--   0        0        0     6434 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/research_indicators.py
--rw-r--r--   0        0        0     6836 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/indicators/sector_components.py
--rw-r--r--   0        0        0      698 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/logger.py
--rw-r--r--   0        0        0      603 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/read_data/README.md
--rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/read_data/__init__.py
--rw-r--r--   0        0        0     2682 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/read_data/read.py
--rw-r--r--   0        0        0    10207 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/Available indicators.md
--rw-r--r--   0        0        0     5540 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/README.md
--rw-r--r--   0        0        0     2570 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/channel_codes.json
--rw-r--r--   0        0        0     6617 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/crs_config.json
--rw-r--r--   0        0        0      862 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/dac1_config.json
--rw-r--r--   0        0        0      859 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/dac2a_config.json
--rw-r--r--   0        0        0     7759 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/donor_groupings.json
--rw-r--r--   0        0        0    27497 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/indicators.json
--rw-r--r--   0        0        0     1506 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/key_columns.json
--rw-r--r--   0        0        0     2762 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/multisystem_config.json
--rw-r--r--   0        0        0    17756 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/settings/recipient_groupings.json
--rw-r--r--   0        0        0       78 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/tools/README.md
--rw-r--r--   0        0        0        0 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/tools/__init__.py
--rw-r--r--   0        0        0      799 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/tools/groupings.py
--rw-r--r--   0        0        0     5658 2023-04-13 16:13:58.606182 oda_data-1.0.1/oda_data/tools/names.py
--rw-r--r--   0        0        0     1039 2023-04-13 16:13:58.606182 oda_data-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5962 1970-01-01 00:00:00.000000 oda_data-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-12 11:56:29.307223 oda_data-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5055 2023-06-12 11:56:29.307223 oda_data-1.0.2/README.md
+-rw-r--r--   0        0        0      157 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/.raw_data/README.md
+-rw-r--r--   0        0        0      184 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/README.md
+-rw-r--r--   0        0        0     1190 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/__init__.py
+-rw-r--r--   0        0        0      782 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/classes/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/classes/__init__.py
+-rw-r--r--   0        0        0    22978 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/classes/oda_data.py
+-rw-r--r--   0        0        0      360 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/classes/representations.py
+-rw-r--r--   0        0        0      476 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/clean_data/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/clean_data/__init__.py
+-rw-r--r--   0        0        0     5283 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/clean_data/common.py
+-rw-r--r--   0        0        0      844 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/config.py
+-rw-r--r--   0        0        0     3189 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/get_data/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/get_data/__init__.py
+-rw-r--r--   0        0        0     6508 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/get_data/common.py
+-rw-r--r--   0        0        0     2030 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/get_data/crs.py
+-rw-r--r--   0        0        0      840 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/get_data/dac1.py
+-rw-r--r--   0        0        0      847 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/get_data/dac2a.py
+-rw-r--r--   0        0        0      889 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/get_data/multisystem.py
+-rw-r--r--   0        0        0      119 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/indicators/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/indicators/__init__.py
+-rw-r--r--   0        0        0     1512 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/indicators/linked_indicators.py
+-rw-r--r--   0        0        0     6434 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/indicators/research_indicators.py
+-rw-r--r--   0        0        0     6836 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/indicators/sector_components.py
+-rw-r--r--   0        0        0      698 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/logger.py
+-rw-r--r--   0        0        0      603 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/read_data/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/read_data/__init__.py
+-rw-r--r--   0        0        0     2682 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/read_data/read.py
+-rw-r--r--   0        0        0    10207 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/Available indicators.md
+-rw-r--r--   0        0        0     5540 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/README.md
+-rw-r--r--   0        0        0     2570 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/channel_codes.json
+-rw-r--r--   0        0        0     6617 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/crs_config.json
+-rw-r--r--   0        0        0      862 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/dac1_config.json
+-rw-r--r--   0        0        0      859 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/dac2a_config.json
+-rw-r--r--   0        0        0     7759 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/donor_groupings.json
+-rw-r--r--   0        0        0    27497 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/indicators.json
+-rw-r--r--   0        0        0     1506 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/key_columns.json
+-rw-r--r--   0        0        0     2762 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/multisystem_config.json
+-rw-r--r--   0        0        0    17756 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/settings/recipient_groupings.json
+-rw-r--r--   0        0        0       78 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/tools/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/tools/__init__.py
+-rw-r--r--   0        0        0      799 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/tools/groupings.py
+-rw-r--r--   0        0        0     5658 2023-06-12 11:56:29.307223 oda_data-1.0.2/oda_data/tools/names.py
+-rw-r--r--   0        0        0     1039 2023-06-12 11:56:29.307223 oda_data-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 oda_data-1.0.2/PKG-INFO
```

### Comparing `oda_data-1.0.1/LICENSE` & `oda_data-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/README.md` & `oda_data-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/__init__.py` & `oda_data-1.0.2/oda_data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 from oda_data.classes.oda_data import ODAData
 from oda_data.get_data.crs import download_crs
 from oda_data.get_data.dac1 import download_dac1
 from oda_data.get_data.dac2a import download_dac2a
 from oda_data.get_data.multisystem import download_multisystem
 from oda_data.read_data.read import read_crs, read_dac1, read_dac2a, read_multisystem
```

### Comparing `oda_data-1.0.1/oda_data/classes/README.md` & `oda_data-1.0.2/oda_data/classes/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/classes/oda_data.py` & `oda_data-1.0.2/oda_data/classes/oda_data.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/clean_data/common.py` & `oda_data-1.0.2/oda_data/clean_data/common.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/config.py` & `oda_data-1.0.2/oda_data/config.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/get_data/README.md` & `oda_data-1.0.2/oda_data/get_data/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/get_data/common.py` & `oda_data-1.0.2/oda_data/get_data/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,48 +52,73 @@
 
 
 def _extract_zip(serialised_content: io.BytesIO, file_name: str) -> csv:
     """Extract a file from a zip file. This creates a deep copy of the content"""
     return zf.ZipFile(serialised_content).open(file_name)
 
 
-def _raw2df(csv_file: csv, sep: str) -> pd.DataFrame:
+def _raw2df(csv_file: csv, sep: str, encoding: str) -> pd.DataFrame:
     """Convert a raw csv to a DataFrame. Check the result if requested"""
 
-    _ = pd.read_csv(
-        csv_file, sep=sep, dtype="str", encoding="ISO-8859-1", low_memory=False
-    )
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
 
     if len(_.columns) < 3:
         raise pd.errors.ParserError
+
     return _
 
 
+def _extract_df(request_content, file_name: str, separator: str) -> pd.DataFrame:
+    import copy
+
+    for encoding in ["utf_16", "ISO-8859-1"]:
+        try:
+            rc = copy.deepcopy(request_content)
+            # serialise the content
+            serialised_content = _serialise_content(rc)
+
+            # extract the file
+            raw_csv = _extract_zip(serialised_content, file_name)
+
+            # convert to a dataframe
+            return _raw2df(csv_file=raw_csv, sep=separator, encoding=encoding)
+        except pd.errors.ParserError:
+            logger.debug(f"{encoding} not valid")
+
+    raise pd.errors.ParserError
+
+
 def read_zip_content(
     request_content, file_name: str, priority_sep: str = "|"
 ) -> pd.DataFrame:
     """Read a zip file and return a DataFrame"""
-    import copy
-
-    rc = copy.deepcopy(request_content)
 
     try:
-        # serialise the content
-        serialised_content = _serialise_content(rc)
-
-        # extract the file
-        raw_csv = _extract_zip(serialised_content, file_name)
-
-        # convert to a dataframe
-        return _raw2df(csv_file=raw_csv, sep=priority_sep)
+        return _extract_df(
+            request_content=request_content, file_name=file_name, separator=priority_sep
+        )
 
     except UnicodeDecodeError:
-        return read_zip_content(rc, file_name=file_name, priority_sep=",")
+        return _extract_df(
+            request_content=request_content, file_name=file_name, separator=","
+        )
     except pd.errors.ParserError:
-        return read_zip_content(rc, file_name=file_name, priority_sep=",")
+        return _extract_df(
+            request_content=request_content, file_name=file_name, separator=","
+        )
 
 
 def extract_file_link_single(url: str) -> str:
     """Parse the OECD website to find the download link"""
     try:
         response = requests.get(url, verify=True)
     except requests.exceptions.SSLError:
```

### Comparing `oda_data-1.0.1/oda_data/get_data/crs.py` & `oda_data-1.0.2/oda_data/get_data/crs.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/get_data/dac1.py` & `oda_data-1.0.2/oda_data/get_data/dac1.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/get_data/dac2a.py` & `oda_data-1.0.2/oda_data/get_data/dac2a.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/get_data/multisystem.py` & `oda_data-1.0.2/oda_data/get_data/multisystem.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/indicators/linked_indicators.py` & `oda_data-1.0.2/oda_data/indicators/linked_indicators.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/indicators/research_indicators.py` & `oda_data-1.0.2/oda_data/indicators/research_indicators.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/indicators/sector_components.py` & `oda_data-1.0.2/oda_data/indicators/sector_components.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/logger.py` & `oda_data-1.0.2/oda_data/logger.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/read_data/README.md` & `oda_data-1.0.2/oda_data/read_data/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/read_data/read.py` & `oda_data-1.0.2/oda_data/read_data/read.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/Available indicators.md` & `oda_data-1.0.2/oda_data/settings/Available indicators.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/README.md` & `oda_data-1.0.2/oda_data/settings/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/channel_codes.json` & `oda_data-1.0.2/oda_data/settings/channel_codes.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/crs_config.json` & `oda_data-1.0.2/oda_data/settings/crs_config.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/dac1_config.json` & `oda_data-1.0.2/oda_data/settings/dac1_config.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/dac2a_config.json` & `oda_data-1.0.2/oda_data/settings/dac2a_config.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/donor_groupings.json` & `oda_data-1.0.2/oda_data/settings/donor_groupings.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/indicators.json` & `oda_data-1.0.2/oda_data/settings/indicators.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/key_columns.json` & `oda_data-1.0.2/oda_data/settings/key_columns.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/multisystem_config.json` & `oda_data-1.0.2/oda_data/settings/multisystem_config.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/settings/recipient_groupings.json` & `oda_data-1.0.2/oda_data/settings/recipient_groupings.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/tools/groupings.py` & `oda_data-1.0.2/oda_data/tools/groupings.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/oda_data/tools/names.py` & `oda_data-1.0.2/oda_data/tools/names.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.0.1/pyproject.toml` & `oda_data-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oda_data"
-version = "1.0.1"
+version = "1.0.2"
 description = "A python package to work with Official Development Assistance data from the OECD DAC."
 readme = "README.md"
 authors = ["Jorge Rivera <jorge.rivera@one.org>"]
 packages = [{ include = "oda_data" }]
 classifiers = ["Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `oda_data-1.0.1/PKG-INFO` & `oda_data-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: oda-data
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package to work with Official Development Assistance data from the OECD DAC.
 Author: Jorge Rivera
 Author-email: jorge.rivera@one.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bblocks (>=1,<2)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pydeflate (>=1.3.1,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
```

