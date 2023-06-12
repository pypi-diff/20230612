# Comparing `tmp/homonim-0.3.1.tar.gz` & `tmp/homonim-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homonim-0.3.1.tar", last modified: Mon Nov  7 08:28:18 2022, max compression
+gzip compressed data, was "homonim-0.3.2.tar", last modified: Mon Jun 12 21:46:09 2023, max compression
```

## Comparing `homonim-0.3.1.tar` & `homonim-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 08:28:18.224132 homonim-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-11-07 08:28:00.000000 homonim-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7601 2022-11-07 08:28:18.224132 homonim-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6858 2022-11-07 08:28:00.000000 homonim-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 08:28:18.224132 homonim-0.3.1/homonim/
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29615 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    13167 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    19914 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/fuse.py
--rw-r--r--   0 runner    (1001) docker     (121)    26452 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    18452 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/matched_pair.py
--rw-r--r--   0 runner    (1001) docker     (121)    22605 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/raster_array.py
--rw-r--r--   0 runner    (1001) docker     (121)    20608 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/raster_pair.py
--rw-r--r--   0 runner    (1001) docker     (121)    11733 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/stats.py
--rw-r--r--   0 runner    (1001) docker     (121)    12617 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-07 08:28:00.000000 homonim-0.3.1/homonim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 08:28:18.224132 homonim-0.3.1/homonim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7601 2022-11-07 08:28:18.000000 homonim-0.3.1/homonim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-07 08:28:18.000000 homonim-0.3.1/homonim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 08:28:18.000000 homonim-0.3.1/homonim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-11-07 08:28:18.000000 homonim-0.3.1/homonim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-07 08:28:18.000000 homonim-0.3.1/homonim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-07 08:28:18.000000 homonim-0.3.1/homonim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-07 08:28:00.000000 homonim-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 08:28:18.224132 homonim-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2655 2022-11-07 08:28:00.000000 homonim-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:46:09.925284 homonim-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-12 21:45:52.000000 homonim-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-06-12 21:46:09.925284 homonim-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-06-12 21:45:52.000000 homonim-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:46:09.925284 homonim-0.3.2/homonim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29615 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26452 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/matched_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/raster_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20719 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/raster_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 21:45:52.000000 homonim-0.3.2/homonim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:46:09.925284 homonim-0.3.2/homonim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-06-12 21:46:09.000000 homonim-0.3.2/homonim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-12 21:46:09.000000 homonim-0.3.2/homonim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:46:09.000000 homonim-0.3.2/homonim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 21:46:09.000000 homonim-0.3.2/homonim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 21:46:09.000000 homonim-0.3.2/homonim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 21:46:09.000000 homonim-0.3.2/homonim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 21:45:52.000000 homonim-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:46:09.925284 homonim-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-12 21:45:52.000000 homonim-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:46:09.925284 homonim-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-06-12 21:45:52.000000 homonim-0.3.2/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-06-12 21:45:52.000000 homonim-0.3.2/tests/test_fuse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22919 2023-06-12 21:45:52.000000 homonim-0.3.2/tests/test_fuse_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-06-12 21:45:52.000000 homonim-0.3.2/tests/test_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-06-12 21:45:52.000000 homonim-0.3.2/tests/test_matched_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-06-12 21:45:52.000000 homonim-0.3.2/tests/test_raster_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17680 2023-06-12 21:45:52.000000 homonim-0.3.2/tests/test_raster_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-12 21:45:52.000000 homonim-0.3.2/tests/test_stats.py
```

### Comparing `homonim-0.3.1/LICENSE` & `homonim-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `homonim-0.3.1/PKG-INFO` & `homonim-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: homonim
-Version: 0.3.1
+Version: 0.3.2
 Summary: Correct aerial and satellite imagery to surface reflectance.
-Home-page: https://github.com/dugalh/homonim
+Home-page: https://github.com/leftfield-geospatial/homonim
 Author: Dugal Harris
 Author-email: dugalh@gmail.com
 License: AGPLv3
 Project-URL: Documentation, https://homonim.readthedocs.io
-Project-URL: Source, https://github.com/dugalh/homonim
+Project-URL: Source, https://github.com/leftfield-geospatial/homonim
 Keywords: drone imagery,aerial imagery,satellite imagery,surface reflectance,correction,harmonization,anisotropy,brdf,atmospheric correction
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |Tests| |codecov| |PyPI version| |conda-forge version| |docs| |License: AGPL v3|
 
 homonim
 =======
 
-.. image:: https://raw.githubusercontent.com/dugalh/homonim/main/docs/readme_eg.webp
+.. image:: https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/docs/readme_eg.webp
    :alt: example
 
 
 .. short_descr_start
 
 Correct aerial and satellite imagery to surface reflectance.
 
@@ -135,19 +135,19 @@
 .. code:: python
 
     from pathlib import Path
     from homonim import RasterFuse, RasterCompare, Model
 
     # urls of source and reference test images
     src_file = (
-        'https://raw.githubusercontent.com/dugalh/homonim/main/'
+        'https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/'
         'tests/data/source/ngi_rgb_byte_1.tif'
     )
     ref_file = (
-        'https://raw.githubusercontent.com/dugalh/homonim/main/'
+        'https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/'
         'tests/data/reference/sentinel2_b432_byte.tif'
     )
 
     # path to corrected file to create
     corr_file = './corrected.tif'
 
     # Correct src_file to surface reflectance by fusion with ref_file, using the
@@ -156,15 +156,15 @@
         fuse.process(corr_file, Model.gain_blk_offset, (5, 5), overwrite=True)
 
 .. api_example_end
 
 Reference imagery
 ~~~~~~~~~~~~~~~~~
 
-`geedim <https://github.com/dugalh/geedim>`_ can be used as a companion tool for searching and downloading cloud-free reference imagery.   Alternatively, satellite imagery is available from a number of sources, including the `Google <https://developers.google.com/earth-engine/datasets>`_, `Amazon <https://aws.amazon.com/earth/>`_ and `Microsoft <https://planetarycomputer.microsoft.com/catalog>`_ repositories.
+`geedim <https://github.com/leftfield-geospatial/geedim>`_ can be used as a companion tool for searching and downloading cloud-free reference imagery.   Alternatively, satellite imagery is available from a number of sources, including the `Google <https://developers.google.com/earth-engine/datasets>`_, `Amazon <https://aws.amazon.com/earth/>`_ and `Microsoft <https://planetarycomputer.microsoft.com/catalog>`_ repositories.
 
 
 Usage
 -----
 
 See the documentation `here <https://homonim.readthedocs.io/>`_.
 
