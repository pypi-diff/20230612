# Comparing `tmp/selfbotclient-1.0.1.tar.gz` & `tmp/selfbotclient-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfbotclient-1.0.1.tar", last modified: Fri Jun  9 22:56:53 2023, max compression
+gzip compressed data, was "selfbotclient-1.0.2.tar", last modified: Mon Jun 12 19:42:16 2023, max compression
```

## Comparing `selfbotclient-1.0.1.tar` & `selfbotclient-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 22:56:53.656158 selfbotclient-1.0.1/
--rw-rw-rw-   0        0        0     1161 2023-06-09 22:56:53.655158 selfbotclient-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-06-09 22:56:48.000000 selfbotclient-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 22:56:53.647157 selfbotclient-1.0.1/SelfBotClient/
--rw-rw-rw-   0        0        0      376 2023-06-09 22:25:15.000000 selfbotclient-1.0.1/SelfBotClient/__init__.py
--rw-rw-rw-   0        0        0      472 2023-06-09 21:55:30.000000 selfbotclient-1.0.1/SelfBotClient/__main__.py
--rw-rw-rw-   0        0        0    16893 2023-06-09 22:56:48.000000 selfbotclient-1.0.1/SelfBotClient/client.py
--rw-rw-rw-   0        0        0     1399 2023-06-07 23:57:30.000000 selfbotclient-1.0.1/SelfBotClient/enums.py
--rw-rw-rw-   0        0        0      826 2023-06-06 22:37:48.000000 selfbotclient-1.0.1/SelfBotClient/errors.py
--rw-rw-rw-   0        0        0    11955 2023-06-09 21:57:25.000000 selfbotclient-1.0.1/SelfBotClient/http.py
--rw-rw-rw-   0        0        0     1046 2023-06-08 23:49:03.000000 selfbotclient-1.0.1/SelfBotClient/logger.py
--rw-rw-rw-   0        0        0      807 2023-06-09 13:27:08.000000 selfbotclient-1.0.1/SelfBotClient/permissionbuilder.py
--rw-rw-rw-   0        0        0      313 2023-06-07 23:24:53.000000 selfbotclient-1.0.1/SelfBotClient/typings.py
--rw-rw-rw-   0        0        0    17057 2023-06-09 21:55:30.000000 selfbotclient-1.0.1/SelfBotClient/user.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:56:53.655158 selfbotclient-1.0.1/selfbotclient.egg-info/
--rw-rw-rw-   0        0        0     1161 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-09 22:56:53.000000 selfbotclient-1.0.1/selfbotclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 22:56:53.656158 selfbotclient-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-06-09 22:56:48.000000 selfbotclient-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 19:42:16.776562 selfbotclient-1.0.2/
+-rw-rw-rw-   0        0        0     1459 2023-06-12 19:42:16.776562 selfbotclient-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2023-06-12 19:38:25.000000 selfbotclient-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 19:42:16.766562 selfbotclient-1.0.2/SelfBotClient/
+-rw-rw-rw-   0        0        0      376 2023-06-12 19:28:12.000000 selfbotclient-1.0.2/SelfBotClient/__init__.py
+-rw-rw-rw-   0        0        0      472 2023-06-09 23:04:28.000000 selfbotclient-1.0.2/SelfBotClient/__main__.py
+-rw-rw-rw-   0        0        0    17005 2023-06-12 19:35:33.000000 selfbotclient-1.0.2/SelfBotClient/client.py
+-rw-rw-rw-   0        0        0     1399 2023-06-07 23:57:30.000000 selfbotclient-1.0.2/SelfBotClient/enums.py
+-rw-rw-rw-   0        0        0      826 2023-06-06 22:37:48.000000 selfbotclient-1.0.2/SelfBotClient/errors.py
+-rw-rw-rw-   0        0        0    11955 2023-06-09 21:57:25.000000 selfbotclient-1.0.2/SelfBotClient/http.py
+-rw-rw-rw-   0        0        0     1046 2023-06-08 23:49:03.000000 selfbotclient-1.0.2/SelfBotClient/logger.py
+-rw-rw-rw-   0        0        0      807 2023-06-09 13:27:08.000000 selfbotclient-1.0.2/SelfBotClient/permissionbuilder.py
+-rw-rw-rw-   0        0        0     1124 2023-06-12 19:29:03.000000 selfbotclient-1.0.2/SelfBotClient/threads.py
+-rw-rw-rw-   0        0        0      313 2023-06-07 23:24:53.000000 selfbotclient-1.0.2/SelfBotClient/typings.py
+-rw-rw-rw-   0        0        0    17057 2023-06-09 21:55:30.000000 selfbotclient-1.0.2/SelfBotClient/user.py
+drwxrwxrwx   0        0        0        0 2023-06-12 19:42:16.775563 selfbotclient-1.0.2/selfbotclient.egg-info/
+-rw-rw-rw-   0        0        0     1459 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-12 19:42:16.000000 selfbotclient-1.0.2/selfbotclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 19:42:16.777562 selfbotclient-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2023-06-12 19:42:13.000000 selfbotclient-1.0.2/setup.py
```

### Comparing `selfbotclient-1.0.1/PKG-INFO` & `selfbotclient-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 Metadata-Version: 2.1
 Name: selfbotclient
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library that will allow you to manage selfbots
-Home-page: UNKNOWN
 Author: xXenvy
 Author-email: <xpimepk01@gmail.com>
