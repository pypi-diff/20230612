# Comparing `tmp/openttd-helpers-1.2.0.tar.gz` & `tmp/openttd-helpers-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openttd-helpers-1.2.0.tar", last modified: Sun Feb 19 15:36:14 2023, max compression
+gzip compressed data, was "openttd-helpers-1.3.0.tar", last modified: Mon Jun 12 12:33:19 2023, max compression
```

## Comparing `openttd-helpers-1.2.0.tar` & `openttd-helpers-1.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:14.839473 openttd-helpers-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-02-19 15:36:14.839473 openttd-helpers-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-19 15:36:14.000000 openttd-helpers-1.2.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:14.835473 openttd-helpers-1.2.0/openttd_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:14.839473 openttd-helpers-1.2.0/openttd_helpers/asyncio_helper/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/asyncio_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/asyncio_helper/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:14.839473 openttd-helpers-1.2.0/openttd_helpers/click_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/click_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/click_helper/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/click_helper/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/click_helper/import_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:14.839473 openttd-helpers-1.2.0/openttd_helpers/logging_helper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/logging_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/logging_helper/click_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:14.839473 openttd-helpers-1.2.0/openttd_helpers/sentry_helper/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/sentry_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/openttd_helpers/sentry_helper/click_sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:14.839473 openttd-helpers-1.2.0/openttd_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-02-19 15:36:14.000000 openttd-helpers-1.2.0/openttd_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-19 15:36:14.000000 openttd-helpers-1.2.0/openttd_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 15:36:14.000000 openttd-helpers-1.2.0/openttd_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-19 15:36:14.000000 openttd-helpers-1.2.0/openttd_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-19 15:36:14.000000 openttd-helpers-1.2.0/openttd_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-19 15:36:14.839473 openttd-helpers-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-02-19 15:36:01.000000 openttd-helpers-1.2.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:19.631637 openttd-helpers-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-12 12:33:19.631637 openttd-helpers-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 12:33:19.000000 openttd-helpers-1.3.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:19.627637 openttd-helpers-1.3.0/openttd_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:19.627637 openttd-helpers-1.3.0/openttd_helpers/asyncio_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/asyncio_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/asyncio_helper/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:19.631637 openttd-helpers-1.3.0/openttd_helpers/click_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/click_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/click_helper/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/click_helper/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/click_helper/import_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:19.631637 openttd-helpers-1.3.0/openttd_helpers/logging_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/logging_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/logging_helper/click_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:19.631637 openttd-helpers-1.3.0/openttd_helpers/sentry_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/sentry_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/openttd_helpers/sentry_helper/click_sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:19.627637 openttd-helpers-1.3.0/openttd_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-12 12:33:19.000000 openttd-helpers-1.3.0/openttd_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-12 12:33:19.000000 openttd-helpers-1.3.0/openttd_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:33:19.000000 openttd-helpers-1.3.0/openttd_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 12:33:19.000000 openttd-helpers-1.3.0/openttd_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 12:33:19.000000 openttd-helpers-1.3.0/openttd_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:33:19.631637 openttd-helpers-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-12 12:33:08.000000 openttd-helpers-1.3.0/version.py
```

### Comparing `openttd-helpers-1.2.0/LICENSE` & `openttd-helpers-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openttd-helpers-1.2.0/PKG-INFO` & `openttd-helpers-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openttd-helpers
-Version: 1.2.0
+Version: 1.3.0
 Summary: Small helpers common in most Python applications for OpenTTD
 Home-page: https://github.com/OpenTTD/py-helpers
 Author: OpenTTD Dev Team
 Author-email: info@openttd.org
 License: UNKNOWN
 Description: # openttd-helpers
```

### Comparing `openttd-helpers-1.2.0/README.md` & `openttd-helpers-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openttd-helpers-1.2.0/openttd_helpers/asyncio_helper/task.py` & `openttd-helpers-1.3.0/openttd_helpers/asyncio_helper/task.py`

 * *Files identical despite different names*

### Comparing `openttd-helpers-1.2.0/openttd_helpers/click_helper/extend.py` & `openttd-helpers-1.3.0/openttd_helpers/click_helper/extend.py`

 * *Files identical despite different names*

### Comparing `openttd-helpers-1.2.0/openttd_helpers/click_helper/import_module.py` & `openttd-helpers-1.3.0/openttd_helpers/click_helper/import_module.py`

 * *Files identical despite different names*

### Comparing `openttd-helpers-1.2.0/openttd_helpers/sentry_helper/click_sentry.py` & `openttd-helpers-1.3.0/openttd_helpers/sentry_helper/click_sentry.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,13 +27,13 @@
     if not sentry_dsn:
         return
 
     # Release is expected to be in the file '.version'
     with open(".version") as f:
         release = f.readline().strip()
 
-    sentry_sdk.init(sentry_dsn, release=release, environment=sentry_environment)
+    sentry_sdk.init(sentry_dsn, release=release, environment=sentry_environment, send_client_reports=False)
     log.info(
         "Sentry initialized with release='%s' and environment='%s'",
         release,
         sentry_environment,
     )
```

### Comparing `openttd-helpers-1.2.0/openttd_helpers.egg-info/PKG-INFO` & `openttd-helpers-1.3.0/openttd_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openttd-helpers
-Version: 1.2.0
+Version: 1.3.0
 Summary: Small helpers common in most Python applications for OpenTTD
 Home-page: https://github.com/OpenTTD/py-helpers
 Author: OpenTTD Dev Team
 Author-email: info@openttd.org
 License: UNKNOWN
 Description: # openttd-helpers
```

### Comparing `openttd-helpers-1.2.0/openttd_helpers.egg-info/SOURCES.txt` & `openttd-helpers-1.3.0/openttd_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openttd-helpers-1.2.0/setup.py` & `openttd-helpers-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `openttd-helpers-1.2.0/version.py` & `openttd-helpers-1.3.0/version.py`

 * *Files identical despite different names*

