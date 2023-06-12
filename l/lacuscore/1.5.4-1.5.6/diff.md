# Comparing `tmp/lacuscore-1.5.4.tar.gz` & `tmp/lacuscore-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.5.4.tar", max compression
+gzip compressed data, was "lacuscore-1.5.6.tar", max compression
```

## Comparing `lacuscore-1.5.4.tar` & `lacuscore-1.5.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.4/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.4/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.4/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.4/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    30256 2023-06-06 15:32:38.124708 lacuscore-1.5.4/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.4/lacuscore/py.typed
--rw-r--r--   0        0        0     1596 2023-06-06 15:46:41.236903 lacuscore-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.6/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.6/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.6/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.6/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    30864 2023-06-12 13:01:08.565874 lacuscore-1.5.6/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.6/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-06-12 13:42:13.284994 lacuscore-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.6/PKG-INFO
```

### Comparing `lacuscore-1.5.4/LICENSE` & `lacuscore-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.4/README.md` & `lacuscore-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.4/lacuscore/lacus_monitoring.py` & `lacuscore-1.5.6/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.4/lacuscore/lacuscore.py` & `lacuscore-1.5.6/lacuscore/lacuscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 import json
 import logging
 import os
 import pickle
 import random
 import re
 import socket
+import sys
 import time
 import unicodedata
+import zlib
 
 from asyncio import Task
 from base64 import b64decode, b64encode
 from enum import IntEnum, unique
 from logging import LoggerAdapter
 from pathlib import Path
 from tempfile import NamedTemporaryFile
@@ -320,34 +322,34 @@
         mapping_capture: Dict[str, Union[bytes, float, int, str]] = {}
         for key, value in to_enqueue.items():
             if isinstance(value, bool):
                 mapping_capture[key] = 1 if value else 0
             elif isinstance(value, (list, dict)):
                 if value:
                     mapping_capture[key] = json.dumps(value)
-            elif value is not None:
+            elif value is not None and value != '':  # we're ok with 0 for example
                 mapping_capture[key] = value  # type: ignore
 
         p = self.redis.pipeline()
         p.set(f'lacus:query_hash:{hash_query}', perma_uuid, nx=True, ex=recapture_interval)
         p.hset(f'lacus:capture_settings:{perma_uuid}', mapping=mapping_capture)  # type: ignore
         p.zadd('lacus:to_capture', {perma_uuid: priority})
         p.execute()
         return perma_uuid
 
-    def _decode_response(self, capture: CaptureResponseJson) -> CaptureResponse:
-        decoded_capture = cast(CaptureResponse, capture)
+    def _encode_response(self, capture: CaptureResponse) -> CaptureResponseJson:
+        encoded_capture = cast(CaptureResponseJson, capture)
         if capture.get('png') and capture['png']:
-            decoded_capture['png'] = b64decode(capture['png'])
+            encoded_capture['png'] = b64encode(capture['png']).decode()
         if capture.get('downloaded_file') and capture['downloaded_file']:
-            decoded_capture['downloaded_file'] = b64decode(capture['downloaded_file'])
+            encoded_capture['downloaded_file'] = b64encode(capture['downloaded_file']).decode()
         if capture.get('children') and capture['children']:
             for child in capture['children']:
-                child = self._decode_response(child)
-        return decoded_capture
+                child = self._encode_response(child)
+        return encoded_capture
 
     @overload
     def get_capture(self, uuid: str, *, decode: Literal[True]=True) -> CaptureResponse:
         ...
 
     @overload
     def get_capture(self, uuid: str, *, decode: Literal[False]) -> CaptureResponseJson:
@@ -357,24 +359,26 @@
         """Get the results of a capture, in a json compatible format or not
 
         :param uuid: The UUID if the capture (given by enqueue)
         :param decode: Decode the capture result or not.
 
         :return: The capture, decoded or not.
         """
-        to_return: CaptureResponseJson = {'status': CaptureStatus.UNKNOWN}
+        to_return: CaptureResponse = {'status': CaptureStatus.UNKNOWN}
         if self.redis.zscore('lacus:to_capture', uuid):
             to_return['status'] = CaptureStatus.QUEUED
         elif self.redis.zscore('lacus:ongoing', uuid) is not None:
             to_return['status'] = CaptureStatus.ONGOING
         elif response := self.redis.get(f'lacus:capture_results:{uuid}'):
             to_return['status'] = CaptureStatus.DONE
-            to_return.update(json.loads(response))
+            response_json = pickle.loads(zlib.decompress(response))
+            to_return.update(response_json)
             if decode:
