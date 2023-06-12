# Comparing `tmp/bgstools-0.1.5.tar.gz` & `tmp/bgstools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgstools-0.1.5.tar", max compression
+gzip compressed data, was "bgstools-0.1.6.tar", max compression
```

## Comparing `bgstools-0.1.5.tar` & `bgstools-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       72 2023-05-22 09:38:31.760561 bgstools-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-03 11:32:59.064694 bgstools-0.1.5/bgstools/__init__.py
--rw-r--r--   0        0        0       64 2023-05-22 20:01:20.000000 bgstools-0.1.5/bgstools/datastorage/__init__.py
--rw-r--r--   0        0        0     5014 2023-05-22 20:29:18.000000 bgstools-0.1.5/bgstools/datastorage/datastorage.py
--rw-r--r--   0        0        0      165 2023-05-23 09:24:52.850097 bgstools-0.1.5/bgstools/io/__init__.py
--rw-r--r--   0        0        0     3990 2023-05-23 08:59:13.676273 bgstools-0.1.5/bgstools/io/io.py
--rw-r--r--   0        0        0     3770 2023-05-24 20:22:39.226612 bgstools-0.1.5/bgstools/io/media.py
--rw-r--r--   0        0        0      122 2023-05-22 20:28:18.000000 bgstools-0.1.5/bgstools/spatial/__init__.py
--rw-r--r--   0        0        0     2654 2023-05-22 17:37:56.000000 bgstools-0.1.5/bgstools/spatial/spatial.py
--rw-r--r--   0        0        0       39 2023-05-22 20:27:28.000000 bgstools-0.1.5/bgstools/stt/__init__.py
--rw-r--r--   0        0        0     2171 2023-05-23 06:03:13.166243 bgstools-0.1.5/bgstools/stt/stt.py
--rw-r--r--   0        0        0       99 2023-05-22 20:25:04.000000 bgstools-0.1.5/bgstools/utils/__init__.py
--rw-r--r--   0        0        0     2971 2023-05-22 20:24:36.000000 bgstools-0.1.5/bgstools/utils/utils.py
--rw-r--r--   0        0        0      433 2023-05-24 20:24:05.236614 bgstools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 bgstools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-06-11 05:11:36.804060 bgstools-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/datastorage/__init__.py
+-rw-r--r--   0        0        0     5014 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/datastorage/datastorage.py
+-rw-r--r--   0        0        0      165 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/io/__init__.py
+-rw-r--r--   0        0        0     4617 2023-06-12 19:14:12.497334 bgstools-0.1.6/bgstools/io/io.py
+-rw-r--r--   0        0        0     3770 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/io/media.py
+-rw-r--r--   0        0        0      122 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/spatial/__init__.py
+-rw-r--r--   0        0        0     2654 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/spatial/spatial.py
+-rw-r--r--   0        0        0       39 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/stt/__init__.py
+-rw-r--r--   0        0        0     3641 2023-06-12 19:12:06.833881 bgstools-0.1.6/bgstools/stt/stt.py
+-rw-r--r--   0        0        0       99 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/utils/__init__.py
+-rw-r--r--   0        0        0     2971 2023-06-11 05:11:36.804060 bgstools-0.1.6/bgstools/utils/utils.py
+-rw-r--r--   0        0        0      433 2023-06-12 19:13:36.586548 bgstools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 bgstools-0.1.6/PKG-INFO
```

### Comparing `bgstools-0.1.5/bgstools/datastorage/datastorage.py` & `bgstools-0.1.6/bgstools/datastorage/datastorage.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.5/bgstools/io/io.py` & `bgstools-0.1.6/bgstools/io/io.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,35 +6,47 @@
 
 def load_yaml(filepath: str) -> dict:
     """
     Loads a YAML file.
 
     Can be used as stand-alone script by providing a command-line argument:
         python load_yaml.py --filepath /file/path/to/filename.yaml
+        python load_yaml.py --filepath http://example.com/path/to/filename.yaml
 
     Args:
-        filepath (str): The absolute path to the YAML file.
+        filepath (str): The absolute path to the YAML file or a URL to the YAML file.
 
     Returns:
         dict: The contents of the YAML file as a dictionary.
 
     Raises:
         FileNotFoundError: If the file does not exist.
         yaml.YAMLError: If there is an error while loading the YAML file.
     """
-    if not os.path.isfile(filepath):
-        raise FileNotFoundError(f"No such file or directory: '{filepath}'")
-
-    with open(filepath, 'r') as file_descriptor:
+    if filepath.startswith('http://') or filepath.startswith('https://'):
         try:
-            yaml_data = yaml.safe_load(file_descriptor)
-        except yaml.YAMLError as msg:
-            raise yaml.YAMLError(f'File `{filepath}` loading error. \n {msg}')
+            response = requests.get(filepath)
+            response.raise_for_status()  # Raises a HTTPError if the response status is 4xx, 5xx
+            yaml_data = yaml.safe_load(response.text)
+        except (requests.RequestException, yaml.YAMLError) as e:
+            raise Exception(f'Error loading YAML from `{filepath}`. \n {str(e)}')
         else:
             return yaml_data
+    else:
+        if not os.path.isfile(filepath):
+            raise FileNotFoundError(f"No such file or directory: '{filepath}'")
+
+        with open(filepath, 'r') as file_descriptor:
+            try:
+                yaml_data = yaml.safe_load(file_descriptor)
+            except yaml.YAMLError as msg:
+                raise yaml.YAMLError(f'File `{filepath}` loading error. \n {msg}')
+            else:
+                return yaml_data
+
 
 def get_available_services(services_filepath: str) -> OrderedDict:
     """
     Retrieves available services from a yaml file. These services can be used to
     create a multi-page app using Streamlit. 
 
     Args:
```

### Comparing `bgstools-0.1.5/bgstools/io/media.py` & `bgstools-0.1.6/bgstools/io/media.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.5/bgstools/spatial/spatial.py` & `bgstools-0.1.6/bgstools/spatial/spatial.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.5/bgstools/utils/utils.py` & `bgstools-0.1.6/bgstools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.5/PKG-INFO` & `bgstools-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: bgstools
-Version: 0.1.5
+Version: 0.1.6
 Summary: BeGeoSpatial Development Tools
 Author: José Beltrán
 Author-email: 102664984+jose-begeospatial@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: certifi (>=2023.5.7,<2024.0.0)
 Requires-Dist: h3 (>=3.7.6,<4.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pyproj (>=3.5.0,<4.0.0)
 Description-Content-Type: text/markdown
```

