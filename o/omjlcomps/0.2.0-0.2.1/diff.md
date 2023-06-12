# Comparing `tmp/omjlcomps-0.2.0.tar.gz` & `tmp/omjlcomps-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omjlcomps-0.2.0.tar", last modified: Wed May 24 02:33:16 2023, max compression
+gzip compressed data, was "omjlcomps-0.2.1.tar", last modified: Mon Jun 12 12:41:27 2023, max compression
```

## Comparing `omjlcomps-0.2.0.tar` & `omjlcomps-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-05-24 02:33:16.290444 omjlcomps-0.2.0/
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      106 2023-01-19 11:27:29.000000 omjlcomps-0.2.0/MANIFEST.in
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      168 2023-05-24 02:33:16.290444 omjlcomps-0.2.0/PKG-INFO
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)       38 2023-01-19 11:27:29.000000 omjlcomps-0.2.0/README.md
-drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-05-24 02:33:16.285444 omjlcomps-0.2.0/omjlcomps/
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)    12319 2023-05-20 11:38:03.000000 omjlcomps-0.2.0/omjlcomps/__init__.py
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      300 2023-05-24 01:37:31.000000 omjlcomps-0.2.0/omjlcomps/juliapkg.json
-drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-05-24 02:33:16.289444 omjlcomps-0.2.0/omjlcomps/test/
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)        0 2023-01-19 11:27:29.000000 omjlcomps-0.2.0/omjlcomps/test/__init__.py
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)     8146 2023-03-17 19:37:43.000000 omjlcomps-0.2.0/omjlcomps/test/test_ecomp.jl
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)    15739 2023-03-17 19:37:43.000000 omjlcomps-0.2.0/omjlcomps/test/test_icomp.jl
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)    15620 2023-03-17 19:37:43.000000 omjlcomps-0.2.0/omjlcomps/test/test_julia_explicit_comp.py
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)    23809 2023-03-17 13:52:15.000000 omjlcomps-0.2.0/omjlcomps/test/test_julia_implicit_comp.py
-drwxr-xr-x   0 dingraha  (1002) dingraha  (1002)        0 2023-05-24 02:33:16.287444 omjlcomps-0.2.0/omjlcomps.egg-info/
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      168 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/PKG-INFO
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      447 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/SOURCES.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)        1 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/dependency_links.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      117 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/entry_points.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)       36 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/requires.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)       10 2023-05-24 02:33:16.000000 omjlcomps-0.2.0/omjlcomps.egg-info/top_level.txt
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)       38 2023-05-24 02:33:16.290444 omjlcomps-0.2.0/setup.cfg
--rw-r--r--   0 dingraha  (1002) dingraha  (1002)      593 2023-05-24 01:43:58.000000 omjlcomps-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:41:27.215833 omjlcomps-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-12 12:41:27.215833 omjlcomps-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:41:27.211833 omjlcomps-0.2.1/omjlcomps/
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/juliapkg.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:41:27.215833 omjlcomps-0.2.1/omjlcomps/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/test_ecomp.jl
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/test_icomp.jl
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/test_julia_explicit_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/test_julia_implicit_comp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:41:27.211833 omjlcomps-0.2.1/omjlcomps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:41:27.215833 omjlcomps-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/setup.py
```

### Comparing `omjlcomps-0.2.0/omjlcomps/__init__.py` & `omjlcomps-0.2.1/omjlcomps/__init__.py`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.0/omjlcomps/test/test_ecomp.jl` & `omjlcomps-0.2.1/omjlcomps/test/test_ecomp.jl`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.0/omjlcomps/test/test_icomp.jl` & `omjlcomps-0.2.1/omjlcomps/test/test_icomp.jl`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.0/omjlcomps/test/test_julia_explicit_comp.py` & `omjlcomps-0.2.1/omjlcomps/test/test_julia_explicit_comp.py`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.0/omjlcomps/test/test_julia_implicit_comp.py` & `omjlcomps-0.2.1/omjlcomps/test/test_julia_implicit_comp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 Unit tests for JuliaImplicitComp
 """
+import juliacall; jl = juliacall.newmodule("OpenMDAOJuliaImplicitCompTest")
 import os
 import time
 import unittest
 
 import numpy as np
 
 import openmdao.api as om
 from openmdao.utils.assert_utils import assert_near_equal
 
-# from juliacall import Main as jl
-import juliacall; jl = juliacall.newmodule("OpenMDAOJuliaImplicitCompTest")
-
 from omjlcomps import JuliaImplicitComp
 
 d = os.path.dirname(os.path.abspath(__file__))
 jl.include(os.path.join(d, "test_icomp.jl"))
 
 
 class TestSimpleJuliaImplicitComp(unittest.TestCase):
```

