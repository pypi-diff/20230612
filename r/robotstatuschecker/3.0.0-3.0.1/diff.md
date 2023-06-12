# Comparing `tmp/robotstatuschecker-3.0.0.tar.gz` & `tmp/robotstatuschecker-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotstatuschecker-3.0.0.tar", last modified: Sun Feb  5 20:20:25 2023, max compression
+gzip compressed data, was "robotstatuschecker-3.0.1.tar", last modified: Mon Jun 12 20:24:44 2023, max compression
```

## Comparing `robotstatuschecker-3.0.0.tar` & `robotstatuschecker-3.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-02-05 20:20:25.890298 robotstatuschecker-3.0.0/
--rw-r--r--   0 tatuaalto   (501) staff       (20)       42 2023-02-05 19:08:27.000000 robotstatuschecker-3.0.0/MANIFEST.in
--rw-r--r--   0 tatuaalto   (501) staff       (20)     7827 2023-02-05 20:20:25.890174 robotstatuschecker-3.0.0/PKG-INFO
--rw-r--r--   0 tatuaalto   (501) staff       (20)     7036 2023-02-05 19:08:27.000000 robotstatuschecker-3.0.0/README.rst
--rw-r--r--   0 tatuaalto   (501) staff       (20)       57 2023-02-05 19:08:27.000000 robotstatuschecker-3.0.0/pyproject.toml
-drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-02-05 20:20:25.889995 robotstatuschecker-3.0.0/robotstatuschecker.egg-info/
--rw-r--r--   0 tatuaalto   (501) staff       (20)     7827 2023-02-05 20:20:25.000000 robotstatuschecker-3.0.0/robotstatuschecker.egg-info/PKG-INFO
--rw-r--r--   0 tatuaalto   (501) staff       (20)      277 2023-02-05 20:20:25.000000 robotstatuschecker-3.0.0/robotstatuschecker.egg-info/SOURCES.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)        1 2023-02-05 20:20:25.000000 robotstatuschecker-3.0.0/robotstatuschecker.egg-info/dependency_links.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)       15 2023-02-05 20:20:25.000000 robotstatuschecker-3.0.0/robotstatuschecker.egg-info/requires.txt
--rw-r--r--   0 tatuaalto   (501) staff       (20)       19 2023-02-05 20:20:25.000000 robotstatuschecker-3.0.0/robotstatuschecker.egg-info/top_level.txt
--rwxr-xr-x   0 tatuaalto   (501) staff       (20)    11639 2023-02-05 20:19:49.000000 robotstatuschecker-3.0.0/robotstatuschecker.py
--rw-r--r--   0 tatuaalto   (501) staff       (20)       38 2023-02-05 20:20:25.890335 robotstatuschecker-3.0.0/setup.cfg
--rwxr-xr-x   0 tatuaalto   (501) staff       (20)     1434 2023-02-05 19:08:27.000000 robotstatuschecker-3.0.0/setup.py
+drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-06-12 20:24:44.633462 robotstatuschecker-3.0.1/
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       42 2023-02-05 19:08:27.000000 robotstatuschecker-3.0.1/MANIFEST.in
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     7955 2023-06-12 20:24:44.633343 robotstatuschecker-3.0.1/PKG-INFO
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     7164 2023-02-05 20:25:34.000000 robotstatuschecker-3.0.1/README.rst
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       57 2023-02-05 20:27:13.000000 robotstatuschecker-3.0.1/pyproject.toml
+drwxr-xr-x   0 tatuaalto   (501) staff       (20)        0 2023-06-12 20:24:44.633182 robotstatuschecker-3.0.1/robotstatuschecker.egg-info/
+-rw-r--r--   0 tatuaalto   (501) staff       (20)     7955 2023-06-12 20:24:44.000000 robotstatuschecker-3.0.1/robotstatuschecker.egg-info/PKG-INFO
+-rw-r--r--   0 tatuaalto   (501) staff       (20)      277 2023-06-12 20:24:44.000000 robotstatuschecker-3.0.1/robotstatuschecker.egg-info/SOURCES.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)        1 2023-06-12 20:24:44.000000 robotstatuschecker-3.0.1/robotstatuschecker.egg-info/dependency_links.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       15 2023-06-12 20:24:44.000000 robotstatuschecker-3.0.1/robotstatuschecker.egg-info/requires.txt
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       19 2023-06-12 20:24:44.000000 robotstatuschecker-3.0.1/robotstatuschecker.egg-info/top_level.txt
+-rwxr-xr-x   0 tatuaalto   (501) staff       (20)    12036 2023-06-12 20:22:18.000000 robotstatuschecker-3.0.1/robotstatuschecker.py
+-rw-r--r--   0 tatuaalto   (501) staff       (20)       38 2023-06-12 20:24:44.633495 robotstatuschecker-3.0.1/setup.cfg
+-rwxr-xr-x   0 tatuaalto   (501) staff       (20)     1434 2023-02-05 19:08:27.000000 robotstatuschecker-3.0.1/setup.py
```

### Comparing `robotstatuschecker-3.0.0/PKG-INFO` & `robotstatuschecker-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotstatuschecker
-Version: 3.0.0
+Version: 3.0.1
 Summary: A tool for checking that Robot Framework test cases have expected statuses and log messages.
 Home-page: https://github.com/robotframework/statuschecker
 Download-URL: https://pypi.python.org/pypi/robotstatuschecker
 Author: Robot Framework Developers
 Author-email: robotframework@gmail.com
 License: Apache License 2.0
 Keywords: robotframework testing testautomation atdd
