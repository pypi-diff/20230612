# Comparing `tmp/fastapi_throttling-0.1.1.tar.gz` & `tmp/fastapi_throttling-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_throttling-0.1.1.tar", max compression
+gzip compressed data, was "fastapi_throttling-0.1.2.tar", max compression
```

## Comparing `fastapi_throttling-0.1.1.tar` & `fastapi_throttling-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/LICENSE
--rw-r--r--   0        0        0     1343 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/README.md
--rw-r--r--   0        0        0     1803 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/src/fastapi_throttling/__init__.py
--rw-r--r--   0        0        0     3068 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/src/fastapi_throttling/throttle.py
--rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1343 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/README.md
+-rw-r--r--   0        0        0     1803 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/src/fastapi_throttling/__init__.py
+-rw-r--r--   0        0        0     3068 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/src/fastapi_throttling/throttle.py
+-rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.2/PKG-INFO
```

### Comparing `fastapi_throttling-0.1.1/LICENSE` & `fastapi_throttling-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.1/README.md` & `fastapi_throttling-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.1/pyproject.toml` & `fastapi_throttling-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-throttling"
-version = "0.1.1"
+version = "0.1.2"
 description = "Limit amount of requests to your FastAPI."
 authors = ["wwnbb <wwnbb1@gmail.com>"]
 license = "GPLv2"
 readme = "README.md"
 packages = [{include = "fastapi_throttling", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `fastapi_throttling-0.1.1/src/fastapi_throttling/throttle.py` & `fastapi_throttling-0.1.2/src/fastapi_throttling/throttle.py`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.1/PKG-INFO` & `fastapi_throttling-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-throttling
-Version: 0.1.1
+Version: 0.1.2
 Summary: Limit amount of requests to your FastAPI.
 License: GPLv2
 Author: wwnbb
 Author-email: wwnbb1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

