# Comparing `tmp/CalibrationCurve-0.0.1.tar.gz` & `tmp/CalibrationCurve-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalibrationCurve-0.0.1.tar", last modified: Mon Jun 12 06:46:31 2023, max compression
+gzip compressed data, was "CalibrationCurve-0.0.2.tar", last modified: Mon Jun 12 10:19:43 2023, max compression
```

## Comparing `CalibrationCurve-0.0.1.tar` & `CalibrationCurve-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-12 06:46:31.561844 CalibrationCurve-0.0.1/
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-12 06:46:31.561844 CalibrationCurve-0.0.1/CalibrationCurve/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-12 06:41:55.000000 CalibrationCurve-0.0.1/CalibrationCurve/__init__.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4659 2023-06-12 06:41:55.000000 CalibrationCurve-0.0.1/CalibrationCurve/_modidx.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4448 2023-06-12 06:41:55.000000 CalibrationCurve-0.0.1/CalibrationCurve/core.py
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-12 06:46:31.561844 CalibrationCurve-0.0.1/CalibrationCurve.egg-info/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-12 06:46:31.000000 CalibrationCurve-0.0.1/CalibrationCurve.egg-info/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-12 06:46:31.000000 CalibrationCurve-0.0.1/CalibrationCurve.egg-info/SOURCES.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-12 06:46:31.000000 CalibrationCurve-0.0.1/CalibrationCurve.egg-info/dependency_links.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-12 06:46:31.000000 CalibrationCurve-0.0.1/CalibrationCurve.egg-info/entry_points.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-12 05:51:02.000000 CalibrationCurve-0.0.1/CalibrationCurve.egg-info/not-zip-safe
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       73 2023-06-12 06:46:31.000000 CalibrationCurve-0.0.1/CalibrationCurve.egg-info/requires.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-12 06:46:31.000000 CalibrationCurve-0.0.1/CalibrationCurve.egg-info/top_level.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 05:47:40.000000 CalibrationCurve-0.0.1/LICENSE
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.1/MANIFEST.in
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-12 06:46:31.561844 CalibrationCurve-0.0.1/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      225 2023-06-12 06:41:58.000000 CalibrationCurve-0.0.1/README.md
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1094 2023-06-12 06:41:46.000000 CalibrationCurve-0.0.1/settings.ini
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-12 06:46:31.561844 CalibrationCurve-0.0.1/setup.cfg
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.1/setup.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/CalibrationCurve/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-12 06:41:55.000000 CalibrationCurve-0.0.2/CalibrationCurve/__init__.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4659 2023-06-12 06:41:55.000000 CalibrationCurve-0.0.2/CalibrationCurve/_modidx.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4448 2023-06-12 06:41:55.000000 CalibrationCurve-0.0.2/CalibrationCurve/core.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/SOURCES.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/dependency_links.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/entry_points.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-12 05:51:02.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/not-zip-safe
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/requires.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/top_level.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 05:47:40.000000 CalibrationCurve-0.0.2/LICENSE
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.2/MANIFEST.in
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      225 2023-06-12 06:41:58.000000 CalibrationCurve-0.0.2/README.md
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1087 2023-06-12 10:19:40.000000 CalibrationCurve-0.0.2/settings.ini
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/setup.cfg
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.2/setup.py
```

### Comparing `CalibrationCurve-0.0.1/CalibrationCurve/_modidx.py` & `CalibrationCurve-0.0.2/CalibrationCurve/_modidx.py`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.1/CalibrationCurve/core.py` & `CalibrationCurve-0.0.2/CalibrationCurve/core.py`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.1/CalibrationCurve.egg-info/PKG-INFO` & `CalibrationCurve-0.0.2/CalibrationCurve.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.1/LICENSE` & `CalibrationCurve-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.1/PKG-INFO` & `CalibrationCurve-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalibrationCurve
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of functions that streamline the process of creating calibration curves using Python.
 Home-page: https://github.com/Rhys-McAlister/CalibrationCurve
 Author: Rhys McAlister
 Author-email: mcalisterrhys@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CalibrationCurve-0.0.1/settings.ini` & `CalibrationCurve-0.0.2/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = CalibrationCurve
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = CalibrationCurve
@@ -34,10 +34,10 @@
 description = A collection of functions that streamline the process of creating calibration curves using Python.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = Rhys-McAlister
 
 ### Optional ###
-requirements = fastcore pandas statsmodels matplotlib.pyplot numpy seaborn scipy
+requirements = fastcore pandas statsmodels matplotlib numpy seaborn scipy
 # dev_requirements = 
 # console_scripts =
```

### Comparing `CalibrationCurve-0.0.1/setup.py` & `CalibrationCurve-0.0.2/setup.py`

 * *Files identical despite different names*

