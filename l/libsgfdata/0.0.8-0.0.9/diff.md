# Comparing `tmp/libsgfdata-0.0.8.tar.gz` & `tmp/libsgfdata-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libsgfdata-0.0.8.tar", last modified: Mon Aug 23 12:12:11 2021, max compression
+gzip compressed data, was "dist/libsgfdata-0.0.9.tar", last modified: Fri Oct 15 15:12:23 2021, max compression
```

## Comparing `libsgfdata-0.0.8.tar` & `libsgfdata-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-08-23 12:12:11.510068 libsgfdata-0.0.8/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2021-07-16 11:21:38.000000 libsgfdata-0.0.8/LICENSE
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       16 2021-07-16 11:18:49.000000 libsgfdata-0.0.8/MANIFEST.in
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      566 2021-08-23 12:12:11.510068 libsgfdata-0.0.8/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1926 2021-08-13 14:03:26.000000 libsgfdata-0.0.8/README.md
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-08-23 12:12:11.510068 libsgfdata-0.0.8/libsgfdata/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)    12392 2021-08-20 14:47:43.000000 libsgfdata-0.0.8/libsgfdata/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     3328 2021-07-16 10:58:30.000000 libsgfdata-0.0.8/libsgfdata/comments.csv
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      138 2021-08-13 16:17:30.000000 libsgfdata-0.0.8/libsgfdata/data-flags.csv
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     4026 2021-08-20 14:47:43.000000 libsgfdata-0.0.8/libsgfdata/data.csv
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1402 2021-08-13 14:03:26.000000 libsgfdata-0.0.8/libsgfdata/main.csv
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2535 2021-07-16 10:58:30.000000 libsgfdata-0.0.8/libsgfdata/method.csv
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     6505 2021-08-20 14:47:43.000000 libsgfdata-0.0.8/libsgfdata/methods.csv
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-08-23 12:12:11.510068 libsgfdata-0.0.8/libsgfdata.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      566 2021-08-23 12:12:11.000000 libsgfdata-0.0.8/libsgfdata.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      365 2021-08-23 12:12:11.000000 libsgfdata-0.0.8/libsgfdata.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2021-08-23 12:12:11.000000 libsgfdata-0.0.8/libsgfdata.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       44 2021-08-23 12:12:11.000000 libsgfdata-0.0.8/libsgfdata.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       11 2021-08-23 12:12:11.000000 libsgfdata-0.0.8/libsgfdata.egg-info/top_level.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2021-08-23 12:12:11.510068 libsgfdata-0.0.8/setup.cfg
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      866 2021-08-23 12:11:33.000000 libsgfdata-0.0.8/setup.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-10-15 15:12:23.093156 libsgfdata-0.0.9/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1077 2021-07-16 11:21:38.000000 libsgfdata-0.0.9/LICENSE
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       16 2021-07-16 11:18:49.000000 libsgfdata-0.0.9/MANIFEST.in
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      566 2021-10-15 15:12:23.093156 libsgfdata-0.0.9/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6427 2021-10-15 14:39:12.000000 libsgfdata-0.0.9/README.md
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-10-15 15:12:23.093156 libsgfdata-0.0.9/libsgfdata/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      145 2021-10-15 14:39:12.000000 libsgfdata-0.0.9/libsgfdata/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     3328 2021-07-16 10:58:30.000000 libsgfdata-0.0.9/libsgfdata/comments.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      138 2021-08-13 16:17:30.000000 libsgfdata-0.0.9/libsgfdata/data-flags.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     4821 2021-10-15 14:39:12.000000 libsgfdata-0.0.9/libsgfdata/data.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     4701 2021-10-15 14:47:01.000000 libsgfdata-0.0.9/libsgfdata/dumper.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1774 2021-10-15 14:39:12.000000 libsgfdata-0.0.9/libsgfdata/main.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     4111 2021-10-15 15:09:24.000000 libsgfdata-0.0.9/libsgfdata/metadata.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2957 2021-10-15 14:39:12.000000 libsgfdata-0.0.9/libsgfdata/method.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6505 2021-08-20 14:47:43.000000 libsgfdata-0.0.9/libsgfdata/methods.csv
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      810 2021-10-15 14:39:12.000000 libsgfdata-0.0.9/libsgfdata/normalizer.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     5782 2021-10-15 14:45:20.000000 libsgfdata-0.0.9/libsgfdata/parser.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2021-10-15 15:12:23.093156 libsgfdata-0.0.9/libsgfdata.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      566 2021-10-15 15:12:23.000000 libsgfdata-0.0.9/libsgfdata.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      455 2021-10-15 15:12:23.000000 libsgfdata-0.0.9/libsgfdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2021-10-15 15:12:23.000000 libsgfdata-0.0.9/libsgfdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       53 2021-10-15 15:12:23.000000 libsgfdata-0.0.9/libsgfdata.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       11 2021-10-15 15:12:23.000000 libsgfdata-0.0.9/libsgfdata.egg-info/top_level.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2021-10-15 15:12:23.093156 libsgfdata-0.0.9/setup.cfg
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      885 2021-10-15 15:11:31.000000 libsgfdata-0.0.9/setup.py
```

### Comparing `libsgfdata-0.0.8/LICENSE` & `libsgfdata-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libsgfdata-0.0.8/PKG-INFO` & `libsgfdata-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsgfdata
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parser for Swedish Geotechnical Society data format
 Home-page: https://github.com/emerald-geomodelling/libsgfdata
 Author: Egil Moeller
 Author-email: em@emeraldgeo.no
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `libsgfdata-0.0.8/libsgfdata/comments.csv` & `libsgfdata-0.0.9/libsgfdata/comments.csv`

 * *Files identical despite different names*

### Comparing `libsgfdata-0.0.8/libsgfdata/methods.csv` & `libsgfdata-0.0.9/libsgfdata/methods.csv`

 * *Files identical despite different names*

### Comparing `libsgfdata-0.0.8/libsgfdata.egg-info/PKG-INFO` & `libsgfdata-0.0.9/libsgfdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsgfdata
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parser for Swedish Geotechnical Society data format
 Home-page: https://github.com/emerald-geomodelling/libsgfdata
 Author: Egil Moeller
 Author-email: em@emeraldgeo.no
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `libsgfdata-0.0.8/setup.py` & `libsgfdata-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 import os
 
 setuptools.setup(
     name='libsgfdata',
-    version='0.0.8',
+    version='0.0.9',
     description='Parser for Swedish Geotechnical Society data format',
     long_description="""Parser for data from geotechnical field
     investigations in the data format specified in Report 3:2012E from
     the Swedish Geotechnical Society, see
     http://www.sgf.net/web/page.aspx?refid=2678 for how to download
     this report.""",
     long_description_content_type="text/markdown",
@@ -20,9 +20,10 @@
     include_package_data=True,
     package_data={'libsgfdata': ['*/*.csv']},
     install_requires=[
         "numpy",
         "pandas",
         "python-slugify",
         "python-dateutil",
+        "cchardet"
     ],
 )
```

