# Comparing `tmp/pyrestack-0.0.24-py3-none-any.whl.zip` & `tmp/pyrestack-0.0.25-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5133 bytes, number of entries: 11
--rw-r--r--  2.0 unx      140 b- defN 23-Jun-11 11:28 pyrestack/__init__.py
--rw-r--r--  2.0 unx      104 b- defN 23-Jun-11 11:28 pyrestack/const.py
--rw-r--r--  2.0 unx     2312 b- defN 23-Jun-11 11:28 pyrestack/decorator.py
--rw-r--r--  2.0 unx      293 b- defN 23-Jun-11 11:28 pyrestack/exceptions.py
--rw-r--r--  2.0 unx     3049 b- defN 23-Jun-11 11:28 pyrestack/models.py
--rw-r--r--  2.0 unx      675 b- defN 23-Jun-11 11:28 pyrestack/restack.py
--rw-r--r--  2.0 unx     1627 b- defN 23-Jun-11 11:29 pyrestack-0.0.24.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 11:29 pyrestack-0.0.24.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-11 11:29 pyrestack-0.0.24.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-11 11:29 pyrestack-0.0.24.dist-info/zip-safe
--rw-rw-r--  2.0 unx      860 b- defN 23-Jun-11 11:29 pyrestack-0.0.24.dist-info/RECORD
-11 files, 9163 bytes uncompressed, 3679 bytes compressed:  59.8%
+Zip file size: 5137 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-11 19:44 pyrestack/__init__.py
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-11 19:44 pyrestack/const.py
+-rw-r--r--  2.0 unx     2312 b- defN 23-Jun-11 19:44 pyrestack/decorator.py
+-rw-r--r--  2.0 unx      293 b- defN 23-Jun-11 19:44 pyrestack/exceptions.py
+-rw-r--r--  2.0 unx     3049 b- defN 23-Jun-11 19:44 pyrestack/models.py
+-rw-r--r--  2.0 unx      679 b- defN 23-Jun-11 19:44 pyrestack/restack.py
+-rw-r--r--  2.0 unx     1627 b- defN 23-Jun-11 19:44 pyrestack-0.0.25.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 19:44 pyrestack-0.0.25.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-11 19:44 pyrestack-0.0.25.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-11 19:44 pyrestack-0.0.25.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      860 b- defN 23-Jun-11 19:44 pyrestack-0.0.25.dist-info/RECORD
+11 files, 9167 bytes uncompressed, 3683 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pyrestack/models.py
 Comment: 
 
 Filename: pyrestack/restack.py
 Comment: 
 
-Filename: pyrestack-0.0.24.dist-info/METADATA
+Filename: pyrestack-0.0.25.dist-info/METADATA
 Comment: 
 
-Filename: pyrestack-0.0.24.dist-info/WHEEL
+Filename: pyrestack-0.0.25.dist-info/WHEEL
 Comment: 
 
-Filename: pyrestack-0.0.24.dist-info/top_level.txt
+Filename: pyrestack-0.0.25.dist-info/top_level.txt
 Comment: 
 
-Filename: pyrestack-0.0.24.dist-info/zip-safe
+Filename: pyrestack-0.0.25.dist-info/zip-safe
 Comment: 
 
-Filename: pyrestack-0.0.24.dist-info/RECORD
+Filename: pyrestack-0.0.25.dist-info/RECORD
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
 
-__version__ = '0.0.24'
+__version__ = '0.0.25'
```

## pyrestack/restack.py

```diff
@@ -11,10 +11,10 @@
         """Initialize"""
         self._base_url = base_url
         self._username = username
         self._password = password
         self._verify_ssl = verify_ssl
         self._session: ClientSession = session
 
-    @api_request("/stack")
+    @api_request("/api/stack")
     async def async_get_stacks(self, **kwargs) -> ReStackApiResponse:
         """Get monitors from API."""
```

## Comparing `pyrestack-0.0.24.dist-info/METADATA` & `pyrestack-0.0.25.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestack
-Version: 0.0.24
+Version: 0.0.25
 Summary: Simple Python wrapper for ReStack
 Home-page: https://github.com/elentriek/restack-integration
 Author: Floris Heyvaert
 Author-email: floris.heyvaert@gmail.com
 License: MIT License
 Keywords: pyrestack,setuptools
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyrestack-0.0.24.dist-info/RECORD` & `pyrestack-0.0.25.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyrestack/__init__.py,sha256=SjnBKv_ymwc3nNOTC8pNM3MYAXoGr8APRuX3B47kGo0,140
+pyrestack/__init__.py,sha256=Eo8VkERJ59MEuyWFhyFJGgZ8WQyJSCPnbot8sT09mlQ,140
 pyrestack/const.py,sha256=Azb3PK-Q14OO2gKZKye26wcvYPNh7FOOo199lxOER0I,104
 pyrestack/decorator.py,sha256=alT_mbLpEsJqTZD66wzOv2ps8OBc0PoZuvBXOREeiEY,2312
 pyrestack/exceptions.py,sha256=xgSXiqEV6hkZdyto34O-viuh4fKGtz0jkwtjgOR0iaw,293
 pyrestack/models.py,sha256=bB6Mn_PyDIXaQlhYd54_-N7sB1FpYEtP9_FzPC6P6G4,3049
-pyrestack/restack.py,sha256=n03zwQK5Tj3ynuJZwjpIHXRNK6Oa-nieW3fI7h0XKKs,675
-pyrestack-0.0.24.dist-info/METADATA,sha256=EhfnyBhYAv4XK4v3n2dVfA0YtS1W0fip28UxeeLBHak,1627
-pyrestack-0.0.24.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyrestack-0.0.24.dist-info/top_level.txt,sha256=9EZedki-jXfc4k1T9TZf0OmFcf8YN5xHRyCkZj0Xhgo,10
-pyrestack-0.0.24.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pyrestack-0.0.24.dist-info/RECORD,,
+pyrestack/restack.py,sha256=PzUqpudNYq53q-k_8PaH9dE3BW9l01l6dZ6T6LzHSUI,679
+pyrestack-0.0.25.dist-info/METADATA,sha256=V2kVOU5aeJ3KRCBkfDch6yqQiugtHS7lNbPJpYley8w,1627
+pyrestack-0.0.25.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyrestack-0.0.25.dist-info/top_level.txt,sha256=9EZedki-jXfc4k1T9TZf0OmFcf8YN5xHRyCkZj0Xhgo,10
+pyrestack-0.0.25.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pyrestack-0.0.25.dist-info/RECORD,,
```

