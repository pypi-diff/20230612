# Comparing `tmp/reliable_queue-0.0.8.tar.gz` & `tmp/reliable_queue-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliable_queue-0.0.8.tar", last modified: Fri Jan 20 17:16:18 2023, max compression
+gzip compressed data, was "reliable_queue-0.0.9.tar", last modified: Thu Jan 26 08:08:59 2023, max compression
```

## Comparing `reliable_queue-0.0.8.tar` & `reliable_queue-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ehsmeng   (1000) ehsmeng   (1000)        0 2023-01-20 17:16:18.838744 reliable_queue-0.0.8/
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     1069 2022-11-23 06:29:34.000000 reliable_queue-0.0.8/LICENSE
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     1054 2023-01-20 17:16:18.838744 reliable_queue-0.0.8/PKG-INFO
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)      368 2022-11-25 19:59:29.000000 reliable_queue-0.0.8/README.md
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     1041 2023-01-20 17:15:34.000000 reliable_queue-0.0.8/pyproject.toml
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)       38 2023-01-20 17:16:18.838744 reliable_queue-0.0.8/setup.cfg
-drwxrwxr-x   0 ehsmeng   (1000) ehsmeng   (1000)        0 2023-01-20 17:16:18.838744 reliable_queue-0.0.8/src/
-drwxrwxr-x   0 ehsmeng   (1000) ehsmeng   (1000)        0 2023-01-20 17:16:18.838744 reliable_queue-0.0.8/src/reliable_queue/
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     3782 2023-01-20 17:15:16.000000 reliable_queue-0.0.8/src/reliable_queue/__init__.py
-drwxrwxr-x   0 ehsmeng   (1000) ehsmeng   (1000)        0 2023-01-20 17:16:18.838744 reliable_queue-0.0.8/src/reliable_queue.egg-info/
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     1054 2023-01-20 17:16:18.000000 reliable_queue-0.0.8/src/reliable_queue.egg-info/PKG-INFO
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)      272 2023-01-20 17:16:18.000000 reliable_queue-0.0.8/src/reliable_queue.egg-info/SOURCES.txt
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)        1 2023-01-20 17:16:18.000000 reliable_queue-0.0.8/src/reliable_queue.egg-info/dependency_links.txt
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)       13 2023-01-20 17:16:18.000000 reliable_queue-0.0.8/src/reliable_queue.egg-info/requires.txt
--rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)       15 2023-01-20 17:16:18.000000 reliable_queue-0.0.8/src/reliable_queue.egg-info/top_level.txt
+drwxrwxr-x   0 ehsmeng   (1000) ehsmeng   (1000)        0 2023-01-26 08:08:59.520968 reliable_queue-0.0.9/
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     1069 2022-11-23 06:29:34.000000 reliable_queue-0.0.9/LICENSE
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     1054 2023-01-26 08:08:59.520968 reliable_queue-0.0.9/PKG-INFO
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)      368 2022-11-25 19:59:29.000000 reliable_queue-0.0.9/README.md
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     1041 2023-01-26 08:03:40.000000 reliable_queue-0.0.9/pyproject.toml
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)       38 2023-01-26 08:08:59.520968 reliable_queue-0.0.9/setup.cfg
+drwxrwxr-x   0 ehsmeng   (1000) ehsmeng   (1000)        0 2023-01-26 08:08:59.520968 reliable_queue-0.0.9/src/
+drwxrwxr-x   0 ehsmeng   (1000) ehsmeng   (1000)        0 2023-01-26 08:08:59.520968 reliable_queue-0.0.9/src/reliable_queue/
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     3869 2023-01-26 08:04:39.000000 reliable_queue-0.0.9/src/reliable_queue/__init__.py
+drwxrwxr-x   0 ehsmeng   (1000) ehsmeng   (1000)        0 2023-01-26 08:08:59.520968 reliable_queue-0.0.9/src/reliable_queue.egg-info/
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)     1054 2023-01-26 08:08:59.000000 reliable_queue-0.0.9/src/reliable_queue.egg-info/PKG-INFO
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)      272 2023-01-26 08:08:59.000000 reliable_queue-0.0.9/src/reliable_queue.egg-info/SOURCES.txt
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)        1 2023-01-26 08:08:59.000000 reliable_queue-0.0.9/src/reliable_queue.egg-info/dependency_links.txt
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)       13 2023-01-26 08:08:59.000000 reliable_queue-0.0.9/src/reliable_queue.egg-info/requires.txt
+-rw-rw-r--   0 ehsmeng   (1000) ehsmeng   (1000)       15 2023-01-26 08:08:59.000000 reliable_queue-0.0.9/src/reliable_queue.egg-info/top_level.txt
```

### Comparing `reliable_queue-0.0.8/LICENSE` & `reliable_queue-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reliable_queue-0.0.8/PKG-INFO` & `reliable_queue-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reliable_queue
-Version: 0.0.8
+Version: 0.0.9
 Summary: A reliable queue for the Manycore-Mail project
 Author-email: Nicolas Toper <ntoper@manycore.io>, Marcus Engene <marcus@manycore.io>
 Maintainer-email: Nicolas Toper <ntoper@manycore.io>, Marcus Engene <marcus@manycore.io>
 Project-URL: Homepage, https://github.com/manycore-com/Manycore-ReliableQueue
 Project-URL: Bug Tracker, https://github.com/manycore-com/Manycore-ReliableQueue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `reliable_queue-0.0.8/pyproject.toml` & `reliable_queue-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
 [project]
 name = "reliable_queue"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Nicolas Toper", email="ntoper@manycore.io" },
   { name="Marcus Engene", email="marcus@manycore.io" },
 ]
 maintainers = [
   { name="Nicolas Toper", email="ntoper@manycore.io" },
   { name="Marcus Engene", email="marcus@manycore.io" },
```

### Comparing `reliable_queue-0.0.8/src/reliable_queue/__init__.py` & `reliable_queue-0.0.9/src/reliable_queue/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 
     def set_shutdown(self, shutdown):
         self._shutdown = shutdown
 
     def get_queue_name(self):
         return self._queue_name
 
+    def get_queue_len(self) -> int:
+        return self._redis.llen(self._queue_name)
+
     def push(self, data: bytes):
         """
         Note: redis.exceptions.ResponseError: WRONGTYPE Operation against a key holding the wrong kind of value
            happens if key exists but is not referring to a list. Ie, key refer to a SET value, not a RPUSH.
 
         :param data:
         :return:
```

### Comparing `reliable_queue-0.0.8/src/reliable_queue.egg-info/PKG-INFO` & `reliable_queue-0.0.9/src/reliable_queue.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reliable-queue
-Version: 0.0.8
+Version: 0.0.9
 Summary: A reliable queue for the Manycore-Mail project
 Author-email: Nicolas Toper <ntoper@manycore.io>, Marcus Engene <marcus@manycore.io>
 Maintainer-email: Nicolas Toper <ntoper@manycore.io>, Marcus Engene <marcus@manycore.io>
 Project-URL: Homepage, https://github.com/manycore-com/Manycore-ReliableQueue
 Project-URL: Bug Tracker, https://github.com/manycore-com/Manycore-ReliableQueue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

