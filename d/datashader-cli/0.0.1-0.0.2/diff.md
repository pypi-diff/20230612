# Comparing `tmp/datashader-cli-0.0.1.tar.gz` & `tmp/datashader-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datashader-cli-0.0.1.tar", last modified: Mon Jun 12 15:32:54 2023, max compression
+gzip compressed data, was "datashader-cli-0.0.2.tar", last modified: Mon Jun 12 16:26:19 2023, max compression
```

## Comparing `datashader-cli-0.0.1.tar` & `datashader-cli-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 15:32:54.528507 datashader-cli-0.0.1/
--rw-r--r--   0 kang       (501) staff       (20)     1070 2023-06-12 04:59:03.000000 datashader-cli-0.0.1/LICENSE
--rw-r--r--   0 kang       (501) staff       (20)      122 2023-06-12 04:59:03.000000 datashader-cli-0.0.1/MANIFEST.in
--rw-r--r--   0 kang       (501) staff       (20)     5148 2023-06-12 15:32:54.528582 datashader-cli-0.0.1/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     4392 2023-06-12 15:20:52.000000 datashader-cli-0.0.1/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 15:32:54.527030 datashader-cli-0.0.1/datashader_cli/
--rw-r--r--   0 kang       (501) staff       (20)      129 2023-06-12 04:59:03.000000 datashader-cli-0.0.1/datashader_cli/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)     7050 2023-06-12 14:55:16.000000 datashader-cli-0.0.1/datashader_cli/cli.py
--rw-r--r--   0 kang       (501) staff       (20)      188 2023-06-12 04:59:03.000000 datashader-cli-0.0.1/datashader_cli/common.py
--rw-r--r--   0 kang       (501) staff       (20)       19 2023-06-12 04:59:03.000000 datashader-cli-0.0.1/datashader_cli/datashader_cli.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 15:32:54.528163 datashader-cli-0.0.1/datashader_cli.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)     5148 2023-06-12 15:32:54.000000 datashader-cli-0.0.1/datashader_cli.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      468 2023-06-12 15:32:54.000000 datashader-cli-0.0.1/datashader_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)       53 2023-06-12 15:32:54.000000 datashader-cli-0.0.1/datashader_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       59 2023-06-12 15:32:54.000000 datashader-cli-0.0.1/datashader_cli.egg-info/entry_points.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-12 05:03:02.000000 datashader-cli-0.0.1/datashader_cli.egg-info/not-zip-safe
--rw-r--r--   0 kang       (501) staff       (20)       53 2023-06-12 15:32:54.000000 datashader-cli-0.0.1/datashader_cli.egg-info/requires.txt
--rw-r--r--   0 kang       (501) staff       (20)       15 2023-06-12 15:32:54.000000 datashader-cli-0.0.1/datashader_cli.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       52 2023-06-12 05:11:48.000000 datashader-cli-0.0.1/requirements.txt
--rw-r--r--   0 kang       (501) staff       (20)      456 2023-06-12 15:32:54.528839 datashader-cli-0.0.1/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)     1910 2023-06-12 04:59:03.000000 datashader-cli-0.0.1/setup.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 15:32:54.528292 datashader-cli-0.0.1/tests/
--rw-r--r--   0 kang       (501) staff       (20)     1014 2023-06-12 04:59:03.000000 datashader-cli-0.0.1/tests/test_datashader_cli.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 16:26:19.226979 datashader-cli-0.0.2/
+-rw-r--r--   0 kang       (501) staff       (20)     1070 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/LICENSE
+-rw-r--r--   0 kang       (501) staff       (20)      122 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/MANIFEST.in
+-rw-r--r--   0 kang       (501) staff       (20)     5228 2023-06-12 16:26:19.227051 datashader-cli-0.0.2/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     4472 2023-06-12 15:51:59.000000 datashader-cli-0.0.2/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 16:26:19.225486 datashader-cli-0.0.2/datashader_cli/
+-rw-r--r--   0 kang       (501) staff       (20)      129 2023-06-12 16:26:13.000000 datashader-cli-0.0.2/datashader_cli/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)     7568 2023-06-12 16:21:20.000000 datashader-cli-0.0.2/datashader_cli/cli.py
+-rw-r--r--   0 kang       (501) staff       (20)      188 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/datashader_cli/common.py
+-rw-r--r--   0 kang       (501) staff       (20)       19 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/datashader_cli/datashader_cli.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 16:26:19.226614 datashader-cli-0.0.2/datashader_cli.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)     5228 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      468 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)       53 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       59 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/entry_points.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-12 05:03:02.000000 datashader-cli-0.0.2/datashader_cli.egg-info/not-zip-safe
+-rw-r--r--   0 kang       (501) staff       (20)       53 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/requires.txt
+-rw-r--r--   0 kang       (501) staff       (20)       15 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       52 2023-06-12 05:11:48.000000 datashader-cli-0.0.2/requirements.txt
+-rw-r--r--   0 kang       (501) staff       (20)      456 2023-06-12 16:26:19.227313 datashader-cli-0.0.2/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)     1910 2023-06-12 16:26:13.000000 datashader-cli-0.0.2/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 16:26:19.226744 datashader-cli-0.0.2/tests/
+-rw-r--r--   0 kang       (501) staff       (20)     1014 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/tests/test_datashader_cli.py
```

### Comparing `datashader-cli-0.0.1/LICENSE` & `datashader-cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datashader-cli-0.0.1/PKG-INFO` & `datashader-cli-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datashader-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Quick visualization of large datasets using CLI based on datashader.
 Home-page: https://github.com/wybert/datashader-cli
 Author: Xiaokang Fu
 Author-email: fxk123@gmail.com
 License: MIT license
 Keywords: datashader_cli
 Classifier: Intended Audience :: Developers
