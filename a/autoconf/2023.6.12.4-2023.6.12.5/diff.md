# Comparing `tmp/autoconf-2023.6.12.4.tar.gz` & `tmp/autoconf-2023.6.12.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoconf-2023.6.12.4.tar", last modified: Mon Jun 12 13:49:10 2023, max compression
+gzip compressed data, was "autoconf-2023.6.12.5.tar", last modified: Mon Jun 12 14:10:15 2023, max compression
```

## Comparing `autoconf-2023.6.12.4.tar` & `autoconf-2023.6.12.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.607373 autoconf-2023.6.12.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-12 13:49:10.607373 autoconf-2023.6.12.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.607373 autoconf-2023.6.12.4/autoconf/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/class_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/dictable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/directory_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.607373 autoconf-2023.6.12.4/autoconf/json_prior/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/json_prior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/json_prior/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/json_prior/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.607373 autoconf-2023.6.12.4/autoconf/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/mock/mock_real.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.607373 autoconf-2023.6.12.4/autoconf/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/autoconf/tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:49:10.607373 autoconf-2023.6.12.4/autoconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 13:49:10.000000 autoconf-2023.6.12.4/autoconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 13:49:10.607373 autoconf-2023.6.12.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-12 13:48:57.000000 autoconf-2023.6.12.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:15.194503 autoconf-2023.6.12.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-12 14:10:15.194503 autoconf-2023.6.12.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:15.194503 autoconf-2023.6.12.5/autoconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 14:10:06.000000 autoconf-2023.6.12.5/autoconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/class_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/dictable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/directory_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:15.194503 autoconf-2023.6.12.5/autoconf/json_prior/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/json_prior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/json_prior/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/json_prior/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:15.194503 autoconf-2023.6.12.5/autoconf/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/mock/mock_real.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:15.194503 autoconf-2023.6.12.5/autoconf/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/autoconf/tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:10:15.194503 autoconf-2023.6.12.5/autoconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-12 14:10:15.000000 autoconf-2023.6.12.5/autoconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 14:10:15.194503 autoconf-2023.6.12.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-12 14:10:05.000000 autoconf-2023.6.12.5/setup.py
```

### Comparing `autoconf-2023.6.12.4/LICENSE` & `autoconf-2023.6.12.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.12.4/PKG-INFO` & `autoconf-2023.6.12.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf
-Version: 2023.6.12.4
+Version: 2023.6.12.5
 Summary: PyAuto Configration
 Home-page: https://github.com/rhayes777/PyAutoConf
 Author: James Nightingale and Richard Hayes
 Author-email: richard@rghsoftware.co.uk
 License: MIT License
 Keywords: cli
 Classifier: Intended Audience :: Science/Research
```

### Comparing `autoconf-2023.6.12.4/autoconf/class_path.py` & `autoconf-2023.6.12.5/autoconf/class_path.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.12.4/autoconf/conf.py` & `autoconf-2023.6.12.5/autoconf/conf.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.12.4/autoconf/dictable.py` & `autoconf-2023.6.12.5/autoconf/dictable.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.12.4/autoconf/directory_config.py` & `autoconf-2023.6.12.5/autoconf/directory_config.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.12.4/autoconf/json_prior/config.py` & `autoconf-2023.6.12.5/autoconf/json_prior/config.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.12.4/autoconf/json_prior/generate.py` & `autoconf-2023.6.12.5/autoconf/json_prior/generate.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.12.4/autoconf/mock/mock_real.py` & `autoconf-2023.6.12.5/autoconf/mock/mock_real.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.12.4/autoconf/tools/decorators.py` & `autoconf-2023.6.12.5/autoconf/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `autoconf-2023.6.12.4/setup.py` & `autoconf-2023.6.12.5/setup.py`

 * *Files identical despite different names*

