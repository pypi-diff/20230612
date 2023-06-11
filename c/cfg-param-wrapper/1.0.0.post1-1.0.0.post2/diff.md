# Comparing `tmp/cfg-param-wrapper-1.0.0.post1.tar.gz` & `tmp/cfg-param-wrapper-1.0.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-param-wrapper-1.0.0.post1.tar", last modified: Sun Jun 11 22:38:01 2023, max compression
+gzip compressed data, was "cfg-param-wrapper-1.0.0.post2.tar", last modified: Sun Jun 11 22:59:07 2023, max compression
```

## Comparing `cfg-param-wrapper-1.0.0.post1.tar` & `cfg-param-wrapper-1.0.0.post2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-param-wrapper-1.0.0.post1/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1585 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      746 2023-06-11 22:36:59.000000 cfg-param-wrapper-1.0.0.post1/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      959 2023-06-11 22:37:48.000000 cfg-param-wrapper-1.0.0.post1/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/argparse_config.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2888 2023-06-11 22:35:08.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/cfg_dict.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2263 2023-06-11 22:35:07.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/function_config_wrapper.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1391 2023-06-07 18:09:29.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/save_handlers.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1585 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      453 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       25 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/requires.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       18 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-param-wrapper-1.0.0.post2/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1587 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      748 2023-06-11 22:58:44.000000 cfg-param-wrapper-1.0.0.post2/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      959 2023-06-11 22:58:36.000000 cfg-param-wrapper-1.0.0.post2/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/argparse_config.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2966 2023-06-11 22:56:57.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/cfg_dict.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2258 2023-06-11 22:57:11.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/function_config_wrapper.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1934 2023-06-11 22:55:59.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/save_handlers.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:59:07.486929 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1587 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      453 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       25 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/requires.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       18 2023-06-11 22:59:07.000000 cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/top_level.txt
```

### Comparing `cfg-param-wrapper-1.0.0.post1/LICENSE` & `cfg-param-wrapper-1.0.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-param-wrapper-1.0.0.post1/PKG-INFO` & `cfg-param-wrapper-1.0.0.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-param-wrapper
-Version: 1.0.0.post1
+Version: 1.0.0.post2
 Summary: A package designed to simplify defaults.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: typer
 License-File: LICENSE
 
-# cfg_param_wrapper 1.0.0
+# cfg_param_wrapper 1.0.0-2
 
 a config wrapper I made. It's made to wrap simple functions, and intercept configurations in tandem with a CfgDict object.
 
 ## Installation
 
 ```bash
 # from pypi:
```

### Comparing `cfg-param-wrapper-1.0.0.post1/README.md` & `cfg-param-wrapper-1.0.0.post2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# cfg_param_wrapper 1.0.0
+# cfg_param_wrapper 1.0.0-2
 
 a config wrapper I made. It's made to wrap simple functions, and intercept configurations in tandem with a CfgDict object.
 
 ## Installation
 
 ```bash
 # from pypi:
```

### Comparing `cfg-param-wrapper-1.0.0.post1/pyproject.toml` & `cfg-param-wrapper-1.0.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfg-param-wrapper"
-version = "1.0.0-1"
+version = "1.0.0-2"
 authors = [{ name = "Zeptofine", email = "zeptofine@gmail.com" }]
 description = "A package designed to simplify defaults."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
```

### Comparing `cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/argparse_config.py` & `cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/argparse_config.py`

 * *Files identical despite different names*

### Comparing `cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/cfg_dict.py` & `cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/cfg_dict.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """A dictionary subclass used for fast dictionary json usage."""
 
-import json
 import os
+from enum import Enum
 from pathlib import Path
 from typing import Any, Literal
+
 from .save_handlers import HANDLERS, SaveHandler
 
 
 class CfgDict(dict):
     """
     A subclass of `dict` with some useful changes, most notably
     storing a path to save, including saving methods
@@ -45,14 +46,15 @@
 
     def save(self, out_dict=None):
         """saves the dict to the file"""
         if not isinstance(out_dict, dict):
             out_dict = self
         if self.sort_on_save:
             out_dict = dict(sorted(out_dict.items()))
+        print(out_dict)
         self.save_handler.save(dict(out_dict))
         return self
 
     def _save_on_change(self) -> bool:
         if self.save_on_change:
             self.save()
             return True
@@ -79,25 +81,25 @@
                 self.update(self.save_handler.load())
             except Exception:
                 print(f"[!] failed to load config from {self.cfg_path}")
         else:
             self.save({})
         return self
 
-    @staticmethod
-    def is_json_serializable(obj: Any) -> bool:
+    def is_serializable(self, obj: Any) -> bool:
         """checks if an object is JSON Serializable"""
-        try:
-            json.dumps(obj)
-            return True
-        except (TypeError, OverflowError):
-            return False
+        return self.save_handler.try_serialize(obj)
 
     def __setitem__(self, key, value):
-        super().__setitem__(key, value)
+        if isinstance(value, Enum):
+            new_val: str = value.value  # I don't like this
+        else:
+            new_val = value
+
+        super().__setitem__(key, new_val)
         if self.save_on_change:
             self.save()
 
     def __delitem__(self, key):
         super().__delitem__(key)
         if self.save_on_change:
             self.save()
```

### Comparing `cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/function_config_wrapper.py` & `cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper/function_config_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def _wrapper(func: Callable) -> Callable:
         # get parameters and defaults
 
         parameters: dict[str, inspect.Parameter] = dict(inspect.signature(func).parameters)
         save_after = False
         for name, param in parameters.items():
             if name not in cfg_dict:
-                if cfg_dict.is_json_serializable(param.default):
+                if cfg_dict.is_serializable(param.default):
                     save_after = True
                     cfg_dict[name] = param.default
         if save_after:
             cfg_dict.save()
         new_defaults = dict(zip(parameters.keys(), map(lambda x: x.default, parameters.values())))
         new_defaults.update({k: v for k, v in cfg_dict.items() if k in new_defaults})
```

### Comparing `cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/PKG-INFO` & `cfg-param-wrapper-1.0.0.post2/src/cfg_param_wrapper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-param-wrapper
-Version: 1.0.0.post1
+Version: 1.0.0.post2
 Summary: A package designed to simplify defaults.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: typer
 License-File: LICENSE
 
-# cfg_param_wrapper 1.0.0
+# cfg_param_wrapper 1.0.0-2
 
 a config wrapper I made. It's made to wrap simple functions, and intercept configurations in tandem with a CfgDict object.
 
 ## Installation
 
 ```bash
 # from pypi:
```