@@ -206,18 +206,18 @@
         year  = {2019},
         publisher = {Taylor & Francis},
         doi = {10.1080/01431161.2018.1528404},
         URL = {https://doi.org/10.1080/01431161.2018.1528404},
     }
 
 
-.. |Tests| image:: https://github.com/dugalh/homonim/actions/workflows/run-unit-tests.yml/badge.svg
-   :target: https://github.com/dugalh/homonim/actions/workflows/run-unit-tests.yml
-.. |codecov| image:: https://codecov.io/gh/dugalh/homonim/branch/main/graph/badge.svg?token=A01698K96C
-   :target: https://codecov.io/gh/dugalh/homonim
+.. |Tests| image:: https://github.com/leftfield-geospatial/homonim/actions/workflows/run-unit-tests.yml/badge.svg
+   :target: https://github.com/leftfield-geospatial/homonim/actions/workflows/run-unit-tests.yml
+.. |codecov| image:: https://codecov.io/gh/leftfield-geospatial/homonim/branch/main/graph/badge.svg?token=A01698K96C
+   :target: https://codecov.io/gh/leftfield-geospatial/homonim
 .. |License: AGPL v3| image:: https://img.shields.io/badge/License-AGPL_v3-blue.svg
    :target: https://www.gnu.org/licenses/agpl-3.0
 .. |PyPI version| image:: https://img.shields.io/pypi/v/homonim?color=blue
    :target: https://pypi.org/project/homonim/
 .. |conda-forge version| image:: https://img.shields.io/conda/vn/conda-forge/homonim.svg?color=blue
    :alt: conda-forge
    :target: https://anaconda.org/conda-forge/homonim
