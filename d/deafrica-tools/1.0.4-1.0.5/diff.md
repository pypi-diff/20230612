# Comparing `tmp/deafrica-tools-1.0.4.tar.gz` & `tmp/deafrica-tools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deafrica-tools-1.0.4.tar", last modified: Mon Mar 27 07:54:24 2023, max compression
+gzip compressed data, was "deafrica-tools-1.0.5.tar", last modified: Mon Jun 12 14:48:47 2023, max compression
```

## Comparing `deafrica-tools-1.0.4.tar` & `deafrica-tools-1.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:54:24.877141 deafrica-tools-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-03-27 07:54:24.877141 deafrica-tools-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:54:24.873141 deafrica-tools-1.0.4/deafrica_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:54:24.877141 deafrica-tools-1.0.4/deafrica_tools/app/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31281 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/animations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/changefilmstrips.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/crophealth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/deacoastlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    37496 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/forestmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/geomedian.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/imageexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    12980 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/wetlandsinsighttool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/app/widgetconstructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/areaofinterest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24544 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/bandindices.py
--rw-r--r--   0 runner    (1001) docker     (123)    61473 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    23347 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/coastal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    35752 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/datahandling.py
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/load_era5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/load_isda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:54:24.873141 deafrica-tools-1.0.4/deafrica_tools/locales/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:54:24.873141 deafrica-tools-1.0.4/deafrica_tools/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:54:24.877141 deafrica-tools-1.0.4/deafrica_tools/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
--rw-r--r--   0 runner    (1001) docker     (123)    50494 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    36679 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)    25800 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/deafrica_tools/wetlands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 07:54:24.877141 deafrica-tools-1.0.4/deafrica_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-03-27 07:54:24.000000 deafrica-tools-1.0.4/deafrica_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-27 07:54:24.000000 deafrica-tools-1.0.4/deafrica_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 07:54:24.000000 deafrica-tools-1.0.4/deafrica_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-27 07:54:24.000000 deafrica-tools-1.0.4/deafrica_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 07:54:24.000000 deafrica-tools-1.0.4/deafrica_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 07:54:24.877141 deafrica-tools-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-03-27 07:54:06.000000 deafrica-tools-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.279860 deafrica-tools-1.0.5/deafrica_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/deafrica_tools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31281 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/changefilmstrips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/crophealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/deacoastlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37648 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/forestmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/geomedian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/imageexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12980 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/wetlandsinsighttool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/app/widgetconstructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/areaofinterest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/bandindices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61473 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23347 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/coastal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35752 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/datahandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/load_era5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/load_isda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.279860 deafrica-tools-1.0.5/deafrica_tools/locales/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.279860 deafrica-tools-1.0.5/deafrica_tools/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
+-rw-r--r--   0 runner    (1001) docker     (123)    50494 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36679 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25800 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/deafrica_tools/wetlands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:47.279860 deafrica-tools-1.0.5/deafrica_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 14:48:47.000000 deafrica-tools-1.0.5/deafrica_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:48:47.283860 deafrica-tools-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-12 14:48:26.000000 deafrica-tools-1.0.5/setup.py
```

### Comparing `deafrica-tools-1.0.4/LICENSE` & `deafrica-tools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/PKG-INFO` & `deafrica-tools-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deafrica-tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: Functions and algorithms for analysing Digital Earth Africa data.
 Home-page: https://github.com/digitalearthafrica/deafrica-sandbox-notebooks
 Author: Digital Earth Africa
 Author-email: systems@digitalearthafrica.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/digitalearthafrica/deafrica-sandbox-notebooks/issues
 Requires-Python: >=3.6.0
```

### Comparing `deafrica-tools-1.0.4/README.md` & `deafrica-tools-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/__init__.py` & `deafrica-tools-1.0.5/deafrica_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 __locales__ = __path__[0] + '/locales'
 
 
 def set_lang(lang=None):
     if lang is None:
         import os
```

### Comparing `deafrica-tools-1.0.4/deafrica_tools/app/animations.py` & `deafrica-tools-1.0.5/deafrica_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/app/changefilmstrips.py` & `deafrica-tools-1.0.5/deafrica_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/app/crophealth.py` & `deafrica-tools-1.0.5/deafrica_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/app/deacoastlines.py` & `deafrica-tools-1.0.5/deafrica_tools/app/deacoastlines.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/app/forestmonitoring.py` & `deafrica-tools-1.0.5/deafrica_tools/app/forestmonitoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+'''
+Functions for loading and interacting with Global Forest Change data in the forest monitoring notebook, inside the Real_world_examples folder.
+'''
+
 import json
 import warnings
 from io import BytesIO
 
 import deafrica_tools.app.widgetconstructors as deawidgets
 import geopandas as gpd
 import ipywidgets as widgets
