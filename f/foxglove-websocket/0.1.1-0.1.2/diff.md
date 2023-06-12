# Comparing `tmp/foxglove-websocket-0.1.1.tar.gz` & `tmp/foxglove-websocket-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-websocket-0.1.1.tar", last modified: Wed May 17 18:12:55 2023, max compression
+gzip compressed data, was "foxglove-websocket-0.1.2.tar", last modified: Mon Jun 12 17:42:44 2023, max compression
```

## Comparing `foxglove-websocket-0.1.1.tar` & `foxglove-websocket-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-17 18:12:55.922429 foxglove-websocket-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.902428 foxglove-websocket-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.906428 foxglove-websocket-0.1.1/src/foxglove_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/json_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/param_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/examples/protobuf_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/src/foxglove_websocket/server/
--rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/server/client_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/src/foxglove_websocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.914428 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:12:39.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 18:12:55.000000 foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:12:55.918428 foxglove-websocket-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/tests/test_client_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-05-17 18:12:26.000000 foxglove-websocket-0.1.1/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:42:44.501534 foxglove-websocket-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-12 17:42:44.501534 foxglove-websocket-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-12 17:42:44.501534 foxglove-websocket-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:42:44.497534 foxglove-websocket-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:42:44.501534 foxglove-websocket-0.1.2/src/foxglove_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/src/foxglove_websocket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:42:44.501534 foxglove-websocket-0.1.2/src/foxglove_websocket/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/src/foxglove_websocket/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/src/foxglove_websocket/examples/json_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/src/foxglove_websocket/examples/param_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/src/foxglove_websocket/examples/protobuf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:42:44.501534 foxglove-websocket-0.1.2/src/foxglove_websocket/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/src/foxglove_websocket/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/src/foxglove_websocket/server/client_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/src/foxglove_websocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:42:44.501534 foxglove-websocket-0.1.2/src/foxglove_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-12 17:42:44.000000 foxglove-websocket-0.1.2/src/foxglove_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-12 17:42:44.000000 foxglove-websocket-0.1.2/src/foxglove_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:42:44.000000 foxglove-websocket-0.1.2/src/foxglove_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:42:30.000000 foxglove-websocket-0.1.2/src/foxglove_websocket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 17:42:44.000000 foxglove-websocket-0.1.2/src/foxglove_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 17:42:44.000000 foxglove-websocket-0.1.2/src/foxglove_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:42:44.501534 foxglove-websocket-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/tests/test_client_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-06-12 17:42:16.000000 foxglove-websocket-0.1.2/tests/test_server.py
```

### Comparing `foxglove-websocket-0.1.1/PKG-INFO` & `foxglove-websocket-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-websocket
-Version: 0.1.1
+Version: 0.1.2
 Summary: Foxglove WebSocket server
 Home-page: https://github.com/foxglove/ws-protocol
 License: MIT
 Project-URL: GitHub Issues, https://github.com/foxglove/ws-protocol/issues
 Project-URL: Foxglove Studio Documentation, https://foxglove.dev/docs
 Keywords: foxglove,websocket,robotics,ros,ros2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `foxglove-websocket-0.1.1/README.md` & `foxglove-websocket-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.1/setup.cfg` & `foxglove-websocket-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-websocket
-version = 0.1.1
+version = 0.1.2
 description = Foxglove WebSocket server
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = foxglove, websocket, robotics, ros, ros2
 license = MIT
 url = https://github.com/foxglove/ws-protocol
 project_urls =
```

### Comparing `foxglove-websocket-0.1.1/src/foxglove_websocket/__init__.py` & `foxglove-websocket-0.1.2/src/foxglove_websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.1/src/foxglove_websocket/examples/json_server.py` & `foxglove-websocket-0.1.2/src/foxglove_websocket/examples/json_server.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.1/src/foxglove_websocket/examples/param_server.py` & `foxglove-websocket-0.1.2/src/foxglove_websocket/examples/param_server.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.1/src/foxglove_websocket/examples/protobuf_server.py` & `foxglove-websocket-0.1.2/src/foxglove_websocket/examples/protobuf_server.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.1/src/foxglove_websocket/server/__init__.py` & `foxglove-websocket-0.1.2/src/foxglove_websocket/server/__init__.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.1/src/foxglove_websocket/server/client_state.py` & `foxglove-websocket-0.1.2/src/foxglove_websocket/server/client_state.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.1/src/foxglove_websocket/types.py` & `foxglove-websocket-0.1.2/src/foxglove_websocket/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 
 class ClientChannel(TypedDict):
     id: ClientChannelId
     topic: str
     encoding: str
     schemaName: str
+    schema: Optional[str]
+    schemaEncoding: Optional[str]
 
 
 class Subscribe(TypedDict):
     op: Literal["subscribe"]
     subscriptions: List[Subscription]
```

### Comparing `foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/PKG-INFO` & `foxglove-websocket-0.1.2/src/foxglove_websocket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-websocket
-Version: 0.1.1
+Version: 0.1.2
 Summary: Foxglove WebSocket server
 Home-page: https://github.com/foxglove/ws-protocol
 License: MIT
 Project-URL: GitHub Issues, https://github.com/foxglove/ws-protocol/issues
 Project-URL: Foxglove Studio Documentation, https://foxglove.dev/docs
 Keywords: foxglove,websocket,robotics,ros,ros2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `foxglove-websocket-0.1.1/src/foxglove_websocket.egg-info/SOURCES.txt` & `foxglove-websocket-0.1.2/src/foxglove_websocket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.1/tests/test_client_state.py` & `foxglove-websocket-0.1.2/tests/test_client_state.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.1.1/tests/test_server.py` & `foxglove-websocket-0.1.2/tests/test_server.py`

 * *Files identical despite different names*

