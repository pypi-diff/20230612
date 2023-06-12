# Comparing `tmp/dicom_csv-0.2.8.tar.gz` & `tmp/dicom_csv-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicom_csv-0.2.8.tar", last modified: Wed Apr 26 07:38:32 2023, max compression
+gzip compressed data, was "dicom_csv-0.2.9.tar", last modified: Mon Jun 12 15:49:19 2023, max compression
```

## Comparing `dicom_csv-0.2.8.tar` & `dicom_csv-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/dicom_csv/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/rtstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/dicom_csv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/dicom_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 07:38:32.000000 dicom_csv-0.2.8/dicom_csv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:38:32.180561 dicom_csv-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-26 07:38:29.000000 dicom_csv-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:49:19.777134 dicom_csv-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-12 15:49:19.777134 dicom_csv-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:49:19.777134 dicom_csv-0.2.9/dicom_csv/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/rtstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/dicom_csv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:49:19.777134 dicom_csv-0.2.9/dicom_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-12 15:49:19.000000 dicom_csv-0.2.9/dicom_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-12 15:49:19.000000 dicom_csv-0.2.9/dicom_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:49:19.000000 dicom_csv-0.2.9/dicom_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-12 15:49:19.000000 dicom_csv-0.2.9/dicom_csv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 15:49:19.000000 dicom_csv-0.2.9/dicom_csv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 15:49:19.000000 dicom_csv-0.2.9/dicom_csv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:49:19.777134 dicom_csv-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-12 15:49:12.000000 dicom_csv-0.2.9/setup.py
```

### Comparing `dicom_csv-0.2.8/LICENSE` & `dicom_csv-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/PKG-INFO` & `dicom_csv-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dicom_csv
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utils for gathering, aggregation and handling metadata from DICOM files.
 Home-page: https://github.com/neuro-ml/dicom-csv
 License: MIT
-Download-URL: https://github.com/neuro-ml/dicom-csv/v0.2.8.tar.gz
+Download-URL: https://github.com/neuro-ml/dicom-csv/v0.2.9.tar.gz
 Keywords: DICOM
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dicom_csv-0.2.8/README.md` & `dicom_csv-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv/aggregation.py` & `dicom_csv-0.2.9/dicom_csv/aggregation.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv/convert.py` & `dicom_csv-0.2.9/dicom_csv/convert.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv/crawler.py` & `dicom_csv-0.2.9/dicom_csv/crawler.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import struct
 from pathlib import Path
 from typing import Sequence, Iterable
 
 import pandas as pd
 from tqdm import tqdm
-from pydicom import valuerep, errors, dcmread, Dataset
+from pydicom import valuerep, errors, dcmread, Dataset, DataElement, sequence
 from pydicom.uid import ImplicitVRLittleEndian
 
 from .convert import is_volumetric_ct, split_volume
 from .utils import PathLike
 
 __all__ = 'get_file_meta', 'join_tree'
 
@@ -33,16 +33,23 @@
             dc = dcmread(str(path), force=True)
             dc.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
             return True, dc
 
         raise
 
 
