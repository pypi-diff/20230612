# Comparing `tmp/qsiprep-container-0.8.0rc3.tar.gz` & `tmp/qsiprep-container-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qsiprep-container-0.8.0rc3.tar", last modified: Wed Feb 19 09:37:59 2020, max compression
+gzip compressed data, was "dist/qsiprep-container-0.9.0b1.tar", last modified: Thu Jun 18 15:13:51 2020, max compression
```

## Comparing `qsiprep-container-0.8.0rc3.tar` & `qsiprep-container-0.9.0b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15466 2020-02-19 09:31:48.000000 qsiprep-container-0.8.0rc3/qsiprep_singularity.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       38 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/setup.cfg
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/qsiprep_container.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      297 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/qsiprep_container.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      103 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/qsiprep_container.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       35 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/qsiprep_container.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      949 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/qsiprep_container.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/qsiprep_container.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/qsiprep_container.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1310 2020-02-19 09:31:48.000000 qsiprep-container-0.8.0rc3/setup.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      949 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/PKG-INFO
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)    15529 2020-02-19 09:37:59.000000 qsiprep-container-0.8.0rc3/qsiprep_docker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:13:51.253168 qsiprep-container-0.9.0b1/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      948 2020-06-18 15:13:51.253168 qsiprep-container-0.9.0b1/PKG-INFO
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:13:51.253168 qsiprep-container-0.9.0b1/qsiprep_container.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      948 2020-06-18 15:13:51.000000 qsiprep-container-0.9.0b1/qsiprep_container.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      297 2020-06-18 15:13:51.000000 qsiprep-container-0.9.0b1/qsiprep_container.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2020-06-18 15:13:51.000000 qsiprep-container-0.9.0b1/qsiprep_container.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      103 2020-06-18 15:13:51.000000 qsiprep-container-0.9.0b1/qsiprep_container.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2020-06-18 15:13:51.000000 qsiprep-container-0.9.0b1/qsiprep_container.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       35 2020-06-18 15:13:51.000000 qsiprep-container-0.9.0b1/qsiprep_container.egg-info/top_level.txt
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)    15531 2020-06-18 15:13:48.000000 qsiprep-container-0.9.0b1/qsiprep_docker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15466 2020-06-18 15:02:34.000000 qsiprep-container-0.9.0b1/qsiprep_singularity.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       38 2020-06-18 15:13:51.253168 qsiprep-container-0.9.0b1/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1310 2020-06-18 15:02:34.000000 qsiprep-container-0.9.0b1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qsiprep-container-0.8.0rc3/qsiprep_singularity.py` & `qsiprep-container-0.9.0b1/qsiprep_singularity.py`

 * *Files identical despite different names*

### Comparing `qsiprep-container-0.8.0rc3/qsiprep_container.egg-info/PKG-INFO` & `qsiprep-container-0.9.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: qsiprep-container
-Version: 0.8.0rc3
+Version: 0.9.0b1
 Summary: qsiprep is a non-DTI diffusion-weighted image pre-processing pipeline that is designed to provide an easily accessible, state-of-the-art interface that is robust to differences in scan acquisition protocols and that requires minimal user input, while providing easily interpretable and comprehensive error and output reporting.
 Home-page: https://github.com/pennbbl/qsiprep
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: 3-clause BSD
```

### Comparing `qsiprep-container-0.8.0rc3/setup.py` & `qsiprep-container-0.9.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `qsiprep-container-0.8.0rc3/PKG-INFO` & `qsiprep-container-0.9.0b1/qsiprep_container.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: qsiprep-container
-Version: 0.8.0rc3
+Version: 0.9.0b1
 Summary: qsiprep is a non-DTI diffusion-weighted image pre-processing pipeline that is designed to provide an easily accessible, state-of-the-art interface that is robust to differences in scan acquisition protocols and that requires minimal user input, while providing easily interpretable and comprehensive error and output reporting.
 Home-page: https://github.com/pennbbl/qsiprep
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: 3-clause BSD
```

### Comparing `qsiprep-container-0.8.0rc3/qsiprep_docker.py` & `qsiprep-container-0.9.0b1/qsiprep_docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 uses (https://qsiprep.readthedocs.io/en/latest/citing.html).
 """
 import sys
 import os
 import re
 import subprocess
 
-__version__ = '0.8.0RC3'
+__version__ = '0.9.0beta1'
 __packagename__ = 'qsiprep-container'
 __author__ = ''
 __copyright__ = 'Copyright 2019, '
 __credits__ = []
 __license__ = '3-clause BSD'
 __maintainer__ = ''
 __email__ = ''
```

