# Comparing `tmp/yaml-extender-0.0.6.tar.gz` & `tmp/yaml-extender-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-extender-0.0.6.tar", last modified: Thu May 11 18:06:56 2023, max compression
+gzip compressed data, was "yaml-extender-0.0.7.tar", last modified: Mon Jun 12 16:44:36 2023, max compression
```

## Comparing `yaml-extender-0.0.6.tar` & `yaml-extender-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.390165 yaml-extender-0.0.6/
--rw-rw-rw-   0        0        0      605 2023-05-11 18:06:24.000000 yaml-extender-0.0.6/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1507 2023-01-31 17:42:46.000000 yaml-extender-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      364 2022-11-12 09:32:28.000000 yaml-extender-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     7135 2023-05-11 18:06:56.389163 yaml-extender-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4580 2023-01-31 18:06:45.000000 yaml-extender-0.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.361138 yaml-extender-0.0.6/docs/
--rw-rw-rw-   0        0        0     6717 2022-11-12 09:32:28.000000 yaml-extender-0.0.6/docs/conf.py
--rw-rw-rw-   0        0        0     1373 2023-01-31 18:53:09.000000 yaml-extender-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-11 18:06:56.390165 yaml-extender-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.351599 yaml-extender-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.373149 yaml-extender-0.0.6/src/yaml_extender/
--rw-rw-rw-   0        0        0       68 2023-05-11 18:05:30.000000 yaml-extender-0.0.6/src/yaml_extender/__init__.py
--rw-rw-rw-   0        0        0       96 2023-02-02 18:58:26.000000 yaml-extender-0.0.6/src/yaml_extender/__main__.py
--rw-rw-rw-   0        0        0     1505 2023-05-11 18:01:55.000000 yaml-extender-0.0.6/src/yaml_extender/cli.py
--rw-rw-rw-   0        0        0      796 2022-11-12 14:08:22.000000 yaml-extender-0.0.6/src/yaml_extender/logger.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.388162 yaml-extender-0.0.6/src/yaml_extender/resolver/
--rw-rw-rw-   0        0        0        0 2022-11-17 17:18:02.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/__init__.py
--rw-rw-rw-   0        0        0     5876 2023-03-01 17:07:08.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/include_resolver.py
--rw-rw-rw-   0        0        0     2975 2023-02-27 17:47:13.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/loop_resolver.py
--rw-rw-rw-   0        0        0     5542 2023-02-27 17:47:13.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/reference_resolver.py
--rw-rw-rw-   0        0        0      683 2023-02-27 18:52:59.000000 yaml-extender-0.0.6/src/yaml_extender/resolver/resolver.py
--rw-rw-rw-   0        0        0      469 2023-02-27 18:50:34.000000 yaml-extender-0.0.6/src/yaml_extender/xyml_exception.py
--rw-rw-rw-   0        0        0     1883 2023-05-11 18:04:26.000000 yaml-extender-0.0.6/src/yaml_extender/xyml_file.py
--rw-rw-rw-   0        0        0      963 2023-01-15 11:35:59.000000 yaml-extender-0.0.6/src/yaml_extender/yaml_loader.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:06:56.385160 yaml-extender-0.0.6/src/yaml_extender.egg-info/
--rw-rw-rw-   0        0        0     7135 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      751 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-11 18:06:56.000000 yaml-extender-0.0.6/src/yaml_extender.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.593024 yaml-extender-0.0.7/
+-rw-rw-rw-   0        0        0      878 2023-06-12 16:43:30.000000 yaml-extender-0.0.7/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1507 2023-01-31 17:42:46.000000 yaml-extender-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      364 2022-11-12 09:32:28.000000 yaml-extender-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     7135 2023-06-12 16:44:36.592023 yaml-extender-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4580 2023-01-31 18:06:45.000000 yaml-extender-0.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.559994 yaml-extender-0.0.7/docs/
+-rw-rw-rw-   0        0        0     6717 2022-11-12 09:32:28.000000 yaml-extender-0.0.7/docs/conf.py
+-rw-rw-rw-   0        0        0     1373 2023-01-31 18:53:09.000000 yaml-extender-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 16:44:36.593024 yaml-extender-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.550986 yaml-extender-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.573005 yaml-extender-0.0.7/src/yaml_extender/
+-rw-rw-rw-   0        0        0       68 2023-06-12 16:43:36.000000 yaml-extender-0.0.7/src/yaml_extender/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-02-02 18:58:26.000000 yaml-extender-0.0.7/src/yaml_extender/__main__.py
+-rw-rw-rw-   0        0        0     1505 2023-05-11 18:01:55.000000 yaml-extender-0.0.7/src/yaml_extender/cli.py
+-rw-rw-rw-   0        0        0      796 2022-11-12 14:08:22.000000 yaml-extender-0.0.7/src/yaml_extender/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.592023 yaml-extender-0.0.7/src/yaml_extender/resolver/
+-rw-rw-rw-   0        0        0        0 2022-11-17 17:18:02.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/__init__.py
+-rw-rw-rw-   0        0        0     5850 2023-06-09 14:42:34.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/include_resolver.py
+-rw-rw-rw-   0        0        0     2975 2023-02-27 17:47:13.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/loop_resolver.py
+-rw-rw-rw-   0        0        0     6044 2023-06-12 16:41:27.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/reference_resolver.py
+-rw-rw-rw-   0        0        0      683 2023-02-27 18:52:59.000000 yaml-extender-0.0.7/src/yaml_extender/resolver/resolver.py
+-rw-rw-rw-   0        0        0      469 2023-02-27 18:50:34.000000 yaml-extender-0.0.7/src/yaml_extender/xyml_exception.py
+-rw-rw-rw-   0        0        0     1883 2023-05-11 18:04:26.000000 yaml-extender-0.0.7/src/yaml_extender/xyml_file.py
+-rw-rw-rw-   0        0        0      963 2023-01-15 11:35:59.000000 yaml-extender-0.0.7/src/yaml_extender/yaml_loader.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:44:36.588020 yaml-extender-0.0.7/src/yaml_extender.egg-info/
+-rw-rw-rw-   0        0        0     7135 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      751 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-12 16:44:36.000000 yaml-extender-0.0.7/src/yaml_extender.egg-info/top_level.txt
```

### Comparing `yaml-extender-0.0.6/LICENSE` & `yaml-extender-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/PKG-INFO` & `yaml-extender-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-extender
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extends the common .yaml syntax to provide more complex configuration options
 Author-email: Simon Gallitscher <adun.sg@gmx.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Simon Gallitscher
         All rights reserved.