-License: UNKNOWN
 Keywords: python,requests,discord selfbot,selfbot,discord.py,aiohttp
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
-# Self Bot Client
-## ⚡ Fast SelfBotClient
+
+# ⚡ Fast Self Bot Client
 - Token Checker | `1` token / `140`ms
 - 3 requests / 1s `(in feature 10 requests / 1s using threads)`
 
-## 🔧 Full control
+
+https://github.com/xXenvy/SelfBotClient/assets/111158232/eb5961eb-0a8d-44f1-93b0-48d7a1f6fce0
+
+
+# 🔧 Full control
 - A separate method to send your own requests
 - Ability to manage individual selfbots
 
-## 📌 Ratelimit handler
+# 📌 Ratelimit handler
 
 - The library itself detects whether you have reached the ratelimit of the discord and, if so, forces you to wait a certain time.
+# 🛠️ Installation
+```shell
+pip install -U selfbotclient
+```
+# 💫 Usage
+```py
+from SelfBotClient import Client
 
-## 💫 Examples
-**See examples on github:** https://github.com/xXenvy?tab=repositories
-
-
+tokens: list[str] = ["TOKEN_1", "TOKEN_2"]
+
+client: Client = Client(api_version=10)
+client.login(token=tokens)
+```
+**See more examples on github:** [Examples](https://github.com/xXenvy/SelfBotClient/tree/master/examples)
```

### Comparing `selfbotclient-1.0.1/SelfBotClient/client.py` & `selfbotclient-1.0.2/SelfBotClient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 from .http import HTTPClient
 from .typings import API_VERSION, ClientResponse, RGB_COLOR
 from .enums import ChannelType
 from .permissionbuilder import PermissionBuilder
+from .threads import Threads
+
 from collections.abc import AsyncIterable
 
 from typing import Union
 from asyncio import AbstractEventLoop
 
 
 class Client(HTTPClient):
-    __version__: str = "1.0.1"
+    __version__: str = "1.0.2"
 
     def __init__(
             self,
             api_version: API_VERSION,
             loop: AbstractEventLoop = None,
             logger: bool = True,
             request_latency: float = 0.1,
-            ratelimit_additional_cooldown: float = 10
+            ratelimit_additional_cooldown: float = 10,
+            use_threading: bool = False
     ):
-
         """
         The __init__ function is called when the class is instantiated.
-        It sets up all of the attributes that we will need for our API wrapper to function properly.
-        The super() call invokes the __init__ method of our parent class, which in this case is BaseClient.
+        It sets up all of the attributes that are needed for the class to function properly.
+
 
         :param self: Represent the instance of the class
-        :param api_version: API_VERSION: Specify the version of the api you want to use
-        :param loop: AbstractEventLoop: Set the event loop for the client
-        :param logger: bool: Enable or disable logging
-        :param request_latency: float: Set the delay between requests
+        :param api_version: API_VERSION: Set the api version of the client
+        :param loop: AbstractEventLoop: Specify the event loop that the client will use
+        :param logger: bool: Enable/disable logging
+        :param request_latency: float: Set the time between requests
         :param ratelimit_additional_cooldown: float: Add a cooldown to the ratelimit
-        :return: The class itself
+        :param use_threading: bool: Determine if the client should use threading
+        :return: None
         """
+
         super().__init__(api_version, loop, logger, request_latency, ratelimit_additional_cooldown)
 
+        if use_threading:
+            self.thread: Threads = Threads(client=self)
+
     def login(self, token: Union[str, list[str]]) -> None:
         """
         The login function is used to check the provided tokens.
 
         :param self: Represent the instance of the class
         :param token: Union[str, list[str]] tokens to check
         :return: None
```

### Comparing `selfbotclient-1.0.1/SelfBotClient/enums.py` & `selfbotclient-1.0.2/SelfBotClient/enums.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.1/SelfBotClient/errors.py` & `selfbotclient-1.0.2/SelfBotClient/errors.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.1/SelfBotClient/http.py` & `selfbotclient-1.0.2/SelfBotClient/http.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.1/SelfBotClient/logger.py` & `selfbotclient-1.0.2/SelfBotClient/logger.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.1/SelfBotClient/permissionbuilder.py` & `selfbotclient-1.0.2/SelfBotClient/permissionbuilder.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.1/SelfBotClient/user.py` & `selfbotclient-1.0.2/SelfBotClient/user.py`

 * *Files identical despite different names*

### Comparing `selfbotclient-1.0.1/selfbotclient.egg-info/PKG-INFO` & `selfbotclient-1.0.2/selfbotclient.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 Metadata-Version: 2.1
 Name: selfbotclient
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library that will allow you to manage selfbots
-Home-page: UNKNOWN
 Author: xXenvy
 Author-email: <xpimepk01@gmail.com>
-License: UNKNOWN
 Keywords: python,requests,discord selfbot,selfbot,discord.py,aiohttp
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
-# Self Bot Client
-## ⚡ Fast SelfBotClient
+
+# ⚡ Fast Self Bot Client
 - Token Checker | `1` token / `140`ms
 - 3 requests / 1s `(in feature 10 requests / 1s using threads)`
 
-## 🔧 Full control
+
+https://github.com/xXenvy/SelfBotClient/assets/111158232/eb5961eb-0a8d-44f1-93b0-48d7a1f6fce0
+
+
+# 🔧 Full control
 - A separate method to send your own requests
 - Ability to manage individual selfbots
 
-## 📌 Ratelimit handler
+# 📌 Ratelimit handler
 
 - The library itself detects whether you have reached the ratelimit of the discord and, if so, forces you to wait a certain time.
+# 🛠️ Installation
+```shell
+pip install -U selfbotclient
+```
+# 💫 Usage
+```py
+from SelfBotClient import Client
 
-## 💫 Examples
-**See examples on github:** https://github.com/xXenvy?tab=repositories
-
-
+tokens: list[str] = ["TOKEN_1", "TOKEN_2"]
+
+client: Client = Client(api_version=10)
+client.login(token=tokens)
+```
+**See more examples on github:** [Examples](https://github.com/xXenvy/SelfBotClient/tree/master/examples)
```

### Comparing `selfbotclient-1.0.1/setup.py` & `selfbotclient-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'Library that will allow you to manage selfbots'
 LONG_DESCRIPTION = 'The library logs into your account thanks to the entered tokens and can manage them. ' \
                    'such as sending messages, deleting roles, etc.'
 
 # Setting up
 setup(
     name="selfbotclient",
```

