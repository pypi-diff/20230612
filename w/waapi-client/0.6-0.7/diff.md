# Comparing `tmp/waapi-client-0.6.tar.gz` & `tmp/waapi-client-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waapi-client-0.6.tar", last modified: Fri Jun 11 12:59:01 2021, max compression
+gzip compressed data, was "waapi-client-0.7.tar", last modified: Mon Jun 12 14:49:34 2023, max compression
```

## Comparing `waapi-client-0.6.tar` & `waapi-client-0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2021-06-11 12:59:01.049740 waapi-client-0.6/
--rw-rw-rw-   0        0        0    11558 2020-05-06 18:50:42.000000 waapi-client-0.6/LICENSE
--rw-rw-rw-   0        0        0     3298 2021-06-11 12:59:01.050720 waapi-client-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2536 2021-05-26 13:51:33.000000 waapi-client-0.6/README.md
--rw-rw-rw-   0        0        0       86 2021-06-11 12:59:01.051803 waapi-client-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1255 2021-06-11 12:50:31.000000 waapi-client-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-11 12:59:01.020738 waapi-client-0.6/waapi/
--rw-rw-rw-   0        0        0      101 2020-05-06 18:50:42.000000 waapi-client-0.6/waapi/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-11 12:59:01.030752 waapi-client-0.6/waapi/client/
--rw-rw-rw-   0        0        0      106 2021-05-19 18:55:33.000000 waapi-client-0.6/waapi/client/__init__.py
--rw-rw-rw-   0        0        0    12064 2021-05-19 21:17:24.000000 waapi-client-0.6/waapi/client/client.py
--rw-rw-rw-   0        0        0     2775 2020-05-06 18:50:42.000000 waapi-client-0.6/waapi/client/event.py
--rw-rw-rw-   0        0        0     1637 2021-05-25 21:08:24.000000 waapi-client-0.6/waapi/client/executor.py
--rw-rw-rw-   0        0        0      917 2021-05-20 12:56:16.000000 waapi-client-0.6/waapi/client/interface.py
-drwxrwxrwx   0        0        0        0 2021-06-11 12:59:01.039819 waapi-client-0.6/waapi/wamp/
--rw-rw-rw-   0        0        0        0 2020-05-06 18:50:42.000000 waapi-client-0.6/waapi/wamp/__init__.py
--rw-rw-rw-   0        0        0    10053 2021-06-11 12:50:02.000000 waapi-client-0.6/waapi/wamp/ak_autobahn.py
--rw-rw-rw-   0        0        0       89 2021-05-18 15:39:39.000000 waapi-client-0.6/waapi/wamp/async_compatibility.py
--rw-rw-rw-   0        0        0     5495 2021-06-11 12:50:02.000000 waapi-client-0.6/waapi/wamp/async_decoupled_client.py
--rw-rw-rw-   0        0        0     1566 2020-05-06 18:50:42.000000 waapi-client-0.6/waapi/wamp/interface.py
-drwxrwxrwx   0        0        0        0 2021-06-11 12:59:01.048784 waapi-client-0.6/waapi_client.egg-info/
--rw-rw-rw-   0        0        0     3298 2021-06-11 12:59:00.000000 waapi-client-0.6/waapi_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2021-06-11 12:59:00.000000 waapi-client-0.6/waapi_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-11 12:59:00.000000 waapi-client-0.6/waapi_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-06-11 12:59:00.000000 waapi-client-0.6/waapi_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-06-11 12:59:00.000000 waapi-client-0.6/waapi_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 14:49:34.765163 waapi-client-0.7/
+-rw-rw-rw-   0        0        0    11558 2022-10-26 22:05:27.000000 waapi-client-0.7/LICENSE
+-rw-rw-rw-   0        0        0     3493 2023-06-12 14:49:34.765163 waapi-client-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2573 2023-06-12 13:12:32.000000 waapi-client-0.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-12 14:49:34.765163 waapi-client-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1412 2023-06-12 13:12:32.000000 waapi-client-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:49:34.665531 waapi-client-0.7/waapi/
+-rw-rw-rw-   0        0        0      101 2022-10-26 22:05:27.000000 waapi-client-0.7/waapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:49:34.665531 waapi-client-0.7/waapi/client/
+-rw-rw-rw-   0        0        0      106 2022-10-26 22:05:27.000000 waapi-client-0.7/waapi/client/__init__.py
+-rw-rw-rw-   0        0        0    12145 2023-06-12 13:12:32.000000 waapi-client-0.7/waapi/client/client.py
+-rw-rw-rw-   0        0        0     2775 2022-10-26 22:05:27.000000 waapi-client-0.7/waapi/client/event.py
+-rw-rw-rw-   0        0        0     1637 2022-10-26 22:05:27.000000 waapi-client-0.7/waapi/client/executor.py
+-rw-rw-rw-   0        0        0      917 2022-10-26 22:05:27.000000 waapi-client-0.7/waapi/client/interface.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:49:34.728024 waapi-client-0.7/waapi/wamp/
+-rw-rw-rw-   0        0        0        0 2022-10-26 22:05:27.000000 waapi-client-0.7/waapi/wamp/__init__.py
+-rw-rw-rw-   0        0        0     9880 2023-06-12 13:12:32.000000 waapi-client-0.7/waapi/wamp/ak_autobahn.py
+-rw-rw-rw-   0        0        0       89 2022-10-26 22:05:27.000000 waapi-client-0.7/waapi/wamp/async_compatibility.py
+-rw-rw-rw-   0        0        0     5634 2023-06-12 13:12:32.000000 waapi-client-0.7/waapi/wamp/async_decoupled_client.py
+-rw-rw-rw-   0        0        0     1566 2022-10-26 22:05:27.000000 waapi-client-0.7/waapi/wamp/interface.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:49:34.765163 waapi-client-0.7/waapi_client.egg-info/
+-rw-rw-rw-   0        0        0     3493 2023-06-12 14:49:34.000000 waapi-client-0.7/waapi_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2023-06-12 14:49:34.000000 waapi-client-0.7/waapi_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:49:34.000000 waapi-client-0.7/waapi_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 14:49:34.000000 waapi-client-0.7/waapi_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 14:49:34.000000 waapi-client-0.7/waapi_client.egg-info/top_level.txt
```

### Comparing `waapi-client-0.6/LICENSE` & `waapi-client-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `waapi-client-0.6/PKG-INFO` & `waapi-client-0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: waapi-client
-Version: 0.6
+Version: 0.7
 Summary: Wwise Authoring API client.
 Home-page: https://github.com/audiokinetic/waapi-client-python
+Download-URL: https://github.com/audiokinetic/waapi-client-python/releases
 Author: Audiokinetic
 Maintainer: Samuel Longchamps
 Maintainer-email: slongchamps@audiokinetic.com
 License: Apache License 2.0
-Download-URL: https://github.com/audiokinetic/waapi-client-python/releases
 Keywords: waapi,wwise,audiokinetic
 Platform: any
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Wwise Authoring API (Waapi) Client for Python
 Decoupled autobahn WAMP client with support for plain options and bindable subscription callbacks.
 
 ## Requirements
-* Python 3.7, 3.8 or 3.9
-* Wwise instance with the Wwise Authoring API enabled (`Project > User Preferences... > Enable Wwise Authoring API`)
+* Python 3.7+ (see `tox.ini` for versions tested)
+* [Wwise](https://www.audiokinetic.com/en/download) instance with the Wwise Authoring API enabled (`Project > User Preferences... > Enable Wwise Authoring API`)
 
 ## Setup
-For compatibility with Python 2 on Windows, it is recommended to use the [Python Launcher for Windows](https://docs.python.org/3/using/windows.html#launcher) which is installed with Python 3 from [python.org](https://www.python.org).
+On Windows, it is recommended to use the [Python Launcher for Windows](https://docs.python.org/3/using/windows.html#launcher) which is installed with Python 3 from [python.org](https://www.python.org).
 
 * Windows: `py -3 -m pip install waapi-client`
 * Other platforms: `python3 -m pip install waapi-client`
 
 ## Usage
 ```python
 from waapi import WaapiClient
