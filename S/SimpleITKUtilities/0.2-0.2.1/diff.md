# Comparing `tmp/SimpleITKUtilities-0.2.tar.gz` & `tmp/SimpleITKUtilities-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleITKUtilities-0.2.tar", last modified: Mon Jun 12 19:16:47 2023, max compression
+gzip compressed data, was "SimpleITKUtilities-0.2.1.tar", last modified: Mon Jun 12 20:24:52 2023, max compression
```

## Comparing `SimpleITKUtilities-0.2.tar` & `SimpleITKUtilities-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.891322 SimpleITKUtilities-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.891322 SimpleITKUtilities-0.2/SimpleITK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/SimpleITK/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/make_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/overlay_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/pyside.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/slice_by_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/vtk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/test_pyside.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.952475 SimpleITKUtilities-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.944475 SimpleITKUtilities-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.944475 SimpleITKUtilities-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.944475 SimpleITKUtilities-0.2.1/SimpleITK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/SimpleITK/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/make_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/overlay_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/pyside.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/slice_by_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/SimpleITK/utilities/vtk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 20:24:52.000000 SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:24:52.952475 SimpleITKUtilities-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:24:52.948475 SimpleITKUtilities-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/test_pyside.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-12 20:24:36.000000 SimpleITKUtilities-0.2.1/test/test_utilities.py
```

### Comparing `SimpleITKUtilities-0.2/.github/workflows/docs.yml` & `SimpleITKUtilities-0.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/.pre-commit-config.yaml` & `SimpleITKUtilities-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/LICENSE` & `SimpleITKUtilities-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/PKG-INFO` & `SimpleITKUtilities-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleITKUtilities
-Version: 0.2
+Version: 0.2.1
 Summary: A collection of utilities and integration tools to enhance SimpleITK.
 Author-email: Bradley Lowekamp <blowekamp@mail.nih.gov>, Ziv Yaniv <zivyaniv@nih.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `SimpleITKUtilities-0.2/README.md` & `SimpleITKUtilities-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/Logger.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/Logger.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/__init__.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/dask.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/dask.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/fft.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/fft.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/make_isotropic.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/make_isotropic.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/overlay_bounding_boxes.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/overlay_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/pyside.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/pyside.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/resize.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/resize.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/slice_by_slice.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITK/utilities/vtk.py` & `SimpleITKUtilities-0.2.1/SimpleITK/utilities/vtk.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/PKG-INFO` & `SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleITKUtilities
-Version: 0.2
+Version: 0.2.1
 Summary: A collection of utilities and integration tools to enhance SimpleITK.
 Author-email: Bradley Lowekamp <blowekamp@mail.nih.gov>, Ziv Yaniv <zivyaniv@nih.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/SOURCES.txt` & `SimpleITKUtilities-0.2.1/SimpleITKUtilities.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE
 NOTICE
 README.md
 pyproject.toml
 requirements.txt
 .github/workflows/docs.yml
 .github/workflows/main.yml
+.github/workflows/publish.yml
 SimpleITK/utilities/Logger.py
 SimpleITK/utilities/__init__.py
 SimpleITK/utilities/_version.py
 SimpleITK/utilities/dask.py
 SimpleITK/utilities/fft.py
 SimpleITK/utilities/make_isotropic.py
 SimpleITK/utilities/overlay_bounding_boxes.py
```

### Comparing `SimpleITKUtilities-0.2/docs/Makefile` & `SimpleITKUtilities-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/docs/make.bat` & `SimpleITKUtilities-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/docs/source/conf.py` & `SimpleITKUtilities-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/pyproject.toml` & `SimpleITKUtilities-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/test/conftest.py` & `SimpleITKUtilities-0.2.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/test/test_dask.py` & `SimpleITKUtilities-0.2.1/test/test_dask.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/test/test_pyside.py` & `SimpleITKUtilities-0.2.1/test/test_pyside.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.2/test/test_utilities.py` & `SimpleITKUtilities-0.2.1/test/test_utilities.py`

 * *Files identical despite different names*

