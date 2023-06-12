# Comparing `tmp/cdk-redisdb-0.0.26.tar.gz` & `tmp/cdk-redisdb-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-redisdb-0.0.26.tar", last modified: Mon Jun 12 02:58:30 2023, max compression
+gzip compressed data, was "cdk-redisdb-0.0.27.tar", last modified: Mon Jun 12 03:53:34 2023, max compression
```

## Comparing `cdk-redisdb-0.0.26.tar` & `cdk-redisdb-0.0.27.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:58:30.143524 cdk-redisdb-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 02:58:18.000000 cdk-redisdb-0.0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 02:58:18.000000 cdk-redisdb-0.0.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-12 02:58:30.139524 cdk-redisdb-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-12 02:58:18.000000 cdk-redisdb-0.0.26/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 02:58:18.000000 cdk-redisdb-0.0.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 02:58:30.143524 cdk-redisdb-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-12 02:58:18.000000 cdk-redisdb-0.0.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:58:30.139524 cdk-redisdb-0.0.26/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:58:30.139524 cdk-redisdb-0.0.26/src/cdk_redisdb/
--rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-06-12 02:58:18.000000 cdk-redisdb-0.0.26/src/cdk_redisdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:58:30.139524 cdk-redisdb-0.0.26/src/cdk_redisdb/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-12 02:58:18.000000 cdk-redisdb-0.0.26/src/cdk_redisdb/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25941 2023-06-12 02:58:18.000000 cdk-redisdb-0.0.26/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.26.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:58:18.000000 cdk-redisdb-0.0.26/src/cdk_redisdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:58:30.139524 cdk-redisdb-0.0.26/src/cdk_redisdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-12 02:58:30.000000 cdk-redisdb-0.0.26/src/cdk_redisdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-12 02:58:30.000000 cdk-redisdb-0.0.26/src/cdk_redisdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:58:30.000000 cdk-redisdb-0.0.26/src/cdk_redisdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 02:58:30.000000 cdk-redisdb-0.0.26/src/cdk_redisdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 02:58:30.000000 cdk-redisdb-0.0.26/src/cdk_redisdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:53:34.692530 cdk-redisdb-0.0.27/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 03:53:20.000000 cdk-redisdb-0.0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 03:53:20.000000 cdk-redisdb-0.0.27/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-12 03:53:34.692530 cdk-redisdb-0.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-12 03:53:20.000000 cdk-redisdb-0.0.27/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 03:53:20.000000 cdk-redisdb-0.0.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:53:34.692530 cdk-redisdb-0.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-12 03:53:20.000000 cdk-redisdb-0.0.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:53:34.692530 cdk-redisdb-0.0.27/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:53:34.692530 cdk-redisdb-0.0.27/src/cdk_redisdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-06-12 03:53:20.000000 cdk-redisdb-0.0.27/src/cdk_redisdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:53:34.692530 cdk-redisdb-0.0.27/src/cdk_redisdb/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-12 03:53:20.000000 cdk-redisdb-0.0.27/src/cdk_redisdb/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26031 2023-06-12 03:53:20.000000 cdk-redisdb-0.0.27/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.27.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:53:20.000000 cdk-redisdb-0.0.27/src/cdk_redisdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:53:34.692530 cdk-redisdb-0.0.27/src/cdk_redisdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-12 03:53:34.000000 cdk-redisdb-0.0.27/src/cdk_redisdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-12 03:53:34.000000 cdk-redisdb-0.0.27/src/cdk_redisdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:53:34.000000 cdk-redisdb-0.0.27/src/cdk_redisdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 03:53:34.000000 cdk-redisdb-0.0.27/src/cdk_redisdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 03:53:34.000000 cdk-redisdb-0.0.27/src/cdk_redisdb.egg-info/top_level.txt
```

### Comparing `cdk-redisdb-0.0.26/LICENSE` & `cdk-redisdb-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.26/PKG-INFO` & `cdk-redisdb-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.26
+Version: 0.0.27
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-redisdb-0.0.26/README.md` & `cdk-redisdb-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.26/setup.py` & `cdk-redisdb-0.0.27/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-redisdb",
-    "version": "0.0.26",
+    "version": "0.0.27",
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "license": "Apache-2.0",
     "url": "https://github.com/forkfork/cdk-redisdb.git",
     "long_description_content_type": "text/markdown",
     "author": "Timothy Downs<timothydowns@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "cdk_redisdb",
         "cdk_redisdb._jsii"
     ],
     "package_data": {
         "cdk_redisdb._jsii": [
-            "cdk-redisdb@0.0.26.jsii.tgz"
+            "cdk-redisdb@0.0.27.jsii.tgz"
         ],
         "cdk_redisdb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.76.0, <3.0.0",
+        "aws-cdk-lib>=2.83.1, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.83.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdk-redisdb-0.0.26/src/cdk_redisdb/__init__.py` & `cdk-redisdb-0.0.27/src/cdk_redisdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.26/src/cdk_redisdb.egg-info/PKG-INFO` & `cdk-redisdb-0.0.27/src/cdk_redisdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.26
+Version: 0.0.27
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