@@ -28,14 +28,22 @@
 [![image](https://pyup.io/repos/github/wybert/datashader-cli/shield.svg)](https://pyup.io/repos/github/wybert/datashader-cli)
 
 
 **Quick visualization of large datasets using CLI based on [datashader](https://github.com/holoviz/datashader).**
 
 ## Installation
 
+### Use pip
+
+````bash
+pip install datashader-cli
+````
+
+### Use pip from Github
+
 ```bash
 pip install git+https://github.com/wybert/datashader-cli.git
 ```
 
 ## Quick Start
 
 Visualize 10 million NYC taxi trip data points in Gigabytes.
```

### Comparing `datashader-cli-0.0.1/README.md` & `datashader-cli-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 [![image](https://pyup.io/repos/github/wybert/datashader-cli/shield.svg)](https://pyup.io/repos/github/wybert/datashader-cli)
 
 
 **Quick visualization of large datasets using CLI based on [datashader](https://github.com/holoviz/datashader).**
 
 ## Installation
 
+### Use pip
+
+````bash
+pip install datashader-cli
+````
+
+### Use pip from Github
+
 ```bash
 pip install git+https://github.com/wybert/datashader-cli.git
 ```
 
 ## Quick Start
 
 Visualize 10 million NYC taxi trip data points in Gigabytes.
```

### Comparing `datashader-cli-0.0.1/datashader_cli/cli.py` & `datashader-cli-0.0.2/datashader_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,31 @@
 import datetime
 import colorcet as cc
 import sys
 
 
 @click.group()
 def main(args=None):
-    """Quick visualization of large datasets using CLI based on datashader.
+    """Quick visualization of large datasets using CLI based on datashader. Supported data format: csv, parquet, hdf, feather, geoparquet, shapefile, geojson, geopackage, etc.
     
-    Supported data format: csv, parquet, hdf, feather, geoparquet, shapefile, geojson, geopackage, etc.
+    Examples:
+
+    1. Create a shaded scatter plot of points and save it to png file, set background color to black.
+    
+    `datashader_cli points nyc_taxi.parquet --x pickup_x --y pickup_y pickup-scatter.png --background black`
+
+    2. Visualize the geospaital data, support Geoparquet, shapefile, geojson, geopackage, etc.
+
+    `datashader_cli points data.geo.parquet data.png --geo true`
+
+    3. Use matplotlib to render the image
+
+    `datashader_cli points data.geo.parquet data.png --geo true --matplotlib true`
+
+
     """
     
     return 0
 
 
 
 # Define a command
```

### Comparing `datashader-cli-0.0.1/datashader_cli.egg-info/PKG-INFO` & `datashader-cli-0.0.2/datashader_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datashader-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Quick visualization of large datasets using CLI based on datashader.
 Home-page: https://github.com/wybert/datashader-cli
 Author: Xiaokang Fu
 Author-email: fxk123@gmail.com
 License: MIT license
 Keywords: datashader_cli
 Classifier: Intended Audience :: Developers
@@ -28,14 +28,22 @@
 [![image](https://pyup.io/repos/github/wybert/datashader-cli/shield.svg)](https://pyup.io/repos/github/wybert/datashader-cli)
 
 
 **Quick visualization of large datasets using CLI based on [datashader](https://github.com/holoviz/datashader).**
 
 ## Installation
 
+### Use pip
+
+````bash
+pip install datashader-cli
+````
+
+### Use pip from Github
+
 ```bash
 pip install git+https://github.com/wybert/datashader-cli.git
 ```
 
 ## Quick Start
 
 Visualize 10 million NYC taxi trip data points in Gigabytes.
```

### Comparing `datashader-cli-0.0.1/setup.py` & `datashader-cli-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords='datashader_cli',
     name='datashader-cli',
     packages=find_packages(include=['datashader_cli', 'datashader_cli.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/wybert/datashader-cli',
-    version='0.0.1',
+    version='0.0.2',
     zip_safe=False,
 )
```

### Comparing `datashader-cli-0.0.1/tests/test_datashader_cli.py` & `datashader-cli-0.0.2/tests/test_datashader_cli.py`

 * *Files identical despite different names*