@@ -231,7 +231,11 @@
         [Documentation]    LOG 1        STARTS: Hello w
         Steps
 
     No message
         [Documentation]    LOG 1:1      Test that we have only 1 msg
         ...                LOG 1:2      NONE
         Steps
+
+    Count Messages
+        [Documentation]    LOG 4 COUNT: 2    # Fourth keyword should have excatly 2 messages.
+        Steps
```

### Comparing `robotstatuschecker-3.0.0/README.rst` & `robotstatuschecker-3.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -212,7 +212,11 @@
         [Documentation]    LOG 1        STARTS: Hello w
         Steps
 
     No message
         [Documentation]    LOG 1:1      Test that we have only 1 msg
         ...                LOG 1:2      NONE
         Steps
+
+    Count Messages
+        [Documentation]    LOG 4 COUNT: 2    # Fourth keyword should have excatly 2 messages.
+        Steps
```

### Comparing `robotstatuschecker-3.0.0/robotstatuschecker.egg-info/PKG-INFO` & `robotstatuschecker-3.0.1/robotstatuschecker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotstatuschecker
-Version: 3.0.0
+Version: 3.0.1
 Summary: A tool for checking that Robot Framework test cases have expected statuses and log messages.
 Home-page: https://github.com/robotframework/statuschecker
 Download-URL: https://pypi.python.org/pypi/robotstatuschecker
 Author: Robot Framework Developers
 Author-email: robotframework@gmail.com
 License: Apache License 2.0
 Keywords: robotframework testing testautomation atdd
@@ -231,7 +231,11 @@
         [Documentation]    LOG 1        STARTS: Hello w
         Steps
 
     No message
         [Documentation]    LOG 1:1      Test that we have only 1 msg
         ...                LOG 1:2      NONE
         Steps
+
+    Count Messages
+        [Documentation]    LOG 4 COUNT: 2    # Fourth keyword should have excatly 2 messages.
+        Steps
```

### Comparing `robotstatuschecker-3.0.0/robotstatuschecker.py` & `robotstatuschecker-3.0.1/robotstatuschecker.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,20 @@
 If an output file is not given, the input file is edited in place.
 """
 
 import re
 import sys
 from os.path import abspath
 
+from robot import __version__ as rf_version
 from robot.api import ExecutionResult, ResultVisitor
 from robot.utils import Matcher
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
+RF_61 = tuple(rf_version.split(".")[:2]) >= ("6", "1")
 
 
 def process_output(inpath, outpath=None, verbose=True):
     """The main programmatic entry point to status checker.
 
     Args:
         inpath (str): Path to Robot Framework XML output file to process.
@@ -104,14 +106,20 @@
     def _get_logs(self, doc):
         return [ExpectedLog(item) for item in doc.split("LOG")[1:]]
 
 
 class ExpectedLog:
     def __init__(self, doc):
         index, message = doc.strip().split(" ", 1)
+        # Prior RF 6.1 when doc had: LOG 1:1    KALA
+        # doc was returned by RF in form LOG 1:1 KALA
+        # By a single space, but with RF 6.2 doc is returned as is.
+        # To keep backwards compatability, left strip message.
+        if RF_61:
+            message = message.lstrip(" ")
         test_setup, kw_index, msg_index, test_teardown = self._split_index(index)
         self.test_setup = test_setup
         self.kw_index = kw_index
         self.msg_index = msg_index
         self.test_teardown = test_teardown
         self.level, self.message = self._split_level(message)
         self.visited_setup = False
```

### Comparing `robotstatuschecker-3.0.0/setup.py` & `robotstatuschecker-3.0.1/setup.py`

 * *Files identical despite different names*

