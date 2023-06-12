# Comparing `tmp/unicorn-multiverse-0.0.2.tar.gz` & `tmp/unicorn-multiverse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicorn-multiverse-0.0.2.tar", last modified: Mon Jun 12 15:19:13 2023, max compression
+gzip compressed data, was "unicorn-multiverse-0.0.3.tar", last modified: Mon Jun 12 15:23:04 2023, max compression
```

## Comparing `unicorn-multiverse-0.0.2.tar` & `unicorn-multiverse-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-06-12 15:19:13.350422 unicorn-multiverse-0.0.2/
--rw-rw-r--   0 phil      (1000) phil      (1000)       30 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.2/CHANGELOG.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1065 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.2/LICENSE.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      110 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.2/MANIFEST.in
--rw-rw-r--   0 phil      (1000) phil      (1000)      879 2023-06-12 15:19:13.350422 unicorn-multiverse-0.0.2/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)       74 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.2/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-06-12 15:19:13.346422 unicorn-multiverse-0.0.2/multiverse/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3572 2023-06-12 15:03:33.000000 unicorn-multiverse-0.0.2/multiverse/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       97 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.2/pyproject.toml
--rw-rw-r--   0 phil      (1000) phil      (1000)      863 2023-06-12 15:19:13.350422 unicorn-multiverse-0.0.2/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)       82 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.2/setup.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-06-12 15:19:13.350422 unicorn-multiverse-0.0.2/unicorn_multiverse.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)      879 2023-06-12 15:19:13.000000 unicorn-multiverse-0.0.2/unicorn_multiverse.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      313 2023-06-12 15:19:13.000000 unicorn-multiverse-0.0.2/unicorn_multiverse.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2023-06-12 15:19:13.000000 unicorn-multiverse-0.0.2/unicorn_multiverse.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       15 2023-06-12 15:19:13.000000 unicorn-multiverse-0.0.2/unicorn_multiverse.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       11 2023-06-12 15:19:13.000000 unicorn-multiverse-0.0.2/unicorn_multiverse.egg-info/top_level.txt
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-06-12 15:23:04.578707 unicorn-multiverse-0.0.3/
+-rw-rw-r--   0 phil      (1000) phil      (1000)       30 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.3/CHANGELOG.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1065 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.3/LICENSE.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      110 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.3/MANIFEST.in
+-rw-rw-r--   0 phil      (1000) phil      (1000)      879 2023-06-12 15:23:04.578707 unicorn-multiverse-0.0.3/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)       74 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.3/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-06-12 15:23:04.578707 unicorn-multiverse-0.0.3/multiverse/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3572 2023-06-12 15:21:56.000000 unicorn-multiverse-0.0.3/multiverse/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       97 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.3/pyproject.toml
+-rw-rw-r--   0 phil      (1000) phil      (1000)      863 2023-06-12 15:23:04.578707 unicorn-multiverse-0.0.3/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)       82 2023-06-12 15:01:02.000000 unicorn-multiverse-0.0.3/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-06-12 15:23:04.578707 unicorn-multiverse-0.0.3/unicorn_multiverse.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      879 2023-06-12 15:23:04.000000 unicorn-multiverse-0.0.3/unicorn_multiverse.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      313 2023-06-12 15:23:04.000000 unicorn-multiverse-0.0.3/unicorn_multiverse.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2023-06-12 15:23:04.000000 unicorn-multiverse-0.0.3/unicorn_multiverse.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       15 2023-06-12 15:23:04.000000 unicorn-multiverse-0.0.3/unicorn_multiverse.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       11 2023-06-12 15:23:04.000000 unicorn-multiverse-0.0.3/unicorn_multiverse.egg-info/top_level.txt
```

### Comparing `unicorn-multiverse-0.0.2/LICENSE.txt` & `unicorn-multiverse-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unicorn-multiverse-0.0.2/PKG-INFO` & `unicorn-multiverse-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicorn-multiverse
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multi USB serial display driver
 Home-page: https://www.github.com/gadgetoid/gu-multiverse
 Author: Philip Howard
 Author-email: phil@gadgetoid.com
 License: MIT
 Project-URL: GitHub, https://www.github.com/gadgetoid/gu-multiverse
 Keywords: Raspberry Pi Pico
```

### Comparing `unicorn-multiverse-0.0.2/multiverse/__init__.py` & `unicorn-multiverse-0.0.3/multiverse/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy
 import serial
 import threading
 import signal
 import time
 
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 # Class to represent a single Galactic Unicorn display
 # handy place to store the serial port opening and such
 class Display:
     # Just in case we get fancy and use RGB565 or RGB332
     BYTES_PER_PIXEL = 4
```

### Comparing `unicorn-multiverse-0.0.2/setup.cfg` & `unicorn-multiverse-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unicorn-multiverse
-version = 0.0.2
+version = 0.0.3
 author = Philip Howard
 author_email = phil@gadgetoid.com
 description = Multi USB serial display driver
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Raspberry Pi Pico
 url = https://www.github.com/gadgetoid/gu-multiverse
```

### Comparing `unicorn-multiverse-0.0.2/unicorn_multiverse.egg-info/PKG-INFO` & `unicorn-multiverse-0.0.3/unicorn_multiverse.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicorn-multiverse
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multi USB serial display driver
 Home-page: https://www.github.com/gadgetoid/gu-multiverse
 Author: Philip Howard
 Author-email: phil@gadgetoid.com
 License: MIT
 Project-URL: GitHub, https://www.github.com/gadgetoid/gu-multiverse
 Keywords: Raspberry Pi Pico
```