```

### Comparing `homonim-0.3.1/README.rst` & `homonim-0.3.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 |Tests| |codecov| |PyPI version| |conda-forge version| |docs| |License: AGPL v3|
 
 homonim
 =======
 
-.. image:: https://raw.githubusercontent.com/dugalh/homonim/main/docs/readme_eg.webp
+.. image:: https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/docs/readme_eg.webp
    :alt: example
 
 
 .. short_descr_start
 
 Correct aerial and satellite imagery to surface reflectance.
 
@@ -117,19 +117,19 @@
 .. code:: python
 
     from pathlib import Path
     from homonim import RasterFuse, RasterCompare, Model
 
     # urls of source and reference test images
     src_file = (
-        'https://raw.githubusercontent.com/dugalh/homonim/main/'
+        'https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/'
         'tests/data/source/ngi_rgb_byte_1.tif'
     )
     ref_file = (
-        'https://raw.githubusercontent.com/dugalh/homonim/main/'
+        'https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/'
         'tests/data/reference/sentinel2_b432_byte.tif'
     )
 
     # path to corrected file to create
     corr_file = './corrected.tif'
 
     # Correct src_file to surface reflectance by fusion with ref_file, using the
@@ -138,15 +138,15 @@
         fuse.process(corr_file, Model.gain_blk_offset, (5, 5), overwrite=True)
 
 .. api_example_end
 
 Reference imagery
 ~~~~~~~~~~~~~~~~~
 
-`geedim <https://github.com/dugalh/geedim>`_ can be used as a companion tool for searching and downloading cloud-free reference imagery.   Alternatively, satellite imagery is available from a number of sources, including the `Google <https://developers.google.com/earth-engine/datasets>`_, `Amazon <https://aws.amazon.com/earth/>`_ and `Microsoft <https://planetarycomputer.microsoft.com/catalog>`_ repositories.
+`geedim <https://github.com/leftfield-geospatial/geedim>`_ can be used as a companion tool for searching and downloading cloud-free reference imagery.   Alternatively, satellite imagery is available from a number of sources, including the `Google <https://developers.google.com/earth-engine/datasets>`_, `Amazon <https://aws.amazon.com/earth/>`_ and `Microsoft <https://planetarycomputer.microsoft.com/catalog>`_ repositories.
 
 
 Usage
 -----
 
 See the documentation `here <https://homonim.readthedocs.io/>`_.
 
@@ -188,18 +188,18 @@
         year  = {2019},
         publisher = {Taylor & Francis},
         doi = {10.1080/01431161.2018.1528404},
         URL = {https://doi.org/10.1080/01431161.2018.1528404},
     }
 
 
