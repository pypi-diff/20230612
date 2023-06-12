# Comparing `tmp/lnbits_extension-0.10.8.tar.gz` & `tmp/lnbits_extension-0.10.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnbits_extension-0.10.8.tar", max compression
+gzip compressed data, was "lnbits_extension-0.10.8.1.tar", max compression
```

## Comparing `lnbits_extension-0.10.8.tar` & `lnbits_extension-0.10.8.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-05 05:31:23.395019 lnbits_extension-0.10.8/extension/__init__.py
--rw-r--r--   0        0        0     2704 2023-06-05 05:31:23.395019 lnbits_extension-0.10.8/extension/extension.py
--rw-r--r--   0        0        0     2538 2023-06-05 05:54:36.183771 lnbits_extension-0.10.8/pyproject.toml
--rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 lnbits_extension-0.10.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 05:31:23.395019 lnbits_extension-0.10.8.1/extension/__init__.py
+-rw-r--r--   0        0        0     2659 2023-06-05 06:38:38.770630 lnbits_extension-0.10.8.1/extension/extension.py
+-rw-r--r--   0        0        0     2539 2023-06-05 06:47:23.533932 lnbits_extension-0.10.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 lnbits_extension-0.10.8.1/PKG-INFO
```

### Comparing `lnbits_extension-0.10.8/extension/extension.py` & `lnbits_extension-0.10.8.1/extension/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import json
 from typing import Any
 
 import httpx
 import uvicorn
 from fastapi import APIRouter, FastAPI
 from fastapi.routing import APIRoute
-from lnbits.core import User
 from pydantic import UUID4, BaseSettings
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 
 
-def check_user_exists(self, usr: UUID4, request: Request) -> User:
-    return User(**json.loads(request.query_params["user"]))
+def check_user_exists(self, usr: UUID4, request: Request):
+    return json.loads(request.query_params["user"])
 
 
 class ExtensionApiRouter(APIRouter):
     def add_api_route(self, *args, **kwargs):
         super().add_api_route(*args, **kwargs)
         route: APIRoute = self.routes[-1]
         for dep in route.dependencies:
```

### Comparing `lnbits_extension-0.10.8/pyproject.toml` & `lnbits_extension-0.10.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lnbits-extension"
-version = "0.10.8"
+version = "0.10.8.1"
 description = "LNbits, free and open-source Lightning wallet and accounts system."
 authors = ["Alan Bits <alan@lnbits.com>"]
 packages = [
   { include = "./extension"}
 ]
 
 [tool.poetry.dependencies]
@@ -27,15 +27,14 @@
 protobuf = "4.21.12"
 Cerberus = "1.3.4"
 async-timeout = "4.0.2"
 pyln-client = "0.11.1"
 cashu = "0.9.0"
 docker = "^6.1.3"
 
-
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.1.2"
 mock = "^4.0.3"
 black = "^22.6.0"
 pytest-asyncio = "^0.19.0"
```

### Comparing `lnbits_extension-0.10.8/PKG-INFO` & `lnbits_extension-0.10.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnbits-extension
-Version: 0.10.8
+Version: 0.10.8.1
 Summary: LNbits, free and open-source Lightning wallet and accounts system.
 Author: Alan Bits
 Author-email: alan@lnbits.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

