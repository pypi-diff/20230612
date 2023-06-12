# Comparing `tmp/pyrestack-0.0.26-py3-none-any.whl.zip` & `tmp/pyrestack-0.0.27-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5293 bytes, number of entries: 11
--rw-r--r--  2.0 unx      140 b- defN 23-Jun-12 18:57 pyrestack/__init__.py
--rw-r--r--  2.0 unx      104 b- defN 23-Jun-12 18:57 pyrestack/const.py
--rw-r--r--  2.0 unx     2312 b- defN 23-Jun-12 18:57 pyrestack/decorator.py
--rw-r--r--  2.0 unx      293 b- defN 23-Jun-12 18:57 pyrestack/exceptions.py
--rw-r--r--  2.0 unx     4245 b- defN 23-Jun-12 18:57 pyrestack/models.py
--rw-r--r--  2.0 unx      862 b- defN 23-Jun-12 18:57 pyrestack/restack.py
--rw-r--r--  2.0 unx     1627 b- defN 23-Jun-12 18:58 pyrestack-0.0.26.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 18:58 pyrestack-0.0.26.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-12 18:58 pyrestack-0.0.26.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-12 18:58 pyrestack-0.0.26.dist-info/zip-safe
--rw-rw-r--  2.0 unx      860 b- defN 23-Jun-12 18:58 pyrestack-0.0.26.dist-info/RECORD
-11 files, 10546 bytes uncompressed, 3839 bytes compressed:  63.6%
+Zip file size: 5407 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-12 19:11 pyrestack/__init__.py
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-12 19:11 pyrestack/const.py
+-rw-r--r--  2.0 unx     2732 b- defN 23-Jun-12 19:11 pyrestack/decorator.py
+-rw-r--r--  2.0 unx      293 b- defN 23-Jun-12 19:11 pyrestack/exceptions.py
+-rw-r--r--  2.0 unx     4245 b- defN 23-Jun-12 19:11 pyrestack/models.py
+-rw-r--r--  2.0 unx      848 b- defN 23-Jun-12 19:11 pyrestack/restack.py
+-rw-r--r--  2.0 unx     1627 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      860 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/RECORD
+11 files, 10952 bytes uncompressed, 3953 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pyrestack/models.py
 Comment: 
 
 Filename: pyrestack/restack.py
 Comment: 
 
-Filename: pyrestack-0.0.26.dist-info/METADATA
+Filename: pyrestack-0.0.27.dist-info/METADATA
 Comment: 
 
-Filename: pyrestack-0.0.26.dist-info/WHEEL
+Filename: pyrestack-0.0.27.dist-info/WHEEL
 Comment: 
 
-Filename: pyrestack-0.0.26.dist-info/top_level.txt
+Filename: pyrestack-0.0.27.dist-info/top_level.txt
 Comment: 
 
-Filename: pyrestack-0.0.26.dist-info/zip-safe
+Filename: pyrestack-0.0.27.dist-info/zip-safe
 Comment: 
 
-Filename: pyrestack-0.0.26.dist-info/RECORD
+Filename: pyrestack-0.0.27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyrestack/__init__.py

```diff
@@ -1,7 +1,7 @@
 """Python API wrapper for ReStack."""
 from .exceptions import *
 from .models import *
 from .restack import ReStack
 
-__version__ = '0.0.26'
+__version__ = '0.0.27'
```

## pyrestack/decorator.py

```diff
@@ -5,30 +5,33 @@
 from typing import TYPE_CHECKING
 
 import aiohttp
 
 from .exceptions import ReStackConnectionException, ReStackException, ReStackAuthenticationException
 
 from .const import LOGGER
-from .models import ReStackApiResponse
+from .models import StacksApiResponse, JobApiResponse
 
 if TYPE_CHECKING:
     from .ReStack import ReStack
 
 
 def api_request(api_path: str, method: str = "GET"):
     """Decorator for ReStack API request"""
 
     def decorator(func):
         """Decorator"""
 
         async def wrapper(*args, **kwargs):
             """Wrapper"""
+            # TODO redo this
+            resolved_api_path = api_path.replace('{id}', f'{args[1]}' if args and len(args) >= 2 else '')
+
             client: ReStack = args[0]
-            url = f"{client._base_url}{api_path}"
+            url = f"{client._base_url}{resolved_api_path}"
             LOGGER.debug("Requesting %s", url)
 
             try:
                 request = await client._session.request(
                     method=method,
                     url=url,
                     timeout=aiohttp.ClientTimeout(total=10),
@@ -55,16 +58,22 @@
 
             except (Exception, BaseException) as exception:
                 raise ReStackException(f"Unexpected exception for '{url}' with - {exception}") from exception
 
             LOGGER.debug("Requesting %s returned %s", url, result)
 
             # print(result)
-            response = ReStackApiResponse.from_prometheus(
-                {"content": result, "_api_path": api_path, "_method": method}
-            )
+            # TODO redo this
+            if (api_path == "/api/stack"):
+                response = StacksApiResponse.from_prometheus(
+                    {"content": result, "_api_path": api_path, "_method": method}
+                )
+            else:
+                response = JobApiResponse.from_prometheus(
+                    {"content": result, "_api_path": api_path, "_method": method}
+                )
 
             return response
 
         return wrapper
 
     return decorator
```

