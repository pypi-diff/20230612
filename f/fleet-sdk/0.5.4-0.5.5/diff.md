# Comparing `tmp/fleet_sdk-0.5.4.tar.gz` & `tmp/fleet_sdk-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleet_sdk-0.5.4.tar", max compression
+gzip compressed data, was "fleet_sdk-0.5.5.tar", max compression
```

## Comparing `fleet_sdk-0.5.4.tar` & `fleet_sdk-0.5.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-05-28 23:24:11.000000 fleet_sdk-0.5.4/LICENSE
--rw-r--r--   0        0        0       39 2023-05-29 20:36:49.448172 fleet_sdk-0.5.4/README.md
--rw-r--r--   0        0        0      536 2023-06-01 19:46:30.814760 fleet_sdk-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-30 17:33:57.142994 fleet_sdk-0.5.4/src/fleet_sdk/.DS_Store
--rw-r--r--   0        0        0     5724 2023-05-31 20:40:01.146348 fleet_sdk-0.5.4/src/fleet_sdk/Tracker.py
--rw-r--r--   0        0        0       56 2023-05-29 21:37:45.269045 fleet_sdk-0.5.4/src/fleet_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 23:36:32.000000 fleet_sdk-0.5.4/src/fleet_sdk/adapters/__init__.py
--rw-r--r--   0        0        0     1243 2023-05-30 17:34:06.613851 fleet_sdk-0.5.4/src/fleet_sdk/adapters/base_adapter.py
--rw-r--r--   0        0        0     2138 2023-05-30 17:34:19.971392 fleet_sdk-0.5.4/src/fleet_sdk/adapters/fastapi_adapter.py
--rw-r--r--   0        0        0     1955 2023-06-01 19:34:06.261840 fleet_sdk-0.5.4/src/fleet_sdk/adapters/flask_adapter.py
--rw-r--r--   0        0        0     2103 2023-06-01 19:33:04.775976 fleet_sdk-0.5.4/src/fleet_sdk/adapters/quart_adapter.py
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 fleet_sdk-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      434 2023-06-11 20:58:38.899112 fleet_sdk-0.5.5/README.md
+-rw-r--r--   0        0        0       56 2023-06-11 20:58:38.899427 fleet_sdk-0.5.5/fleet_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 20:58:38.899514 fleet_sdk-0.5.5/fleet_sdk/adapters/__init__.py
+-rw-r--r--   0        0        0     1243 2023-06-11 20:58:38.899799 fleet_sdk-0.5.5/fleet_sdk/adapters/base_adapter.py
+-rw-r--r--   0        0        0     2143 2023-06-11 20:58:38.900146 fleet_sdk-0.5.5/fleet_sdk/adapters/fastapi_adapter.py
+-rw-r--r--   0        0        0     1955 2023-06-11 20:58:38.900371 fleet_sdk-0.5.5/fleet_sdk/adapters/flask_adapter.py
+-rw-r--r--   0        0        0     2103 2023-06-11 20:58:38.900580 fleet_sdk-0.5.5/fleet_sdk/adapters/quart_adapter.py
+-rw-r--r--   0        0        0     2829 2023-06-11 20:58:38.900918 fleet_sdk-0.5.5/fleet_sdk/base.py
+-rw-r--r--   0        0        0     2167 2023-06-11 20:58:38.901133 fleet_sdk-0.5.5/fleet_sdk/fastapi.py
+-rw-r--r--   0        0        0     2236 2023-06-11 20:58:38.901280 fleet_sdk-0.5.5/fleet_sdk/flask.py
+-rw-r--r--   0        0        0     2247 2023-06-11 20:58:38.901421 fleet_sdk-0.5.5/fleet_sdk/quart.py
+-rw-r--r--   0        0        0      536 2023-06-11 22:41:15.014486 fleet_sdk-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 fleet_sdk-0.5.5/PKG-INFO
```

### Comparing `fleet_sdk-0.5.4/pyproject.toml` & `fleet_sdk-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fleet-sdk"
-version = "0.5.4"
+version = "0.5.5"
 description = "Fleet SDK for building and managing chatGPT plugins"
 authors = ["fleet_team <fleet.ai.team@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 fastapi = "^0.95.0"
```

### Comparing `fleet_sdk-0.5.4/src/fleet_sdk/adapters/base_adapter.py` & `fleet_sdk-0.5.5/fleet_sdk/adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.4/src/fleet_sdk/adapters/fastapi_adapter.py` & `fleet_sdk-0.5.5/fleet_sdk/adapters/fastapi_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Union, Dict
 
 
 class FastAPIAdapter(BaseAdapter):
 
   async def extract_data(self, event_name, request: Request,
                          response: Response, latency):
+    
     # Extract the data from the request and response
     request_data = await self.extract_request_data(request)
     response_data = await self.extract_response_data(response)
 
     # Combine request data and response data into one dictionary
     data = request_data
     data.update(response_data)
```

### Comparing `fleet_sdk-0.5.4/src/fleet_sdk/adapters/flask_adapter.py` & `fleet_sdk-0.5.5/fleet_sdk/adapters/flask_adapter.py`

 * *Files identical despite different names*

### Comparing `fleet_sdk-0.5.4/src/fleet_sdk/adapters/quart_adapter.py` & `fleet_sdk-0.5.5/fleet_sdk/adapters/quart_adapter.py`

 * *Files identical despite different names*

