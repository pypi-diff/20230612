# Comparing `tmp/argbind-0.3.6.tar.gz` & `tmp/argbind-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/argbind-0.3.6.tar", last modified: Fri Sep  9 06:36:29 2022, max compression
+gzip compressed data, was "dist/argbind-0.3.7.tar", last modified: Mon Jun 12 17:49:59 2023, max compression
```

## Comparing `argbind-0.3.6.tar` & `argbind-0.3.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 prem       (501) staff       (20)        0 2022-09-09 06:36:29.054943 argbind-0.3.6/
--rw-r--r--   0 prem       (501) staff       (20)     1073 2020-10-13 23:57:31.000000 argbind-0.3.6/LICENSE.md
--rw-r--r--   0 prem       (501) staff       (20)    14775 2022-09-09 06:36:29.055086 argbind-0.3.6/PKG-INFO
--rw-r--r--   0 prem       (501) staff       (20)    11452 2022-03-22 16:26:55.000000 argbind-0.3.6/README.md
-drwxr-xr-x   0 prem       (501) staff       (20)        0 2022-09-09 06:36:29.054250 argbind-0.3.6/argbind/
--rw-r--r--   0 prem       (501) staff       (20)      189 2022-09-09 06:07:00.000000 argbind-0.3.6/argbind/__init__.py
--rw-r--r--   0 prem       (501) staff       (20)    16787 2022-09-09 06:36:12.000000 argbind-0.3.6/argbind/argbind.py
-drwxr-xr-x   0 prem       (501) staff       (20)        0 2022-09-09 06:36:29.054845 argbind-0.3.6/argbind.egg-info/
--rw-r--r--   0 prem       (501) staff       (20)    14775 2022-09-09 06:36:28.000000 argbind-0.3.6/argbind.egg-info/PKG-INFO
--rw-r--r--   0 prem       (501) staff       (20)      232 2022-09-09 06:36:28.000000 argbind-0.3.6/argbind.egg-info/SOURCES.txt
--rw-r--r--   0 prem       (501) staff       (20)        1 2022-09-09 06:36:28.000000 argbind-0.3.6/argbind.egg-info/dependency_links.txt
--rw-r--r--   0 prem       (501) staff       (20)       99 2022-09-09 06:36:28.000000 argbind-0.3.6/argbind.egg-info/requires.txt
--rw-r--r--   0 prem       (501) staff       (20)        8 2022-09-09 06:36:28.000000 argbind-0.3.6/argbind.egg-info/top_level.txt
--rw-r--r--   0 prem       (501) staff       (20)      245 2022-09-09 06:36:29.055375 argbind-0.3.6/setup.cfg
--rw-r--r--   0 prem       (501) staff       (20)     1518 2022-09-09 06:36:12.000000 argbind-0.3.6/setup.py
+drwxr-xr-x   0 prem       (501) staff       (20)        0 2023-06-12 17:49:59.278294 argbind-0.3.7/
+-rw-r--r--   0 prem       (501) staff       (20)     1073 2020-10-13 23:57:31.000000 argbind-0.3.7/LICENSE.md
+-rw-r--r--   0 prem       (501) staff       (20)    14855 2023-06-12 17:49:59.278446 argbind-0.3.7/PKG-INFO
+-rw-r--r--   0 prem       (501) staff       (20)    11524 2023-06-12 17:49:42.000000 argbind-0.3.7/README.md
+drwxr-xr-x   0 prem       (501) staff       (20)        0 2023-06-12 17:49:59.277473 argbind-0.3.7/argbind/
+-rw-r--r--   0 prem       (501) staff       (20)      189 2022-09-09 06:07:00.000000 argbind-0.3.7/argbind/__init__.py
+-rw-r--r--   0 prem       (501) staff       (20)    17169 2023-06-12 17:49:42.000000 argbind-0.3.7/argbind/argbind.py
+drwxr-xr-x   0 prem       (501) staff       (20)        0 2023-06-12 17:49:59.278178 argbind-0.3.7/argbind.egg-info/
+-rw-r--r--   0 prem       (501) staff       (20)    14855 2023-06-12 17:49:59.000000 argbind-0.3.7/argbind.egg-info/PKG-INFO
+-rw-r--r--   0 prem       (501) staff       (20)      232 2023-06-12 17:49:59.000000 argbind-0.3.7/argbind.egg-info/SOURCES.txt
+-rw-r--r--   0 prem       (501) staff       (20)        1 2023-06-12 17:49:59.000000 argbind-0.3.7/argbind.egg-info/dependency_links.txt
+-rw-r--r--   0 prem       (501) staff       (20)       99 2023-06-12 17:49:59.000000 argbind-0.3.7/argbind.egg-info/requires.txt
+-rw-r--r--   0 prem       (501) staff       (20)        8 2023-06-12 17:49:59.000000 argbind-0.3.7/argbind.egg-info/top_level.txt
+-rw-r--r--   0 prem       (501) staff       (20)      245 2023-06-12 17:49:59.278727 argbind-0.3.7/setup.cfg
+-rw-r--r--   0 prem       (501) staff       (20)     1518 2023-06-12 17:49:42.000000 argbind-0.3.7/setup.py
```

### Comparing `argbind-0.3.6/LICENSE.md` & `argbind-0.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `argbind-0.3.6/PKG-INFO` & `argbind-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argbind
-Version: 0.3.6
+Version: 0.3.7
 Summary: Simple way to bind function arguments to the command line.
 Home-page: https://github.com/pseeth/argbind/
 Author: Prem Seetharaman
 Author-email: prem@descript.com
 License: UNKNOWN
 Description: # ArgBind
         
@@ -69,14 +69,15 @@
         - [Example 5: Loading, saving, and using .yml files](./examples/yaml)
         - [Example 6: Multi-stage programs](./examples/multistage)
         - [Example 7: Mimic more traditional CLI, without `func.arg` notation](./examples/without_prefix)
         - [Example 8: Debug mode](./examples/debug)
         - [Example 9: Migrating from ArgParse](./examples/migration)
         - [Example 10: Binding existing functions and classes](./examples/bind_existing)
         - [Example 11: Binding entire modules](./examples/bind_module)
+        - [Example 12: Binding functions to specific groups](./examples/groups)
         
         ## Usage
         
         There are six main functions.
         
         - `bind`: Binds keyword arguments (and positional arguments if `positional=True`) of a function or class to ArgBind.
         - `parse_args`: Actually parses command line arguments into a dictionary.
```

