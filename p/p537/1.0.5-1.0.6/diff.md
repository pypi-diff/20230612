# Comparing `tmp/p537-1.0.5.tar.gz` & `tmp/p537-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p537-1.0.5.tar", last modified: Sun Sep 18 20:58:05 2022, max compression
+gzip compressed data, was "p537-1.0.6.tar", last modified: Mon Jun 12 19:19:19 2023, max compression
```

## Comparing `p537-1.0.5.tar` & `p537-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 20:58:05.575457 p537-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-18 20:57:48.000000 p537-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-09-18 20:58:05.575457 p537-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-18 20:57:48.000000 p537-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 20:58:05.575457 p537-1.0.5/p537.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-09-18 20:58:05.000000 p537-1.0.5/p537.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-18 20:58:05.000000 p537-1.0.5/p537.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 20:58:05.000000 p537-1.0.5/p537.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-18 20:58:05.000000 p537-1.0.5/p537.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-18 20:58:05.000000 p537-1.0.5/p537.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-09-18 20:57:48.000000 p537-1.0.5/p537module.c
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-18 20:58:05.575457 p537-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-09-18 20:57:48.000000 p537-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:19:19.394184 p537-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 19:19:03.000000 p537-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-12 19:19:19.394184 p537-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-12 19:19:03.000000 p537-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:19:19.394184 p537-1.0.6/p537.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-12 19:19:19.000000 p537-1.0.6/p537.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-12 19:19:19.000000 p537-1.0.6/p537.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:19:19.000000 p537-1.0.6/p537.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 19:19:19.000000 p537-1.0.6/p537.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 19:19:19.000000 p537-1.0.6/p537.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-12 19:19:03.000000 p537-1.0.6/p537module.c
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 19:19:03.000000 p537-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:19:19.394184 p537-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-12 19:19:03.000000 p537-1.0.6/setup.py
```

### Comparing `p537-1.0.5/LICENSE` & `p537-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `p537-1.0.5/PKG-INFO` & `p537-1.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p537
-Version: 1.0.5
+Version: 1.0.6
 Summary: A tiny platform-specific distribution with a console script.
 Home-page: https://github.com/jsirois/p537
 Author: John Sirois
 Author-email: john.sirois@gmail.com
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,19 +13,21 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6,<3.13
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-.. image:: https://travis-ci.org/jsirois/p537.svg?branch=master
-    :target: https://travis-ci.org/jsirois/p537
+.. image:: https://github.com/jsirois/p537/workflows/CI/badge.svg?branch=master
+    :target: https://github.com/jsirois/p537/actions?query=branch%3Amaster+workflow%3ACI
 .. image:: https://img.shields.io/pypi/l/p537.svg
     :target: https://pypi.org/project/p537/
 .. image:: https://img.shields.io/pypi/v/p537.svg
     :target: https://pypi.org/project/p537/
 .. image:: https://img.shields.io/pypi/pyversions/p537.svg
     :target: https://pypi.org/project/p537/
 .. image:: https://img.shields.io/pypi/wheel/p537.svg
```

### Comparing `p537-1.0.5/README.rst` & `p537-1.0.6/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.. image:: https://travis-ci.org/jsirois/p537.svg?branch=master
-    :target: https://travis-ci.org/jsirois/p537
+.. image:: https://github.com/jsirois/p537/workflows/CI/badge.svg?branch=master
+    :target: https://github.com/jsirois/p537/actions?query=branch%3Amaster+workflow%3ACI
 .. image:: https://img.shields.io/pypi/l/p537.svg
     :target: https://pypi.org/project/p537/
 .. image:: https://img.shields.io/pypi/v/p537.svg
     :target: https://pypi.org/project/p537/
 .. image:: https://img.shields.io/pypi/pyversions/p537.svg
     :target: https://pypi.org/project/p537/
 .. image:: https://img.shields.io/pypi/wheel/p537.svg
```

### Comparing `p537-1.0.5/p537.egg-info/PKG-INFO` & `p537-1.0.6/p537.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p537
-Version: 1.0.5
+Version: 1.0.6
 Summary: A tiny platform-specific distribution with a console script.
 Home-page: https://github.com/jsirois/p537
 Author: John Sirois
 Author-email: john.sirois@gmail.com
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,19 +13,21 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6,<3.13
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-.. image:: https://travis-ci.org/jsirois/p537.svg?branch=master
-    :target: https://travis-ci.org/jsirois/p537
+.. image:: https://github.com/jsirois/p537/workflows/CI/badge.svg?branch=master
+    :target: https://github.com/jsirois/p537/actions?query=branch%3Amaster+workflow%3ACI
 .. image:: https://img.shields.io/pypi/l/p537.svg
     :target: https://pypi.org/project/p537/
 .. image:: https://img.shields.io/pypi/v/p537.svg
     :target: https://pypi.org/project/p537/
 .. image:: https://img.shields.io/pypi/pyversions/p537.svg
     :target: https://pypi.org/project/p537/
 .. image:: https://img.shields.io/pypi/wheel/p537.svg
```

### Comparing `p537-1.0.5/p537module.c` & `p537-1.0.6/p537module.c`

 * *Files identical despite different names*

### Comparing `p537-1.0.5/setup.py` & `p537-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def long_description():
   with open('README.rst') as fp:
     return fp.read()
 
 
 setup(
   name='p537',
-  version='1.0.5',
+  version='1.0.6',
   author="John Sirois",
   author_email="john.sirois@gmail.com",
   description='A tiny platform-specific distribution with a console script.',
   long_description=long_description(),
   long_description_content_type="text/x-rst",
   url='https://github.com/jsirois/p537',
   license='Apache License, Version 2.0',
@@ -24,15 +24,17 @@
     'Operating System :: Microsoft :: Windows',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
   ],
+  python_requires=">=3.6,<3.13",
   ext_modules=[
     Extension('p537', sources=['p537module.c']),
   ],
   entry_points={
     'console_scripts': [
       'p537 = p537:greet',
     ],
```

