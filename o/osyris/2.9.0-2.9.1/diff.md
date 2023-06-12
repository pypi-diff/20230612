# Comparing `tmp/osyris-2.9.0.tar.gz` & `tmp/osyris-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osyris-2.9.0.tar", last modified: Sat May 28 17:34:06 2022, max compression
+gzip compressed data, was "osyris-2.9.1.tar", last modified: Tue May 31 14:13:48 2022, max compression
```

## Comparing `osyris-2.9.0.tar` & `osyris-2.9.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 17:34:06.467310 osyris-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-05-28 17:29:50.000000 osyris-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-05-28 17:34:06.467310 osyris-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-05-28 17:29:50.000000 osyris-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-28 17:29:50.000000 osyris-2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-05-28 17:34:06.467310 osyris-2.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 17:34:06.459309 osyris-2.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 17:34:06.463310 osyris-2.9.0/src/osyris/
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 17:34:06.463310 osyris-2.9.0/src/osyris/config/
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/config/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 17:34:06.463310 osyris-2.9.0/src/osyris/core/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6898 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/core/array.py
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/core/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/core/datagroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3625 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/core/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     7780 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/core/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 17:34:06.463310 osyris-2.9.0/src/osyris/io/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8248 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/amr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/grav.py
--rw-r--r--   0 runner    (1001) docker     (121)     6418 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/hilbert.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/hydro.py
--rw-r--r--   0 runner    (1001) docker     (121)     9719 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2752 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/part.py
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/rt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/sink.py
--rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 17:34:06.467310 osyris-2.9.0/src/osyris/plot/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4506 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/direction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3813 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/histogram1d.py
--rw-r--r--   0 runner    (1001) docker     (121)     7891 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/histogram2d.py
--rw-r--r--   0 runner    (1001) docker     (121)    16677 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/map.py
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/plane.py
--rw-r--r--   0 runner    (1001) docker     (121)     4424 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/render.py
--rw-r--r--   0 runner    (1001) docker     (121)     4093 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3768 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8121 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/plot/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-05-28 17:29:50.000000 osyris-2.9.0/src/osyris/units.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 17:34:06.463310 osyris-2.9.0/src/osyris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-05-28 17:34:05.000000 osyris-2.9.0/src/osyris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-05-28 17:34:06.000000 osyris-2.9.0/src/osyris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-28 17:34:05.000000 osyris-2.9.0/src/osyris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-28 17:34:06.000000 osyris-2.9.0/src/osyris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-28 17:34:06.000000 osyris-2.9.0/src/osyris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 17:34:06.467310 osyris-2.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)    24157 2022-05-28 17:29:50.000000 osyris-2.9.0/test/test_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-05-28 17:29:50.000000 osyris-2.9.0/test/test_datagroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     4298 2022-05-28 17:29:50.000000 osyris-2.9.0/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    28469 2022-05-28 17:29:50.000000 osyris-2.9.0/test/test_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 14:13:48.703055 osyris-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-05-31 14:10:03.000000 osyris-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-05-31 14:13:48.703055 osyris-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-05-31 14:10:03.000000 osyris-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-31 14:10:03.000000 osyris-2.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-05-31 14:13:48.707054 osyris-2.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 14:13:48.699055 osyris-2.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 14:13:48.699055 osyris-2.9.1/src/osyris/
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 14:13:48.699055 osyris-2.9.1/src/osyris/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/config/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 14:13:48.703055 osyris-2.9.1/src/osyris/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6898 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/core/array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/core/datagroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3625 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/core/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7780 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/core/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 14:13:48.703055 osyris-2.9.1/src/osyris/io/
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8248 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/amr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/grav.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6418 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/hilbert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/hydro.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9719 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2752 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/part.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/rt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/sink.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 14:13:48.703055 osyris-2.9.1/src/osyris/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4506 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/direction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3813 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/histogram1d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7891 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/histogram2d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16677 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/plane.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4424 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4093 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3768 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8121 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/plot/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-05-31 14:10:03.000000 osyris-2.9.1/src/osyris/units.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 14:13:48.699055 osyris-2.9.1/src/osyris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-05-31 14:13:48.000000 osyris-2.9.1/src/osyris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-05-31 14:13:48.000000 osyris-2.9.1/src/osyris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 14:13:48.000000 osyris-2.9.1/src/osyris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-31 14:13:48.000000 osyris-2.9.1/src/osyris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-31 14:13:48.000000 osyris-2.9.1/src/osyris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 14:13:48.703055 osyris-2.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (121)    24157 2022-05-31 14:10:03.000000 osyris-2.9.1/test/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5804 2022-05-31 14:10:03.000000 osyris-2.9.1/test/test_datagroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4298 2022-05-31 14:10:03.000000 osyris-2.9.1/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28469 2022-05-31 14:10:03.000000 osyris-2.9.1/test/test_vector.py
```

### Comparing `osyris-2.9.0/LICENSE` & `osyris-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/PKG-INFO` & `osyris-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osyris
-Version: 2.9.0
+Version: 2.9.1
 Summary: A package to visualize AMR data from the RAMSES code
 Home-page: https://github.com/osyris-project/osyris
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 Project-URL: Bug Tracker, https://github.com/osyris-project/osyris/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `osyris-2.9.0/README.md` & `osyris-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/setup.cfg` & `osyris-2.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osyris
-version = 2.9.0
+version = 2.9.1
 author = Neil Vaytet
 author_email = neil.vaytet@esss.se
 description = A package to visualize AMR data from the RAMSES code
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/osyris-project/osyris
 project_urls =