-.. |Tests| image:: https://github.com/dugalh/homonim/actions/workflows/run-unit-tests.yml/badge.svg
-   :target: https://github.com/dugalh/homonim/actions/workflows/run-unit-tests.yml
-.. |codecov| image:: https://codecov.io/gh/dugalh/homonim/branch/main/graph/badge.svg?token=A01698K96C
-   :target: https://codecov.io/gh/dugalh/homonim
+.. |Tests| image:: https://github.com/leftfield-geospatial/homonim/actions/workflows/run-unit-tests.yml/badge.svg
+   :target: https://github.com/leftfield-geospatial/homonim/actions/workflows/run-unit-tests.yml
+.. |codecov| image:: https://codecov.io/gh/leftfield-geospatial/homonim/branch/main/graph/badge.svg?token=A01698K96C
+   :target: https://codecov.io/gh/leftfield-geospatial/homonim
 .. |License: AGPL v3| image:: https://img.shields.io/badge/License-AGPL_v3-blue.svg
    :target: https://www.gnu.org/licenses/agpl-3.0
 .. |PyPI version| image:: https://img.shields.io/pypi/v/homonim?color=blue
    :target: https://pypi.org/project/homonim/
 .. |conda-forge version| image:: https://img.shields.io/conda/vn/conda-forge/homonim.svg?color=blue
    :alt: conda-forge
    :target: https://anaconda.org/conda-forge/homonim
```

### Comparing `homonim-0.3.1/homonim/__init__.py` & `homonim-0.3.2/homonim/__init__.py`

 * *Files identical despite different names*

### Comparing `homonim-0.3.1/homonim/cli.py` & `homonim-0.3.2/homonim/cli.py`

 * *Files identical despite different names*

### Comparing `homonim-0.3.1/homonim/compare.py` & `homonim-0.3.2/homonim/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         Where source and reference images are RGB, or have ``center_wavelength`` metadata, bands are matched
         automatically based on wavelength.  Where there are the same number of source and reference bands, and no
         ``center_wavelength`` metadata, bands are assumed to be in matching order.  Subsets and ordering of source
         and reference bands can be specified with the ``src_bands`` and ``ref_bands`` parameters.
 
         .. note::
 
-            Images downloaded with `geedim <https://github.com/dugalh/geedim>`_ have ``center_wavelength`` metadata
+            Images downloaded with `geedim <https://github.com/leftfield-geospatial/geedim>`_ have ``center_wavelength`` metadata
             compatible with ``homonim``.
 
         Parameters
         ----------
         src_filename: str, pathlib.Path
             Path or URL of the source image file.
         ref_filename: str, pathlib.Path
```

### Comparing `homonim-0.3.1/homonim/enums.py` & `homonim-0.3.2/homonim/enums.py`

 * *Files identical despite different names*

### Comparing `homonim-0.3.1/homonim/errors.py` & `homonim-0.3.2/homonim/errors.py`

 * *Files identical despite different names*

### Comparing `homonim-0.3.1/homonim/fuse.py` & `homonim-0.3.2/homonim/fuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         Where source and reference images are RGB, or have ``center_wavelength`` metadata, bands are matched
         automatically based on wavelength.  Where there are the same number of source and reference bands, and no
         ``center_wavelength`` metadata, bands are assumed to be in matching order.  Subsets and ordering of source
         and reference bands can be specified with the ``src_bands`` and ``ref_bands`` parameters.
 
         .. note::
 
-            Images downloaded with `geedim <https://github.com/dugalh/geedim>`_ have ``center_wavelength`` metadata
+            Images downloaded with `geedim <https://github.com/leftfield-geospatial/geedim>`_ have ``center_wavelength`` metadata
             compatible with ``homonim``.
 
         Parameters
         ----------
         src_filename: str, Path
             Path to a source image file.
         ref_filename: str, Path
```

### Comparing `homonim-0.3.1/homonim/kernel_model.py` & `homonim-0.3.2/homonim/kernel_model.py`

 * *Files identical despite different names*

### Comparing `homonim-0.3.1/homonim/matched_pair.py` & `homonim-0.3.2/homonim/matched_pair.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         Where source and reference images are RGB, or have ``center_wavelength`` metadata, bands are matched
         automatically based on wavelength.  Where there are the same number of source and reference bands, and no
         ``center_wavelength`` metadata, bands are assumed to be in matching order.  Subsets and ordering of source
         and reference bands can be specified with the ``src_bands`` and ``ref_bands`` parameters.
 
         .. note::
 
