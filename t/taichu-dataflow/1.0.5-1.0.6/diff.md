# Comparing `tmp/taichu-dataflow-1.0.5.tar.gz` & `tmp/taichu-dataflow-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taichu-dataflow-1.0.5.tar", last modified: Mon Jun 12 08:23:11 2023, max compression
+gzip compressed data, was "taichu-dataflow-1.0.6.tar", last modified: Mon Jun 12 08:27:44 2023, max compression
```

## Comparing `taichu-dataflow-1.0.5.tar` & `taichu-dataflow-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/
--rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/PKG-INFO
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/taichu_dataflow.egg-info/
--rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/taichu_dataflow.egg-info/PKG-INFO
--rw-r--r--   0 shenli     (501) staff       (20)      444 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/taichu_dataflow.egg-info/SOURCES.txt
--rw-r--r--   0 shenli     (501) staff       (20)       13 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/taichu_dataflow.egg-info/requires.txt
--rw-r--r--   0 shenli     (501) staff       (20)       16 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/taichu_dataflow.egg-info/top_level.txt
--rw-r--r--   0 shenli     (501) staff       (20)        1 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/taichu_dataflow.egg-info/dependency_links.txt
--rw-r--r--   0 shenli     (501) staff       (20)      194 2023-06-12 03:14:29.000000 taichu-dataflow-1.0.5/README.md
--rw-r--r--   0 shenli     (501) staff       (20)      699 2023-06-12 08:23:00.000000 taichu-dataflow-1.0.5/setup.py
--rw-r--r--   0 shenli     (501) staff       (20)       38 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/setup.cfg
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/taichu_dataflow/
--rwxrwxrwx   0 shenli     (501) staff       (20)     1151 2023-06-12 08:16:05.000000 taichu-dataflow-1.0.5/taichu_dataflow/filebeat.sh
--rw-r--r--   0 shenli     (501) staff       (20)      534 2023-06-12 08:16:05.000000 taichu-dataflow-1.0.5/taichu_dataflow/__init__.py
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 08:23:11.000000 taichu-dataflow-1.0.5/taichu_dataflow/storage/
--rw-r--r--   0 shenli     (501) staff       (20)      437 2023-06-09 10:38:26.000000 taichu-dataflow-1.0.5/taichu_dataflow/storage/env.py
--rw-r--r--   0 shenli     (501) staff       (20)     1317 2023-06-12 08:16:52.000000 taichu-dataflow-1.0.5/taichu_dataflow/storage/alluxio.py
--rw-r--r--   0 shenli     (501) staff       (20)        0 2023-06-09 10:38:26.000000 taichu-dataflow-1.0.5/taichu_dataflow/storage/__init__.py
--rw-r--r--   0 shenli     (501) staff       (20)     1881 2023-06-12 08:16:52.000000 taichu-dataflow-1.0.5/taichu_dataflow/storage/export_back.py
--rw-r--r--   0 shenli     (501) staff       (20)      451 2023-06-12 08:16:52.000000 taichu-dataflow-1.0.5/taichu_dataflow/storage/storage.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:27:44.360399 taichu-dataflow-1.0.6/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 08:27:44.360113 taichu-dataflow-1.0.6/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      194 2023-06-12 02:53:15.000000 taichu-dataflow-1.0.6/README.md
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-06-12 08:27:44.360703 taichu-dataflow-1.0.6/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      640 2023-06-12 08:27:31.000000 taichu-dataflow-1.0.6/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:27:44.357928 taichu-dataflow-1.0.6/taichu_dataflow/
+-rw-r--r--   0 wangkun    (501) staff       (20)      534 2023-06-12 08:21:43.000000 taichu-dataflow-1.0.6/taichu_dataflow/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1317 2023-06-12 07:27:41.000000 taichu-dataflow-1.0.6/taichu_dataflow/alluxio.py
+-rw-r--r--   0 wangkun    (501) staff       (20)      437 2023-06-12 02:48:22.000000 taichu-dataflow-1.0.6/taichu_dataflow/env.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1881 2023-06-12 07:27:41.000000 taichu-dataflow-1.0.6/taichu_dataflow/export_back.py
+-rw-r--r--   0 wangkun    (501) staff       (20)      451 2023-06-12 07:27:41.000000 taichu-dataflow-1.0.6/taichu_dataflow/storage.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-12 08:27:44.359671 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      348 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       13 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       16 2023-06-12 08:27:44.000000 taichu-dataflow-1.0.6/taichu_dataflow.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `taichu-dataflow-1.0.5/setup.py` & `taichu-dataflow-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,18 @@
 
     long_description = ''
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='1.0.5',
+        version='1.0.6',
         description='taichu serve is a tool for serving dataflow',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
         install_requires=requirements,
         include_package_data=True,
-        package_data={
-            '': ['*.sh'],
-        }
     )
```

### Comparing `taichu-dataflow-1.0.5/taichu_dataflow/__init__.py` & `taichu-dataflow-1.0.6/taichu_dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-dataflow-1.0.5/taichu_dataflow/storage/alluxio.py` & `taichu-dataflow-1.0.6/taichu_dataflow/alluxio.py`

 * *Files identical despite different names*

### Comparing `taichu-dataflow-1.0.5/taichu_dataflow/storage/export_back.py` & `taichu-dataflow-1.0.6/taichu_dataflow/export_back.py`

 * *Files identical despite different names*

