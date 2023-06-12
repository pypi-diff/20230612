# Comparing `tmp/cbcmgr-1.2.3.tar.gz` & `tmp/cbcmgr-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.2.3.tar", last modified: Mon Jun 12 14:24:46 2023, max compression
+gzip compressed data, was "cbcmgr-1.2.4.tar", last modified: Mon Jun 12 14:43:06 2023, max compression
```

## Comparing `cbcmgr-1.2.3.tar` & `cbcmgr-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-12 14:24:46.062376 cbcmgr-1.2.3/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.2.3/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-06-12 14:24:46.062209 cbcmgr-1.2.3/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.2.3/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-12 14:24:45.979958 cbcmgr-1.2.3/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.2.3/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.2.3/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.2.3/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.2.3/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     4148 2023-06-12 14:23:34.000000 cbcmgr-1.2.3/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    10955 2023-06-12 14:23:34.000000 cbcmgr-1.2.3/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.2.3/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.2.3/cbcmgr/schema.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-12 14:24:46.061793 cbcmgr-1.2.3/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-06-12 14:24:45.000000 cbcmgr-1.2.3/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      343 2023-06-12 14:24:45.000000 cbcmgr-1.2.3/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-12 14:24:45.000000 cbcmgr-1.2.3/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       57 2023-06-12 14:24:45.000000 cbcmgr-1.2.3/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-06-12 14:24:45.000000 cbcmgr-1.2.3/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-12 14:24:46.062430 cbcmgr-1.2.3/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      705 2023-06-12 14:24:29.000000 cbcmgr-1.2.3/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-12 14:43:06.391038 cbcmgr-1.2.4/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.2.4/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-06-12 14:43:06.390906 cbcmgr-1.2.4/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.2.4/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-12 14:43:06.378163 cbcmgr-1.2.4/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.2.4/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.2.4/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.2.4/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.2.4/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     4197 2023-06-12 14:40:15.000000 cbcmgr-1.2.4/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.2.4/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.2.4/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.2.4/cbcmgr/schema.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-12 14:43:06.390664 cbcmgr-1.2.4/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      343 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       57 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-06-12 14:43:06.000000 cbcmgr-1.2.4/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-12 14:43:06.391085 cbcmgr-1.2.4/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      705 2023-06-12 14:43:01.000000 cbcmgr-1.2.4/setup.py
```

### Comparing `cbcmgr-1.2.3/LICENSE.txt` & `cbcmgr-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.3/PKG-INFO` & `cbcmgr-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.2.3
+Version: 1.2.4
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.2.3/README.md` & `cbcmgr-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.3/cbcmgr/cb_connect.py` & `cbcmgr-1.2.4/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.3/cbcmgr/cb_management.py` & `cbcmgr-1.2.4/cbcmgr/cb_management.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.3/cbcmgr/cb_session.py` & `cbcmgr-1.2.4/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.3/cbcmgr/exceptions.py` & `cbcmgr-1.2.4/cbcmgr/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,14 +278,18 @@
     pass
 
 
 class PreconditionFailed(CBException):
     pass
 
 
+class ConflictException(CBException):
+    pass
+
+
 class PaginationDataNotFound(CBException):
     pass
 
 
 class SyncGatewayOperationException(CBException):
     pass
```

### Comparing `cbcmgr-1.2.3/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.2.4/cbcmgr/httpsessionmgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import datetime
 import hmac
 import hashlib
 import warnings
 from urllib.parse import urlparse
 from requests.auth import AuthBase
 from .exceptions import (NotAuthorized, HTTPForbidden, HTTPNotImplemented, RequestValidationError, InternalServerError,
-                         PaginationDataNotFound, SyncGatewayOperationException, PreconditionFailed)
+                         PaginationDataNotFound, SyncGatewayOperationException, PreconditionFailed, ConflictException)
 
 
 class CapellaToken(object):
 
     def __init__(self, key: str, secret: str):
         self.cbc_api_signature = None
         self.cbc_api_now = None
@@ -143,14 +143,16 @@
             return True
         elif code == 401:
             raise NotAuthorized("API: Unauthorized")
         elif code == 403:
             raise HTTPForbidden("API: Forbidden: Insufficient privileges")
         elif code == 404:
             raise HTTPNotImplemented("API: Not Found")
+        elif code == 409:
+            raise ConflictException("Conflict")
         elif code == 412:
             raise PreconditionFailed("Precondition Failed")
         elif code == 415:
             raise RequestValidationError("API: invalid body contents")
         elif code == 422:
             raise RequestValidationError("API: Request Validation Error")
         elif code == 500:
```

### Comparing `cbcmgr-1.2.3/cbcmgr/retry.py` & `cbcmgr-1.2.4/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.3/cbcmgr/schema.py` & `cbcmgr-1.2.4/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.3/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.2.4/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.2.3
+Version: 1.2.4
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.2.3/setup.py` & `cbcmgr-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.2.3',
+    version='1.2.4',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```

