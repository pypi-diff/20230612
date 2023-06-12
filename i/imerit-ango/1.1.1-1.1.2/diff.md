# Comparing `tmp/imerit-ango-1.1.1.tar.gz` & `tmp/imerit-ango-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imerit-ango-1.1.1.tar", last modified: Fri Jun  9 09:14:23 2023, max compression
+gzip compressed data, was "imerit-ango-1.1.2.tar", last modified: Mon Jun 12 07:10:08 2023, max compression
```

## Comparing `imerit-ango-1.1.1.tar` & `imerit-ango-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 imerit-ango-1.1.1/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/imerit_ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 imerit-ango-1.1.1/imerit_ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/imerit_ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 imerit-ango-1.1.1/imerit_ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 imerit-ango-1.1.1/imerit_ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-06-09 09:11:15.000000 imerit-ango-1.1.1/imerit_ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 imerit-ango-1.1.1/imerit_ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5652 2023-06-09 09:11:54.000000 imerit-ango-1.1.1/imerit_ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14443 2023-06-09 09:11:54.000000 imerit-ango-1.1.1/imerit_ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/imerit_ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      383 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       12 2023-06-09 09:14:23.000000 imerit-ango-1.1.1/imerit_ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-09 09:14:23.996730 imerit-ango-1.1.1/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      892 2023-06-09 09:14:22.000000 imerit-ango-1.1.1/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:10:08.794593 imerit-ango-1.1.2/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-12 07:10:08.794593 imerit-ango-1.1.2/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 imerit-ango-1.1.2/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:10:08.794593 imerit-ango-1.1.2/imerit_ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-12 06:48:10.000000 imerit-ango-1.1.2/imerit_ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:10:08.794593 imerit-ango-1.1.2/imerit_ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-06-12 06:48:10.000000 imerit-ango-1.1.2/imerit_ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-06-12 06:48:10.000000 imerit-ango-1.1.2/imerit_ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-06-12 06:48:10.000000 imerit-ango-1.1.2/imerit_ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-06-12 06:48:10.000000 imerit-ango-1.1.2/imerit_ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5807 2023-06-12 07:09:17.000000 imerit-ango-1.1.2/imerit_ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14443 2023-06-12 06:48:10.000000 imerit-ango-1.1.2/imerit_ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-12 07:10:08.794593 imerit-ango-1.1.2/imerit_ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1665 2023-06-12 07:10:08.000000 imerit-ango-1.1.2/imerit_ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      383 2023-06-12 07:10:08.000000 imerit-ango-1.1.2/imerit_ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-12 07:10:08.000000 imerit-ango-1.1.2/imerit_ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      137 2023-06-12 07:10:08.000000 imerit-ango-1.1.2/imerit_ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       12 2023-06-12 07:10:08.000000 imerit-ango-1.1.2/imerit_ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-12 07:10:08.794593 imerit-ango-1.1.2/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      892 2023-06-12 07:09:17.000000 imerit-ango-1.1.2/setup.py
```

### Comparing `imerit-ango-1.1.1/PKG-INFO` & `imerit-ango-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.1.1
+Version: 1.1.2
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imerit-ango-1.1.1/README.md` & `imerit-ango-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.1/imerit_ango/models/label_category.py` & `imerit-ango-1.1.2/imerit_ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.1/imerit_ango/plugin_logger.py` & `imerit-ango-1.1.2/imerit_ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.1/imerit_ango/plugins.py` & `imerit-ango-1.1.2/imerit_ango/plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import time
 from io import BytesIO
 from typing import Callable, Tuple
 import queue
 import requests
 import socketio
-from apscheduler.schedulers.asyncio import AsyncIOScheduler
 from apscheduler.schedulers.background import BackgroundScheduler
 
 from imerit_ango.plugin_logger import PluginLogger
 from imerit_ango.sdk import SDK
 
 try:
     import asyncio
@@ -21,29 +20,33 @@
 class Plugin(socketio.ClientNamespace):
 
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__('/plugin')
         self.id = id
         self.secret = secret
         scheduler = BackgroundScheduler()
-        scheduler.add_job(self.heartbeat, 'interval', seconds=60)
+        scheduler.add_job(self.heartbeat, 'interval', seconds=10)
         scheduler.start()
         self.logger = logging.getLogger()
         self.callback = callback
         self.loop = asyncio.get_event_loop()
 
     def on_connect(self):
-        self.heartbeat()
+        #self.heartbeat()
         self.logger.warning("Connected")
 
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
@@ -129,14 +132,15 @@
         self.queue.put(data)
 
     def start(self):
         tasks = [self.work() for i in range(self.concurrency)]
         future = asyncio.gather(*tasks)
         asyncio.get_event_loop().run_until_complete(future)
 
+
 class FileExplorerPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
 
 class BatchModelPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
@@ -149,15 +153,19 @@
 
 
 class MarkdownPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
 
-def run(plugin, host="https://plugin.imerit.ango.ai"):
+def _connect(plugin, host):
     sio = socketio.Client()
     sio.register_namespace(plugin)
-    sio.connect(host, namespaces=["/plugin"], wait_timeout=100)
+    sio.connect(host, namespaces=["/plugin"], wait=True)
+
+
+def run(plugin, host="https://plugin.imerit.ango.ai"):
+    _connect(plugin, host)
     try:
         plugin.start()
     except (KeyboardInterrupt, SystemExit):
         logging.getLogger().warning("Plugin Stopped")
```

### Comparing `imerit-ango-1.1.1/imerit_ango/sdk.py` & `imerit-ango-1.1.2/imerit_ango/sdk.py`

 * *Files identical despite different names*

### Comparing `imerit-ango-1.1.1/imerit_ango.egg-info/PKG-INFO` & `imerit-ango-1.1.2/imerit_ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.1.1
+Version: 1.1.2
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `imerit-ango-1.1.1/setup.py` & `imerit-ango-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="imerit-ango",
-    version="1.1.1",
+    version="1.1.2",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```