### Comparing `argbind-0.3.6/README.md` & `argbind-0.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 - [Example 5: Loading, saving, and using .yml files](./examples/yaml)
 - [Example 6: Multi-stage programs](./examples/multistage)
 - [Example 7: Mimic more traditional CLI, without `func.arg` notation](./examples/without_prefix)
 - [Example 8: Debug mode](./examples/debug)
 - [Example 9: Migrating from ArgParse](./examples/migration)
 - [Example 10: Binding existing functions and classes](./examples/bind_existing)
 - [Example 11: Binding entire modules](./examples/bind_module)
+- [Example 12: Binding functions to specific groups](./examples/groups)
 
 ## Usage
 
 There are six main functions.
 
 - `bind`: Binds keyword arguments (and positional arguments if `positional=True`) of a function or class to ArgBind.
 - `parse_args`: Actually parses command line arguments into a dictionary.
```

### Comparing `argbind-0.3.6/argbind/argbind.py` & `argbind-0.3.7/argbind/argbind.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 from contextlib import contextmanager
 import argparse
-from typing import List, Dict
+from typing import List, Dict, Union
 import docstring_parser
 import textwrap
 import yaml
 import sys
 import os
 from pathlib import Path
 import ast
@@ -56,15 +56,15 @@
     if scope is not None:
         formatted.append(f"  # scope = {scope}")
     for key, val in func_kwargs.items():
         formatted.append(f"  {key} : {type(val).__name__} = {val}")
     formatted.append(")")
     return '\n'.join(formatted)
 
