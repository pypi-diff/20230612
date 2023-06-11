# Comparing `tmp/fleet_sdk-0.5.5.tar.gz` & `tmp/fleet_sdk-0.5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleet_sdk-0.5.5.tar", max compression
+gzip compressed data, was "fleet_sdk-0.5.5.1.tar", max compression
```

## Comparing `fleet_sdk-0.5.5.tar` & `fleet_sdk-0.5.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      434 2023-06-11 20:58:38.899112 fleet_sdk-0.5.5/README.md
--rw-r--r--   0        0        0       56 2023-06-11 20:58:38.899427 fleet_sdk-0.5.5/fleet_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 20:58:38.899514 fleet_sdk-0.5.5/fleet_sdk/adapters/__init__.py
--rw-r--r--   0        0        0     1243 2023-06-11 20:58:38.899799 fleet_sdk-0.5.5/fleet_sdk/adapters/base_adapter.py
--rw-r--r--   0        0        0     2143 2023-06-11 20:58:38.900146 fleet_sdk-0.5.5/fleet_sdk/adapters/fastapi_adapter.py
--rw-r--r--   0        0        0     1955 2023-06-11 20:58:38.900371 fleet_sdk-0.5.5/fleet_sdk/adapters/flask_adapter.py
--rw-r--r--   0        0        0     2103 2023-06-11 20:58:38.900580 fleet_sdk-0.5.5/fleet_sdk/adapters/quart_adapter.py
--rw-r--r--   0        0        0     2829 2023-06-11 20:58:38.900918 fleet_sdk-0.5.5/fleet_sdk/base.py
--rw-r--r--   0        0        0     2167 2023-06-11 20:58:38.901133 fleet_sdk-0.5.5/fleet_sdk/fastapi.py
--rw-r--r--   0        0        0     2236 2023-06-11 20:58:38.901280 fleet_sdk-0.5.5/fleet_sdk/flask.py
--rw-r--r--   0        0        0     2247 2023-06-11 20:58:38.901421 fleet_sdk-0.5.5/fleet_sdk/quart.py
--rw-r--r--   0        0        0      536 2023-06-11 22:41:15.014486 fleet_sdk-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 fleet_sdk-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      434 2023-06-11 20:58:38.899112 fleet_sdk-0.5.5.1/README.md
+-rw-r--r--   0        0        0       56 2023-06-11 20:58:38.899427 fleet_sdk-0.5.5.1/fleet_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 20:58:38.899514 fleet_sdk-0.5.5.1/fleet_sdk/adapters/__init__.py
+-rw-r--r--   0        0        0     1243 2023-06-11 20:58:38.899799 fleet_sdk-0.5.5.1/fleet_sdk/adapters/base_adapter.py
+-rw-r--r--   0        0        0     2143 2023-06-11 20:58:38.900146 fleet_sdk-0.5.5.1/fleet_sdk/adapters/fastapi_adapter.py
+-rw-r--r--   0        0        0     1955 2023-06-11 20:58:38.900371 fleet_sdk-0.5.5.1/fleet_sdk/adapters/flask_adapter.py
+-rw-r--r--   0        0        0     2103 2023-06-11 20:58:38.900580 fleet_sdk-0.5.5.1/fleet_sdk/adapters/quart_adapter.py
+-rw-r--r--   0        0        0     2829 2023-06-11 20:58:38.900918 fleet_sdk-0.5.5.1/fleet_sdk/base.py
+-rw-r--r--   0        0        0     2167 2023-06-11 20:58:38.901133 fleet_sdk-0.5.5.1/fleet_sdk/fastapi.py
+-rw-r--r--   0        0        0     2236 2023-06-11 20:58:38.901280 fleet_sdk-0.5.5.1/fleet_sdk/flask.py
+-rw-r--r--   0        0        0     2247 2023-06-11 20:58:38.901421 fleet_sdk-0.5.5.1/fleet_sdk/quart.py
+-rw-r--r--   0        0        0      531 2023-06-11 22:45:57.311050 fleet_sdk-0.5.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 fleet_sdk-0.5.5.1/PKG-INFO
```

### Comparing `fleet_sdk-0.5.5/fleet_sdk/adapters/base_adapter.py` & `fleet_sdk-0.5.5.1/fleet_sdk/adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.5/fleet_sdk/adapters/fastapi_adapter.py` & `fleet_sdk-0.5.5.1/fleet_sdk/adapters/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.5/fleet_sdk/adapters/flask_adapter.py` & `fleet_sdk-0.5.5.1/fleet_sdk/adapters/flask_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.5/fleet_sdk/adapters/quart_adapter.py` & `fleet_sdk-0.5.5.1/fleet_sdk/adapters/quart_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.5/fleet_sdk/base.py` & `fleet_sdk-0.5.5.1/fleet_sdk/base.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.5/fleet_sdk/fastapi.py` & `fleet_sdk-0.5.5.1/fleet_sdk/fastapi.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.5/fleet_sdk/flask.py` & `fleet_sdk-0.5.5.1/fleet_sdk/flask.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.5/fleet_sdk/quart.py` & `fleet_sdk-0.5.5.1/fleet_sdk/quart.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.5/PKG-INFO` & `fleet_sdk-0.5.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fleet-sdk
-Version: 0.5.5
+Version: 0.5.5.1
 Summary: Fleet SDK for building and managing chatGPT plugins
 Author: fleet_team
-Author-email: fleet.ai.team@gmail.com
+Author-email: team@usefleet.ai
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

