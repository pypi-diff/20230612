# Comparing `tmp/datashader-cli-0.0.2.tar.gz` & `tmp/datashader-cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datashader-cli-0.0.2.tar", last modified: Mon Jun 12 16:26:19 2023, max compression
+gzip compressed data, was "datashader-cli-0.0.4.tar", last modified: Mon Jun 12 16:56:57 2023, max compression
```

## Comparing `datashader-cli-0.0.2.tar` & `datashader-cli-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 16:26:19.226979 datashader-cli-0.0.2/
--rw-r--r--   0 kang       (501) staff       (20)     1070 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/LICENSE
--rw-r--r--   0 kang       (501) staff       (20)      122 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/MANIFEST.in
--rw-r--r--   0 kang       (501) staff       (20)     5228 2023-06-12 16:26:19.227051 datashader-cli-0.0.2/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     4472 2023-06-12 15:51:59.000000 datashader-cli-0.0.2/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 16:26:19.225486 datashader-cli-0.0.2/datashader_cli/
--rw-r--r--   0 kang       (501) staff       (20)      129 2023-06-12 16:26:13.000000 datashader-cli-0.0.2/datashader_cli/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)     7568 2023-06-12 16:21:20.000000 datashader-cli-0.0.2/datashader_cli/cli.py
--rw-r--r--   0 kang       (501) staff       (20)      188 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/datashader_cli/common.py
--rw-r--r--   0 kang       (501) staff       (20)       19 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/datashader_cli/datashader_cli.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 16:26:19.226614 datashader-cli-0.0.2/datashader_cli.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)     5228 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      468 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)       53 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       59 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/entry_points.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-12 05:03:02.000000 datashader-cli-0.0.2/datashader_cli.egg-info/not-zip-safe
--rw-r--r--   0 kang       (501) staff       (20)       53 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/requires.txt
--rw-r--r--   0 kang       (501) staff       (20)       15 2023-06-12 16:26:19.000000 datashader-cli-0.0.2/datashader_cli.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       52 2023-06-12 05:11:48.000000 datashader-cli-0.0.2/requirements.txt
--rw-r--r--   0 kang       (501) staff       (20)      456 2023-06-12 16:26:19.227313 datashader-cli-0.0.2/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)     1910 2023-06-12 16:26:13.000000 datashader-cli-0.0.2/setup.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-12 16:26:19.226744 datashader-cli-0.0.2/tests/
--rw-r--r--   0 kang       (501) staff       (20)     1014 2023-06-12 04:59:03.000000 datashader-cli-0.0.2/tests/test_datashader_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:56:57.206232 datashader-cli-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 16:56:43.000000 datashader-cli-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-12 16:56:43.000000 datashader-cli-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-12 16:56:57.206232 datashader-cli-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-12 16:56:43.000000 datashader-cli-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:56:57.206232 datashader-cli-0.0.4/datashader_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-12 16:56:43.000000 datashader-cli-0.0.4/datashader_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-12 16:56:43.000000 datashader-cli-0.0.4/datashader_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 16:56:43.000000 datashader-cli-0.0.4/datashader_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 16:56:43.000000 datashader-cli-0.0.4/datashader_cli/datashader_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:56:57.206232 datashader-cli-0.0.4/datashader_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-06-12 16:56:57.000000 datashader-cli-0.0.4/datashader_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-12 16:56:57.000000 datashader-cli-0.0.4/datashader_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 16:56:57.000000 datashader-cli-0.0.4/datashader_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-12 16:56:57.000000 datashader-cli-0.0.4/datashader_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:56:57.000000 datashader-cli-0.0.4/datashader_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 16:56:57.000000 datashader-cli-0.0.4/datashader_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 16:56:57.000000 datashader-cli-0.0.4/datashader_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 16:56:43.000000 datashader-cli-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-12 16:56:57.206232 datashader-cli-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-12 16:56:43.000000 datashader-cli-0.0.4/setup.py
```

### Comparing `datashader-cli-0.0.2/LICENSE` & `datashader-cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datashader-cli-0.0.2/PKG-INFO` & `datashader-cli-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datashader-cli
-Version: 0.0.2
+Version: 0.0.4
 Summary: Quick visualization of large datasets using CLI based on datashader.
 Home-page: https://github.com/wybert/datashader-cli
 Author: Xiaokang Fu
 Author-email: fxk123@gmail.com
 License: MIT license
 Keywords: datashader_cli
 Classifier: Intended Audience :: Developers
@@ -53,15 +53,15 @@
 ```bash
 datashader_cli points nyc_taxi.parquet --x pickup_x --y pickup_y pickup-scatter.png --background black
 
 ```
 
 ![](./docs/pickup-scatter.png)
 
-Visualize the geospaital data, support Geoparquet, shapefile, geojson, geopackage, etc.
+Visualize the geospaital data, support Geoparquet, Shapefile, Geojson, Geopackage, etc.
 
 
 ```bash
 datashader_cli points data.geo.parquet data.png --geo true
 ```
 
 ![](./docs/data1.png)
```

### Comparing `datashader-cli-0.0.2/README.md` & `datashader-cli-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ```bash
 datashader_cli points nyc_taxi.parquet --x pickup_x --y pickup_y pickup-scatter.png --background black
 
 ```
 
 ![](./docs/pickup-scatter.png)
 
-Visualize the geospaital data, support Geoparquet, shapefile, geojson, geopackage, etc.
+Visualize the geospaital data, support Geoparquet, Shapefile, Geojson, Geopackage, etc.
 
 
 ```bash
 datashader_cli points data.geo.parquet data.png --geo true
 ```
 
 ![](./docs/data1.png)
```

### Comparing `datashader-cli-0.0.2/datashader_cli/cli.py` & `datashader-cli-0.0.4/datashader_cli/cli.py`

 * *Files identical despite different names*

### Comparing `datashader-cli-0.0.2/datashader_cli.egg-info/PKG-INFO` & `datashader-cli-0.0.4/datashader_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datashader-cli
-Version: 0.0.2
+Version: 0.0.4
 Summary: Quick visualization of large datasets using CLI based on datashader.
 Home-page: https://github.com/wybert/datashader-cli
 Author: Xiaokang Fu
 Author-email: fxk123@gmail.com
 License: MIT license
 Keywords: datashader_cli
 Classifier: Intended Audience :: Developers
@@ -53,15 +53,15 @@
 ```bash
 datashader_cli points nyc_taxi.parquet --x pickup_x --y pickup_y pickup-scatter.png --background black
 
 ```
 
 ![](./docs/pickup-scatter.png)
 
-Visualize the geospaital data, support Geoparquet, shapefile, geojson, geopackage, etc.
+Visualize the geospaital data, support Geoparquet, Shapefile, Geojson, Geopackage, etc.
 
 
 ```bash
 datashader_cli points data.geo.parquet data.png --geo true
 ```
 
 ![](./docs/data1.png)
```

### Comparing `datashader-cli-0.0.2/setup.py` & `datashader-cli-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords='datashader_cli',
     name='datashader-cli',
     packages=find_packages(include=['datashader_cli', 'datashader_cli.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/wybert/datashader-cli',
-    version='0.0.2',
+    version='0.0.4',
     zip_safe=False,
 )
```

