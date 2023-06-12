# Comparing `tmp/nowcasting_datamodel-1.4.0.tar.gz` & `tmp/nowcasting_datamodel-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.4.0.tar", last modified: Mon Jun  5 15:51:27 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.4.1.tar", last modified: Mon Jun 12 13:48:20 2023, max compression
```

## Comparing `nowcasting_datamodel-1.4.0.tar` & `nowcasting_datamodel-1.4.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.258225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.258225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.258225 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 15:51:27.000000 nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:51:27.262225 nowcasting_datamodel-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-05 15:51:17.000000 nowcasting_datamodel-1.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:20.715355 nowcasting_datamodel-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-12 13:48:20.715355 nowcasting_datamodel-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:20.711355 nowcasting_datamodel-1.4.1/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:20.711355 nowcasting_datamodel-1.4.1/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:20.715355 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:20.715355 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:20.715355 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:20.715355 nowcasting_datamodel-1.4.1/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:20.711355 nowcasting_datamodel-1.4.1/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-12 13:48:20.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-12 13:48:20.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:48:20.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 13:48:20.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 13:48:20.000000 nowcasting_datamodel-1.4.1/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:48:20.715355 nowcasting_datamodel-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:20.715355 nowcasting_datamodel-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-12 13:48:07.000000 nowcasting_datamodel-1.4.1/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.4.0/PKG-INFO` & `nowcasting_datamodel-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.4.0
+Version: 1.4.1
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.0/README.md` & `nowcasting_datamodel-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/diagram.png` & `nowcasting_datamodel-1.4.1/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/diagram_pv.png` & `nowcasting_datamodel-1.4.1/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/api.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/api.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/blend/blend.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/blend/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,17 @@
         query = query.join(MLModelSQL)
         query = query.filter(MLModelSQL.name == model_name)
 
     # get all results
     metric_values = query.all()
 
     # add timezone, show be the same datetime interval for all
-    datetime_interval = metric_values[0].datetime_interval
-    datetime_interval.start_datetime_utc = datetime_interval.start_datetime_utc.replace(
-        tzinfo=timezone.utc
-    )
-    datetime_interval.end_datetime_utc = datetime_interval.end_datetime_utc.replace(
-        tzinfo=timezone.utc
-    )
+    if len(metric_values) > 0:
+        datetime_interval = metric_values[0].datetime_interval
+        datetime_interval.start_datetime_utc = datetime_interval.start_datetime_utc.replace(
+            tzinfo=timezone.utc
+        )
+        datetime_interval.end_datetime_utc = datetime_interval.end_datetime_utc.replace(
+            tzinfo=timezone.utc
+        )
 
     return metric_values
```

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/read/read_user.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/read/read_user.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/save/adjust.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Methods for adding adjust values to the forecast"""
 import logging
 from datetime import datetime, timedelta
 from typing import List, Union
 
+import numpy as np
 import pandas as pd
 
 from nowcasting_datamodel.models import Forecast, ForecastSQL, MetricValue, MetricValueSQL
 from nowcasting_datamodel.read.read_metric import read_latest_me_national
 
 logger = logging.getLogger()
 
@@ -52,16 +53,18 @@
     logger.debug(
         f"Adding adjuster to national forecast for "
         f"{datetime_now} and {model_name}, {last_datetime=}"
     )
 
     # 1. read metric values
     latest_me = read_latest_me_national(session=session, model_name=model_name)
-    assert len(latest_me) > 0
-    logger.debug(f"Found {len(latest_me)} latest ME values")
+    if len(latest_me) == 0:
+        logger.warning(f"Found no ME values found for {model_name=}")
+    else:
+        logger.debug(f"Found {len(latest_me)} latest ME values")
 
     # 2. filter value down to now onwards
     # get the number of hours to go ahead, we've added 1 to make sure we use the last one as well
     hours_ahead = get_forecast_horizon_from_forecast(forecast)
     # change to dataframe
     latest_me_df = reduce_metric_values_to_correct_forecast_horizon(
         latest_me=latest_me, datetime_now=datetime_now, hours_ahead=hours_ahead
@@ -74,17 +77,27 @@
         try:
             # get value from df
             value = latest_me_df[latest_me_df["datetime"] == forecast_value.target_time]
             value = value.iloc[0].value
 
             # add value to ForecastValueSQL
             forecast_value.adjust_mw = value
+            if np.isnan(value):
+                logger.debug(
+                    f"Found ME value for {target_time} in {latest_me_df}, "
+                    f"but it was NaN, therefore adding adjust_mw as 0"
+                )
+                forecast_value.adjust_mw = 0.0
 
         except Exception:
-            logger.debug(f"Could not find ME value for {target_time} in {latest_me_df}")
+            logger.debug(
+                f"Could not find ME value for {target_time} in {latest_me_df}, "
+                f"therefore adding adjust_mw as 0"
+            )
+            forecast_value.adjust_mw = 0.0
 
 
 def get_forecast_horizon_from_forecast(forecast: Union[ForecastSQL, Forecast]):
     """
     Get the number of hours ahead from the forecast
 
     :param forecast:
@@ -140,28 +153,30 @@
     """
 
     logger.debug(
         f"Reducing metric values to correct forecast horizon {datetime_now=} {hours_ahead=}"
     )
 
     latest_me_df = pd.DataFrame([MetricValue.from_orm(m).dict() for m in latest_me])
+    if len(latest_me_df) == 0:
+        # no latest ME values, so just making an empty dataframe
+        latest_me_df = pd.DataFrame(columns=["forecast_horizon_minutes", "time_of_day", "value"])
 
     # Let now big a dataframe of datetimes from now onwards. Lets say the time is 04.30, then
     # time forecast_horizon value
     # 04.30 0  0.1
     # 05.00 30 0.2
     # 05.30 60 0.6
     # .....
 
     results_df = pd.DataFrame(
         index=pd.date_range(
             start=datetime_now, end=datetime_now + timedelta(hours=hours_ahead), freq="30T"
         ),
     )
-    print(results_df)
     results_df["datetime"] = results_df.index
     results_df["time_of_day"] = results_df.index.time
     results_df["forecast_horizon_minutes"] = range(0, 30 * len(results_df), 30)
     latest_me_df["forecast_horizon_minutes"] = latest_me_df["forecast_horizon_minutes"].astype(int)
     results_df["forecast_horizon_minutes"] = results_df["forecast_horizon_minutes"].astype(int)
     latest_me_df["value"] = latest_me_df["value"].astype(float)
```

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.4.0
+Version: 1.4.1
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.0/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.4.1/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/setup.py` & `nowcasting_datamodel-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.4.1/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/tests/test_fake.py` & `nowcasting_datamodel-1.4.1/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/tests/test_fake_pv.py` & `nowcasting_datamodel-1.4.1/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/tests/test_national.py` & `nowcasting_datamodel-1.4.1/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.0/tests/test_utils.py` & `nowcasting_datamodel-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

