# Comparing `tmp/innerscope-0.6.0.tar.gz` & `tmp/innerscope-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerscope-0.6.0.tar", last modified: Mon Jun 12 19:55:15 2023, max compression
+gzip compressed data, was "innerscope-0.6.0a0.tar", last modified: Mon Jun 12 17:51:19 2023, max compression
```

## Comparing `innerscope-0.6.0.tar` & `innerscope-0.6.0a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:55:15.723470 innerscope-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-12 19:54:57.000000 innerscope-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-12 19:54:57.000000 innerscope-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-06-12 19:55:15.723470 innerscope-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-12 19:54:57.000000 innerscope-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 19:54:57.000000 innerscope-0.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:55:15.723470 innerscope-0.6.0/innerscope/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-12 19:54:57.000000 innerscope-0.6.0/innerscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 19:54:57.000000 innerscope-0.6.0/innerscope/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    33653 2023-06-12 19:54:57.000000 innerscope-0.6.0/innerscope/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:55:15.723470 innerscope-0.6.0/innerscope/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:54:57.000000 innerscope-0.6.0/innerscope/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-12 19:54:57.000000 innerscope-0.6.0/innerscope/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-06-12 19:54:57.000000 innerscope-0.6.0/innerscope/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-06-12 19:54:57.000000 innerscope-0.6.0/innerscope/tests/test_repr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:55:15.723470 innerscope-0.6.0/innerscope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-06-12 19:55:15.000000 innerscope-0.6.0/innerscope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-12 19:55:15.000000 innerscope-0.6.0/innerscope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:55:15.000000 innerscope-0.6.0/innerscope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 19:55:15.000000 innerscope-0.6.0/innerscope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 19:55:15.000000 innerscope-0.6.0/innerscope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-12 19:54:57.000000 innerscope-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:55:15.723470 innerscope-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 19:54:57.000000 innerscope-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:19.518545 innerscope-0.6.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-12 17:51:19.518545 innerscope-0.6.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:19.514544 innerscope-0.6.0a0/innerscope/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33653 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:19.518545 innerscope-0.6.0a0/innerscope/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/innerscope/tests/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:19.514544 innerscope-0.6.0a0/innerscope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 17:51:19.000000 innerscope-0.6.0a0/innerscope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:51:19.518545 innerscope-0.6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 17:50:59.000000 innerscope-0.6.0a0/setup.py
```

### Comparing `innerscope-0.6.0/LICENSE` & `innerscope-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `innerscope-0.6.0/PKG-INFO` & `innerscope-0.6.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: innerscope
-Version: 0.6.0
+Version: 0.6.0a0
 Summary: Expose the inner scope of functions
 Author: Innerscope contributors
 Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>
 License: Copyright (c) 2020 Erik Welch
         
         All rights reserved.
```

### Comparing `innerscope-0.6.0/README.md` & `innerscope-0.6.0a0/README.md`

 * *Files identical despite different names*

### Comparing `innerscope-0.6.0/innerscope/__init__.py` & `innerscope-0.6.0a0/innerscope/__init__.py`

 * *Files identical despite different names*

### Comparing `innerscope-0.6.0/innerscope/core.py` & `innerscope-0.6.0a0/innerscope/core.py`

 * *Files identical despite different names*

### Comparing `innerscope-0.6.0/innerscope/tests/conftest.py` & `innerscope-0.6.0a0/innerscope/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `innerscope-0.6.0/innerscope/tests/test_core.py` & `innerscope-0.6.0a0/innerscope/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `innerscope-0.6.0/innerscope/tests/test_repr.py` & `innerscope-0.6.0a0/innerscope/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `innerscope-0.6.0/innerscope.egg-info/PKG-INFO` & `innerscope-0.6.0a0/innerscope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: innerscope
-Version: 0.6.0
+Version: 0.6.0a0
 Summary: Expose the inner scope of functions
 Author: Innerscope contributors
 Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>
 License: Copyright (c) 2020 Erik Welch
         
         All rights reserved.
```

### Comparing `innerscope-0.6.0/pyproject.toml` & `innerscope-0.6.0a0/pyproject.toml`

 * *Files identical despite different names*

