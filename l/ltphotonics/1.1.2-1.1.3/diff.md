# Comparing `tmp/ltphotonics-1.1.2.tar.gz` & `tmp/ltphotonics-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltphotonics-1.1.2.tar", last modified: Mon Jun 12 15:48:45 2023, max compression
+gzip compressed data, was "ltphotonics-1.1.3.tar", last modified: Mon Jun 12 15:55:35 2023, max compression
```

## Comparing `ltphotonics-1.1.2.tar` & `ltphotonics-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jakebiele7   (501) staff       (20)        0 2023-06-12 15:48:45.019837 ltphotonics-1.1.2/
--rw-r--r--   0 jakebiele7   (501) staff       (20)     1082 2023-06-01 09:27:52.000000 ltphotonics-1.1.2/LICENSE
--rw-r--r--   0 jakebiele7   (501) staff       (20)     3805 2023-06-12 15:48:45.019123 ltphotonics-1.1.2/PKG-INFO
--rw-r--r--   0 jakebiele7   (501) staff       (20)     3387 2023-06-07 16:50:39.000000 ltphotonics-1.1.2/README.md
--rw-r--r--   0 jakebiele7   (501) staff       (20)    26696 2023-06-12 15:39:39.000000 ltphotonics-1.1.2/lightrig.py
-drwxr-xr-x   0 jakebiele7   (501) staff       (20)        0 2023-06-12 15:48:45.018258 ltphotonics-1.1.2/ltphotonics.egg-info/
--rw-r--r--   0 jakebiele7   (501) staff       (20)     3805 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/PKG-INFO
--rw-r--r--   0 jakebiele7   (501) staff       (20)      212 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/SOURCES.txt
--rw-r--r--   0 jakebiele7   (501) staff       (20)        1 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/dependency_links.txt
--rw-r--r--   0 jakebiele7   (501) staff       (20)       51 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/requires.txt
--rw-r--r--   0 jakebiele7   (501) staff       (20)        9 2023-06-12 15:48:44.000000 ltphotonics-1.1.2/ltphotonics.egg-info/top_level.txt
--rw-r--r--   0 jakebiele7   (501) staff       (20)       38 2023-06-12 15:48:45.020021 ltphotonics-1.1.2/setup.cfg
--rw-r--r--   0 jakebiele7   (501) staff       (20)      819 2023-06-12 15:48:17.000000 ltphotonics-1.1.2/setup.py
+drwxr-xr-x   0 jakebiele7   (501) staff       (20)        0 2023-06-12 15:55:35.205399 ltphotonics-1.1.3/
+-rw-r--r--   0 jakebiele7   (501) staff       (20)     1082 2023-06-01 09:27:52.000000 ltphotonics-1.1.3/LICENSE
+-rw-r--r--   0 jakebiele7   (501) staff       (20)     3805 2023-06-12 15:55:35.204441 ltphotonics-1.1.3/PKG-INFO
+-rw-r--r--   0 jakebiele7   (501) staff       (20)     3387 2023-06-07 16:50:39.000000 ltphotonics-1.1.3/README.md
+-rw-r--r--   0 jakebiele7   (501) staff       (20)    26696 2023-06-12 15:54:54.000000 ltphotonics-1.1.3/lightrig.py
+drwxr-xr-x   0 jakebiele7   (501) staff       (20)        0 2023-06-12 15:55:35.203745 ltphotonics-1.1.3/ltphotonics.egg-info/
+-rw-r--r--   0 jakebiele7   (501) staff       (20)     3805 2023-06-12 15:55:35.000000 ltphotonics-1.1.3/ltphotonics.egg-info/PKG-INFO
+-rw-r--r--   0 jakebiele7   (501) staff       (20)      212 2023-06-12 15:55:35.000000 ltphotonics-1.1.3/ltphotonics.egg-info/SOURCES.txt
+-rw-r--r--   0 jakebiele7   (501) staff       (20)        1 2023-06-12 15:55:35.000000 ltphotonics-1.1.3/ltphotonics.egg-info/dependency_links.txt
+-rw-r--r--   0 jakebiele7   (501) staff       (20)       51 2023-06-12 15:55:35.000000 ltphotonics-1.1.3/ltphotonics.egg-info/requires.txt
+-rw-r--r--   0 jakebiele7   (501) staff       (20)        9 2023-06-12 15:55:35.000000 ltphotonics-1.1.3/ltphotonics.egg-info/top_level.txt
+-rw-r--r--   0 jakebiele7   (501) staff       (20)       38 2023-06-12 15:55:35.205659 ltphotonics-1.1.3/setup.cfg
+-rw-r--r--   0 jakebiele7   (501) staff       (20)      819 2023-06-12 15:55:23.000000 ltphotonics-1.1.3/setup.py
```

### Comparing `ltphotonics-1.1.2/LICENSE` & `ltphotonics-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ltphotonics-1.1.2/PKG-INFO` & `ltphotonics-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltphotonics
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python Library for interfacing with Light Trace Photonics hardware.
 Home-page: https://github.com/ltphotonics/ltphotonics
 Author: Light Trace Photonics Ltd
 Author-email: contact@ltphotonics.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ltphotonics-1.1.2/README.md` & `ltphotonics-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ltphotonics-1.1.2/lightrig.py` & `ltphotonics-1.1.3/lightrig.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from collections import deque as fifo
 from random import shuffle, randrange
 import qontrol
 import numpy as np
 import pyvisa
 import math
 
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 # Errors realting to the driver, as defined by Qontrol Systems
 QONTROL_ERRORS = {
 	0:'Unknown error.',
 	3:'Power error.',
 	4:'Calibration error.',
 	5:'Output error.',
```

### Comparing `ltphotonics-1.1.2/ltphotonics.egg-info/PKG-INFO` & `ltphotonics-1.1.3/ltphotonics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltphotonics
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python Library for interfacing with Light Trace Photonics hardware.
 Home-page: https://github.com/ltphotonics/ltphotonics
 Author: Light Trace Photonics Ltd
 Author-email: contact@ltphotonics.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ltphotonics-1.1.2/setup.py` & `ltphotonics-1.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 import setuptools
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 setuptools.setup(
     name="ltphotonics",
     version=__version__,
     description="Python Library for interfacing with Light Trace Photonics hardware.",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -17,9 +17,9 @@
     author="Light Trace Photonics Ltd",
     author_email="contact@ltphotonics.co.uk",
     py_modules=["lightrig"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    install_requires=["libsub", "pyvisa-py", "pyusb", "pyserial", "qontrol", "numpy", "math"],
+    install_requires=["libusb", "pyvisa-py", "pyusb", "pyserial", "qontrol", "numpy", "math"],
 )
```

