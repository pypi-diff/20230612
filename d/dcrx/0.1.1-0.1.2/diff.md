# Comparing `tmp/dcrx-0.1.1.tar.gz` & `tmp/dcrx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-0.1.1.tar", last modified: Mon Jun 12 04:10:11 2023, max compression
+gzip compressed data, was "dcrx-0.1.2.tar", last modified: Mon Jun 12 15:19:21 2023, max compression
```

## Comparing `dcrx-0.1.1.tar` & `dcrx-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:10:11.071250 dcrx-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 04:10:01.000000 dcrx-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-12 04:10:11.071250 dcrx-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-12 04:10:01.000000 dcrx-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:10:11.067250 dcrx-0.1.1/dcrx/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:10:11.071250 dcrx-0.1.1/dcrx/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/expose.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:10:11.071250 dcrx-0.1.1/dcrx/layers/mount_types/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/mount_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/mount_types/bind_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/mount_types/cache_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/mount_types/secret_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/mount_types/ssh_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/mount_types/tmpfs_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/layers/workdir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:10:11.071250 dcrx-0.1.1/dcrx/memory_file/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/memory_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-12 04:10:01.000000 dcrx-0.1.1/dcrx/memory_file/memory_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:10:11.067250 dcrx-0.1.1/dcrx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-12 04:10:11.000000 dcrx-0.1.1/dcrx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-12 04:10:11.000000 dcrx-0.1.1/dcrx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:10:11.000000 dcrx-0.1.1/dcrx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 04:10:11.000000 dcrx-0.1.1/dcrx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 04:10:11.000000 dcrx-0.1.1/dcrx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 04:10:11.071250 dcrx-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-12 04:10:01.000000 dcrx-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:21.248179 dcrx-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 15:19:12.000000 dcrx-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-12 15:19:21.248179 dcrx-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-12 15:19:12.000000 dcrx-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:21.244179 dcrx-0.1.2/dcrx/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:21.248179 dcrx-0.1.2/dcrx/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/expose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:21.248179 dcrx-0.1.2/dcrx/layers/mount_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/mount_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/mount_types/bind_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/mount_types/cache_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/mount_types/secret_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/mount_types/ssh_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/mount_types/tmpfs_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/layers/workdir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:21.248179 dcrx-0.1.2/dcrx/memory_file/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/memory_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-12 15:19:12.000000 dcrx-0.1.2/dcrx/memory_file/memory_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:21.244179 dcrx-0.1.2/dcrx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-12 15:19:21.000000 dcrx-0.1.2/dcrx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-12 15:19:21.000000 dcrx-0.1.2/dcrx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:19:21.000000 dcrx-0.1.2/dcrx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 15:19:21.000000 dcrx-0.1.2/dcrx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 15:19:21.000000 dcrx-0.1.2/dcrx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:19:21.248179 dcrx-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-12 15:19:12.000000 dcrx-0.1.2/setup.py
```

### Comparing `dcrx-0.1.1/LICENSE` & `dcrx-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/PKG-INFO` & `dcrx-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for typesafe, programmatic generation of Docker images via SQL-builder like API.
 Home-page: https://github.com/scorbettUM/dcrx
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-0.1.1/README.md` & `dcrx-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx/image.py` & `dcrx-0.1.2/dcrx/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,16 +159,17 @@
 
         with open(self.filename, 'w') as dockerfile:
             dockerfile.write(
                 self.to_string()
             )
 
     def clear(self):
-        os.remove(self.filename)
-        self.layers.clear()
+        if os.path.exists(self.filename):
+            os.remove(self.filename)
+            self.layers.clear()
     
     def add(
         self,
         source: str,
         destination: str,
         user_id: Optional[str]=None,
         group_id: Optional[str]=None,
```

### Comparing `dcrx-0.1.1/dcrx/layers/add.py` & `dcrx-0.1.2/dcrx/layers/add.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx/layers/arg.py` & `dcrx-0.1.2/dcrx/layers/arg.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx/layers/copy.py` & `dcrx-0.1.2/dcrx/layers/copy.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx/layers/healthcheck.py` & `dcrx-0.1.2/dcrx/layers/healthcheck.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx/layers/mount_types/bind_mount.py` & `dcrx-0.1.2/dcrx/layers/mount_types/bind_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx/layers/mount_types/cache_mount.py` & `dcrx-0.1.2/dcrx/layers/mount_types/cache_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx/layers/mount_types/secret_mount.py` & `dcrx-0.1.2/dcrx/layers/mount_types/secret_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx/layers/mount_types/ssh_mount.py` & `dcrx-0.1.2/dcrx/layers/mount_types/ssh_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx/layers/run.py` & `dcrx-0.1.2/dcrx/layers/run.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/dcrx.egg-info/PKG-INFO` & `dcrx-0.1.2/dcrx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for typesafe, programmatic generation of Docker images via SQL-builder like API.
 Home-page: https://github.com/scorbettUM/dcrx
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-0.1.1/dcrx.egg-info/SOURCES.txt` & `dcrx-0.1.2/dcrx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-0.1.1/setup.py` & `dcrx-0.1.2/setup.py`

 * *Files identical despite different names*

