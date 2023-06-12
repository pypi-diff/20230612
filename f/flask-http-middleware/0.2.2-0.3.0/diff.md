# Comparing `tmp/flask-http-middleware-0.2.2.tar.gz` & `tmp/flask-http-middleware-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-http-middleware-0.2.2.tar", last modified: Mon Jun 12 14:21:51 2023, max compression
+gzip compressed data, was "flask-http-middleware-0.3.0.tar", last modified: Mon Jun 12 14:24:06 2023, max compression
```

## Comparing `flask-http-middleware-0.2.2.tar` & `flask-http-middleware-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:21:51.206378 flask-http-middleware-0.2.2/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1068 2022-03-20 12:47:01.000000 flask-http-middleware-0.2.2/LICENSE
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7286 2023-06-12 14:21:51.206378 flask-http-middleware-0.2.2/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     6347 2022-12-30 02:41:47.000000 flask-http-middleware-0.2.2/README.md
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:21:51.202379 flask-http-middleware-0.2.2/flask_http_middleware/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2022-03-20 12:14:27.000000 flask-http-middleware-0.2.2/flask_http_middleware/__init__.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1707 2022-03-20 12:35:18.000000 flask-http-middleware-0.2.2/flask_http_middleware/base.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7493 2023-06-12 14:20:09.000000 flask-http-middleware-0.2.2/flask_http_middleware/manager.py
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:21:51.202379 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7286 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      347 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/SOURCES.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/dependency_links.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       15 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/requires.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/top_level.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-06-12 14:21:51.206378 flask-http-middleware-0.2.2/setup.cfg
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1384 2023-06-12 14:21:28.000000 flask-http-middleware-0.2.2/setup.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1068 2022-03-20 12:47:01.000000 flask-http-middleware-0.3.0/LICENSE
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7309 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     6370 2023-06-12 14:24:02.000000 flask-http-middleware-0.3.0/README.md
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/flask_http_middleware/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2022-03-20 12:14:27.000000 flask-http-middleware-0.3.0/flask_http_middleware/__init__.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1707 2022-03-20 12:35:18.000000 flask-http-middleware-0.3.0/flask_http_middleware/base.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7493 2023-06-12 14:20:09.000000 flask-http-middleware-0.3.0/flask_http_middleware/manager.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7309 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      347 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/SOURCES.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/dependency_links.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       15 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/requires.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2023-06-12 14:24:06.000000 flask-http-middleware-0.3.0/flask_http_middleware.egg-info/top_level.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-06-12 14:24:06.539530 flask-http-middleware-0.3.0/setup.cfg
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1384 2023-06-12 14:23:32.000000 flask-http-middleware-0.3.0/setup.py
```

### Comparing `flask-http-middleware-0.2.2/LICENSE` & `flask-http-middleware-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-http-middleware-0.2.2/PKG-INFO` & `flask-http-middleware-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-http-middleware
-Version: 0.2.2
+Version: 0.3.0
 Summary: A module to create middleware with direct access to `request` and `response`
 Home-page: https://github.com/Danangjoyoo/flask-http-middleware
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
 Keywords: flask,middleware,http,request,response
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -36,15 +36,17 @@
 
 ## Changelogs
 - v0.0
     - First Upload
 - v0.1
     - Allow middlewares stacking
 - v0.2
-    - Adjusting wsgi middleware update for `flask>=2.2.x`
+    - Add support for `flask>=2.2.x`
+- v0.3
+    - Add support for `flask>=2.3.x`
 
 ## How to use ?
 
 ### Example: adding a response header
 ```
 import time
 from flask import Flask
```

### Comparing `flask-http-middleware-0.2.2/README.md` & `flask-http-middleware-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 ## Changelogs
 - v0.0
     - First Upload
 - v0.1
     - Allow middlewares stacking
 - v0.2
-    - Adjusting wsgi middleware update for `flask>=2.2.x`
+    - Add support for `flask>=2.2.x`
+- v0.3
+    - Add support for `flask>=2.3.x`
 
 ## How to use ?
 
 ### Example: adding a response header
 ```
 import time
 from flask import Flask
```

### Comparing `flask-http-middleware-0.2.2/flask_http_middleware/base.py` & `flask-http-middleware-0.3.0/flask_http_middleware/base.py`

 * *Files identical despite different names*

### Comparing `flask-http-middleware-0.2.2/flask_http_middleware/manager.py` & `flask-http-middleware-0.3.0/flask_http_middleware/manager.py`

 * *Files identical despite different names*

### Comparing `flask-http-middleware-0.2.2/flask_http_middleware.egg-info/PKG-INFO` & `flask-http-middleware-0.3.0/flask_http_middleware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-http-middleware
-Version: 0.2.2
+Version: 0.3.0
 Summary: A module to create middleware with direct access to `request` and `response`
 Home-page: https://github.com/Danangjoyoo/flask-http-middleware
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
 Keywords: flask,middleware,http,request,response
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -36,15 +36,17 @@
 
 ## Changelogs
 - v0.0
     - First Upload
 - v0.1
     - Allow middlewares stacking
 - v0.2
-    - Adjusting wsgi middleware update for `flask>=2.2.x`
+    - Add support for `flask>=2.2.x`
+- v0.3
+    - Add support for `flask>=2.3.x`
 
 ## How to use ?
 
 ### Example: adding a response header
 ```
 import time
 from flask import Flask
```

### Comparing `flask-http-middleware-0.2.2/setup.py` & `flask-http-middleware-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = "0.2.2"
+VERSION = "0.3.0"
 DESCRIPTION = "A module to create middleware with direct access to `request` and `response`"
 
 # Setting up
 setup(
     name="flask-http-middleware",
     version=VERSION,
     author="danangjoyoo (Agus Danangjoyo)",
```