```

### Comparing `osyris-2.9.0/src/osyris/config/__init__.py` & `osyris-2.9.1/src/osyris/config/__init__.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/config/defaults.py` & `osyris-2.9.1/src/osyris/config/defaults.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/core/array.py` & `osyris-2.9.1/src/osyris/core/array.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/core/base.py` & `osyris-2.9.1/src/osyris/core/base.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/core/datagroup.py` & `osyris-2.9.1/src/osyris/core/datagroup.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/core/dataset.py` & `osyris-2.9.1/src/osyris/core/dataset.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/core/tools.py` & `osyris-2.9.1/src/osyris/core/tools.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/core/vector.py` & `osyris-2.9.1/src/osyris/core/vector.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/io/amr.py` & `osyris-2.9.1/src/osyris/io/amr.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/io/grav.py` & `osyris-2.9.1/src/osyris/io/grav.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/io/hilbert.py` & `osyris-2.9.1/src/osyris/io/hilbert.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/io/hydro.py` & `osyris-2.9.1/src/osyris/io/hydro.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/io/loader.py` & `osyris-2.9.1/src/osyris/io/loader.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/io/part.py` & `osyris-2.9.1/src/osyris/io/part.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/io/reader.py` & `osyris-2.9.1/src/osyris/io/reader.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/io/rt.py` & `osyris-2.9.1/src/osyris/io/rt.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/io/sink.py` & `osyris-2.9.1/src/osyris/io/sink.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         t = units['time']  # noqa: F841
         for u in unit_combinations:
             if u.strip().replace("[", "").replace("]", "") == '1':
                 unit_list.append(1.0 * ureg('dimensionless'))
             else:
                 if all(x in u for x in ["[", "]"]):
                     # Legacy sink format quantities are not in code units
-                    unit_list.append(ureg(u.replace("[", "").replace("]", "")))
+                    unit_list.append(1.0 * ureg(u.replace("[", "").replace("]", "")))
                 else:
                     unit_list.append(eval(u.replace(' ', '*')))
 
         sink = Datagroup()
         for i, (key, unit) in enumerate(zip(key_list, unit_list)):
             sink[key] = Array(values=sink_data[:, i] * unit.magnitude, unit=unit.units)
         utils.make_vector_arrays(sink, ndim=meta["ndim"])
```

### Comparing `osyris-2.9.0/src/osyris/io/utils.py` & `osyris-2.9.1/src/osyris/io/utils.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/direction.py` & `osyris-2.9.1/src/osyris/plot/direction.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/histogram1d.py` & `osyris-2.9.1/src/osyris/plot/histogram1d.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/histogram2d.py` & `osyris-2.9.1/src/osyris/plot/histogram2d.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/map.py` & `osyris-2.9.1/src/osyris/plot/map.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/parser.py` & `osyris-2.9.1/src/osyris/plot/parser.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/plot.py` & `osyris-2.9.1/src/osyris/plot/plot.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/render.py` & `osyris-2.9.1/src/osyris/plot/render.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/scatter.py` & `osyris-2.9.1/src/osyris/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/utils.py` & `osyris-2.9.1/src/osyris/plot/utils.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/plot/wrappers.py` & `osyris-2.9.1/src/osyris/plot/wrappers.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris/units.py` & `osyris-2.9.1/src/osyris/units.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/src/osyris.egg-info/PKG-INFO` & `osyris-2.9.1/src/osyris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osyris
-Version: 2.9.0
+Version: 2.9.1
 Summary: A package to visualize AMR data from the RAMSES code
 Home-page: https://github.com/osyris-project/osyris
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 Project-URL: Bug Tracker, https://github.com/osyris-project/osyris/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `osyris-2.9.0/src/osyris.egg-info/SOURCES.txt` & `osyris-2.9.1/src/osyris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/test/test_array.py` & `osyris-2.9.1/test/test_array.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/test/test_datagroup.py` & `osyris-2.9.1/test/test_datagroup.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/test/test_dataset.py` & `osyris-2.9.1/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `osyris-2.9.0/test/test_vector.py` & `osyris-2.9.1/test/test_vector.py`

 * *Files identical despite different names*

