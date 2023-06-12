# Comparing `tmp/mlighter-utils-1.1.0.tar.gz` & `tmp/mlighter-utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlighter-utils-1.1.0.tar", last modified: Fri Jun  9 18:23:17 2023, max compression
+gzip compressed data, was "mlighter-utils-1.1.1.tar", last modified: Mon Jun 12 20:13:17 2023, max compression
```

## Comparing `mlighter-utils-1.1.0.tar` & `mlighter-utils-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:17.302523 mlighter-utils-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:17.298523 mlighter-utils-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:17.298523 mlighter-utils-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 18:23:17.302523 mlighter-utils-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-09 18:23:17.302523 mlighter-utils-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:17.302523 mlighter-utils-1.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:17.302523 mlighter-utils-1.1.0/src/mlighter_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/src/mlighter_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/src/mlighter_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/src/mlighter_utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/src/mlighter_utils/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:17.302523 mlighter-utils-1.1.0/src/mlighter_utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/src/mlighter_utils/data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/src/mlighter_utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:17.302523 mlighter-utils-1.1.0/src/mlighter_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 18:23:17.000000 mlighter-utils-1.1.0/src/mlighter_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-09 18:23:17.000000 mlighter-utils-1.1.0/src/mlighter_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:23:17.000000 mlighter-utils-1.1.0/src/mlighter_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 18:23:17.000000 mlighter-utils-1.1.0/src/mlighter_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 18:23:17.000000 mlighter-utils-1.1.0/src/mlighter_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:17.302523 mlighter-utils-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-09 18:23:05.000000 mlighter-utils-1.1.0/tests/test_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:17.562578 mlighter-utils-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:17.558578 mlighter-utils-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:17.562578 mlighter-utils-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-12 20:13:17.562578 mlighter-utils-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-12 20:13:17.562578 mlighter-utils-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:17.562578 mlighter-utils-1.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:17.562578 mlighter-utils-1.1.1/src/mlighter_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/src/mlighter_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/src/mlighter_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/src/mlighter_utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/src/mlighter_utils/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:17.562578 mlighter-utils-1.1.1/src/mlighter_utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/src/mlighter_utils/data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/src/mlighter_utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:17.562578 mlighter-utils-1.1.1/src/mlighter_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-12 20:13:17.000000 mlighter-utils-1.1.1/src/mlighter_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-12 20:13:17.000000 mlighter-utils-1.1.1/src/mlighter_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:13:17.000000 mlighter-utils-1.1.1/src/mlighter_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 20:13:17.000000 mlighter-utils-1.1.1/src/mlighter_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 20:13:17.000000 mlighter-utils-1.1.1/src/mlighter_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:17.562578 mlighter-utils-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-12 20:13:08.000000 mlighter-utils-1.1.1/tests/test_training.py
```

### Comparing `mlighter-utils-1.1.0/.gitignore` & `mlighter-utils-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.1.0/LICENSE` & `mlighter-utils-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.1.0/PKG-INFO` & `mlighter-utils-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlighter-utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlighter-utils-1.1.0/setup.cfg` & `mlighter-utils-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.1.0/src/mlighter_utils/conversion.py` & `mlighter-utils-1.1.1/src/mlighter_utils/conversion.py`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.1.0/src/mlighter_utils/core.py` & `mlighter-utils-1.1.1/src/mlighter_utils/core.py`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.1.0/src/mlighter_utils/data/iris.csv` & `mlighter-utils-1.1.1/src/mlighter_utils/data/iris.csv`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.1.0/src/mlighter_utils.egg-info/PKG-INFO` & `mlighter-utils-1.1.1/src/mlighter_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlighter-utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: A set of utility functions for testing templates within mlighter
 Home-page: https://github.com/dakaidan/FuzzingUtils
 Author: Aidan Dakhama
 Author-email: ai.dakhama@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlighter-utils-1.1.0/src/mlighter_utils.egg-info/SOURCES.txt` & `mlighter-utils-1.1.1/src/mlighter_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlighter-utils-1.1.0/tests/test_conversion.py` & `mlighter-utils-1.1.1/tests/test_conversion.py`

 * *Files identical despite different names*

