# Comparing `tmp/ango-1.1.0.tar.gz` & `tmp/ango-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.1.0.tar", last modified: Fri Jun  9 07:30:29 2023, max compression
+gzip compressed data, was "ango-1.1.1.tar", last modified: Mon Jun 12 07:13:44 2023, max compression
```

## Comparing `ango-1.1.0.tar` & `ango-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 07:30:29.560179 ango-1.1.0/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-09 07:30:29.560179 ango-1.1.0/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.1.0/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 07:30:29.560179 ango-1.1.0/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.1.0/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 07:30:29.560179 ango-1.1.0/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.1.0/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.1.0/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5445 2023-06-09 07:29:48.000000 ango-1.1.0/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.1.0/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5511 2023-06-09 07:29:48.000000 ango-1.1.0/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14965 2023-06-09 07:29:48.000000 ango-1.1.0/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 07:30:29.560179 ango-1.1.0/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-09 07:30:29.000000 ango-1.1.0/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-09 07:30:29.560179 ango-1.1.0/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      871 2023-06-09 07:30:23.000000 ango-1.1.0/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:13:44.470739 ango-1.1.1/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-12 07:13:44.470739 ango-1.1.1/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.1.1/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:13:44.470739 ango-1.1.1/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:10:53.000000 ango-1.1.1/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:13:44.470739 ango-1.1.1/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:10:53.000000 ango-1.1.1/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-12 07:10:53.000000 ango-1.1.1/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5445 2023-06-12 07:10:53.000000 ango-1.1.1/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-12 07:10:53.000000 ango-1.1.1/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5722 2023-06-12 07:13:06.000000 ango-1.1.1/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14965 2023-06-12 07:10:53.000000 ango-1.1.1/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:13:44.470739 ango-1.1.1/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-12 07:13:44.000000 ango-1.1.1/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-12 07:13:44.000000 ango-1.1.1/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-12 07:13:44.000000 ango-1.1.1/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-12 07:13:44.000000 ango-1.1.1/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-12 07:13:44.000000 ango-1.1.1/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-12 07:13:44.470739 ango-1.1.1/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      871 2023-06-12 07:13:29.000000 ango-1.1.1/setup.py
```

### Comparing `ango-1.1.0/PKG-INFO` & `ango-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.1.0
+Version: 1.1.1
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.1.0/README.md` & `ango-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.1.0/ango/models/label_category.py` & `ango-1.1.1/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.1.0/ango/plugin_logger.py` & `ango-1.1.1/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.1.0/ango/plugins.py` & `ango-1.1.1/ango/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,19 @@
         self.logger.warning("Connected")
         self.heartbeat()
 
     def on_disconnect(self):
         self.logger.warning("Disconnected")
 
     def heartbeat(self):
-        self.emit('heartbeat', {"id": self.id, "secret": self.secret})
+        try:
+            self.emit('heartbeat', {"id": self.id, "secret": self.secret})
+        except:
+            _connect(self, self.client.connection_url)
+            self.emit('heartbeat', {"id": self.id, "secret": self.secret})
         self.logger.warning("Heartbeat at %s" % str(time.time()))
 
     def on_plugin(self, data):
         data["logger"] = self._get_logger(data)
         data["batches"] = data.get('tags', [])
         response = {
             "response": self.callback(**data),
@@ -137,16 +141,18 @@
         super().__init__(id, secret, callback)
 
 
 class MarkdownPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
-
-def run(plugin, host="https://api.ango.ai"):
+def _connect(plugin, host):
     sio = socketio.Client()
     sio.register_namespace(plugin)
-    sio.connect(host, namespaces=["/plugin"], wait_timeout=100)
+    sio.connect(host, namespaces=["/plugin"], wait=True)
+
+def run(plugin, host="https://api.ango.ai"):
+    _connect(plugin, host)
     try:
         asyncio.get_event_loop().run_forever()
     except (KeyboardInterrupt, SystemExit):
         logging.getLogger().warning("Plugin Stopped")
```

### Comparing `ango-1.1.0/ango/sdk.py` & `ango-1.1.1/ango/sdk.py`

 * *Files identical despite different names*

### Comparing `ango-1.1.0/ango.egg-info/PKG-INFO` & `ango-1.1.1/ango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.1.0
+Version: 1.1.1
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.1.0/setup.py` & `ango-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.1.0",
+    version="1.1.1",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

