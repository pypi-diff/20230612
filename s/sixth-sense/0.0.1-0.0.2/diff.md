# Comparing `tmp/sixth-sense-0.0.1.tar.gz` & `tmp/sixth-sense-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sixth-sense-0.0.1.tar", last modified: Mon Jun 12 01:08:16 2023, max compression
+gzip compressed data, was "dist/sixth-sense-0.0.2.tar", last modified: Mon Jun 12 01:10:20 2023, max compression
```

## Comparing `sixth-sense-0.0.1.tar` & `sixth-sense-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/
--rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)       20 2023-06-09 19:50:05.000000 sixth-sense-0.0.1/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     2014 2023-06-12 01:07:15.000000 sixth-sense-0.0.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/six_python/
--rw-r--r--   0 mac        (501) staff       (20)       45 2023-06-11 23:24:34.000000 sixth-sense-0.0.1/six_python/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/six_python/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-sense-0.0.1/six_python/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3738 2023-06-11 22:37:24.000000 sixth-sense-0.0.1/six_python/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-sense-0.0.1/six_python/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3993 2023-06-11 23:09:53.000000 sixth-sense-0.0.1/six_python/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     4007 2023-06-12 00:04:10.000000 sixth-sense-0.0.1/six_python/middlewares/six_rate_limiter_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)      624 2023-06-10 23:02:11.000000 sixth-sense-0.0.1/six_python/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     3165 2023-06-11 23:24:27.000000 sixth-sense-0.0.1/six_python/sixth_sense.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/six_python/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-sense-0.0.1/six_python/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4309 2023-06-10 10:44:01.000000 sixth-sense-0.0.1/six_python/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-sense-0.0.1/six_python/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/sixth_sense.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/sixth_sense.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      603 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/sixth_sense.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/sixth_sense.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/sixth_sense.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2023-06-12 01:08:16.000000 sixth-sense-0.0.1/sixth_sense.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/
+-rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)       20 2023-06-09 19:50:05.000000 sixth-sense-0.0.2/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     2014 2023-06-12 01:10:18.000000 sixth-sense-0.0.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/sixth_sense/
+-rw-r--r--   0 mac        (501) staff       (20)       46 2023-06-12 01:09:39.000000 sixth-sense-0.0.2/sixth_sense/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/sixth_sense/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 sixth-sense-0.0.2/sixth_sense/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3740 2023-06-12 01:09:39.000000 sixth-sense-0.0.2/sixth_sense/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 sixth-sense-0.0.2/sixth_sense/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3994 2023-06-12 01:09:39.000000 sixth-sense-0.0.2/sixth_sense/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     4008 2023-06-12 01:09:39.000000 sixth-sense-0.0.2/sixth_sense/middlewares/six_rate_limiter_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)      624 2023-06-10 23:02:11.000000 sixth-sense-0.0.2/sixth_sense/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     3170 2023-06-12 01:09:39.000000 sixth-sense-0.0.2/sixth_sense/sixth_sense.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/sixth_sense/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 sixth-sense-0.0.2/sixth_sense/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4309 2023-06-10 10:44:01.000000 sixth-sense-0.0.2/sixth_sense/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 sixth-sense-0.0.2/sixth_sense/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/sixth_sense.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      759 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/sixth_sense.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      614 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/sixth_sense.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/sixth_sense.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/sixth_sense.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       12 2023-06-12 01:10:20.000000 sixth-sense-0.0.2/sixth_sense.egg-info/top_level.txt
```

### Comparing `sixth-sense-0.0.1/PKG-INFO` & `sixth-sense-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-sense
-Version: 0.0.1
+Version: 0.0.2
 Summary: Six offical python ackage
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: Six is a package that helps you automate pen testing and also helps you protect your API from cybersecurity threats. Visit https://withsix.co to get started.
 Keywords: python,cybersecurity,pentesting,encryption,rate limiting,xss prevention
