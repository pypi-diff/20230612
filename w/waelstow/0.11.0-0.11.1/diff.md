# Comparing `tmp/waelstow-0.11.0.tar.gz` & `tmp/waelstow-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waelstow-0.11.0.tar", last modified: Fri Jan  6 17:38:21 2023, max compression
+gzip compressed data, was "waelstow-0.11.1.tar", last modified: Mon Jun 12 20:28:09 2023, max compression
```

## Comparing `waelstow-0.11.0.tar` & `waelstow-0.11.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-01-06 17:38:21.769730 waelstow-0.11.0/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1089 2020-02-20 16:56:39.000000 waelstow-0.11.0/LICENSE
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1491 2023-01-06 17:38:21.769284 waelstow-0.11.0/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      449 2023-01-06 16:57:08.000000 waelstow-0.11.0/README.rst
--rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2023-01-06 17:38:21.769860 waelstow-0.11.0/setup.cfg
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1797 2023-01-06 16:32:54.000000 waelstow-0.11.0/setup.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-01-06 17:38:21.768796 waelstow-0.11.0/waelstow.egg-info/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1491 2023-01-06 17:38:21.000000 waelstow-0.11.0/waelstow.egg-info/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      167 2023-01-06 17:38:21.000000 waelstow-0.11.0/waelstow.egg-info/SOURCES.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-01-06 17:38:21.000000 waelstow-0.11.0/waelstow.egg-info/dependency_links.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        9 2023-01-06 17:38:21.000000 waelstow-0.11.0/waelstow.egg-info/top_level.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)     9055 2023-01-06 17:36:37.000000 waelstow-0.11.0/waelstow.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-12 20:28:09.569873 waelstow-0.11.1/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1089 2020-02-20 16:56:39.000000 waelstow-0.11.1/LICENSE
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1491 2023-06-12 20:28:09.569556 waelstow-0.11.1/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      449 2023-01-06 16:57:08.000000 waelstow-0.11.1/README.rst
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       38 2023-06-12 20:28:09.569943 waelstow-0.11.1/setup.cfg
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1797 2023-01-06 16:32:54.000000 waelstow-0.11.1/setup.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-06-12 20:28:09.569088 waelstow-0.11.1/waelstow.egg-info/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1491 2023-06-12 20:28:09.000000 waelstow-0.11.1/waelstow.egg-info/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      167 2023-06-12 20:28:09.000000 waelstow-0.11.1/waelstow.egg-info/SOURCES.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-06-12 20:28:09.000000 waelstow-0.11.1/waelstow.egg-info/dependency_links.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        9 2023-06-12 20:28:09.000000 waelstow-0.11.1/waelstow.egg-info/top_level.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     9388 2023-06-12 20:27:34.000000 waelstow-0.11.1/waelstow.py
```

### Comparing `waelstow-0.11.0/LICENSE` & `waelstow-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `waelstow-0.11.0/PKG-INFO` & `waelstow-0.11.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waelstow
-Version: 0.11.0
+Version: 0.11.1
 Summary: A small collection of tools for unit testing.  Includes methods for test suite discovery for use in your runner and contexts for capturing STDIO or STDERR and temporarily moving directories.
 Home-page: https://github.com/cltrudeau/waelstow
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
 Keywords: test,testing,unit test,unittest,test runner
 Classifier: Development Status :: 4 - Beta
```

### Comparing `waelstow-0.11.0/setup.py` & `waelstow-0.11.1/setup.py`

 * *Files identical despite different names*

### Comparing `waelstow-0.11.0/waelstow.egg-info/PKG-INFO` & `waelstow-0.11.1/waelstow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waelstow
-Version: 0.11.0
+Version: 0.11.1
 Summary: A small collection of tools for unit testing.  Includes methods for test suite discovery for use in your runner and contexts for capturing STDIO or STDERR and temporarily moving directories.
 Home-page: https://github.com/cltrudeau/waelstow
 Author: Christopher Trudeau
 Author-email: ctrudeau+pypi@arsensa.com
 License: MIT
 Keywords: test,testing,unit test,unittest,test runner
 Classifier: Development Status :: 4 - Beta
```

### Comparing `waelstow-0.11.0/waelstow.py` & `waelstow-0.11.1/waelstow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # waelstow.py
-__version__ = '0.11.0'
+__version__ = '0.11.1'
 
 import contextlib, os, shutil, sys, tempfile, json
 from io import StringIO
 from unittest import TestCase, TestSuite, TestLoader
+from unittest.loader import _FailedTest
 
 # =============================================================================
 # Test Suite Discovery & Management
 # =============================================================================
 
 def list_tests(suites):
     """Takes a list of suites and returns an iterable of all the tests in
@@ -57,21 +58,27 @@
 
     :param suites:
         A single or iterable of :class:`TestSuite` objects to create the test
         subset from
     :param shortcut_labels:
         A list of short-cut labels to use to cull the list
     :returns:
-        A list of :class:`TestCase` objects 
+        A list of :class:`TestCase` objects
     """
     # strip the '=' from the front of each label
     labels = [label[1:] for label in shortcut_labels]
 
     results = []
     for test in list_tests(suites):
+        if isinstance(test, _FailedTest):
+            # If a test fails to load there is something wrong with the code
+            # it imports, put it in the suite so the runner shows the
+            # appropriate exception even if it doesn't match the label
+            results.append(test)
+
         name = '%s.%s.%s' % (test.__module__, test.__class__.__name__,
             test._testMethodName)
         for label in labels:
             if label in name:
                 results.append(test)
 
     return results
```

