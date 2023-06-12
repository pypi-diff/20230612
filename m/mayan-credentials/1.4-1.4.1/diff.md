# Comparing `tmp/mayan-credentials-1.4.tar.gz` & `tmp/mayan-credentials-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayan-credentials-1.4.tar", last modified: Tue Jan 25 08:25:41 2022, max compression
+gzip compressed data, was "mayan-credentials-1.4.1.tar", last modified: Mon Jun 12 09:47:23 2023, max compression
```

## Comparing `mayan-credentials-1.4.tar` & `mayan-credentials-1.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-01-25 08:25:41.804379 mayan-credentials-1.4/
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)      721 2022-01-25 08:24:22.000000 mayan-credentials-1.4/HISTORY.rst
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)      555 2020-09-02 03:45:36.000000 mayan-credentials-1.4/LICENSE
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)       39 2020-09-02 04:35:02.000000 mayan-credentials-1.4/MANIFEST.in
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3726 2022-01-25 08:25:41.808379 mayan-credentials-1.4/PKG-INFO
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     1073 2020-09-02 08:06:16.000000 mayan-credentials-1.4/README.rst
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-01-25 08:25:41.804379 mayan-credentials-1.4/credentials/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       55 2021-06-03 17:32:51.000000 mayan-credentials-1.4/credentials/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      200 2021-02-07 08:22:13.000000 mayan-credentials-1.4/credentials/admin.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1648 2020-12-15 07:19:44.000000 mayan-credentials-1.4/credentials/api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2832 2022-01-25 08:23:34.000000 mayan-credentials-1.4/credentials/apps.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1395 2022-01-25 08:16:45.000000 mayan-credentials-1.4/credentials/classes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4577 2021-02-23 15:40:48.000000 mayan-credentials-1.4/credentials/credential_backends.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      527 2020-09-02 07:29:30.000000 mayan-credentials-1.4/credentials/events.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1613 2021-06-03 17:29:16.000000 mayan-credentials-1.4/credentials/forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      534 2020-09-02 06:56:57.000000 mayan-credentials-1.4/credentials/icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1800 2022-01-25 08:09:48.000000 mayan-credentials-1.4/credentials/links.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-01-25 08:25:41.804379 mayan-credentials-1.4/credentials/migrations/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1364 2020-09-07 05:54:00.000000 mayan-credentials-1.4/credentials/migrations/0001_initial.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1268 2021-02-07 08:26:23.000000 mayan-credentials-1.4/credentials/migrations/0002_auto_20201215_0523.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1037 2021-02-07 08:24:02.000000 mayan-credentials-1.4/credentials/migrations/0003_auto_20210207_0823.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      737 2021-02-07 08:39:56.000000 mayan-credentials-1.4/credentials/migrations/0004_auto_20210207_0823.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      768 2021-02-07 08:40:52.000000 mayan-credentials-1.4/credentials/migrations/0005_auto_20210207_0840.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-09-02 06:51:02.000000 mayan-credentials-1.4/credentials/migrations/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3126 2021-02-23 15:35:57.000000 mayan-credentials-1.4/credentials/models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      763 2020-09-02 06:57:40.000000 mayan-credentials-1.4/credentials/permissions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      478 2020-12-15 07:19:22.000000 mayan-credentials-1.4/credentials/serializers.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-01-25 08:25:41.804379 mayan-credentials-1.4/credentials/tests/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-08-31 04:43:36.000000 mayan-credentials-1.4/credentials/tests/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      406 2020-12-15 05:44:26.000000 mayan-credentials-1.4/credentials/tests/literals.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3774 2020-12-15 07:18:51.000000 mayan-credentials-1.4/credentials/tests/mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6800 2020-12-15 07:19:03.000000 mayan-credentials-1.4/credentials/tests/test_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4661 2022-01-25 08:20:57.000000 mayan-credentials-1.4/credentials/tests/test_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1442 2020-12-15 06:59:49.000000 mayan-credentials-1.4/credentials/urls.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4660 2021-06-03 17:29:05.000000 mayan-credentials-1.4/credentials/views.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-01-25 08:25:41.804379 mayan-credentials-1.4/mayan_credentials.egg-info/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3726 2022-01-25 08:25:41.000000 mayan-credentials-1.4/mayan_credentials.egg-info/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1039 2022-01-25 08:25:41.000000 mayan-credentials-1.4/mayan_credentials.egg-info/SOURCES.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2022-01-25 08:25:41.000000 mayan-credentials-1.4/mayan_credentials.egg-info/dependency_links.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2022-01-25 08:25:41.000000 mayan-credentials-1.4/mayan_credentials.egg-info/not-zip-safe
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       12 2022-01-25 08:25:41.000000 mayan-credentials-1.4/mayan_credentials.egg-info/top_level.txt
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)      129 2022-01-25 08:25:41.808379 mayan-credentials-1.4/setup.cfg
--rwxr-xr-x   0 rosarior  (1000) rosarior  (1000)     2975 2022-01-25 08:24:32.000000 mayan-credentials-1.4/setup.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:47:23.064259 mayan-credentials-1.4.1/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      805 2023-06-12 09:33:38.000000 mayan-credentials-1.4.1/HISTORY.rst
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/LICENSE
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/MANIFEST.in
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3111 2023-06-12 09:47:23.064259 mayan-credentials-1.4.1/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1073 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/README.rst
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:47:23.064259 mayan-credentials-1.4.1/credentials/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       55 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      200 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/admin.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1648 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2832 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/apps.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1395 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/classes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4577 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/credential_backends.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      527 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/events.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1613 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      534 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1800 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/links.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:47:23.064259 mayan-credentials-1.4.1/credentials/migrations/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1364 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/migrations/0001_initial.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1268 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/migrations/0002_auto_20201215_0523.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1037 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/migrations/0003_auto_20210207_0823.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      737 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/migrations/0004_auto_20210207_0823.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      768 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/migrations/0005_auto_20210207_0840.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/migrations/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3271 2023-06-12 09:32:45.000000 mayan-credentials-1.4.1/credentials/models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      763 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/permissions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      478 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/serializers.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:47:23.064259 mayan-credentials-1.4.1/credentials/tests/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/tests/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      406 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/tests/literals.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3774 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/tests/mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6800 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/tests/test_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4661 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/tests/test_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1442 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/urls.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4660 2023-06-12 09:31:31.000000 mayan-credentials-1.4.1/credentials/views.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:47:23.064259 mayan-credentials-1.4.1/mayan_credentials.egg-info/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3111 2023-06-12 09:47:23.000000 mayan-credentials-1.4.1/mayan_credentials.egg-info/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1039 2023-06-12 09:47:23.000000 mayan-credentials-1.4.1/mayan_credentials.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2023-06-12 09:47:23.000000 mayan-credentials-1.4.1/mayan_credentials.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2023-06-12 09:47:23.000000 mayan-credentials-1.4.1/mayan_credentials.egg-info/not-zip-safe
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       12 2023-06-12 09:47:23.000000 mayan-credentials-1.4.1/mayan_credentials.egg-info/top_level.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2023-06-12 09:47:23.064259 mayan-credentials-1.4.1/setup.cfg
+-rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     2977 2023-06-12 09:33:50.000000 mayan-credentials-1.4.1/setup.py
```

### Comparing `mayan-credentials-1.4/HISTORY.rst` & `mayan-credentials-1.4.1/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+1.4.1 (2023-06-12)
+==================
+- Support new event manager module location.
+
 1.4 (2022-01-25)
 ================
 - Update for Mayan EDMS version 4.2.
 
 1.3 (2021-06-03)
 ================
 - Update for version 4.0.
