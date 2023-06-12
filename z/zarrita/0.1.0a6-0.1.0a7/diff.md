# Comparing `tmp/zarrita-0.1.0a6.tar.gz` & `tmp/zarrita-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarrita-0.1.0a6.tar", max compression
+gzip compressed data, was "zarrita-0.1.0a7.tar", max compression
```

## Comparing `zarrita-0.1.0a6.tar` & `zarrita-0.1.0a7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     2311 2023-06-11 20:17:59.556412 zarrita-0.1.0a6/README.md
--rw-r--r--   0        0        0      737 2023-06-12 12:49:19.575716 zarrita-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0     1144 2023-06-11 20:17:59.559200 zarrita-0.1.0a6/zarrita/__init__.py
--rw-r--r--   0        0        0    19654 2023-06-11 20:17:59.559624 zarrita-0.1.0a6/zarrita/array.py
--rw-r--r--   0        0        0    13103 2023-06-11 20:17:59.559984 zarrita-0.1.0a6/zarrita/array_v2.py
--rw-r--r--   0        0        0    12363 2023-06-09 11:37:23.257106 zarrita-0.1.0a6/zarrita/codecs.py
--rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a6/zarrita/common.py
--rw-r--r--   0        0        0     3830 2023-06-11 20:17:59.560239 zarrita-0.1.0a6/zarrita/group.py
--rw-r--r--   0        0        0     4353 2023-06-11 20:17:59.560496 zarrita-0.1.0a6/zarrita/group_v2.py
--rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a6/zarrita/indexing.py
--rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a6/zarrita/metadata.py
--rw-r--r--   0        0        0    20531 2023-06-08 12:06:20.763281 zarrita-0.1.0a6/zarrita/sharding.py
--rw-r--r--   0        0        0     8466 2023-06-11 20:17:59.560828 zarrita-0.1.0a6/zarrita/store.py
--rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a6/zarrita/sync.py
--rw-r--r--   0        0        0     3783 2023-06-11 20:17:59.561195 zarrita-0.1.0a6/zarrita/value_handle.py
--rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 zarrita-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a7/LICENSE
+-rw-r--r--   0        0        0     2311 2023-06-11 20:17:59.556412 zarrita-0.1.0a7/README.md
+-rw-r--r--   0        0        0      736 2023-06-12 13:26:23.271313 zarrita-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0     1144 2023-06-11 20:17:59.559200 zarrita-0.1.0a7/zarrita/__init__.py
+-rw-r--r--   0        0        0    19648 2023-06-12 13:25:15.776807 zarrita-0.1.0a7/zarrita/array.py
+-rw-r--r--   0        0        0    13103 2023-06-11 20:17:59.559984 zarrita-0.1.0a7/zarrita/array_v2.py
+-rw-r--r--   0        0        0    12363 2023-06-09 11:37:23.257106 zarrita-0.1.0a7/zarrita/codecs.py
+-rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a7/zarrita/common.py
+-rw-r--r--   0        0        0     3830 2023-06-11 20:17:59.560239 zarrita-0.1.0a7/zarrita/group.py
+-rw-r--r--   0        0        0     4353 2023-06-11 20:17:59.560496 zarrita-0.1.0a7/zarrita/group_v2.py
+-rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a7/zarrita/indexing.py
+-rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a7/zarrita/metadata.py
+-rw-r--r--   0        0        0    20531 2023-06-08 12:06:20.763281 zarrita-0.1.0a7/zarrita/sharding.py
+-rw-r--r--   0        0        0     8466 2023-06-11 20:17:59.560828 zarrita-0.1.0a7/zarrita/store.py
+-rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a7/zarrita/sync.py
+-rw-r--r--   0        0        0     3783 2023-06-11 20:17:59.561195 zarrita-0.1.0a7/zarrita/value_handle.py
+-rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 zarrita-0.1.0a7/PKG-INFO
```

### Comparing `zarrita-0.1.0a6/LICENSE` & `zarrita-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/README.md` & `zarrita-0.1.0a7/README.md`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/pyproject.toml` & `zarrita-0.1.0a7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "zarrita"
-version = "0.1.0a6"
+version = "0.1.0a7"
 description = ""
 authors = ["Norman Rzepka <code@normanrz.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8,<4.0"
 fsspec = ">=2022.0.0"
 numpy = "^1.24.2"
 numcodecs = "^0.11.0"
 cattrs = ">=22.2.0"
 attrs = ">=22.2.0"
 crc32c = ">=2.3"
```

### Comparing `zarrita-0.1.0a6/zarrita/__init__.py` & `zarrita-0.1.0a7/zarrita/__init__.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/array.py` & `zarrita-0.1.0a7/zarrita/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
                 json.loads(v3_metadata_bytes),
                 runtime_configuration=runtime_configuration
                 or ArrayRuntimeConfiguration(),
             )
         return await ArrayV2.open_async(store_path)
 
     @classmethod
-    async def open_auto(
+    def open_auto(
         cls,
         store: StoreLike,
         runtime_configuration: Optional[ArrayRuntimeConfiguration] = None,
     ) -> Union["Array", ArrayV2]:
         return sync(cls.open_auto_async(store, runtime_configuration))
 
     async def _save_metadata(self) -> None:
```

### Comparing `zarrita-0.1.0a6/zarrita/array_v2.py` & `zarrita-0.1.0a7/zarrita/array_v2.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/codecs.py` & `zarrita-0.1.0a7/zarrita/codecs.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/common.py` & `zarrita-0.1.0a7/zarrita/common.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/group.py` & `zarrita-0.1.0a7/zarrita/group.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/group_v2.py` & `zarrita-0.1.0a7/zarrita/group_v2.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/indexing.py` & `zarrita-0.1.0a7/zarrita/indexing.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/metadata.py` & `zarrita-0.1.0a7/zarrita/metadata.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/sharding.py` & `zarrita-0.1.0a7/zarrita/sharding.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/store.py` & `zarrita-0.1.0a7/zarrita/store.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/sync.py` & `zarrita-0.1.0a7/zarrita/sync.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/zarrita/value_handle.py` & `zarrita-0.1.0a7/zarrita/value_handle.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a6/PKG-INFO` & `zarrita-0.1.0a7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: zarrita
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: 
 License: MIT
 Author: Norman Rzepka
 Author-email: code@normanrz.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=22.2.0)
```

