# Comparing `tmp/omjlcomps-0.2.2.tar.gz` & `tmp/omjlcomps-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omjlcomps-0.2.2.tar", last modified: Mon Jun 12 12:56:43 2023, max compression
+gzip compressed data, was "omjlcomps-0.2.3.tar", last modified: Mon Jun 12 16:37:34 2023, max compression
```

## Comparing `omjlcomps-0.2.2.tar` & `omjlcomps-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:43.583619 omjlcomps-0.2.2/omjlcomps/
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/juliapkg.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/omjlcomps/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/test_ecomp.jl
--rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/test_icomp.jl
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/test_julia_explicit_comp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/test_julia_implicit_comp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/omjlcomps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:37:34.498352 omjlcomps-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 16:37:34.498352 omjlcomps-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:37:34.494352 omjlcomps-0.2.3/omjlcomps/
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/omjlcomps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/omjlcomps/juliapkg.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:37:34.498352 omjlcomps-0.2.3/omjlcomps/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/omjlcomps/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/omjlcomps/test/test_ecomp.jl
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/omjlcomps/test/test_icomp.jl
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/omjlcomps/test/test_julia_explicit_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/omjlcomps/test/test_julia_implicit_comp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:37:34.498352 omjlcomps-0.2.3/omjlcomps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 16:37:34.000000 omjlcomps-0.2.3/omjlcomps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-12 16:37:34.000000 omjlcomps-0.2.3/omjlcomps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:37:34.000000 omjlcomps-0.2.3/omjlcomps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 16:37:34.000000 omjlcomps-0.2.3/omjlcomps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 16:37:34.000000 omjlcomps-0.2.3/omjlcomps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 16:37:34.000000 omjlcomps-0.2.3/omjlcomps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:37:34.498352 omjlcomps-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 16:36:47.000000 omjlcomps-0.2.3/setup.py
```

### Comparing `omjlcomps-0.2.2/LICENSE` & `omjlcomps-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.2/PKG-INFO` & `omjlcomps-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omjlcomps
-Version: 0.2.2
+Version: 0.2.3
 Summary: Create OpenMDAO Components using the Julia programming language
 License: MIT
 Keywords: openmdao_component
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # omjlcomps: OpenMDAO Julia Components
```

### Comparing `omjlcomps-0.2.2/README.md` & `omjlcomps-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.2/omjlcomps/__init__.py` & `omjlcomps-0.2.3/omjlcomps/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import juliacall; jl = juliacall.newmodule("OpenMDAOJuliaComps")
 from types import MethodType
 
 import openmdao.api as om
 from openmdao.core.analysis_error import AnalysisError
 
-import juliacall; jl = juliacall.newmodule("OpenMDAOJuliaComps")
 from juliacall import JuliaError
 # This imports the Julia package OpenMDAOCore:
 jl.seval("using OpenMDAOCore: OpenMDAOCore")
 
 
 def _initialize_common(self):
     self.options.declare('jlcomp', recordable=False)
```

### Comparing `omjlcomps-0.2.2/omjlcomps/test/test_ecomp.jl` & `omjlcomps-0.2.3/omjlcomps/test/test_ecomp.jl`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.2/omjlcomps/test/test_icomp.jl` & `omjlcomps-0.2.3/omjlcomps/test/test_icomp.jl`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.2/omjlcomps/test/test_julia_explicit_comp.py` & `omjlcomps-0.2.3/omjlcomps/test/test_julia_explicit_comp.py`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.2/omjlcomps/test/test_julia_implicit_comp.py` & `omjlcomps-0.2.3/omjlcomps/test/test_julia_implicit_comp.py`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.2/omjlcomps.egg-info/PKG-INFO` & `omjlcomps-0.2.3/omjlcomps.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omjlcomps
-Version: 0.2.2
+Version: 0.2.3
 Summary: Create OpenMDAO Components using the Julia programming language
 License: MIT
 Keywords: openmdao_component
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # omjlcomps: OpenMDAO Julia Components
```

### Comparing `omjlcomps-0.2.2/setup.py` & `omjlcomps-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,11 +17,11 @@
        ]
     },
    'install_requires': ['openmdao~=3.26.0', 'juliapkg~=0.1.10', 'juliacall~=0.9.13'],
    'keywords': ['openmdao_component'],
    'license': 'MIT',
    'name': 'omjlcomps',
    'packages': ['omjlcomps', 'omjlcomps.test'],
-   'version': '0.2.2',
+   'version': '0.2.3',
    'include_package_data': True}
 
 setup(**setup_args)
```