```

### Comparing `deafrica-tools-1.0.4/deafrica_tools/app/geomedian.py` & `deafrica-tools-1.0.5/deafrica_tools/app/geomedian.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/app/imageexport.py` & `deafrica-tools-1.0.5/deafrica_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/app/wetlandsinsighttool.py` & `deafrica-tools-1.0.5/deafrica_tools/app/wetlandsinsighttool.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/app/widgetconstructors.py` & `deafrica-tools-1.0.5/deafrica_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/areaofinterest.py` & `deafrica-tools-1.0.5/deafrica_tools/areaofinterest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Function for defining an area of interest using either a point and buffer or a shapefile file. 
+"""
+
 import geopandas as gpd
 from shapely.geometry import box
 from geojson import Feature, Point, FeatureCollection
 
 def define_area(lat=None, lon=None, buffer=None, shapefile_path=None):
     '''
     Define an area of interest using either a point and buffer or a shapefile.
```

### Comparing `deafrica-tools-1.0.4/deafrica_tools/bandindices.py` & `deafrica-tools-1.0.5/deafrica_tools/bandindices.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,20 +137,20 @@
 
     # Dictionary containing remote sensing index band recipes
     index_dict = {
         # Normalised Difference Vegation Index, Rouse 1973
         "NDVI": lambda ds: (ds.nir - ds.red) / (ds.nir + ds.red),
         # Enhanced Vegetation Index, Huete 2002
         "EVI": lambda ds: (
-            (2.5 * (ds.nir - ds.red)) / (ds.nir + 6 * ds.red - 7.5 * ds.blue + 1)
+            2.5 * ((ds.nir - ds.red) / (ds.nir + 6 * ds.red - 7.5 * ds.blue + 1))
         ),
         # Leaf Area Index, Boegh 2002
         "LAI": lambda ds: (
             3.618
-            * ((2.5 * (ds.nir - ds.red)) / (ds.nir + 6 * ds.red - 7.5 * ds.blue + 1))
+            * ((2.5 * (ds.nir - ds.red)) / (ds.nir + (6 * ds.red) - (7.5 * ds.blue) + 1))
             - 0.118
         ),
         # Soil Adjusted Vegetation Index, Huete 1988
         "SAVI": lambda ds: ((1.5 * (ds.nir - ds.red)) / (ds.nir + ds.red + 0.5)),
         # Mod. Soil Adjusted Vegetation Index, Qi et al. 1994
         "MSAVI": lambda ds: (
             (2 * ds.nir + 1 - ((2 * ds.nir + 1) ** 2 - 8 * (ds.nir - ds.red)) ** 0.5)
```

### Comparing `deafrica-tools-1.0.4/deafrica_tools/classification.py` & `deafrica-tools-1.0.5/deafrica_tools/classification.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/coastal.py` & `deafrica-tools-1.0.5/deafrica_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/dask.py` & `deafrica-tools-1.0.5/deafrica_tools/dask.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/datahandling.py` & `deafrica-tools-1.0.5/deafrica_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/load_era5.py` & `deafrica-tools-1.0.5/deafrica_tools/load_era5.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/load_isda.py` & `deafrica-tools-1.0.5/deafrica_tools/load_isda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Functions to retrieve iSDAsoil data.
+"""
+
 import numpy as np
 import pandas as pd
 import xarray as xr
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 import rasterio as rio
 from pyproj import Transformer
```

### Comparing `deafrica-tools-1.0.4/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo` & `deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po` & `deafrica-tools-1.0.5/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/plotting.py` & `deafrica-tools-1.0.5/deafrica_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/spatial.py` & `deafrica-tools-1.0.5/deafrica_tools/spatial.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/temporal.py` & `deafrica-tools-1.0.5/deafrica_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools/wetlands.py` & `deafrica-tools-1.0.5/deafrica_tools/wetlands.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/deafrica_tools.egg-info/PKG-INFO` & `deafrica-tools-1.0.5/deafrica_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deafrica-tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: Functions and algorithms for analysing Digital Earth Africa data.
 Home-page: https://github.com/digitalearthafrica/deafrica-sandbox-notebooks
 Author: Digital Earth Africa
 Author-email: systems@digitalearthafrica.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/digitalearthafrica/deafrica-sandbox-notebooks/issues
 Requires-Python: >=3.6.0
```

### Comparing `deafrica-tools-1.0.4/deafrica_tools.egg-info/SOURCES.txt` & `deafrica-tools-1.0.5/deafrica_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/pyproject.toml` & `deafrica-tools-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deafrica-tools-1.0.4/setup.py` & `deafrica-tools-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 EXTRAS = {
     'jupyter': ['IPython', 'ipywidgets', 'ipyleaflet'],
     'boto': ['boto3'],
 }
 
 # Package meta-data.
 NAME = 'deafrica-tools'
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 DESCRIPTION = 'Functions and algorithms for analysing Digital Earth Africa data.'
 # Set the value of long_description to the contents (not the path) of the README file itself.
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / 'README.md').read_text()
 # Set the long_description_content_type to an accepted Content-Type-style value for your README file’s markup.
 LONG_DESCRIPTION_CONTENT_TYPE = 'text/markdown'
 AUTHOR = 'Digital Earth Africa'
```