-                return self._decode_response(to_return)
+                return to_return
+            return self._encode_response(to_return)
         return to_return
 
     def get_capture_status(self, uuid: str) -> CaptureStatus:
         """Get the status of a capture
 
         :param uuid: The UUID if the capture (given by enqueue)
 
@@ -469,26 +473,30 @@
                 raise CaptureError
 
             if document_as_bytes:
                 # we do not have a URL yet.
                 name = to_capture.pop('document_name', None)
                 if not name:
                     raise LacusCoreException('No document name provided, settings are invalid')
+                if not Path(name).suffix:
+                    # The browser will simply display the file as text if there is no extension.
+                    # Just add HTML as a fallback, as it will be the most comon one.
+                    name = f'{name}.html'
                 document_name = Path(name).name
                 tmp_f = NamedTemporaryFile(suffix=document_name, delete=False)
                 with open(tmp_f.name, "wb") as f:
                     f.write(document_as_bytes)
                 url = f'file://{tmp_f.name}'
             elif to_capture.get('url') and to_capture['url'] is not None:
                 url = to_capture['url'].strip()
                 url = refang(url)  # In case we get a defanged url at this stage.
-                if url.lower().startswith('file') and self.only_global_lookups:
+                if url.lower().startswith('file:') and self.only_global_lookups:
                     result = {'error': f'Not allowed to capture a file on disk: {url}'}
                     raise CaptureError
-                if not url.lower().startswith('data') and not url.lower().startswith('http') and not url.lower().startswith('file'):
+                if not url.lower().startswith('data') and not url.lower().startswith('http') and not url.lower().startswith('file:'):
                     url = f'http://{url}'
             else:
                 result = {'error': f'No valid URL to capture for {uuid} - {to_capture}'}
                 raise CaptureError
 
             splitted_url = urlsplit(url)
             proxy = to_capture.get('proxy')
@@ -528,15 +536,14 @@
                 browser_family = parsed_string['family'].lower()
                 if browser_family.startswith('chrom'):
                     browser_engine = 'chromium'
                 elif browser_family.startswith('firefox'):
                     browser_engine = 'firefox'
                 else:
                     browser_engine = 'webkit'
-
             try:
                 logger.debug(f'Capturing {url}')
                 # NOTE: starting with python 3.11, we can use asyncio.timeout
                 # async with asyncio.timeout(self.max_capture_time):
                 general_timeout = to_capture.get('general_timeout_in_sec')
                 async with Capture(
                         browser=browser_engine,
@@ -625,31 +632,34 @@
 
             if to_capture.get('document'):
                 os.unlink(tmp_f.name)
 
             retry_redis_error = 3
             while retry_redis_error > 0:
                 try:
+                    to_store = b''
                     p = self.redis.pipeline()
                     if retry:
                         p.zadd('lacus:to_capture', {uuid: priority - 1})
                     else:
-                        p.setex(f'lacus:capture_results:{uuid}', 36000, json.dumps(result, default=_json_encode))
+                        to_store = zlib.compress(pickle.dumps(result))
+                        p.setex(f'lacus:capture_results:{uuid}', 36000, to_store)
                         p.delete(f'lacus:capture_settings:{uuid}')
                     p.zrem('lacus:ongoing', uuid)
                     p.execute()
                     break
                 except RedisConnectionError as e:
-                    logger.warning(f'Redis Connection Error: {e}')
+                    logger.warning(f'Unable to store capture result (size: {sys.getsizeof(to_store)} - Redis Connection Error: {e}')
                     retry_redis_error -= 1
                     await asyncio.sleep(random.randint(5, 10))
             else:
                 logger.critical('Unable to connect to redis and to push the result of the capture.')
 
     def clear_capture(self, uuid: str, reason: str):
         '''Remove a capture from the list, shouldn't happen unless it is in error'''
         result = {'error': reason}
         p = self.redis.pipeline()
-        p.setex(f'lacus:capture_results:{uuid}', 36000, json.dumps(result, default=_json_encode))
+        to_store = zlib.compress(pickle.dumps(result))
+        p.setex(f'lacus:capture_results:{uuid}', 36000, to_store)
         p.delete(f'lacus:capture_settings:{uuid}')
         p.zrem('lacus:ongoing', uuid)
         p.execute()
```

### Comparing `lacuscore-1.5.4/pyproject.toml` & `lacuscore-1.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.5.4"
+version = "1.5.6"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -28,15 +28,15 @@
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 Sphinx = { version = "^7.0.1", optional = true }
-playwrightcapture = {extras = ["recaptcha"], version = "^1.20.3"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.20.4"}
 defang = "^0.5.3"
 ua-parser = "^0.16.1"
 redis = {version = "^4.5.5", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
@@ -44,12 +44,12 @@
 types-redis = {version = "^4.5.5.2"}
 mypy = "^1.3.0"
 types-requests = "^2.31.0.1"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.13.0", python = ">=3.9"}
 ]
-pytest = "^7.3.1"
+pytest = "^7.3.2"
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lacuscore-1.5.4/PKG-INFO` & `lacuscore-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.5.4
+Version: 1.5.6
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=7.0.1,<8.0.0) ; extra == "docs"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.20.3,<2.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.20.4,<2.0.0)
 Requires-Dist: redis[hiredis] (>=4.5.5,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
```