-def bind(*args, without_prefix=False, positional=False):
+def bind(*args, without_prefix=False, positional=False, group: Union[list, str] = "default"):
     """Binds a functions arguments so that it looks up argument
     values in a dictionary scoped by ArgBind.
 
     Parameters
     ----------
     args : List[str] or [fn or Object] + List[str], optional
         List of patterns to bind the function under. If the first item
@@ -90,14 +90,16 @@
 
     if positional and patterns:
         warnings.warn(
             f"Combining positional arguments with scoping patterns is not allowed. Removing scoping patterns {patterns}. \n"
             "See https://github.com/pseeth/argbind/tree/main/examples/hello_world#argbind-with-positional-arguments")
         patterns = []
 
+    if isinstance(group, str):
+        group = [group]
 
     def decorator(object_or_func):
         func = object_or_func
         is_class = inspect.isclass(func)
         if is_class:
             func = getattr(func, "__init__")            
 
@@ -106,15 +108,15 @@
             prefix = prefix.split(".")[0]
         
         # Check if function is bound already. If it is, just re-wrap it,
         # instead of wrapping the function twice.
         if prefix in PARSE_FUNCS:
             func = PARSE_FUNCS[prefix][0]
         else:
-            PARSE_FUNCS[prefix] = (func, patterns, without_prefix, positional)
+            PARSE_FUNCS[prefix] = (func, patterns, without_prefix, positional, group)
         
         @wraps(func)
         def cmd_func(*args, **kwargs):
             parameters = list(inspect.signature(func).parameters.items())
             
             cmd_kwargs = {}
             pos_kwargs = {parameters[i][0]: arg for i, arg in enumerate(args)}
@@ -311,15 +313,15 @@
             key, val = elem.split('=', 1)
             key = self._guess_type(key)
             val = self._guess_type(val)
             _values[key] = val
 
         return _values
 
-def build_parser():
+def build_parser(group: Union[list, str] = "default"):
     """Builds the argument parser from all of the bound functions.
 
     Returns
     -------
     ArgumentParser
         Argument parser built by ArgBind.
     """
@@ -330,17 +332,24 @@
     p.add_argument('--args.save', type=str, required=False, 
         help="Path to save all arguments used to run script to.")
     p.add_argument('--args.load', type=str, required=False,
         help="Path to load arguments from, stored as a .yml file.")
     p.add_argument('--args.debug', type=int, required=False, default=0, 
         help="Print arguments as they are passed to each function.")
 
+    if isinstance(group, str):
+        group = [group]
+    if "default" not in group:
+        group.append("default")
     # Add kwargs from function to parser
     for prefix in PARSE_FUNCS:
-        func, patterns, without_prefix, positional = PARSE_FUNCS[prefix]
+        func, patterns, without_prefix, positional, fn_group = PARSE_FUNCS[prefix]
+        if not set(fn_group) & set(group):
+            continue
+
         sig = inspect.signature(func)
 
         docstring = docstring_parser.parse(func.__doc__)
         parameter_help = docstring.params
         parameter_help = {
             x.arg_name: x.description for x in parameter_help
         }
@@ -428,20 +437,20 @@
             )
 
         desc = textwrap.fill(desc, width=HELP_WIDTH)
         f.description = desc
     
     return p
 
-def parse_args(p=None):
+def parse_args(p=None, group: Union[list, str] = "default"):
     """
     Parses the command line and returns a dictionary.
     Builds the argument parser if p is None.
     """
-    p = build_parser() if p is None else p
+    p = build_parser(group=group) if p is None else p
     used_args = [x.replace('--', '').split('=')[0] for x in sys.argv if x.startswith('--')]
     used_args.extend(['args.save', 'args.load'])
 
     args = vars(p.parse_args())
     load_args_path = args.pop('args.load')
     save_args_path = args.pop('args.save')
     debug_args = args.pop('args.debug')
```

### Comparing `argbind-0.3.6/argbind.egg-info/PKG-INFO` & `argbind-0.3.7/argbind.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argbind
-Version: 0.3.6
+Version: 0.3.7
 Summary: Simple way to bind function arguments to the command line.
 Home-page: https://github.com/pseeth/argbind/
 Author: Prem Seetharaman
 Author-email: prem@descript.com
 License: UNKNOWN
 Description: # ArgBind
         
@@ -69,14 +69,15 @@
         - [Example 5: Loading, saving, and using .yml files](./examples/yaml)
         - [Example 6: Multi-stage programs](./examples/multistage)
         - [Example 7: Mimic more traditional CLI, without `func.arg` notation](./examples/without_prefix)
         - [Example 8: Debug mode](./examples/debug)
         - [Example 9: Migrating from ArgParse](./examples/migration)
         - [Example 10: Binding existing functions and classes](./examples/bind_existing)
         - [Example 11: Binding entire modules](./examples/bind_module)
+        - [Example 12: Binding functions to specific groups](./examples/groups)
         
         ## Usage
         
         There are six main functions.
         
         - `bind`: Binds keyword arguments (and positional arguments if `positional=True`) of a function or class to ArgBind.
         - `parse_args`: Actually parses command line arguments into a dictionary.
```

### Comparing `argbind-0.3.6/setup.py` & `argbind-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='argbind',
-    version='0.3.6', 
+    version='0.3.7', 
     description='Simple way to bind function arguments to the command line.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pseeth/argbind/',
     author='Prem Seetharaman',
     author_email='prem@descript.com', 
     classifiers=[
```

