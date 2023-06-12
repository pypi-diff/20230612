# Comparing `tmp/taichu-dataflow-1.0.6.tar.gz` & `tmp/taichu-dataflow-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-dataflow-1.0.6.tar", last modified: Mon Jun 12 08:27:44 2023, max compression
+gzip compressed data, was "taichu-dataflow-1.0.7.tar", last modified: Mon Jun 12 08:58:54 2023, max compression
```

## Comparing `taichu-dataflow-1.0.6.tar` & `taichu-dataflow-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:27:44.360399 taichu-dataflow-1.0.6/
--rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 08:27:44.360113 taichu-dataflow-1.0.6/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)      194 2023-06-12 02:53:15.000000 taichu-dataflow-1.0.6/README.md
--rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-06-12 08:27:44.360703 taichu-dataflow-1.0.6/setup.cfg
--rw-r--r--   0 wangkun    (501) staff       (20)      640 2023-06-12 08:27:31.000000 taichu-dataflow-1.0.6/setup.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:27:44.357928 taichu-dataflow-1.0.6/taichu_dataflow/
--rw-r--r--   0 wangkun    (501) staff       (20)      534 2023-06-12 08:21:43.000000 taichu-dataflow-1.0.6/taichu_dataflow/__init__.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1317 2023-06-12 07:27:41.000000 taichu-dataflow-1.0.6/taichu_dataflow/alluxio.py
--rw-r--r--   0 wangkun    (501) staff       (20)      437 2023-06-12 02:48:22.000000 taichu-dataflow-1.0.6/taichu_dataflow/env.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1881 2023-06-12 07:27:41.000000 taichu-dataflow-1.0.6/taichu_dataflow/export_back.py
--rw-r--r--   0 wangkun    (501) staff       (20)      451 2023-06-12 07:27:41.000000 taichu-dataflow-1.0.6/taichu_dataflow/storage.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:27:44.359671 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/
--rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)      348 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/SOURCES.txt
--rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/dependency_links.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       13 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/requires.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       16 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/top_level.txt
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:58:54.478292 taichu-dataflow-1.0.7/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 08:58:54.477875 taichu-dataflow-1.0.7/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      194 2023-06-12 02:53:15.000000 taichu-dataflow-1.0.7/README.md
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-06-12 08:58:54.478405 taichu-dataflow-1.0.7/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      699 2023-06-12 08:58:51.000000 taichu-dataflow-1.0.7/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:58:54.474876 taichu-dataflow-1.0.7/taichu_dataflow/
+-rw-r--r--   0 wangkun    (501) staff       (20)      534 2023-06-12 08:21:43.000000 taichu-dataflow-1.0.7/taichu_dataflow/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1928 2023-06-12 08:58:26.000000 taichu-dataflow-1.0.7/taichu_dataflow/export_back.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:58:54.477147 taichu-dataflow-1.0.7/taichu_dataflow/storage/
+-rw-r--r--   0 wangkun    (501) staff       (20)      475 2023-06-12 08:56:58.000000 taichu-dataflow-1.0.7/taichu_dataflow/storage/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1340 2023-06-12 08:56:58.000000 taichu-dataflow-1.0.7/taichu_dataflow/storage/alluxio.py
+-rw-r--r--   0 wangkun    (501) staff       (20)      437 2023-06-12 02:48:22.000000 taichu-dataflow-1.0.7/taichu_dataflow/storage/env.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:58:54.476148 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      373 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       13 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       16 2023-06-12 08:58:54.000000 taichu-dataflow-1.0.7/taichu_dataflow.egg-info/top_level.txt
```

### Comparing `taichu-dataflow-1.0.6/setup.py` & `taichu-dataflow-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 
     long_description = ''
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='1.0.6',
+        version='1.0.7',
         description='taichu serve is a tool for serving dataflow',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
         install_requires=requirements,
         include_package_data=True,
+        package_data={
+            '': ['*.sh'],
+        }
     )
```

### Comparing `taichu-dataflow-1.0.6/taichu_dataflow/__init__.py` & `taichu-dataflow-1.0.7/taichu_dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-dataflow-1.0.6/taichu_dataflow/alluxio.py` & `taichu-dataflow-1.0.7/taichu_dataflow/storage/alluxio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import logging
 
-from storage import StorageInterface
+from taichu_dataflow.storage import StorageInterface
 import boto.s3.connection
-import env
+from taichu_dataflow.storage.env import *
 import boto.exception
 
 
 class StorageAlluxio(StorageInterface):
     _client = None
     _bucket = None
 
     def __init__(self, storage_type):
         self._client = boto.connect_s3(
-            aws_access_key_id=env.S3_ACCESS_KEY_ID,
-            aws_secret_access_key=env.S3_SECRET_ACCESS_KEY,
-            host=env.ALLUXIO_HOST,
-            port=env.ALLUXIO_PORT,
-            path=env.ALLUXIO_PATH,
+            aws_access_key_id=S3_ACCESS_KEY_ID,
+            aws_secret_access_key=S3_SECRET_ACCESS_KEY,
+            host=ALLUXIO_HOST,
+            port=ALLUXIO_PORT,
+            path=ALLUXIO_PATH,
             is_secure=False,
             calling_format=boto.s3.connection.OrdinaryCallingFormat(),
         )
-        self._bucket = self._client.get_bucket(env.STORAGE_BUCKET)
+        self._bucket = self._client.get_bucket(STORAGE_BUCKET)
 
     def write_bytes(self, content_bytes, key):
         pass
 
     def write_string(self, content_string, key):
         try:
             s3_key = self._bucket.new_key(key)
```

### Comparing `taichu-dataflow-1.0.6/taichu_dataflow/export_back.py` & `taichu-dataflow-1.0.7/taichu_dataflow/export_back.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 import os.path
 import random
 import threading
 import time
+import uuid
 
-from storage import create_storage
+from taichu_dataflow.storage import create_storage
 from datetime import datetime
-from env import STORAGE_TYPE
+from taichu_dataflow.storage.env import STORAGE_TYPE
 
 storage_mgr = create_storage(STORAGE_TYPE)
 storage_prefix = 'sys/export_back/' + os.getenv('SERVICE_NAME', 'anonymous')
 
 
 def gen_path(suffix=''):
     suffix = suffix.lower().lstrip('.')
@@ -34,18 +35,18 @@
 
 def _logfmt(suffix, key):
     logging.info({
         'suffix': suffix,
         'key': key
     })
     logging.info({
-        "id": "da116e7b-dee7-4395-bac2-65813334b03a",
+        "id": str(uuid.uuid4()),
         "app_name": "aigc-backend",
-        "create_time": "2023-06-12 15:52:12",
-        "user_id": "1889531xx35",
+        "create_time": datetime.now().strftime("%Y-%m-%d"),
+        # "user_id": "1889531xx35",
         "action": "export_back",
         "action_params": {
             "suffix": suffix,
             "key": key
         }
     })
```

