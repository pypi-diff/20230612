# Comparing `tmp/gcsfs-2023.5.0.tar.gz` & `tmp/gcsfs-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcsfs-2023.5.0.tar", last modified: Sun May  7 19:22:00 2023, max compression
+gzip compressed data, was "gcsfs-2023.6.0.tar", last modified: Mon Jun 12 13:54:55 2023, max compression
```

## Comparing `gcsfs-2023.5.0.tar` & `gcsfs-2023.6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.342964 gcsfs-2023.5.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1536 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/LICENSE.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-05-07 19:22:00.343070 gcsfs-2023.5.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      526 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.332376 gcsfs-2023.5.0/docs/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.335776 gcsfs-2023.5.0/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      800 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/docs/source/api.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     4254 2023-05-07 19:21:12.000000 gcsfs-2023.5.0/docs/source/changelog.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      906 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/docs/source/developer.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     1776 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/docs/source/fuse.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     6393 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/docs/source/index.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.343814 gcsfs-2023.5.0/gcsfs/
--rw-r--r--   0 mdurant    (502) staff       (20)      192 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-05-07 19:22:00.343870 gcsfs-2023.5.0/gcsfs/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3618 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/checkers.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.340256 gcsfs-2023.5.0/gcsfs/cli/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/cli/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1942 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/cli/gcsfuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)    60829 2023-05-07 19:16:48.000000 gcsfs-2023.5.0/gcsfs/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8947 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/credentials.py
--rw-r--r--   0 mdurant    (502) staff       (20)       68 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/dask_link.py
--rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4691 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/retry.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.342782 gcsfs-2023.5.0/gcsfs/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/tests/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3885 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)      178 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/settings.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_checkers.py
--rw-r--r--   0 mdurant    (502) staff       (20)    41351 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/gcsfs/tests/test_core.py
--rw-r--r--   0 mdurant    (502) staff       (20)      222 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/tests/test_credentials.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1822 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_fuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_manyopens.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3064 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3429 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_retry.py
--rw-r--r--   0 mdurant    (502) staff       (20)      911 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.339760 gcsfs-2023.5.0/gcsfs.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      842 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-27 12:31:48.000000 gcsfs-2023.5.0/gcsfs.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      160 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        6 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      129 2023-05-07 19:21:12.000000 gcsfs-2023.5.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      445 2023-05-07 19:22:00.343480 gcsfs-2023.5.0/setup.cfg
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1184 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    68739 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-12 13:54:55.662608 gcsfs-2023.6.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1536 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/LICENSE.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.6.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-06-12 13:54:55.662689 gcsfs-2023.6.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      526 2022-09-18 01:28:26.000000 gcsfs-2023.6.0/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-12 13:54:55.652589 gcsfs-2023.6.0/docs/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-12 13:54:55.656081 gcsfs-2023.6.0/docs/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      800 2023-02-24 20:42:20.000000 gcsfs-2023.6.0/docs/source/api.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     4407 2023-06-12 13:54:19.000000 gcsfs-2023.6.0/docs/source/changelog.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      906 2022-09-18 01:28:26.000000 gcsfs-2023.6.0/docs/source/developer.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     1776 2023-02-24 20:42:20.000000 gcsfs-2023.6.0/docs/source/fuse.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     6577 2023-05-12 17:24:09.000000 gcsfs-2023.6.0/docs/source/index.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-12 13:54:55.663487 gcsfs-2023.6.0/gcsfs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      192 2022-09-18 01:28:26.000000 gcsfs-2023.6.0/gcsfs/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-06-12 13:54:55.663541 gcsfs-2023.6.0/gcsfs/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3618 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/checkers.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-12 13:54:55.659860 gcsfs-2023.6.0/gcsfs/cli/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.6.0/gcsfs/cli/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1942 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/cli/gcsfuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    61442 2023-05-12 17:07:14.000000 gcsfs-2023.6.0/gcsfs/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9137 2023-05-23 13:46:33.000000 gcsfs-2023.6.0/gcsfs/credentials.py
+-rw-r--r--   0 mdurant    (502) staff       (20)       68 2022-09-18 01:28:26.000000 gcsfs-2023.6.0/gcsfs/dask_link.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.6.0/gcsfs/mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4691 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/retry.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-12 13:54:55.662454 gcsfs-2023.6.0/gcsfs/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.6.0/gcsfs/tests/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3885 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/tests/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      178 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/tests/settings.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/tests/test_checkers.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    41597 2023-05-12 16:54:39.000000 gcsfs-2023.6.0/gcsfs/tests/test_core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      563 2023-05-23 13:46:33.000000 gcsfs-2023.6.0/gcsfs/tests/test_credentials.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1822 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/tests/test_fuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/tests/test_manyopens.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3064 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/tests/test_mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3429 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/tests/test_retry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      911 2023-01-02 14:01:40.000000 gcsfs-2023.6.0/gcsfs/tests/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-12 13:54:55.659543 gcsfs-2023.6.0/gcsfs.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-06-12 13:54:55.000000 gcsfs-2023.6.0/gcsfs.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      842 2023-06-12 13:54:55.000000 gcsfs-2023.6.0/gcsfs.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-06-12 13:54:55.000000 gcsfs-2023.6.0/gcsfs.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-27 12:31:48.000000 gcsfs-2023.6.0/gcsfs.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      160 2023-06-12 13:54:55.000000 gcsfs-2023.6.0/gcsfs.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        6 2023-06-12 13:54:55.000000 gcsfs-2023.6.0/gcsfs.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      129 2023-06-12 13:54:19.000000 gcsfs-2023.6.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      445 2023-06-12 13:54:55.663115 gcsfs-2023.6.0/setup.cfg
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1184 2023-02-24 20:42:20.000000 gcsfs-2023.6.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    68739 2022-09-18 01:28:26.000000 gcsfs-2023.6.0/versioneer.py
```

### Comparing `gcsfs-2023.5.0/LICENSE.txt` & `gcsfs-2023.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/PKG-INFO` & `gcsfs-2023.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcsfs
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Convenient Filesystem interface over GCS
 Home-page: https://github.com/fsspec/gcsfs
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Keywords: google-cloud-storage,gcloud,file-system
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gcsfs-2023.5.0/README.rst` & `gcsfs-2023.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/docs/source/api.rst` & `gcsfs-2023.6.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/docs/source/changelog.rst` & `gcsfs-2023.6.0/docs/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2023.6.0
+--------
+
+* allow raw/session token for auth (#554)
+* fix listings_expiry_time kwargs (#551)
+* allow setting fixed metadata on put/pipe (#550)
+
 2023.5.0
 --------
 
 * Allow emulator host without protocol (#548)
 * Prevent upload retry from closing the file being sent (#540)
 
 2023.4.0
```

### Comparing `gcsfs-2023.5.0/docs/source/developer.rst` & `gcsfs-2023.6.0/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/docs/source/fuse.rst` & `gcsfs-2023.6.0/docs/source/fuse.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/docs/source/index.rst` & `gcsfs-2023.6.0/docs/source/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -146,30 +146,31 @@
 If you wish to call ``gcsfs`` from async code, then you should pass
 ``asynchronous=True, loop=loop`` to the constructor (the latter is optional,
 if you wish to use both async and sync methods). You must also explicitly
 await the client creation before making any GCS call.
 
 .. code-block:: python
 
-    loop = ...  # however you create your loop
+    async def run_program():
+        gcs = GCSFileSystem(asynchronous=True)
+        print(await gcs._ls(""))
 
-    async def run_program(loop):
-        gcs = GCSFileSystem(..., asynchronous=True, loop=loop)
-        await gcs.set_session()
-        ...  # perform work
-
-    asyncio.run(run_program(loop))  # or call from your async code
+    asyncio.run(run_program())  # or call from your async code
 
 Concurrent async operations are also used internally for bulk operations
 such as ``pipe/cat``, ``get/put``, ``cp/mv/rm``. The async calls are
 hidden behind a synchronisation layer, so are designed to be called
 from normal code. If you are *not*
 using async-style programming, you do not need to know about how this
 works, but you might find the implementation interesting.
 
+For every synchronous function there is asynchronous one prefixed by ``_``, but
+the ``open`` operation does not support async operation. If you need it to open
+some file in async manner, it's better to asynchronously download it to
+temporary location and working with it from there.
 
 Proxy
 -----
 
 ``gcsfs`` uses ``aiohttp`` for calls to the storage api, which by default
 ignores ``HTTP_PROXY/HTTPS_PROXY`` environment variables. To read
 proxy settings from the environment provide ``session_kwargs`` as follows:
```

### Comparing `gcsfs-2023.5.0/gcsfs/checkers.py` & `gcsfs-2023.6.0/gcsfs/checkers.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs/cli/gcsfuse.py` & `gcsfs-2023.6.0/gcsfs/cli/gcsfuse.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs/core.py` & `gcsfs-2023.6.0/gcsfs/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,17 +280,18 @@
         loop=None,
         timeout=None,
         endpoint_url=None,
         default_location=None,
         version_aware=False,
         **kwargs,
     ):
+        if cache_timeout:
+            kwargs["listings_expiry_time"] = cache_timeout
         super().__init__(
             self,
-            listings_expiry_time=cache_timeout,
             asynchronous=asynchronous,
             loop=loop,
             **kwargs,
         )
         if access not in self.scopes:
             raise ValueError("access must be one of {}", self.scopes)
         if project is None:
@@ -1101,27 +1102,42 @@
     async def _pipe_file(
         self,
         path,
         data,
         metadata=None,
         consistency=None,
         content_type="application/octet-stream",
+        fixed_key_metadata=None,
         chunksize=50 * 2**20,
     ):
         # enforce blocksize should be a multiple of 2**18
         consistency = consistency or self.consistency
         bucket, key, generation = self.split_path(path)
         size = len(data)
         out = None
         if size < 5 * 2**20:
             location = await simple_upload(
-                self, bucket, key, data, metadata, consistency, content_type
+                self,
+                bucket,
+                key,
+                data,
+                metadata,
+                consistency,
+                content_type,
+                fixed_key_metadata=fixed_key_metadata,
             )
         else:
-            location = await initiate_upload(self, bucket, key, content_type, metadata)
+            location = await initiate_upload(
+                self,
+                bucket,
+                key,
+                content_type,
+                metadata,
+                fixed_key_metadata=fixed_key_metadata,
+            )
             for offset in range(0, len(data), chunksize):
                 bit = data[offset : offset + chunksize]
                 out = await upload_chunk(
                     self, location, bit, offset, size, content_type
                 )
 
             checker = get_consistency_checker(consistency)
@@ -1136,14 +1152,15 @@
         lpath,
         rpath,
         metadata=None,
         consistency=None,
         content_type="application/octet-stream",
         chunksize=50 * 2**20,
         callback=None,
+        fixed_key_metadata=None,
         **kwargs,
     ):
         # enforce blocksize should be a multiple of 2**18
         if os.path.isdir(lpath):
             return
         callback = callback or NoOpCallback()
         consistency = consistency or self.consistency
@@ -1161,20 +1178,26 @@
                     self,
                     bucket,
                     key,
                     f0.read(),
                     consistency=consistency,
                     metadatain=metadata,
                     content_type=content_type,
+                    fixed_key_metadata=fixed_key_metadata,
                 )
                 callback.absolute_update(size)
 
             else:
                 location = await initiate_upload(
-                    self, bucket, key, content_type, metadata
+                    self,
+                    bucket,
+                    key,
+                    content_type,
+                    metadata=metadata,
+                    fixed_key_metadata=fixed_key_metadata,
                 )
                 offset = 0
                 while True:
                     bit = f0.read(chunksize)
                     if not bit:
                         break
                     out = await upload_chunk(
```

### Comparing `gcsfs-2023.5.0/gcsfs/credentials.py` & `gcsfs-2023.6.0/gcsfs/credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,30 +135,32 @@
     def _connect_token(self, token):
         """
         Connect using a concrete token
 
         Parameters
         ----------
         token: str, dict or Credentials
-            If a str, try to load as a Service file, or next as a JSON; if
+            If a str and a valid file name, try to load as a Service file, or next as a JSON;
+            if not a valid file name, assume it's a valid raw (non-renewable/session) token, and pass to Credentials. If
             dict, try to interpret as credentials; if Credentials, use directly.
         """
         if isinstance(token, str):
-            if not os.path.exists(token):
-                raise FileNotFoundError(token)
-            try:
-                # is this a "service" token?
-                self._connect_service(token)
-                return
-            except:  # noqa: E722
-                # TODO: catch specific exceptions
-                # some other kind of token file
-                # will raise exception if is not json
-                with open(token) as data:
-                    token = json.load(data)
+            if os.path.exists(token):
+                try:
+                    # is this a "service" token?
+                    self._connect_service(token)
+                    return
+                except:  # noqa: E722
+                    # TODO: catch specific exceptions
+                    # some other kind of token file
+                    # will raise exception if is not json
+                    with open(token) as data:
+                        token = json.load(data)
+            else:
+                token = Credentials(token)
         if isinstance(token, dict):
             credentials = self._dict_to_credentials(token)
         elif isinstance(token, google.auth.credentials.Credentials):
             credentials = token
         else:
             raise ValueError("Token format not understood")
         self.credentials = credentials
```

### Comparing `gcsfs-2023.5.0/gcsfs/retry.py` & `gcsfs-2023.6.0/gcsfs/retry.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs/tests/conftest.py` & `gcsfs-2023.6.0/gcsfs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs/tests/test_checkers.py` & `gcsfs-2023.6.0/gcsfs/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs/tests/test_core.py` & `gcsfs-2023.6.0/gcsfs/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1360,7 +1360,14 @@
     gcs.touch(leaf2)
     gcs.touch(leaf3)
     gcs.invalidate_cache()
 
     assert gcs.ls(gparent, detail=False) == [f"{root}/t1/t2/t3"]
     gcs.glob(ggparent + "/")
     assert gcs.ls(gparent, detail=False) == [f"{root}/t1/t2/t3"]
+
+
+def test_expiry_keyword():
+    gcs = GCSFileSystem(listings_expiry_time=1, token="anon")
+    assert gcs.dircache.listings_expiry_time == 1
+    gcs = GCSFileSystem(cache_timeout=1, token="anon")
+    assert gcs.dircache.listings_expiry_time == 1
```

### Comparing `gcsfs-2023.5.0/gcsfs/tests/test_fuse.py` & `gcsfs-2023.6.0/gcsfs/tests/test_fuse.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs/tests/test_manyopens.py` & `gcsfs-2023.6.0/gcsfs/tests/test_manyopens.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs/tests/test_mapping.py` & `gcsfs-2023.6.0/gcsfs/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs/tests/test_retry.py` & `gcsfs-2023.6.0/gcsfs/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs/tests/utils.py` & `gcsfs-2023.6.0/gcsfs/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/gcsfs.egg-info/PKG-INFO` & `gcsfs-2023.6.0/gcsfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcsfs
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Convenient Filesystem interface over GCS
 Home-page: https://github.com/fsspec/gcsfs
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Keywords: google-cloud-storage,gcloud,file-system
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gcsfs-2023.5.0/gcsfs.egg-info/SOURCES.txt` & `gcsfs-2023.6.0/gcsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/setup.py` & `gcsfs-2023.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.5.0/versioneer.py` & `gcsfs-2023.6.0/versioneer.py`

 * *Files identical despite different names*

