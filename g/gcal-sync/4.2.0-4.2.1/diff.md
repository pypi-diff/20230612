# Comparing `tmp/gcal-sync-4.2.0.tar.gz` & `tmp/gcal-sync-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcal-sync-4.2.0.tar", last modified: Sat Apr 29 21:56:05 2023, max compression
+gzip compressed data, was "gcal-sync-4.2.1.tar", last modified: Mon Jun 12 04:00:05 2023, max compression
```

## Comparing `gcal-sync-4.2.0.tar` & `gcal-sync-4.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/gcal_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24793 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/gcal_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    26414 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    29841 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:00:05.409475 gcal-sync-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-12 04:00:05.409475 gcal-sync-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:00:05.409475 gcal-sync-4.2.1/gcal_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/gcal_sync/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:00:05.409475 gcal-sync-4.2.1/gcal_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-12 04:00:05.000000 gcal-sync-4.2.1/gcal_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-12 04:00:05.000000 gcal-sync-4.2.1/gcal_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:00:05.000000 gcal-sync-4.2.1/gcal_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 04:00:05.000000 gcal-sync-4.2.1/gcal_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 04:00:05.000000 gcal-sync-4.2.1/gcal_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-12 04:00:05.409475 gcal-sync-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:00:05.409475 gcal-sync-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26414 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29841 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-06-12 03:59:55.000000 gcal-sync-4.2.1/tests/test_timeline.py
```

### Comparing `gcal-sync-4.2.0/LICENSE` & `gcal-sync-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/PKG-INFO` & `gcal-sync-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcal-sync
-Version: 4.2.0
+Version: 4.2.1
 Summary: A python library for syncing Google Calendar to local storage
 Home-page: https://github.com/allenporter/gcal_sync
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `gcal-sync-4.2.0/README.md` & `gcal-sync-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/gcal_sync/api.py` & `gcal-sync-4.2.1/gcal_sync/api.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/gcal_sync/auth.py` & `gcal-sync-4.2.1/gcal_sync/auth.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/gcal_sync/exceptions.py` & `gcal-sync-4.2.1/gcal_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/gcal_sync/model.py` & `gcal-sync-4.2.1/gcal_sync/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,15 +449,15 @@
     minutes: int
     """Number of minutes before the start of the event to trigger."""
 
 
 class Reminders(BaseModel):
     """Information about the event's reminders for the authenticated user."""
 
-    use_default: bool = Field(alias="useDefault", default=False)
+    use_default: bool = Field(alias="useDefault", default=True)
 
     overrides: list[ReminderOverride] = Field(default_factory=list)
     """Reminders to use instead of the default reminders.
 
     If the event doesn't use the default reminders, this lists the reminders
     specific to the event, or, if not set, indicates that no reminders are
     set for this event. The maximum number of override reminders is 5.
```

### Comparing `gcal-sync-4.2.0/gcal_sync/store.py` & `gcal-sync-4.2.1/gcal_sync/store.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/gcal_sync/sync.py` & `gcal-sync-4.2.1/gcal_sync/sync.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/gcal_sync/timeline.py` & `gcal-sync-4.2.1/gcal_sync/timeline.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/gcal_sync.egg-info/PKG-INFO` & `gcal-sync-4.2.1/gcal_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcal-sync
-Version: 4.2.0
+Version: 4.2.1
 Summary: A python library for syncing Google Calendar to local storage
 Home-page: https://github.com/allenporter/gcal_sync
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `gcal-sync-4.2.0/gcal_sync.egg-info/SOURCES.txt` & `gcal-sync-4.2.1/gcal_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/setup.cfg` & `gcal-sync-4.2.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gcal-sync
-version = 4.2.0
+version = 4.2.1
 description = A python library for syncing Google Calendar to local storage
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/gcal_sync
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `gcal-sync-4.2.0/tests/test_api.py` & `gcal-sync-4.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/tests/test_auth.py` & `gcal-sync-4.2.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/tests/test_model.py` & `gcal-sync-4.2.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/tests/test_store.py` & `gcal-sync-4.2.1/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/tests/test_sync.py` & `gcal-sync-4.2.1/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.2.0/tests/test_timeline.py` & `gcal-sync-4.2.1/tests/test_timeline.py`

 * *Files identical despite different names*

