# Comparing `tmp/emr-sfn-waiter-0.0.2.tar.gz` & `tmp/emr-sfn-waiter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emr-sfn-waiter-0.0.2.tar", last modified: Sun May 14 10:48:29 2023, max compression
+gzip compressed data, was "emr-sfn-waiter-0.0.3.tar", last modified: Mon Jun 12 13:43:48 2023, max compression
```

## Comparing `emr-sfn-waiter-0.0.2.tar` & `emr-sfn-waiter-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:48:29.832137 emr-sfn-waiter-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-14 10:48:14.000000 emr-sfn-waiter-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 10:48:14.000000 emr-sfn-waiter-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-14 10:48:29.828137 emr-sfn-waiter-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 10:48:14.000000 emr-sfn-waiter-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-14 10:48:14.000000 emr-sfn-waiter-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 10:48:29.832137 emr-sfn-waiter-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-14 10:48:14.000000 emr-sfn-waiter-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:48:29.828137 emr-sfn-waiter-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:48:29.828137 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:48:29.828137 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-14 10:48:14.000000 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    80051 2023-05-14 10:48:14.000000 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter/_jsii/emr-sfn-waiter@0.0.2.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:48:29.828137 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-14 10:48:29.000000 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-14 10:48:29.000000 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 10:48:29.000000 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-14 10:48:29.000000 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-14 10:48:29.000000 emr-sfn-waiter-0.0.2/src/emr_sfn_waiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:43:48.959012 emr-sfn-waiter-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-12 13:43:33.000000 emr-sfn-waiter-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 13:43:33.000000 emr-sfn-waiter-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-12 13:43:48.959012 emr-sfn-waiter-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 13:43:33.000000 emr-sfn-waiter-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 13:43:33.000000 emr-sfn-waiter-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:43:48.959012 emr-sfn-waiter-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-12 13:43:33.000000 emr-sfn-waiter-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:43:48.955012 emr-sfn-waiter-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:43:48.955012 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:43:48.959012 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-12 13:43:33.000000 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80096 2023-06-12 13:43:33.000000 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter/_jsii/emr-sfn-waiter@0.0.3.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:43:48.959012 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-12 13:43:48.000000 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-12 13:43:48.000000 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:43:48.000000 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 13:43:48.000000 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 13:43:48.000000 emr-sfn-waiter-0.0.3/src/emr_sfn_waiter.egg-info/top_level.txt
```

### Comparing `emr-sfn-waiter-0.0.2/LICENSE` & `emr-sfn-waiter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `emr-sfn-waiter-0.0.2/PKG-INFO` & `emr-sfn-waiter-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emr-sfn-waiter
-Version: 0.0.2
+Version: 0.0.3
 Summary: CDK library for an SFN workflow that polls for EMR Serverless job completion
 Home-page: https://github.com/alexgelman/emr-sfn-waiter
 Author: Alex Gelman<6887237+alexgelman@users.noreply.github.com>
 License: MIT
 Project-URL: Source, https://github.com/alexgelman/emr-sfn-waiter
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `emr-sfn-waiter-0.0.2/setup.py` & `emr-sfn-waiter-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "emr-sfn-waiter",
-    "version": "0.0.2",
+    "version": "0.0.3",
     "description": "CDK library for an SFN workflow that polls for EMR Serverless job completion",
     "license": "MIT",
     "url": "https://github.com/alexgelman/emr-sfn-waiter",
     "long_description_content_type": "text/markdown",
     "author": "Alex Gelman<6887237+alexgelman@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -21,22 +21,22 @@
         "": "src"
     },
     "packages": [
         "emr_sfn_waiter._jsii"
     ],
     "package_data": {
         "emr_sfn_waiter._jsii": [
-            "emr-sfn-waiter@0.0.2.jsii.tgz"
+            "emr-sfn-waiter@0.0.3.jsii.tgz"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.79.1",
-        "constructs>=10.2.23, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "aws-cdk-lib==2.83.1",
+        "constructs>=10.2.50, <11.0.0",
+        "jsii>=1.83.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `emr-sfn-waiter-0.0.2/src/emr_sfn_waiter.egg-info/PKG-INFO` & `emr-sfn-waiter-0.0.3/src/emr_sfn_waiter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emr-sfn-waiter
-Version: 0.0.2
+Version: 0.0.3
 Summary: CDK library for an SFN workflow that polls for EMR Serverless job completion
 Home-page: https://github.com/alexgelman/emr-sfn-waiter
 Author: Alex Gelman<6887237+alexgelman@users.noreply.github.com>
 License: MIT
 Project-URL: Source, https://github.com/alexgelman/emr-sfn-waiter
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