## pyrestack/restack.py

```diff
@@ -15,10 +15,10 @@
         self._verify_ssl = verify_ssl
         self._session: ClientSession = session
 
     @api_request("/api/stack")
     async def async_get_stacks(self, **kwargs) -> StacksApiResponse:
         """Get stacks from API."""
 
-    @api_request("/api/stack/{id}/execute", method="GET")
+    @api_request("/api/stack/{id}/execute")
     async def async_execute_stack(self, id: int, **kwargs) -> JobApiResponse:
         """Execute stack on API"""
```

## Comparing `pyrestack-0.0.26.dist-info/METADATA` & `pyrestack-0.0.27.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestack
-Version: 0.0.26
+Version: 0.0.27
 Summary: Simple Python wrapper for ReStack
 Home-page: https://github.com/elentriek/restack-integration
 Author: Floris Heyvaert
 Author-email: floris.heyvaert@gmail.com
 License: MIT License
 Keywords: pyrestack,setuptools
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyrestack-0.0.26.dist-info/RECORD` & `pyrestack-0.0.27.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyrestack/__init__.py,sha256=qFHj36aTT-4ilZUsuV1CKFPhx9BwMRUMph2emo9Yw_E,140
+pyrestack/__init__.py,sha256=5NUFcfPtGZ4KFtwujLNIOSCcKCenVOd2moGLEbb_NsM,140
 pyrestack/const.py,sha256=Azb3PK-Q14OO2gKZKye26wcvYPNh7FOOo199lxOER0I,104
-pyrestack/decorator.py,sha256=alT_mbLpEsJqTZD66wzOv2ps8OBc0PoZuvBXOREeiEY,2312
+pyrestack/decorator.py,sha256=m7qlhwAWH8i-UJ_1tuVR2hHx4VMNz4VOt-hRmOY39tg,2732
 pyrestack/exceptions.py,sha256=xgSXiqEV6hkZdyto34O-viuh4fKGtz0jkwtjgOR0iaw,293
 pyrestack/models.py,sha256=HNiPOampZ5jtMwy43UMOzskWvYxvwkSP6f_wIJsE12M,4245
-pyrestack/restack.py,sha256=NkPzXT3GGHjkjv4vLuzv_tHjX0KnTDspzWNAuA6pCYY,862
-pyrestack-0.0.26.dist-info/METADATA,sha256=TYOeCn69J7WZlZqXNTQkl0KI73UO9k5_1qlJb-ceqdQ,1627
-pyrestack-0.0.26.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyrestack-0.0.26.dist-info/top_level.txt,sha256=9EZedki-jXfc4k1T9TZf0OmFcf8YN5xHRyCkZj0Xhgo,10
-pyrestack-0.0.26.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pyrestack-0.0.26.dist-info/RECORD,,
+pyrestack/restack.py,sha256=miJXa4QOaHIoNin9n31gV2M1DWBYsjmAw1ZGZxSelBU,848
+pyrestack-0.0.27.dist-info/METADATA,sha256=7SrGKmEfVKvAPuHb6Gcsv7jXAuus1eqSIZ_bA-N08tg,1627
+pyrestack-0.0.27.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyrestack-0.0.27.dist-info/top_level.txt,sha256=9EZedki-jXfc4k1T9TZf0OmFcf8YN5xHRyCkZj0Xhgo,10
+pyrestack-0.0.27.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pyrestack-0.0.27.dist-info/RECORD,,
```

