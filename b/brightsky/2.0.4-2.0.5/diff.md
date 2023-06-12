# Comparing `tmp/brightsky-2.0.4.tar.gz` & `tmp/brightsky-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightsky-2.0.4.tar", last modified: Mon Jun 12 09:38:54 2023, max compression
+gzip compressed data, was "brightsky-2.0.5.tar", last modified: Mon Jun 12 10:08:20 2023, max compression
```

## Comparing `brightsky-2.0.4.tar` & `brightsky-2.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:54.229065 brightsky-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 09:38:49.000000 brightsky-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-12 09:38:54.229065 brightsky-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-12 09:38:49.000000 brightsky-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:54.225065 brightsky-2.0.4/brightsky/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:54.229065 brightsky-2.0.4/brightsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 09:38:49.000000 brightsky-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:38:54.229065 brightsky-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-12 09:38:49.000000 brightsky-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:54.229065 brightsky-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:08:20.388107 brightsky-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 10:08:11.000000 brightsky-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-12 10:08:20.388107 brightsky-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-12 10:08:11.000000 brightsky-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:08:20.384106 brightsky-2.0.5/brightsky/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:08:20.388107 brightsky-2.0.5/brightsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 10:08:11.000000 brightsky-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 10:08:20.388107 brightsky-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-12 10:08:11.000000 brightsky-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:08:20.388107 brightsky-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_web.py
```

### Comparing `brightsky-2.0.4/LICENSE` & `brightsky-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/PKG-INFO` & `brightsky-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.4
+Version: 2.0.5
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.4/README.md` & `brightsky-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/__main__.py` & `brightsky-2.0.5/brightsky/__main__.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/cli.py` & `brightsky-2.0.5/brightsky/cli.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/db.py` & `brightsky-2.0.5/brightsky/db.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/export.py` & `brightsky-2.0.5/brightsky/export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/parsers.py` & `brightsky-2.0.5/brightsky/parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/polling.py` & `brightsky-2.0.5/brightsky/polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/query.py` & `brightsky-2.0.5/brightsky/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 IGNORED_MISSING_FIELDS = {
     # Not available in MOSMIX
     'relative_humidity',
     'wind_gust_direction',
     # Not available in recent and historical measurements
     'precipitation_probability',
     'precipitation_probability_6h',
+    # Not measured at many stations
+    'solar',
 }
 
 
 def _fill_missing_fields(weather_rows, date, last_date, source_ids, partial):
     incomplete_rows = []
     missing_fields = set()
     for row in weather_rows:
```

### Comparing `brightsky-2.0.4/brightsky/settings.py` & `brightsky-2.0.5/brightsky/settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/tasks.py` & `brightsky-2.0.5/brightsky/tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/utils.py` & `brightsky-2.0.5/brightsky/utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/web.py` & `brightsky-2.0.5/brightsky/web.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky/worker.py` & `brightsky-2.0.5/brightsky/worker.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/brightsky.egg-info/PKG-INFO` & `brightsky-2.0.5/brightsky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.4
+Version: 2.0.5
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.4/brightsky.egg-info/SOURCES.txt` & `brightsky-2.0.5/brightsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/setup.py` & `brightsky-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/tests/test_export.py` & `brightsky-2.0.5/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/tests/test_parsers.py` & `brightsky-2.0.5/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/tests/test_polling.py` & `brightsky-2.0.5/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/tests/test_settings.py` & `brightsky-2.0.5/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/tests/test_tasks.py` & `brightsky-2.0.5/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/tests/test_utils.py` & `brightsky-2.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.4/tests/test_web.py` & `brightsky-2.0.5/tests/test_web.py`

 * *Files identical despite different names*