-            Images downloaded with `geedim <https://github.com/dugalh/geedim>`_ have ``center_wavelength`` metadata
+            Images downloaded with `geedim <https://github.com/leftfield-geospatial/geedim>`_ have ``center_wavelength`` metadata
             compatible with ``homonim``.
 
         Parameters
         ----------
         src_filename: str, pathlib.Path
             Path or URL of the source image file.
         ref_filename: str, pathlib.Path
```

### Comparing `homonim-0.3.1/homonim/raster_array.py` & `homonim-0.3.2/homonim/raster_array.py`

 * *Files identical despite different names*

### Comparing `homonim-0.3.1/homonim/raster_pair.py` & `homonim-0.3.2/homonim/raster_pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,16 @@
     def close(self):
         """ Close the source and reference image datasets. """
         self._src_im.close()
         self._ref_im.close()
 
     def __enter__(self):
         self._stack = ExitStack()
-        self._stack.enter_context(rio.Env(GDAL_NUM_THREADS='ALL_CPUs', GTIFF_FORCE_RGBA=False))
+        # TODO: revert to GDAL_NUM_THREADS='ALL_CPUS' when https://github.com/rasterio/rasterio/issues/2847 is resolved
+        self._stack.enter_context(rio.Env(GDAL_NUM_THREADS=1, GTIFF_FORCE_RGBA=False))
         self._stack.enter_context(logging_redirect_tqdm([logging.getLogger(__package__)]))
         self.open()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
         self._stack.__exit__(exc_type, exc_val, exc_tb)
```

### Comparing `homonim-0.3.1/homonim/stats.py` & `homonim-0.3.2/homonim/stats.py`

 * *Files identical despite different names*

### Comparing `homonim-0.3.1/homonim/utils.py` & `homonim-0.3.2/homonim/utils.py`

 * *Files identical despite different names*

### Comparing `homonim-0.3.1/homonim.egg-info/PKG-INFO` & `homonim-0.3.2/homonim.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: homonim
-Version: 0.3.1
+Version: 0.3.2
 Summary: Correct aerial and satellite imagery to surface reflectance.
-Home-page: https://github.com/dugalh/homonim
+Home-page: https://github.com/leftfield-geospatial/homonim
 Author: Dugal Harris
 Author-email: dugalh@gmail.com
 License: AGPLv3
 Project-URL: Documentation, https://homonim.readthedocs.io
-Project-URL: Source, https://github.com/dugalh/homonim
+Project-URL: Source, https://github.com/leftfield-geospatial/homonim
 Keywords: drone imagery,aerial imagery,satellite imagery,surface reflectance,correction,harmonization,anisotropy,brdf,atmospheric correction
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |Tests| |codecov| |PyPI version| |conda-forge version| |docs| |License: AGPL v3|
 
 homonim
 =======
 
-.. image:: https://raw.githubusercontent.com/dugalh/homonim/main/docs/readme_eg.webp
+.. image:: https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/docs/readme_eg.webp
    :alt: example
 
 
 .. short_descr_start
 
 Correct aerial and satellite imagery to surface reflectance.
 
@@ -135,19 +135,19 @@
 .. code:: python
 
     from pathlib import Path
     from homonim import RasterFuse, RasterCompare, Model
 
     # urls of source and reference test images
     src_file = (
-        'https://raw.githubusercontent.com/dugalh/homonim/main/'
+        'https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/'
         'tests/data/source/ngi_rgb_byte_1.tif'
     )
     ref_file = (
-        'https://raw.githubusercontent.com/dugalh/homonim/main/'
+        'https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/'
         'tests/data/reference/sentinel2_b432_byte.tif'
     )
 
     # path to corrected file to create
     corr_file = './corrected.tif'
 
     # Correct src_file to surface reflectance by fusion with ref_file, using the
@@ -156,15 +156,15 @@
         fuse.process(corr_file, Model.gain_blk_offset, (5, 5), overwrite=True)
 
 .. api_example_end
 
 Reference imagery
 ~~~~~~~~~~~~~~~~~
 
