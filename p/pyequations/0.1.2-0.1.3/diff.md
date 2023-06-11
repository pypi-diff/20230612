# Comparing `tmp/pyequations-0.1.2.tar.gz` & `tmp/pyequations-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyequations-0.1.2.tar", max compression
+gzip compressed data, was "pyequations-0.1.3.tar", max compression
```

## Comparing `pyequations-0.1.2.tar` & `pyequations-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-05-29 01:58:26.642083 pyequations-0.1.2/LICENSE
--rw-r--r--   0        0        0    12419 2023-06-11 22:14:30.784358 pyequations-0.1.2/README.md
--rw-r--r--   0        0        0      426 2023-06-11 22:13:40.401945 pyequations-0.1.2/pyequations/__init__.py
--rw-r--r--   0        0        0     6303 2023-06-10 18:08:24.869111 pyequations-0.1.2/pyequations/context_stack.py
--rw-r--r--   0        0        0      471 2023-05-31 00:06:36.282730 pyequations-0.1.2/pyequations/decorators.py
--rw-r--r--   0        0        0     9349 2023-06-10 18:08:24.869275 pyequations-0.1.2/pyequations/generate_units_subs.py
--rw-r--r--   0        0        0    24128 2023-06-10 20:37:48.132386 pyequations-0.1.2/pyequations/inheritables.py
--rw-r--r--   0        0        0     9294 2023-06-10 18:08:24.869792 pyequations-0.1.2/pyequations/utils.py
--rw-r--r--   0        0        0      460 2023-06-11 22:13:40.399078 pyequations-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 pyequations-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 01:58:26.642083 pyequations-0.1.3/LICENSE
+-rw-r--r--   0        0        0    12419 2023-06-11 22:14:30.784358 pyequations-0.1.3/README.md
+-rw-r--r--   0        0        0      426 2023-06-11 22:26:08.185092 pyequations-0.1.3/pyequations/__init__.py
+-rw-r--r--   0        0        0     6303 2023-06-10 18:08:24.869111 pyequations-0.1.3/pyequations/context_stack.py
+-rw-r--r--   0        0        0      471 2023-05-31 00:06:36.282730 pyequations-0.1.3/pyequations/decorators.py
+-rw-r--r--   0        0        0     9349 2023-06-10 18:08:24.869275 pyequations-0.1.3/pyequations/generate_units_subs.py
+-rw-r--r--   0        0        0    24128 2023-06-10 20:37:48.132386 pyequations-0.1.3/pyequations/inheritables.py
+-rw-r--r--   0        0        0     9294 2023-06-10 18:08:24.869792 pyequations-0.1.3/pyequations/utils.py
+-rw-r--r--   0        0        0      538 2023-06-11 22:26:08.181772 pyequations-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    13011 1970-01-01 00:00:00.000000 pyequations-0.1.3/PKG-INFO
```

### Comparing `pyequations-0.1.2/LICENSE` & `pyequations-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.2/README.md` & `pyequations-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.2/pyequations/context_stack.py` & `pyequations-0.1.3/pyequations/context_stack.py`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.2/pyequations/generate_units_subs.py` & `pyequations-0.1.3/pyequations/generate_units_subs.py`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.2/pyequations/inheritables.py` & `pyequations-0.1.3/pyequations/inheritables.py`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.2/pyequations/utils.py` & `pyequations-0.1.3/pyequations/utils.py`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.2/PKG-INFO` & `pyequations-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: pyequations
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for solving a bunch of equations with a bunch of unknowns.
+Home-page: https://github.com/mbryant2025/PyEquations
+Keywords: Math
 Author: Michael Bryant
 Author-email: mbryant2025@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sympy (>=1.12,<2.0)
+Project-URL: Repository, https://github.com/mbryant2025/PyEquations
 Description-Content-Type: text/markdown
 
 ![Tests](https://github.com/mbryant2025/PyEquations/actions/workflows/python-package.yml/badge.svg)
 
 # PyEquations
 
 ## Table of Contents
```

