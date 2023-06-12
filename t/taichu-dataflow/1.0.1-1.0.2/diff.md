# Comparing `tmp/taichu-dataflow-1.0.1.tar.gz` & `tmp/taichu-dataflow-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taichu-dataflow-1.0.1.tar", last modified: Mon Jun 12 02:03:24 2023, max compression
+gzip compressed data, was "taichu-dataflow-1.0.2.tar", last modified: Mon Jun 12 06:26:23 2023, max compression
```

## Comparing `taichu-dataflow-1.0.1.tar` & `taichu-dataflow-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/
--rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/PKG-INFO
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/taichu_dataflow.egg-info/
--rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/taichu_dataflow.egg-info/PKG-INFO
--rw-r--r--   0 shenli     (501) staff       (20)      408 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/taichu_dataflow.egg-info/SOURCES.txt
--rw-r--r--   0 shenli     (501) staff       (20)       13 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/taichu_dataflow.egg-info/requires.txt
--rw-r--r--   0 shenli     (501) staff       (20)       16 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/taichu_dataflow.egg-info/top_level.txt
--rw-r--r--   0 shenli     (501) staff       (20)        1 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/taichu_dataflow.egg-info/dependency_links.txt
--rw-r--r--   0 shenli     (501) staff       (20)      169 2023-06-09 10:38:26.000000 taichu-dataflow-1.0.1/README.md
--rw-r--r--   0 shenli     (501) staff       (20)      640 2023-06-12 02:02:42.000000 taichu-dataflow-1.0.1/setup.py
--rw-r--r--   0 shenli     (501) staff       (20)       38 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/setup.cfg
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/taichu_dataflow/
--rw-r--r--   0 shenli     (501) staff       (20)      397 2023-06-09 10:38:26.000000 taichu-dataflow-1.0.1/taichu_dataflow/__init__.py
--rw-r--r--   0 shenli     (501) staff       (20)     1020 2023-06-09 10:38:26.000000 taichu-dataflow-1.0.1/taichu_dataflow/export_back.py
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 02:03:24.000000 taichu-dataflow-1.0.1/taichu_dataflow/storage/
--rw-r--r--   0 shenli     (501) staff       (20)      437 2023-06-09 10:38:26.000000 taichu-dataflow-1.0.1/taichu_dataflow/storage/env.py
--rw-r--r--   0 shenli     (501) staff       (20)     1190 2023-06-09 10:38:26.000000 taichu-dataflow-1.0.1/taichu_dataflow/storage/alluxio.py
--rw-r--r--   0 shenli     (501) staff       (20)        0 2023-06-09 10:38:26.000000 taichu-dataflow-1.0.1/taichu_dataflow/storage/__init__.py
--rw-r--r--   0 shenli     (501) staff       (20)      383 2023-06-09 10:38:26.000000 taichu-dataflow-1.0.1/taichu_dataflow/storage/storage.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 06:26:23.784853 taichu-dataflow-1.0.2/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 06:26:23.784563 taichu-dataflow-1.0.2/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      194 2023-06-12 02:53:15.000000 taichu-dataflow-1.0.2/README.md
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-06-12 06:26:23.784968 taichu-dataflow-1.0.2/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      640 2023-06-12 06:26:17.000000 taichu-dataflow-1.0.2/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 06:26:23.780348 taichu-dataflow-1.0.2/taichu_dataflow/
+-rw-r--r--   0 wangkun    (501) staff       (20)      397 2023-06-12 02:48:22.000000 taichu-dataflow-1.0.2/taichu_dataflow/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1578 2023-06-12 03:51:52.000000 taichu-dataflow-1.0.2/taichu_dataflow/export_back.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 06:26:23.783931 taichu-dataflow-1.0.2/taichu_dataflow/storage/
+-rw-r--r--   0 wangkun    (501) staff       (20)        0 2023-06-12 02:48:22.000000 taichu-dataflow-1.0.2/taichu_dataflow/storage/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1381 2023-06-12 03:50:52.000000 taichu-dataflow-1.0.2/taichu_dataflow/storage/alluxio.py
+-rw-r--r--   0 wangkun    (501) staff       (20)      437 2023-06-12 02:48:22.000000 taichu-dataflow-1.0.2/taichu_dataflow/storage/env.py
+-rw-r--r--   0 wangkun    (501) staff       (20)      459 2023-06-12 03:47:46.000000 taichu-dataflow-1.0.2/taichu_dataflow/storage/storage.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 06:26:23.782066 taichu-dataflow-1.0.2/taichu_dataflow.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 06:26:23.000000 taichu-dataflow-1.0.2/taichu_dataflow.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      408 2023-06-12 06:26:23.000000 taichu-dataflow-1.0.2/taichu_dataflow.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-06-12 06:26:23.000000 taichu-dataflow-1.0.2/taichu_dataflow.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       13 2023-06-12 06:26:23.000000 taichu-dataflow-1.0.2/taichu_dataflow.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       16 2023-06-12 06:26:23.000000 taichu-dataflow-1.0.2/taichu_dataflow.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `taichu-dataflow-1.0.1/setup.py` & `taichu-dataflow-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     long_description = ''
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='1.0.1',
+        version='1.0.2',
         description='taichu serve is a tool for serving dataflow',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
```

### Comparing `taichu-dataflow-1.0.1/taichu_dataflow/storage/alluxio.py` & `taichu-dataflow-1.0.2/taichu_dataflow/storage/alluxio.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import logging
 
 from storage.storage import StorageInterface
 import boto.s3.connection
 import storage.env
 import boto.exception
 
+
 class StorageAlluxio(StorageInterface):
     _client = None
     _bucket = None
 
     def __init__(self, storage_type):
         self._client = boto.connect_s3(
             aws_access_key_id=storage.env.S3_ACCESS_KEY_ID,
             aws_secret_access_key=storage.env.S3_SECRET_ACCESS_KEY,
-            # host='alluxio-master-0.infra',
             host=storage.env.ALLUXIO_HOST,
             port=storage.env.ALLUXIO_PORT,
             path=storage.env.ALLUXIO_PATH,
             is_secure=False,
             calling_format=boto.s3.connection.OrdinaryCallingFormat(),
         )
         self._bucket = self._client.get_bucket(storage.env.STORAGE_BUCKET)
@@ -30,7 +30,15 @@
             s3_key = self._bucket.new_key(key)
             s3_key.set_contents_from_string(content_string)
         except boto.exception.BotoClientError:
             pass
         except Exception as e:
             logging.info("key: " + key)
             logging.error("TaichuStorageError", e)
+
+    def write_file(self, file_path, key):
+        s3_key = self._bucket.new_key(key)
+        with open(file_path, "rb") as f:
+            try:
+                s3_key.set_contents_from_file(f)
+            except:
+                return
```

