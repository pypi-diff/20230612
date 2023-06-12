# Comparing `tmp/SimpleITKUtilities-0.1.tar.gz` & `tmp/SimpleITKUtilities-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleITKUtilities-0.1.tar", last modified: Fri Apr 28 22:24:41 2023, max compression
+gzip compressed data, was "SimpleITKUtilities-0.2.tar", last modified: Mon Jun 12 19:16:47 2023, max compression
```

## Comparing `SimpleITKUtilities-0.1.tar` & `SimpleITKUtilities-0.2.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:24:41.179920 SimpleITKUtilities-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:24:41.175920 SimpleITKUtilities-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:24:41.175920 SimpleITKUtilities-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-28 22:24:41.179920 SimpleITKUtilities-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:24:41.175920 SimpleITKUtilities-0.1/SimpleITK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:24:41.175920 SimpleITKUtilities-0.1/SimpleITK/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/SimpleITK/utilities/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/SimpleITK/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-28 22:24:41.000000 SimpleITKUtilities-0.1/SimpleITK/utilities/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/SimpleITK/utilities/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/SimpleITK/utilities/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/SimpleITK/utilities/make_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/SimpleITK/utilities/overlay_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/SimpleITK/utilities/slice_by_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/SimpleITK/utilities/vtk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:24:41.179920 SimpleITKUtilities-0.1/SimpleITKUtilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-28 22:24:41.000000 SimpleITKUtilities-0.1/SimpleITKUtilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-28 22:24:41.000000 SimpleITKUtilities-0.1/SimpleITKUtilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:24:41.000000 SimpleITKUtilities-0.1/SimpleITKUtilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 22:24:41.000000 SimpleITKUtilities-0.1/SimpleITKUtilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 22:24:41.000000 SimpleITKUtilities-0.1/SimpleITKUtilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:24:41.179920 SimpleITKUtilities-0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:24:41.179920 SimpleITKUtilities-0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:24:41.179920 SimpleITKUtilities-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:24:41.179920 SimpleITKUtilities-0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/test/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-28 22:24:25.000000 SimpleITKUtilities-0.1/test/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.891322 SimpleITKUtilities-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.891322 SimpleITKUtilities-0.2/SimpleITK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/SimpleITK/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/make_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/overlay_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/pyside.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/slice_by_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/SimpleITK/utilities/vtk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 19:16:47.000000 SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:47.895322 SimpleITKUtilities-0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/test_pyside.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-12 19:16:31.000000 SimpleITKUtilities-0.2/test/test_utilities.py
```

### Comparing `SimpleITKUtilities-0.1/.github/workflows/docs.yml` & `SimpleITKUtilities-0.2/.github/workflows/docs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: 3.11
           cache: 'pip'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install -r docs/requirements.txt .[vtk,dask]
+          python -m pip install -r docs/requirements.txt .[vtk,dask,pyside]
       - name: Build Sphinx Documentation
         run: |
           make -C docs html
           rm docs/build/html/.buildinfo
 
       - name: Upload documentation
         uses: actions/upload-artifact@v3
```

### Comparing `SimpleITKUtilities-0.1/.github/workflows/main.yml` & `SimpleITKUtilities-0.2/.github/workflows/main.yml`

 * *Files 15% similar despite different names*

```diff
@@ -44,28 +44,34 @@
       with:
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install -e .[vtk,dask] -r test/requirements.txt
+        python -m pip install -e .[vtk,dask,pyside] -r test/requirements.txt
+        sudo apt install libegl1
 
     - name: Test with pytest
+      env:
+        QT_QPA_PLATFORM: offscreen
       run: |
         python -m pytest
 
 
   publish:
     needs: test
-    name: Upload release to PyPI
+    name: Upload release to GitHub Releases and PyPI
     runs-on: ubuntu-latest
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
       contents: write
+    environment:
+      name: pypi
+      url: https://pypi.org/p/<your-pypi-project-name>
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python 3.11
       uses: actions/setup-python@v4
       with:
```

### Comparing `SimpleITKUtilities-0.1/.pre-commit-config.yaml` & `SimpleITKUtilities-0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/LICENSE` & `SimpleITKUtilities-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/PKG-INFO` & `SimpleITKUtilities-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: SimpleITKUtilities
-Version: 0.1
+Version: 0.2
 Summary: A collection of utilities and integration tools to enhance SimpleITK.
 Author-email: Bradley Lowekamp <blowekamp@mail.nih.gov>, Ziv Yaniv <zivyaniv@nih.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: vtk
 Provides-Extra: dask
