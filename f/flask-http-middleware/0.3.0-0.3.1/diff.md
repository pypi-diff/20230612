# Comparing `tmp/flask-http-middleware-0.3.0.tar.gz` & `tmp/flask-http-middleware-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-http-middleware-0.3.0.tar", last modified: Mon Jun 12 14:24:06 2023, max compression
+gzip compressed data, was "flask-http-middleware-0.3.1.tar", last modified: Mon Jun 12 14:29:37 2023, max compression
```

## Comparing `flask-http-middleware-0.3.0.tar` & `flask-http-middleware-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1068 2022-03-20 12:47:01.000000 flask-http-middleware-0.3.0/LICENSE
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7309 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     6370 2023-06-12 14:24:02.000000 flask-http-middleware-0.3.0/README.md
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/flask_http_middleware/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2022-03-20 12:14:27.000000 flask-http-middleware-0.3.0/flask_http_middleware/__init__.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1707 2022-03-20 12:35:18.000000 flask-http-middleware-0.3.0/flask_http_middleware/base.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7493 2023-06-12 14:20:09.000000 flask-http-middleware-0.3.0/flask_http_middleware/manager.py
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7309 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      347 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/SOURCES.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/dependency_links.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       15 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/requires.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/top_level.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/setup.cfg
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1384 2023-06-12 14:23:32.000000 flask-http-middleware-0.3.0/setup.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:29:37.502854 flask-http-middleware-0.3.1/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1068 2022-03-20 12:47:01.000000 flask-http-middleware-0.3.1/LICENSE
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7309 2023-06-12 14:29:37.502854 flask-http-middleware-0.3.1/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     6370 2023-06-12 14:24:02.000000 flask-http-middleware-0.3.1/README.md
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:29:37.498854 flask-http-middleware-0.3.1/flask_http_middleware/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2022-03-20 12:14:27.000000 flask-http-middleware-0.3.1/flask_http_middleware/__init__.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1726 2023-06-12 14:28:56.000000 flask-http-middleware-0.3.1/flask_http_middleware/base.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7493 2023-06-12 14:20:09.000000 flask-http-middleware-0.3.1/flask_http_middleware/manager.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:29:37.502854 flask-http-middleware-0.3.1/flask_http_middleware.egg-info/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7309 2023-06-12 14:29:37.000000 flask-http-middleware-0.3.1/flask_http_middleware.egg-info/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      347 2023-06-12 14:29:37.000000 flask-http-middleware-0.3.1/flask_http_middleware.egg-info/SOURCES.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-06-12 14:29:37.000000 flask-http-middleware-0.3.1/flask_http_middleware.egg-info/dependency_links.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       15 2023-06-12 14:29:37.000000 flask-http-middleware-0.3.1/flask_http_middleware.egg-info/requires.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2023-06-12 14:29:37.000000 flask-http-middleware-0.3.1/flask_http_middleware.egg-info/top_level.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-06-12 14:29:37.502854 flask-http-middleware-0.3.1/setup.cfg
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1384 2023-06-12 14:29:29.000000 flask-http-middleware-0.3.1/setup.py
```

### Comparing `flask-http-middleware-0.3.0/LICENSE` & `flask-http-middleware-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-http-middleware-0.3.0/PKG-INFO` & `flask-http-middleware-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-http-middleware
-Version: 0.3.0
+Version: 0.3.1
 Summary: A module to create middleware with direct access to `request` and `response`
 Home-page: https://github.com/Danangjoyoo/flask-http-middleware
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
 Keywords: flask,middleware,http,request,response
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `flask-http-middleware-0.3.0/README.md` & `flask-http-middleware-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flask-http-middleware-0.3.0/flask_http_middleware/base.py` & `flask-http-middleware-0.3.1/flask_http_middleware/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import typing as t
 from abc import ABC, abstractmethod
 from flask import Request, Response
+from typing import Any, Callable
 
 class BaseHTTPMiddleware(ABC):
     """
     BaseHTTPMiddleware
 
     A base class to create an HTTP Middleware by using dispatch function.
     Inherit this class to make it
@@ -12,21 +12,21 @@
     @abstractmethod
     def __init__(self):
         """
         You have to add `__init__` function into your classes.
         Error will raised if you dont have this function
         """
         pass
-    
+
     @abstractmethod
-    def dispatch(self, request: Request, call_next: callable) -> Response:
+    def dispatch(self, request: Request, call_next: Callable) -> Response:
         """
         You have to override this function in your custom middleware class.
         Error will raised if you dont have this function
-        
+
         The templates are :
         ```
         def dispatch(self, request, call_next):
             ## put your pre-process/before-request here
             response = call_next(request)
             ## put your post-process/after-request here
             return response
@@ -37,19 +37,19 @@
         - you could:
             - modify the `response`
             - return custom `response`
             - raise the `exception`
         """
         pass
 
-    def error_handler(self, error: t.Any):
+    def error_handler(self, error: Any):
         """
         Override this function if you want to add error handling in your middleware.
         if not, any exception will be raised
         """
         raise error
 
-    def _dispatch_with_handler(self, request, call_next):
+    def _dispatch_with_handler(self, request: Request, call_next: Callable):
         try:
             return self.dispatch(request, call_next)
         except Exception as e:
             return self.error_handler(e)
```

### Comparing `flask-http-middleware-0.3.0/flask_http_middleware/manager.py` & `flask-http-middleware-0.3.1/flask_http_middleware/manager.py`

 * *Files identical despite different names*

### Comparing `flask-http-middleware-0.3.0/flask_http_middleware.egg-info/PKG-INFO` & `flask-http-middleware-0.3.1/flask_http_middleware.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-http-middleware
-Version: 0.3.0
+Version: 0.3.1
 Summary: A module to create middleware with direct access to `request` and `response`
 Home-page: https://github.com/Danangjoyoo/flask-http-middleware
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
 Keywords: flask,middleware,http,request,response
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `flask-http-middleware-0.3.0/setup.py` & `flask-http-middleware-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 DESCRIPTION = "A module to create middleware with direct access to `request` and `response`"
 
 # Setting up
 setup(
     name="flask-http-middleware",
     version=VERSION,
     author="danangjoyoo (Agus Danangjoyo)",
```

