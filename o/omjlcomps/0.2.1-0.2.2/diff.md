# Comparing `tmp/omjlcomps-0.2.1.tar.gz` & `tmp/omjlcomps-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omjlcomps-0.2.1.tar", last modified: Mon Jun 12 12:41:27 2023, max compression
+gzip compressed data, was "omjlcomps-0.2.2.tar", last modified: Mon Jun 12 12:56:43 2023, max compression
```

## Comparing `omjlcomps-0.2.1.tar` & `omjlcomps-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:41:27.215833 omjlcomps-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-12 12:41:27.215833 omjlcomps-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:41:27.211833 omjlcomps-0.2.1/omjlcomps/
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/juliapkg.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:41:27.215833 omjlcomps-0.2.1/omjlcomps/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/test_ecomp.jl
--rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/test_icomp.jl
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/test_julia_explicit_comp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/omjlcomps/test/test_julia_implicit_comp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:41:27.211833 omjlcomps-0.2.1/omjlcomps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 12:41:27.000000 omjlcomps-0.2.1/omjlcomps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:41:27.215833 omjlcomps-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-12 12:40:55.000000 omjlcomps-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:43.583619 omjlcomps-0.2.2/omjlcomps/
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/juliapkg.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/omjlcomps/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/test_ecomp.jl
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/test_icomp.jl
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/test_julia_explicit_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/omjlcomps/test/test_julia_implicit_comp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/omjlcomps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 12:56:43.000000 omjlcomps-0.2.2/omjlcomps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:56:43.587619 omjlcomps-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 12:56:14.000000 omjlcomps-0.2.2/setup.py
```

### Comparing `omjlcomps-0.2.1/LICENSE` & `omjlcomps-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.1/PKG-INFO` & `omjlcomps-0.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: omjlcomps
-Version: 0.2.1
-Summary: Create OpenMDAO Components using the Julia programming language
-License: MIT
-Keywords: openmdao_component
-License-File: LICENSE
-
 # omjlcomps: OpenMDAO Julia Components
 
 `omjlcomps` is a small Python package (actually, a [OpenMDAO Plugin](https://openmdao.org/newdocs/versions/latest/features/experimental/plugins.html)) that defines two classes, `JuliaExplicitComp` and `JuliaImplicitComp`, which inherit from OpenMDAO's `ExplicitComponent` and `ImplicitComponent`, respectively.
 These components work with a Julia package called [OpenMDAOCore.jl](https://github.com/byuflowlab/OpenMDAO.jl) to create OpenMDAO `Components` that call Julia code.
 Specifically, `JuliaExplicitComp` and `JuliaImplicitComp` take instances of concrete subtypes of `OpenMDAOCore.ExplicitComponent` and `OpenMDAOCore.ImplicitComponent` and turn them into instances of `JuliaExplicitComp` and `JuliaImplicitComp`.
 Like any other OpenMDAO `ExplicitComponent` or `ImplicitComponent` objects, `JuliaExplicitComp` and `JuliaImplicitComp` instances can be used in an OpenMDAO model, but call Julia code in their methods (`compute`, `apply_nonlinear`, etc.).
 See the [OpenMDAO.jl docs](http://flow.byu.edu/OpenMDAO.jl/dev/) for more information and examples.
```

### Comparing `omjlcomps-0.2.1/omjlcomps/__init__.py` & `omjlcomps-0.2.2/omjlcomps/__init__.py`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.1/omjlcomps/test/test_ecomp.jl` & `omjlcomps-0.2.2/omjlcomps/test/test_ecomp.jl`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.1/omjlcomps/test/test_icomp.jl` & `omjlcomps-0.2.2/omjlcomps/test/test_icomp.jl`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.1/omjlcomps/test/test_julia_explicit_comp.py` & `omjlcomps-0.2.2/omjlcomps/test/test_julia_explicit_comp.py`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.1/omjlcomps/test/test_julia_implicit_comp.py` & `omjlcomps-0.2.2/omjlcomps/test/test_julia_implicit_comp.py`

 * *Files identical despite different names*

### Comparing `omjlcomps-0.2.1/omjlcomps.egg-info/PKG-INFO` & `omjlcomps-0.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: omjlcomps
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create OpenMDAO Components using the Julia programming language
 License: MIT
 Keywords: openmdao_component
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # omjlcomps: OpenMDAO Julia Components
 
 `omjlcomps` is a small Python package (actually, a [OpenMDAO Plugin](https://openmdao.org/newdocs/versions/latest/features/experimental/plugins.html)) that defines two classes, `JuliaExplicitComp` and `JuliaImplicitComp`, which inherit from OpenMDAO's `ExplicitComponent` and `ImplicitComponent`, respectively.
 These components work with a Julia package called [OpenMDAOCore.jl](https://github.com/byuflowlab/OpenMDAO.jl) to create OpenMDAO `Components` that call Julia code.
 Specifically, `JuliaExplicitComp` and `JuliaImplicitComp` take instances of concrete subtypes of `OpenMDAOCore.ExplicitComponent` and `OpenMDAOCore.ImplicitComponent` and turn them into instances of `JuliaExplicitComp` and `JuliaImplicitComp`.
```

### Comparing `omjlcomps-0.2.1/setup.py` & `omjlcomps-0.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 with open(Path(__file__).parent / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup_args = {
    'description': 'Create OpenMDAO Components using the Julia programming language',
    'long_description': long_description,
+   'long_description_content_type': 'text/markdown',
    'entry_points': {
        'openmdao_component': [
            'juliaexplicitcomp=omjlcomps:JuliaExplicitComp',
            'juliaimplicitcomp=omjlcomps:JuliaImplicitComp'
        ]
     },
    'install_requires': ['openmdao~=3.26.0', 'juliapkg~=0.1.10', 'juliacall~=0.9.13'],
    'keywords': ['openmdao_component'],
    'license': 'MIT',
    'name': 'omjlcomps',
    'packages': ['omjlcomps', 'omjlcomps.test'],
-   'version': '0.2.1',
+   'version': '0.2.2',
    'include_package_data': True}
 
 setup(**setup_args)
```

