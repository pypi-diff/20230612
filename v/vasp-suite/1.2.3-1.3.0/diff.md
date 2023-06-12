# Comparing `tmp/vasp_suite-1.2.3.tar.gz` & `tmp/vasp_suite-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.2.3.tar", last modified: Mon Jun 12 18:39:31 2023, max compression
+gzip compressed data, was "vasp_suite-1.3.0.tar", last modified: Mon Jun 12 20:29:36 2023, max compression
```

## Comparing `vasp_suite-1.2.3.tar` & `vasp_suite-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:39:31.193776 vasp_suite-1.2.3/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 18:39:31.193776 vasp_suite-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 18:39:31.193776 vasp_suite-1.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-06-12 18:39:28.000000 vasp_suite-1.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:39:31.192776 vasp_suite-1.2.3/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-12 18:39:28.000000 vasp_suite-1.2.3/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    16153 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5158 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/vasp_suite/core.py
--rwxrwxrwx   0 root         (0) root         (0)    19084 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     3714 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)    20919 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-12 18:39:07.000000 vasp_suite-1.2.3/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:39:31.193776 vasp_suite-1.2.3/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 18:39:31.000000 vasp_suite-1.2.3/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-12 18:39:31.000000 vasp_suite-1.2.3/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 18:39:31.000000 vasp_suite-1.2.3/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-12 18:39:31.000000 vasp_suite-1.2.3/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-12 18:39:31.000000 vasp_suite-1.2.3/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 18:39:31.000000 vasp_suite-1.2.3/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 20:29:36.671545 vasp_suite-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 20:29:36.671545 vasp_suite-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 20:29:36.671545 vasp_suite-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-06-12 20:29:34.000000 vasp_suite-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 20:29:36.669545 vasp_suite-1.3.0/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-12 20:29:34.000000 vasp_suite-1.3.0/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16153 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/vasp_suite/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    19084 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     3714 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)    20919 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-12 20:29:03.000000 vasp_suite-1.3.0/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 20:29:36.670545 vasp_suite-1.3.0/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-06-12 20:29:36.000000 vasp_suite-1.3.0/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-12 20:29:36.000000 vasp_suite-1.3.0/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 20:29:36.000000 vasp_suite-1.3.0/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-12 20:29:36.000000 vasp_suite-1.3.0/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-12 20:29:36.000000 vasp_suite-1.3.0/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 20:29:36.000000 vasp_suite-1.3.0/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.2.3/LICENSE` & `vasp_suite-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.3/PKG-INFO` & `vasp_suite-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.2.3
+Version: 1.3.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.2.3/README.md` & `vasp_suite-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.3/setup.py` & `vasp_suite-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.2.3"
+__version__ = "1.3.0"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.2.3/vasp_suite/cli.py` & `vasp_suite-1.3.0/vasp_suite/cli.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.3/vasp_suite/core.py` & `vasp_suite-1.3.0/vasp_suite/core.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.3/vasp_suite/ewald.py` & `vasp_suite-1.3.0/vasp_suite/ewald.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.3/vasp_suite/input.py` & `vasp_suite-1.3.0/vasp_suite/input.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.3/vasp_suite/structure.py` & `vasp_suite-1.3.0/vasp_suite/structure.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.3/vasp_suite/submission.py` & `vasp_suite-1.3.0/vasp_suite/submission.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.2.3/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.3.0/vasp_suite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.2.3
+Version: 1.3.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