+def iter_private_tags(ds: Dataset) -> Iterable[DataElement]:
+    ds.__repr__() # https://github.com/pydicom/pydicom/issues/1805
+    for tag in ds.values():
+        if tag.is_private:
+            yield tag
+
+
 def get_file_meta(path: PathLike, force: bool = True, read_pixel_array: bool = False,
-                  unpack_volumetric: bool = False) -> Iterable[dict]:
+                  unpack_volumetric: bool = False, extract_private: bool = False) -> Iterable[dict]:
     """
     Get a dict containing the metadata from the DICOM file located at ``path``.
 
     Parameters
     ---
 
     path - PathLike,
@@ -75,20 +82,20 @@
 
     if unpack_volumetric and is_volumetric_ct(instance, errors=False):
         instances = split_volume(instance)
     else:
         instances = [instance]
 
     for instance in instances:
-        result = extract_meta(instance, read_pixel_array)
+        result = extract_meta(instance, read_pixel_array, extract_private)
         result.setdefault('NoError', True)
         yield result
 
 
-def extract_meta(instance: Dataset, read_pixel_array: bool = False) -> dict:
+def extract_meta(instance: Dataset, read_pixel_array: bool = False, extract_private: bool = False) -> dict:
     result = {}
     if read_pixel_array:
         try:
             has_px = hasattr(instance, 'pixel_array')
         except (TypeError, NotImplementedError):
             has_px = False
         except (ValueError, RuntimeError):
@@ -113,19 +120,30 @@
         elif isinstance(value, (int, float, str)):
             result[attr] = value
 
         elif attr in SERIAL:
             for pos, num in enumerate(value):
                 result[f'{attr}{pos}'] = num
 
+    if extract_private:
+        for private_tag in iter_private_tags(instance):
+            if isinstance(private_tag, sequence.Sequence):
+                pass
+            if private_tag.VR not in valuerep.LONG_VALUE_VR:
+                value = instance.get(private_tag.tag).value
+                if isinstance(value, (int, float)):
+                    result[private_tag.name] = value
+                if isinstance(value, str):
+                    result[private_tag.name] = value[:100] # just in case
+
     return result
 
 
 def join_tree(top: PathLike, ignore_extensions: Sequence[str] = (), relative: bool = True, verbose: int = 0,
-              read_pixel_array: bool = False, force: bool = True, unpack_volumetric: bool = True,
+              read_pixel_array: bool = False, force: bool = True, unpack_volumetric: bool = True, extract_private: bool = False,
               total: bool = False) -> pd.DataFrame:
     """
     Returns a dataframe containing metadata for each file in all the subfolders of ``top``.
 
     Parameters
     ----------
     top: PathLike
@@ -186,13 +204,13 @@
                 continue
 
             bar.update()
             if verbose > 1:
                 bar.set_description(str(rel_path / filename))
 
             for entry in get_file_meta(root / filename, force=force, read_pixel_array=read_pixel_array,
-                                       unpack_volumetric=unpack_volumetric):
+                                       unpack_volumetric=unpack_volumetric, extract_private=extract_private):
                 entry['PathToFolder'] = str(rel_path if relative else root)
                 entry['FileName'] = filename
                 result.append(entry)
 
     return pd.DataFrame(result)
```

### Comparing `dicom_csv-0.2.8/dicom_csv/interface.py` & `dicom_csv-0.2.9/dicom_csv/interface.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv/misc.py` & `dicom_csv-0.2.9/dicom_csv/misc.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv/rtstruct.py` & `dicom_csv-0.2.9/dicom_csv/rtstruct.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv/scripts.py` & `dicom_csv-0.2.9/dicom_csv/scripts.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv/spatial.py` & `dicom_csv-0.2.9/dicom_csv/spatial.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv/tags.py` & `dicom_csv-0.2.9/dicom_csv/tags.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv/utils.py` & `dicom_csv-0.2.9/dicom_csv/utils.py`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/dicom_csv.egg-info/PKG-INFO` & `dicom_csv-0.2.9/dicom_csv.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dicom-csv
-Version: 0.2.8
+Version: 0.2.9
 Summary: Utils for gathering, aggregation and handling metadata from DICOM files.
 Home-page: https://github.com/neuro-ml/dicom-csv
 License: MIT
-Download-URL: https://github.com/neuro-ml/dicom-csv/v0.2.8.tar.gz
+Download-URL: https://github.com/neuro-ml/dicom-csv/v0.2.9.tar.gz
 Keywords: DICOM
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dicom_csv-0.2.8/dicom_csv.egg-info/SOURCES.txt` & `dicom_csv-0.2.9/dicom_csv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/pyproject.toml` & `dicom_csv-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dicom_csv-0.2.8/setup.py` & `dicom_csv-0.2.9/setup.py`

 * *Files identical despite different names*