```

### Comparing `sixth-sense-0.0.1/setup.py` & `sixth-sense-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Six offical python ackage'
 LONG_DESCRIPTION = 'Six is a package that helps you automate pen testing and also helps you protect your API from cybersecurity threats. Visit https://withsix.co to get started.'
 
 # Setting up
 setup(
     name="sixth-sense",
     version=VERSION,
```

### Comparing `sixth-sense-0.0.1/six_python/middlewares/encryption_middleware.py` & `sixth-sense-0.0.2/sixth_sense/middlewares/encryption_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from starlette.types import ASGIApp, Message
 from fastapi import FastAPI, Request
 from starlette.concurrency import iterate_in_threadpool
 import ast
 from dotenv import load_dotenv
 import os
 import requests
-from six_python.utils import encryption_utils
+from sixth_sense.utils import encryption_utils
 import copy
 import json
 from fastapi import Response, Header
-from six_python.middlewares.six_base_http_middleware import SixBaseHTTPMiddleware
+from sixth_sense.middlewares.six_base_http_middleware import SixBaseHTTPMiddleware
 from fastapi import HTTPException
 load_dotenv()
 
 
 class EncryptionMiddleware(SixBaseHTTPMiddleware):
     def __init__(self, app: ASGIApp, apikey: str, fastapi_app: FastAPI):
         super().__init__(app)
```

### Comparing `sixth-sense-0.0.1/six_python/middlewares/six_base_http_middleware.py` & `sixth-sense-0.0.2/sixth_sense/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.1/six_python/middlewares/six_independent_rate_limiter.py` & `sixth-sense-0.0.2/sixth_sense/middlewares/six_independent_rate_limiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from starlette.middleware.base import BaseHTTPMiddleware
 from starlette.types import ASGIApp
 from starlette.types import ASGIApp, Message
 from fastapi import FastAPI,Response, Request
 import time
 import json
-from six_python import schemas
+from sixth_sense import schemas
 import re
 import requests
 import ast
 
 
 class SixRateIndependentLimiterMiddleware(BaseHTTPMiddleware):
     def __init__(self, app: ASGIApp, apikey: str, fastapi_app: FastAPI, project_config: schemas.ProjectConfig):
```

### Comparing `sixth-sense-0.0.1/six_python/middlewares/six_rate_limiter_middleware.py` & `sixth-sense-0.0.2/sixth_sense/middlewares/six_rate_limiter_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from starlette.responses import PlainTextResponse, Response
 from starlette.types import ASGIApp, Message, Receive, Scope, Send
 from fastapi import FastAPI,Depends,Response,HTTPException, Request
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.middleware import Middleware
 import time
 import json
-from six_python import schemas
+from sixth_sense import schemas
 import re
 import requests
 from dotenv import load_dotenv
 import os
 import ast
```

### Comparing `sixth-sense-0.0.1/six_python/schemas.py` & `sixth-sense-0.0.2/sixth_sense/schemas.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.1/six_python/sixth_sense.py` & `sixth-sense-0.0.2/sixth_sense/sixth_sense.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from fastapi import FastAPI, status, Depends
-from six_python.middlewares.six_rate_limiter_middleware import SixRateLimiterMiddleware
-from six_python.middlewares.encryption_middleware import EncryptionMiddleware
-from six_python.middlewares.six_independent_rate_limiter import SixRateIndependentLimiterMiddleware
+from sixth_sense.middlewares.six_rate_limiter_middleware import SixRateLimiterMiddleware
+from sixth_sense.middlewares.encryption_middleware import EncryptionMiddleware
+from sixth_sense.middlewares.six_independent_rate_limiter import SixRateIndependentLimiterMiddleware
 import requests
 from dotenv import load_dotenv
-from six_python import schemas
+from sixth_sense import schemas
 import os
-from six_python.utils.time_utils import get_time_now
+from sixth_sense.utils.time_utils import get_time_now
 import json
 import re
 
 load_dotenv()
 
 
 class SixthSense():
```

### Comparing `sixth-sense-0.0.1/six_python/utils/encryption_utils.py` & `sixth-sense-0.0.2/sixth_sense/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.1/six_python/utils/time_utils.py` & `sixth-sense-0.0.2/sixth_sense/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `sixth-sense-0.0.1/sixth_sense.egg-info/PKG-INFO` & `sixth-sense-0.0.2/sixth_sense.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sixth-sense
-Version: 0.0.1
+Version: 0.0.2
 Summary: Six offical python ackage
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: Six is a package that helps you automate pen testing and also helps you protect your API from cybersecurity threats. Visit https://withsix.co to get started.
 Keywords: python,cybersecurity,pentesting,encryption,rate limiting,xss prevention
```

### Comparing `sixth-sense-0.0.1/sixth_sense.egg-info/requires.txt` & `sixth-sense-0.0.2/sixth_sense.egg-info/requires.txt`

 * *Files identical despite different names*