```

### Comparing `mayan-credentials-1.4/LICENSE` & `mayan-credentials-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/README.rst` & `mayan-credentials-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/api_views.py` & `mayan-credentials-1.4.1/credentials/api_views.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/apps.py` & `mayan-credentials-1.4.1/credentials/apps.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/classes.py` & `mayan-credentials-1.4.1/credentials/classes.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/credential_backends.py` & `mayan-credentials-1.4.1/credentials/credential_backends.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/events.py` & `mayan-credentials-1.4.1/credentials/events.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/forms.py` & `mayan-credentials-1.4.1/credentials/forms.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/icons.py` & `mayan-credentials-1.4.1/credentials/icons.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/links.py` & `mayan-credentials-1.4.1/credentials/links.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/migrations/0001_initial.py` & `mayan-credentials-1.4.1/credentials/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/migrations/0002_auto_20201215_0523.py` & `mayan-credentials-1.4.1/credentials/migrations/0002_auto_20201215_0523.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/migrations/0003_auto_20210207_0823.py` & `mayan-credentials-1.4.1/credentials/migrations/0003_auto_20210207_0823.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/migrations/0004_auto_20210207_0823.py` & `mayan-credentials-1.4.1/credentials/migrations/0004_auto_20210207_0823.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/migrations/0005_auto_20210207_0840.py` & `mayan-credentials-1.4.1/credentials/migrations/0005_auto_20210207_0840.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/models.py` & `mayan-credentials-1.4.1/credentials/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import json
 
 from django.db import models
 from django.utils.module_loading import import_string
 from django.utils.translation import ugettext_lazy as _
 
 from mayan.apps.common.validators import validate_internal_name
-from mayan.apps.events.classes import (
-    EventManagerMethodAfter, EventManagerSave
-)
+try:
+    from mayan.apps.events.classes import (
+        EventManagerMethodAfter, EventManagerSave
+    )
+except ImportError:
+    from mayan.apps.events.event_managers import (
+        EventManagerMethodAfter, EventManagerSave
+    )
+
 from mayan.apps.events.decorators import method_event
 
 from .classes import NullBackend
 from .events import (
     event_credential_created, event_credential_edited, event_credential_used
 )
```

### Comparing `mayan-credentials-1.4/credentials/permissions.py` & `mayan-credentials-1.4.1/credentials/permissions.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/tests/mixins.py` & `mayan-credentials-1.4.1/credentials/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/tests/test_api.py` & `mayan-credentials-1.4.1/credentials/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/tests/test_views.py` & `mayan-credentials-1.4.1/credentials/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/urls.py` & `mayan-credentials-1.4.1/credentials/urls.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/credentials/views.py` & `mayan-credentials-1.4.1/credentials/views.py`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/mayan_credentials.egg-info/SOURCES.txt` & `mayan-credentials-1.4.1/mayan_credentials.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayan-credentials-1.4/setup.py` & `mayan-credentials-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,10 +92,10 @@
     license='Apache 2.0',
     long_description=readme + '\n\n' + history,
     name=PACKAGE_NAME,
     packages=find_packages(PACKAGE_DIR),
     platforms=['any'],
     python_requires='!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
     url='https://gitlab.com/mayan-edms/credentials',
-    version='1.4',
+    version='1.4.1',
     zip_safe=False,
 )
```