+Provides-Extra: pyside
 License-File: LICENSE
 License-File: NOTICE
 
 # SimpleITKUtilities
 
 ![SimpleITK Utilities Testing](https://github.com/SimpleITK/SimpleITKUtilities/actions/workflows/main.yml/badge.svg)&nbsp;&nbsp;[![SimpleITK Utilities Website](https://img.shields.io/website-up-down-brightgreen-red/http/shields.io.svg)](http://simpleitk.org/SimpleITKUtilities/)
```

### Comparing `SimpleITKUtilities-0.1/README.md` & `SimpleITKUtilities-0.2/README.md`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/SimpleITK/utilities/Logger.py` & `SimpleITKUtilities-0.2/SimpleITK/utilities/Logger.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/SimpleITK/utilities/__init__.py` & `SimpleITKUtilities-0.2/SimpleITK/utilities/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,27 +17,29 @@
 # ========================================================================
 
 from .Logger import Logger
 from .slice_by_slice import slice_by_slice
 from .make_isotropic import make_isotropic
 from .fft import fft_based_translation_initialization
 from .overlay_bounding_boxes import overlay_bounding_boxes
+from .resize import resize
 
 try:
     from ._version import version as __version__
 except ImportError:
     __version__ = "unknown version"
 
 
 __all__ = [
     "Logger",
     "slice_by_slice",
     "make_isotropic",
     "fft_based_translation_initialization",
     "overlay_bounding_boxes",
+    "resize",
     "__version__",
 ]
 
 from importlib.util import find_spec
 
 try:
     find_spec("vtk")
```

### Comparing `SimpleITKUtilities-0.1/SimpleITK/utilities/dask.py` & `SimpleITKUtilities-0.2/SimpleITK/utilities/dask.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/SimpleITK/utilities/fft.py` & `SimpleITKUtilities-0.2/SimpleITK/utilities/fft.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/SimpleITK/utilities/make_isotropic.py` & `SimpleITKUtilities-0.2/SimpleITK/utilities/make_isotropic.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/SimpleITK/utilities/overlay_bounding_boxes.py` & `SimpleITKUtilities-0.2/SimpleITK/utilities/overlay_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/SimpleITK/utilities/slice_by_slice.py` & `SimpleITKUtilities-0.2/SimpleITK/utilities/slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/SimpleITK/utilities/vtk.py` & `SimpleITKUtilities-0.2/SimpleITK/utilities/vtk.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/SimpleITKUtilities.egg-info/PKG-INFO` & `SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: SimpleITKUtilities
-Version: 0.1
+Version: 0.2
 Summary: A collection of utilities and integration tools to enhance SimpleITK.
 Author-email: Bradley Lowekamp <blowekamp@mail.nih.gov>, Ziv Yaniv <zivyaniv@nih.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: vtk
 Provides-Extra: dask
+Provides-Extra: pyside
 License-File: LICENSE
 License-File: NOTICE
 
 # SimpleITKUtilities
 
 ![SimpleITK Utilities Testing](https://github.com/SimpleITK/SimpleITKUtilities/actions/workflows/main.yml/badge.svg)&nbsp;&nbsp;[![SimpleITK Utilities Website](https://img.shields.io/website-up-down-brightgreen-red/http/shields.io.svg)](http://simpleitk.org/SimpleITKUtilities/)
```

### Comparing `SimpleITKUtilities-0.1/SimpleITKUtilities.egg-info/SOURCES.txt` & `SimpleITKUtilities-0.2/SimpleITKUtilities.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 SimpleITK/utilities/Logger.py
 SimpleITK/utilities/__init__.py
 SimpleITK/utilities/_version.py
 SimpleITK/utilities/dask.py
 SimpleITK/utilities/fft.py
 SimpleITK/utilities/make_isotropic.py
 SimpleITK/utilities/overlay_bounding_boxes.py
+SimpleITK/utilities/pyside.py
+SimpleITK/utilities/resize.py
 SimpleITK/utilities/slice_by_slice.py
 SimpleITK/utilities/vtk.py
 SimpleITKUtilities.egg-info/PKG-INFO
 SimpleITKUtilities.egg-info/SOURCES.txt
 SimpleITKUtilities.egg-info/dependency_links.txt
 SimpleITKUtilities.egg-info/requires.txt
 SimpleITKUtilities.egg-info/top_level.txt
@@ -26,8 +28,9 @@
 docs/requirements.txt
 docs/source/api.rst
 docs/source/conf.py
 docs/source/index.rst
 test/conftest.py
 test/requirements.txt
 test/test_dask.py
+test/test_pyside.py
 test/test_utilities.py
```

### Comparing `SimpleITKUtilities-0.1/docs/Makefile` & `SimpleITKUtilities-0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/docs/make.bat` & `SimpleITKUtilities-0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/docs/source/conf.py` & `SimpleITKUtilities-0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/pyproject.toml` & `SimpleITKUtilities-0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 ]
 dynamic = ["dependencies", "version"]
 
 
 [project.optional-dependencies]
 vtk=['vtk>=9.0']
 dask=['dask']
+pyside=['PySide6']
 
 [tool.setuptools]
 packages = ["SimpleITK.utilities"]
 
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools_scm]
-write_to = "SimpleITK/utilities/_version.py"
+write_to = "SimpleITK/utilities/_version.py"
```

### Comparing `SimpleITKUtilities-0.1/test/conftest.py` & `SimpleITKUtilities-0.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `SimpleITKUtilities-0.1/test/test_dask.py` & `SimpleITKUtilities-0.2/test/test_dask.py`

 * *Files identical despite different names*

