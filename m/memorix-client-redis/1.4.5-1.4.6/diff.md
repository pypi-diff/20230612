# Comparing `tmp/memorix_client_redis-1.4.5.tar.gz` & `tmp/memorix_client_redis-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memorix_client_redis-1.4.5.tar", max compression
+gzip compressed data, was "memorix_client_redis-1.4.6.tar", max compression
```

## Comparing `memorix_client_redis-1.4.5.tar` & `memorix_client_redis-1.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      706 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/cache/__init__.py
--rw-r--r--   0        0        0      140 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/cache/cache_base.py
--rw-r--r--   0        0        0     6028 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/cache/cache_item.py
--rw-r--r--   0        0        0     1120 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/cache/cache_options.py
--rw-r--r--   0        0        0      456 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/default_options.py
--rw-r--r--   0        0        0      496 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/example-schema.memorix
--rw-r--r--   0        0        0     2021 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/example_schema_generated.py
--rw-r--r--   0        0        0      369 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/hash_key.py
--rw-r--r--   0        0        0     1488 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/json.py
--rw-r--r--   0        0        0     1037 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/memorix_base.py
--rw-r--r--   0        0        0        0 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/pubsub/__init__.py
--rw-r--r--   0        0        0      141 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/pubsub/pubsub_base.py
--rw-r--r--   0        0        0     3892 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/pubsub/pubsub_item.py
--rw-r--r--   0        0        0        0 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/py.typed
--rw-r--r--   0        0        0      217 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/redis_connection.py
--rw-r--r--   0        0        0     1415 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/start.py
--rw-r--r--   0        0        0        0 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/task/__init__.py
--rw-r--r--   0        0        0      158 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/task/task_base.py
--rw-r--r--   0        0        0    10093 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/task/task_item.py
--rw-r--r--   0        0        0      454 2023-06-11 15:49:47.945125 memorix_client_redis-1.4.5/memorix_client_redis/task/task_options.py
--rw-r--r--   0        0        0      580 2023-06-11 15:50:48.032842 memorix_client_redis-1.4.5/pyproject.toml
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 memorix_client_redis-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/cache/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/cache/cache_base.py
+-rw-r--r--   0        0        0     6028 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/cache/cache_item.py
+-rw-r--r--   0        0        0     1120 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/cache/cache_options.py
+-rw-r--r--   0        0        0      456 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/default_options.py
+-rw-r--r--   0        0        0      496 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/example-schema.memorix
+-rw-r--r--   0        0        0     2021 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/example_schema_generated.py
+-rw-r--r--   0        0        0      369 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/hash_key.py
+-rw-r--r--   0        0        0     1488 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/json.py
+-rw-r--r--   0        0        0     1037 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/memorix_base.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/pubsub/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/pubsub/pubsub_base.py
+-rw-r--r--   0        0        0     3892 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/pubsub/pubsub_item.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/py.typed
+-rw-r--r--   0        0        0      217 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/redis_connection.py
+-rw-r--r--   0        0        0     1415 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/start.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/task/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/task/task_base.py
+-rw-r--r--   0        0        0    10093 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/task/task_item.py
+-rw-r--r--   0        0        0      454 2023-06-12 07:26:23.625943 memorix_client_redis-1.4.6/memorix_client_redis/task/task_options.py
+-rw-r--r--   0        0        0      580 2023-06-12 07:27:12.030021 memorix_client_redis-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 memorix_client_redis-1.4.6/PKG-INFO
```

### Comparing `memorix_client_redis-1.4.5/memorix_client_redis/__init__.py` & `memorix_client_redis-1.4.6/memorix_client_redis/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .memorix_base import MemorixBase
+from .memorix_base import MemorixBase as MemorixBase
 from .cache.cache_base import CacheBase as MemorixCacheBase
 from .cache.cache_item import (
     CacheItem as MemorixCacheItem,
     CacheItemNoKey as MemorixCacheItemNoKey,
 )
 from .pubsub.pubsub_base import PubSubBase as MemorixPubSubBase
 from .pubsub.pubsub_item import (
@@ -12,8 +12,8 @@
 from .task.task_base import TaskBase as MemorixTaskBase
 from .task.task_item import (
     TaskItem as MemorixTaskItem,
     TaskItemNoKey as MemorixTaskItemNoKey,
     TaskItemNoReturns as MemorixTaskItemNoReturns,
     TaskItemNoKeyNoReturns as MemorixTaskItemNoKeyNoReturns,
 )
-from dataclasses import dataclass
+from dataclasses import dataclass as dataclass
```

### Comparing `memorix_client_redis-1.4.5/memorix_client_redis/cache/cache_item.py` & `memorix_client_redis-1.4.6/memorix_client_redis/cache/cache_item.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.4.5/memorix_client_redis/cache/cache_options.py` & `memorix_client_redis-1.4.6/memorix_client_redis/cache/cache_options.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.4.5/memorix_client_redis/example_schema_generated.py` & `memorix_client_redis-1.4.6/memorix_client_redis/example_schema_generated.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.4.5/memorix_client_redis/json.py` & `memorix_client_redis-1.4.6/memorix_client_redis/json.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.4.5/memorix_client_redis/memorix_base.py` & `memorix_client_redis-1.4.6/memorix_client_redis/memorix_base.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.4.5/memorix_client_redis/pubsub/pubsub_item.py` & `memorix_client_redis-1.4.6/memorix_client_redis/pubsub/pubsub_item.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.4.5/memorix_client_redis/start.py` & `memorix_client_redis-1.4.6/memorix_client_redis/start.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.4.5/memorix_client_redis/task/task_item.py` & `memorix_client_redis-1.4.6/memorix_client_redis/task/task_item.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.4.5/pyproject.toml` & `memorix_client_redis-1.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "memorix_client_redis"
-version = "1.4.5"
+version = "1.4.6"
 description = ""
 authors = ["Yuval Saraf <unimonkiez@gmail.com>"]
 
 [tool.poetry.scripts]
 start = "memorix_client_redis.start:start"
 
 [tool.poetry.dependencies]
```