```

### Comparing `yaml-extender-0.0.6/README.rst` & `yaml-extender-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/docs/conf.py` & `yaml-extender-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/pyproject.toml` & `yaml-extender-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/src/yaml_extender/cli.py` & `yaml-extender-0.0.7/src/yaml_extender/cli.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/src/yaml_extender/logger.py` & `yaml-extender-0.0.7/src/yaml_extender/logger.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/src/yaml_extender/resolver/include_resolver.py` & `yaml-extender-0.0.7/src/yaml_extender/resolver/include_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,16 @@
                     self.update_content_with_include_content(cur_value, include_content)
                     del cur_value[INCLUDE_KEY]
                 else:
                     if len(cur_value) > 1:
                         raise ExtYamlSyntaxError(f"Unable to resolve {cur_value}."
                                                  f"Included file does not return a dictionary.")
                     cur_value = include_content
-            else:
-                for k, v in cur_value.items():
-                    cur_value[k] = self.__resolve_inc(cur_value[k], config)
+            for k, v in cur_value.items():
+                cur_value[k] = self.__resolve_inc(cur_value[k], config)
         elif isinstance(cur_value, list):
             new_content = []
             for i, x in enumerate(cur_value):
                 new_value = (self.__resolve_inc(x, config))
                 if isinstance(new_value, list):
                     new_content.extend(new_value)
                 else:
```

### Comparing `yaml-extender-0.0.6/src/yaml_extender/resolver/loop_resolver.py` & `yaml-extender-0.0.7/src/yaml_extender/resolver/loop_resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/src/yaml_extender/resolver/reference_resolver.py` & `yaml-extender-0.0.7/src/yaml_extender/resolver/reference_resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from yaml_extender import yaml_loader
 from yaml_extender.resolver.resolver import Resolver
 from yaml_extender.xyml_exception import RecursiveReferenceError, ReferenceNotFoundError, ExtYamlSyntaxError
 
 REFERENCE_REGEX = r'\{\{(.+?)(?::(.*?))?\}\}'
 ARRAY_REGEX = r'(.*)?\[(\d*)\]'
+LIST_FLATTEN_CHARACTER = " "
 
 MAXIMUM_REFERENCE_DEPTH = 30
 
 
 class ArithmeticOperation:
 
     SUPPORTED_FUNCS = {"+": lambda x, y: x + y,
@@ -51,16 +52,23 @@
     def _Resolver__resolve(self, cur_value: Any, config: dict):
         """Resolves all references in a given value using the provided content dict"""
         new_value = cur_value
         if isinstance(cur_value, dict):
             for k in cur_value.keys():
                 cur_value[k] = self._Resolver__resolve(cur_value[k], config)
         elif isinstance(cur_value, list):
+            new_list = []
             for i, x in enumerate(cur_value):
-                cur_value[i] = self._Resolver__resolve(x, config)
+                resolved_value = self._Resolver__resolve(x, config)
+                if isinstance(resolved_value, list):
+                    # If the returned value is also a list, extend the current list with it
+                    new_list.extend(resolved_value)
+                else:
+                    new_list.append(self._Resolver__resolve(x, config))
+            new_value = new_list
         else:
             new_value = self.resolve_reference(cur_value, config)
         return new_value
 
     def resolve_reference(self, value: Any, config: dict, depth: int = 0) -> Any:
         if not isinstance(value, str) or "{" not in value:
             return value
@@ -119,14 +127,16 @@
                     ref_val = operation.apply(ref_val)
                 if ref_match.group(0) == value:
                     # If the whole string is just a reference return the value without string replacement
                     # in order to preserve float & int types
                     return ref_val
                 else:
                     # Replace the reference string with the value
+                    if isinstance(ref_val, list):
+                        ref_val = LIST_FLATTEN_CHARACTER.join(ref_val)
                     new_value = new_value.replace(ref_match.group(0), str(ref_val))
 
         if new_value == value:
             if self.fail_on_resolve:
                 raise ReferenceNotFoundError(value)
             else:
                 return value
```

### Comparing `yaml-extender-0.0.6/src/yaml_extender/resolver/resolver.py` & `yaml-extender-0.0.7/src/yaml_extender/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/src/yaml_extender/xyml_file.py` & `yaml-extender-0.0.7/src/yaml_extender/xyml_file.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/src/yaml_extender/yaml_loader.py` & `yaml-extender-0.0.7/src/yaml_extender/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.0.6/src/yaml_extender.egg-info/PKG-INFO` & `yaml-extender-0.0.7/src/yaml_extender.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-extender
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extends the common .yaml syntax to provide more complex configuration options
 Author-email: Simon Gallitscher <adun.sg@gmx.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Simon Gallitscher
         All rights reserved.
```

### Comparing `yaml-extender-0.0.6/src/yaml_extender.egg-info/SOURCES.txt` & `yaml-extender-0.0.7/src/yaml_extender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