-`geedim <https://github.com/dugalh/geedim>`_ can be used as a companion tool for searching and downloading cloud-free reference imagery.   Alternatively, satellite imagery is available from a number of sources, including the `Google <https://developers.google.com/earth-engine/datasets>`_, `Amazon <https://aws.amazon.com/earth/>`_ and `Microsoft <https://planetarycomputer.microsoft.com/catalog>`_ repositories.
+`geedim <https://github.com/leftfield-geospatial/geedim>`_ can be used as a companion tool for searching and downloading cloud-free reference imagery.   Alternatively, satellite imagery is available from a number of sources, including the `Google <https://developers.google.com/earth-engine/datasets>`_, `Amazon <https://aws.amazon.com/earth/>`_ and `Microsoft <https://planetarycomputer.microsoft.com/catalog>`_ repositories.
 
 
 Usage
 -----
 
 See the documentation `here <https://homonim.readthedocs.io/>`_.
 
@@ -206,18 +206,18 @@
         year  = {2019},
         publisher = {Taylor & Francis},
         doi = {10.1080/01431161.2018.1528404},
         URL = {https://doi.org/10.1080/01431161.2018.1528404},
     }
 
 
-.. |Tests| image:: https://github.com/dugalh/homonim/actions/workflows/run-unit-tests.yml/badge.svg
-   :target: https://github.com/dugalh/homonim/actions/workflows/run-unit-tests.yml
-.. |codecov| image:: https://codecov.io/gh/dugalh/homonim/branch/main/graph/badge.svg?token=A01698K96C
-   :target: https://codecov.io/gh/dugalh/homonim
+.. |Tests| image:: https://github.com/leftfield-geospatial/homonim/actions/workflows/run-unit-tests.yml/badge.svg
+   :target: https://github.com/leftfield-geospatial/homonim/actions/workflows/run-unit-tests.yml
+.. |codecov| image:: https://codecov.io/gh/leftfield-geospatial/homonim/branch/main/graph/badge.svg?token=A01698K96C
+   :target: https://codecov.io/gh/leftfield-geospatial/homonim
 .. |License: AGPL v3| image:: https://img.shields.io/badge/License-AGPL_v3-blue.svg
    :target: https://www.gnu.org/licenses/agpl-3.0
 .. |PyPI version| image:: https://img.shields.io/pypi/v/homonim?color=blue
    :target: https://pypi.org/project/homonim/
 .. |conda-forge version| image:: https://img.shields.io/conda/vn/conda-forge/homonim.svg?color=blue
    :alt: conda-forge
    :target: https://anaconda.org/conda-forge/homonim
```

### Comparing `homonim-0.3.1/setup.py` & `homonim-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     name='homonim',
     version=__version__,
     description='Correct aerial and satellite imagery to surface reflectance.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Dugal Harris',
     author_email='dugalh@gmail.com',
-    url='https://github.com/dugalh/homonim',
+    url='https://github.com/leftfield-geospatial/homonim',
     license='AGPLv3',
     packages=find_packages(include=['homonim']),
     install_requires=[
         'numpy>=1.19',
         'rasterio>=1.1',
         'opencv-python-headless>=4.5',
         'click>=8',
@@ -69,10 +69,10 @@
     keywords=[
         'drone imagery', 'aerial imagery', 'satellite imagery', 'surface reflectance', 'correction', 'harmonization',
         'anisotropy', 'brdf', 'atmospheric correction',
     ],
     entry_points={'console_scripts': ['homonim=homonim.cli:cli']},
     project_urls={
         'Documentation': 'https://homonim.readthedocs.io',
-        'Source': 'https://github.com/dugalh/homonim',
+        'Source': 'https://github.com/leftfield-geospatial/homonim',
     },
 )  # yapf: disable
```

