# Comparing `tmp/ltphotonics-1.1.1.tar.gz` & `tmp/ltphotonics-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltphotonics-1.1.1.tar", last modified: Mon Jun 12 15:20:56 2023, max compression
+gzip compressed data, was "ltphotonics-1.1.2.tar", last modified: Mon Jun 12 15:48:45 2023, max compression
```

## Comparing `ltphotonics-1.1.1.tar` & `ltphotonics-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jakebiele7   (501) staff       (20)        0 2023-06-12 15:20:56.475764 ltphotonics-1.1.1/
--rw-r--r--   0 jakebiele7   (501) staff       (20)     1082 2023-06-01 09:27:52.000000 ltphotonics-1.1.1/LICENSE
--rw-r--r--   0 jakebiele7   (501) staff       (20)     3805 2023-06-12 15:20:56.474918 ltphotonics-1.1.1/PKG-INFO
--rw-r--r--   0 jakebiele7   (501) staff       (20)     3387 2023-06-07 16:50:39.000000 ltphotonics-1.1.1/README.md
--rw-r--r--   0 jakebiele7   (501) staff       (20)    26696 2023-06-12 14:53:43.000000 ltphotonics-1.1.1/lightrig.py
-drwxr-xr-x   0 jakebiele7   (501) staff       (20)        0 2023-06-12 15:20:56.474040 ltphotonics-1.1.1/ltphotonics.egg-info/
--rw-r--r--   0 jakebiele7   (501) staff       (20)     3805 2023-06-12 15:20:56.000000 ltphotonics-1.1.1/ltphotonics.egg-info/PKG-INFO
--rw-r--r--   0 jakebiele7   (501) staff       (20)      212 2023-06-12 15:20:56.000000 ltphotonics-1.1.1/ltphotonics.egg-info/SOURCES.txt
--rw-r--r--   0 jakebiele7   (501) staff       (20)        1 2023-06-12 15:20:56.000000 ltphotonics-1.1.1/ltphotonics.egg-info/dependency_links.txt
--rw-r--r--   0 jakebiele7   (501) staff       (20)       51 2023-06-12 15:20:56.000000 ltphotonics-1.1.1/ltphotonics.egg-info/requires.txt
--rw-r--r--   0 jakebiele7   (501) staff       (20)        9 2023-06-12 15:20:56.000000 ltphotonics-1.1.1/ltphotonics.egg-info/top_level.txt
--rw-r--r--   0 jakebiele7   (501) staff       (20)       38 2023-06-12 15:20:56.475962 ltphotonics-1.1.1/setup.cfg
--rw-r--r--   0 jakebiele7   (501) staff       (20)      837 2023-06-12 15:20:33.000000 ltphotonics-1.1.1/setup.py
+drwxr-xr-x   0 jakebiele7   (501) staff       (20)        0 2023-06-12 15:48:45.019837 ltphotonics-1.1.2/
+-rw-r--r--   0 jakebiele7   (501) staff       (20)     1082 2023-06-01 09:27:52.000000 ltphotonics-1.1.2/LICENSE
+-rw-r--r--   0 jakebiele7   (501) staff       (20)     3805 2023-06-12 15:48:45.019123 ltphotonics-1.1.2/PKG-INFO
+-rw-r--r--   0 jakebiele7   (501) staff       (20)     3387 2023-06-07 16:50:39.000000 ltphotonics-1.1.2/README.md
+-rw-r--r--   0 jakebiele7   (501) staff       (20)    26696 2023-06-12 15:39:39.000000 ltphotonics-1.1.2/lightrig.py
+drwxr-xr-x   0 jakebiele7   (501) staff       (20)        0 2023-06-12 15:48:45.018258 ltphotonics-1.1.2/ltphotonics.egg-info/
+-rw-r--r--   0 jakebiele7   (501) staff       (20)     3805 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/PKG-INFO
+-rw-r--r--   0 jakebiele7   (501) staff       (20)      212 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/SOURCES.txt
+-rw-r--r--   0 jakebiele7   (501) staff       (20)        1 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/dependency_links.txt
+-rw-r--r--   0 jakebiele7   (501) staff       (20)       51 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/requires.txt
+-rw-r--r--   0 jakebiele7   (501) staff       (20)        9 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/top_level.txt
+-rw-r--r--   0 jakebiele7   (501) staff       (20)       38 2023-06-12 15:48:45.020021 ltphotonics-1.1.2/setup.cfg
+-rw-r--r--   0 jakebiele7   (501) staff       (20)      819 2023-06-12 15:48:17.000000 ltphotonics-1.1.2/setup.py
```

### Comparing `ltphotonics-1.1.1/LICENSE` & `ltphotonics-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ltphotonics-1.1.1/PKG-INFO` & `ltphotonics-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltphotonics
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python Library for interfacing with Light Trace Photonics hardware.
 Home-page: https://github.com/ltphotonics/ltphotonics
 Author: Light Trace Photonics Ltd
 Author-email: contact@ltphotonics.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ltphotonics-1.1.1/README.md` & `ltphotonics-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ltphotonics-1.1.1/lightrig.py` & `ltphotonics-1.1.2/lightrig.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from collections import deque as fifo
 from random import shuffle, randrange
 import qontrol
 import numpy as np
 import pyvisa
 import math
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 # Errors realting to the driver, as defined by Qontrol Systems
 QONTROL_ERRORS = {
 	0:'Unknown error.',
 	3:'Power error.',
 	4:'Calibration error.',
 	5:'Output error.',
```

### Comparing `ltphotonics-1.1.1/ltphotonics.egg-info/PKG-INFO` & `ltphotonics-1.1.2/ltphotonics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltphotonics
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python Library for interfacing with Light Trace Photonics hardware.
 Home-page: https://github.com/ltphotonics/ltphotonics
 Author: Light Trace Photonics Ltd
 Author-email: contact@ltphotonics.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