@@ -95,8 +98,7 @@
 * Windows: `py -3 -m pip install tox`
 * Other platforms: `python3 -m pip install tox`
 
 Open a blank project in Wwise, then you may execute `tox` in the terminal from the root of the repository
 
 The test suite will run for all supported versions of Python.
 Use `-e pyXX` to run for a single version, e.g., `tox -e py37` for Python 3.7).
-
```

### Comparing `waapi-client-0.6/README.md` & `waapi-client-0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Wwise Authoring API (Waapi) Client for Python
 Decoupled autobahn WAMP client with support for plain options and bindable subscription callbacks.
 
 ## Requirements
-* Python 3.7, 3.8 or 3.9
-* Wwise instance with the Wwise Authoring API enabled (`Project > User Preferences... > Enable Wwise Authoring API`)
+* Python 3.7+ (see `tox.ini` for versions tested)
+* [Wwise](https://www.audiokinetic.com/en/download) instance with the Wwise Authoring API enabled (`Project > User Preferences... > Enable Wwise Authoring API`)
 
 ## Setup
-For compatibility with Python 2 on Windows, it is recommended to use the [Python Launcher for Windows](https://docs.python.org/3/using/windows.html#launcher) which is installed with Python 3 from [python.org](https://www.python.org).
+On Windows, it is recommended to use the [Python Launcher for Windows](https://docs.python.org/3/using/windows.html#launcher) which is installed with Python 3 from [python.org](https://www.python.org).
 
 * Windows: `py -3 -m pip install waapi-client`
 * Other platforms: `python3 -m pip install waapi-client`
 
 ## Usage
 ```python
 from waapi import WaapiClient
```

### Comparing `waapi-client-0.6/setup.py` & `waapi-client-0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,25 +13,28 @@
     test_suite='waapi.test',
     install_requires=[
       'autobahn'
     ],
     license='Apache License 2.0',
     platforms=['any'],
     scripts=[],
-    version='0.6',
+    version='0.7',
     description='Wwise Authoring API client.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Audiokinetic',
     maintainer='Samuel Longchamps',
     maintainer_email='slongchamps@audiokinetic.com',
     url='https://github.com/audiokinetic/waapi-client-python',
     download_url='https://github.com/audiokinetic/waapi-client-python/releases',
     keywords=['waapi', 'wwise', 'audiokinetic'],
     classifiers=[
         'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3 :: Only',
         'License :: OSI Approved :: Apache Software License',
         'Topic :: Software Development :: Libraries :: Python Modules',
-        'Development Status :: 4 - Beta'
+        'Development Status :: 4 - Beta',
+        'Operating System :: Microsoft :: Windows',
+        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: POSIX :: Linux'
     ],
 )
```

### Comparing `waapi-client-0.6/waapi/client/client.py` & `waapi-client-0.7/waapi/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from sys import platform
+import logging
+from sys import platform, stdout
 from copy import copy
 
 from waapi.client.event import EventHandler
 from waapi.client.interface import UnsubscribeHandler
 from waapi.client.executor import SequentialThreadExecutor
 from waapi.wamp.interface import WampRequest, WampRequestType, CannotConnectToWaapiException, WaapiRequestFailed
 from waapi.wamp.async_decoupled_client import WampClientAutobahn
@@ -19,19 +20,18 @@
     :return: WaapiClient | None
     """
     try:
         return WaapiClient(url)
     except CannotConnectToWaapiException:
         return None
 
-
 def enable_debug_log():
+    logging.basicConfig(stream=stdout, level=logging.DEBUG)
     WampClientAutobahn.enable_debug_log()
 
-
 class WaapiClient(UnsubscribeHandler):
     """
     Pythonic Wwise Authoring API client with a synchronous looking API.
 
     Uses asyncio under the hood in a separate thread to which WAMP requests are dispatched.
     Use as a normal API for interacting with Wwise, requires no other special setup.
     Each subscription to a topic is managed by a EventHandler instance for a reference is kept in this client.
```

### Comparing `waapi-client-0.6/waapi/client/event.py` & `waapi-client-0.7/waapi/client/event.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.6/waapi/client/executor.py` & `waapi-client-0.7/waapi/client/executor.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.6/waapi/client/interface.py` & `waapi-client-0.7/waapi/client/interface.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.6/waapi/wamp/ak_autobahn.py` & `waapi-client-0.7/waapi/wamp/ak_autobahn.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,18 +126,14 @@
     def run(self):
         try:
             asyncio.set_event_loop(self._loop)
 
             txaio.use_asyncio()
             txaio.config.loop = self._loop
 
-            # Info is too verbose, use error by default
-            # TODO: Make logging level for autobahn configurable
-            txaio.start_logging(level='error')
-
             # create a WAMP-over-WebSocket transport client factory
             transport_factory = WampWebSocketClientFactory(
                 lambda: self._akcomponent_factory(self._decoupler, self._callback_executor, self._allow_exception),
                 url=self._url
             )
 
             # Basic settings with most features disabled
```

### Comparing `waapi-client-0.6/waapi/wamp/async_decoupled_client.py` & `waapi-client-0.7/waapi/wamp/async_decoupled_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import logging
+from txaio import make_logger
 from pprint import pformat
 from threading import Thread
 
 from autobahn.wamp import ApplicationError
 
 from waapi.client.interface import CallbackExecutor
 from waapi.wamp.interface import WampRequestType, WampRequest, WaapiRequestFailed
 from waapi.wamp.ak_autobahn import AkComponent
 from waapi.wamp.async_compatibility import asyncio
 
+logger = make_logger()
 
 class WampClientAutobahn(AkComponent):
     """
     Implementation class of a Waapi client using the autobahn library
     """
-    logger = logging.getLogger("WampClientAutobahn")
 
     def __init__(self, decoupler, callback_executor, allow_exception):
         """
         :type decoupler: AutobahnClientDecoupler
         :type callback_executor: CallbackExecutor
         :param allow_exception: True to allow exception, False to ignore them.
                                 In any case they are logged to stderr.
@@ -27,19 +27,19 @@
         super(WampClientAutobahn, self).__init__()
         self._decoupler = decoupler
         self._callback_executor = callback_executor
         self._allow_exception = allow_exception
 
     @classmethod
     def enable_debug_log(cls):
-        cls.logger.setLevel(logging.DEBUG)
+        logger._set_log_level('debug')
 
     @classmethod
     def _log(cls, msg):
-        cls.logger.debug("WampClientAutobahn: %s", msg)
+        logger.debug("WampClientAutobahn: {}".format(msg))
 
     async def stop_handler(self, request):
         """
         :param request: WampRequest
         """
         self._log("Received STOP, stopping and setting the result")
         self._callback_executor.stop()
@@ -110,15 +110,17 @@
                     }.get(request.request_type)
 
                     if handler:
                         await handler(request)
                     else:
                         self._log("Undefined WampRequestType")
                 except ApplicationError as e:
-                    self.logger.error("WampClientAutobahn (ERROR): " + pformat(str(e)))
+                    sanitized_exception_str = str(e).replace("{", "{{").replace("}", "}}")
+                    error_message = "WampClientAutobahn (ERROR): " + pformat(sanitized_exception_str)
+                    logger.error(error_message)
 
                     if self._allow_exception:
                         request.future.set_exception(WaapiRequestFailed(e))
                     else:
                         request.future.set_result(None)
 
                 self._log("Done treating request")
```

### Comparing `waapi-client-0.6/waapi/wamp/interface.py` & `waapi-client-0.7/waapi/wamp/interface.py`

 * *Files identical despite different names*

### Comparing `waapi-client-0.6/waapi_client.egg-info/PKG-INFO` & `waapi-client-0.7/waapi_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: waapi-client
-Version: 0.6
+Version: 0.7
 Summary: Wwise Authoring API client.
 Home-page: https://github.com/audiokinetic/waapi-client-python
+Download-URL: https://github.com/audiokinetic/waapi-client-python/releases
 Author: Audiokinetic
 Maintainer: Samuel Longchamps
 Maintainer-email: slongchamps@audiokinetic.com
 License: Apache License 2.0
-Download-URL: https://github.com/audiokinetic/waapi-client-python/releases
 Keywords: waapi,wwise,audiokinetic
 Platform: any
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Wwise Authoring API (Waapi) Client for Python
 Decoupled autobahn WAMP client with support for plain options and bindable subscription callbacks.
 
 ## Requirements
-* Python 3.7, 3.8 or 3.9
-* Wwise instance with the Wwise Authoring API enabled (`Project > User Preferences... > Enable Wwise Authoring API`)
+* Python 3.7+ (see `tox.ini` for versions tested)
+* [Wwise](https://www.audiokinetic.com/en/download) instance with the Wwise Authoring API enabled (`Project > User Preferences... > Enable Wwise Authoring API`)
 
 ## Setup
-For compatibility with Python 2 on Windows, it is recommended to use the [Python Launcher for Windows](https://docs.python.org/3/using/windows.html#launcher) which is installed with Python 3 from [python.org](https://www.python.org).
+On Windows, it is recommended to use the [Python Launcher for Windows](https://docs.python.org/3/using/windows.html#launcher) which is installed with Python 3 from [python.org](https://www.python.org).
 
 * Windows: `py -3 -m pip install waapi-client`
 * Other platforms: `python3 -m pip install waapi-client`
 
 ## Usage
 ```python
 from waapi import WaapiClient
@@ -95,8 +98,7 @@
 * Windows: `py -3 -m pip install tox`
 * Other platforms: `python3 -m pip install tox`
 
 Open a blank project in Wwise, then you may execute `tox` in the terminal from the root of the repository
 
 The test suite will run for all supported versions of Python.
 Use `-e pyXX` to run for a single version, e.g., `tox -e py37` for Python 3.7).
-
```

