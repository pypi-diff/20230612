# Comparing `tmp/prodot-0.3.6.tar.gz` & `tmp/prodot-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodot-0.3.6.tar", max compression
+gzip compressed data, was "prodot-0.3.7.tar", max compression
```

## Comparing `prodot-0.3.6.tar` & `prodot-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-06-08 15:23:39.052025 prodot-0.3.6/LICENSE
--rw-r--r--   0        0        0     3615 2023-06-08 15:23:39.052025 prodot-0.3.6/README.md
--rw-r--r--   0        0        0      106 2023-06-08 15:23:39.052025 prodot-0.3.6/prodot/__init__.py
--rw-r--r--   0        0        0     2615 2023-06-08 19:51:16.247848 prodot-0.3.6/prodot/_base_object.py
--rw-r--r--   0        0        0     2510 2023-06-08 19:34:38.298107 prodot-0.3.6/prodot/_dot_object.py
--rw-r--r--   0        0        0     1741 2023-06-08 19:34:10.768114 prodot-0.3.6/prodot/_path_object.py
--rw-r--r--   0        0        0      443 2023-06-08 15:23:39.052025 prodot-0.3.6/prodot/_pro_object.py
--rw-r--r--   0        0        0      105 2023-06-08 15:23:39.052025 prodot-0.3.6/prodot/json_tools/__init__.py
--rw-r--r--   0        0        0       73 2023-06-08 15:23:39.052025 prodot-0.3.6/prodot/json_tools/_filter/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-08 15:23:39.052025 prodot-0.3.6/prodot/json_tools/_filter/__main__.py
--rw-r--r--   0        0        0     1535 2023-06-08 15:23:39.052025 prodot-0.3.6/prodot/json_tools/_filter/_filter_byPath.py
--rw-r--r--   0        0        0     2158 2023-06-08 19:36:47.368074 prodot-0.3.6/prodot/json_tools/_filter/_filter_byValue.py
--rw-r--r--   0        0        0     1169 2023-06-08 15:23:39.062025 prodot-0.3.6/prodot/json_tools/_filter/_filtered_object.py
--rw-r--r--   0        0        0      803 2023-06-08 15:23:39.062025 prodot-0.3.6/prodot/json_tools/_get_all_paths.py
--rw-r--r--   0        0        0      392 2023-06-08 19:56:05.547773 prodot-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 prodot-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-08 15:23:39.052025 prodot-0.3.7/LICENSE
+-rw-r--r--   0        0        0     3615 2023-06-08 15:23:39.052025 prodot-0.3.7/README.md
+-rw-r--r--   0        0        0      106 2023-06-08 15:23:39.052025 prodot-0.3.7/prodot/__init__.py
+-rw-r--r--   0        0        0     2816 2023-06-12 02:30:45.757321 prodot-0.3.7/prodot/_base_object.py
+-rw-r--r--   0        0        0     2297 2023-06-12 02:29:18.387344 prodot-0.3.7/prodot/_dot_object.py
+-rw-r--r--   0        0        0     1892 2023-06-12 02:26:31.197387 prodot-0.3.7/prodot/_path_object.py
+-rw-r--r--   0        0        0      443 2023-06-08 15:23:39.052025 prodot-0.3.7/prodot/_pro_object.py
+-rw-r--r--   0        0        0      105 2023-06-08 15:23:39.052025 prodot-0.3.7/prodot/json_tools/__init__.py
+-rw-r--r--   0        0        0       73 2023-06-08 15:23:39.052025 prodot-0.3.7/prodot/json_tools/_filter/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-08 15:23:39.052025 prodot-0.3.7/prodot/json_tools/_filter/__main__.py
+-rw-r--r--   0        0        0     1535 2023-06-08 15:23:39.052025 prodot-0.3.7/prodot/json_tools/_filter/_filter_byPath.py
+-rw-r--r--   0        0        0     2158 2023-06-08 19:36:47.368074 prodot-0.3.7/prodot/json_tools/_filter/_filter_byValue.py
+-rw-r--r--   0        0        0     1169 2023-06-08 15:23:39.062025 prodot-0.3.7/prodot/json_tools/_filter/_filtered_object.py
+-rw-r--r--   0        0        0      803 2023-06-08 15:23:39.062025 prodot-0.3.7/prodot/json_tools/_get_all_paths.py
+-rw-r--r--   0        0        0      392 2023-06-12 02:32:23.317296 prodot-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 prodot-0.3.7/PKG-INFO
```

### Comparing `prodot-0.3.6/LICENSE` & `prodot-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prodot-0.3.6/README.md` & `prodot-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `prodot-0.3.6/prodot/_base_object.py` & `prodot-0.3.7/prodot/_base_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,20 +40,25 @@
         return Scope(self, self.main_object)
 
     def __contains__(self, value: str)-> t.Any:
         if value in self.main_object:
             return True
         return False
 
-    def __init__(self, main_object: t.Union[t.Dict, t.List, None] = dict()):
+    def __init__(self, main_object: t.Union[t.Dict, t.List, None] = {}, *args, **kwargs):
         '''
         The init will receive the main object as parameter, 
         or will create an initialize with an empty dictionary
         '''
-        self.main_object = main_object
+        if main_object or kwargs.get('maintain'):
+            self.main_object = main_object
+        elif isinstance(main_object, list):
+            self.main_object = list()
+        else:
+            self.main_object = dict()
 
     def __repr__(self) -> t.Dict:
         return str(self.main_object)
     
     def true_repr(self)-> str:
         '''
         returns the original representation of the base
```

### Comparing `prodot-0.3.6/prodot/_dot_object.py` & `prodot-0.3.7/prodot/_dot_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,41 +13,33 @@
 
     ## Parameters
     `main_object:` a Dict or List object that will be interpreted
     by the children objects
     '''
     arrayTypes = [list]
     numberIndexKey = 'n'
-    _temp_path = '$'
 
     def __getattr__(self, name: str) -> t.Self:
         if type(self.main_object) in self.arrayTypes:
             res = self._get_array(name)
         else:
             res = self._get_map(name)
 
         if isinstance(res, list) or isinstance(res, dict):
-            return self.__class__(res)
+            return self.__class__(res, maintain=True)
         return res
         
     def __setattr__(self, name: str, value: t.Any) -> None:
         if name in dir(self):
             return super().__setattr__(name, value)
 
         if name == 'main_object':
             self.__dict__[name] = value
             return
 
-        if self._temp_path != '$':
-
-            json_path = self.__treat_path(f'{self._temp_path}.{name}')
-
-            parse(json_path).update_or_create(self.main_object, value)
-            return
-        
         if type(self.main_object) in self.arrayTypes:
             self._set_array(name, value)
             return
         self._set_map(name, value)
             
     def _get_map(self, name:str) -> t.Any:
         if name in self.main_object:
```

### Comparing `prodot-0.3.6/prodot/_path_object.py` & `prodot-0.3.7/prodot/_path_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,23 +32,27 @@
         returns a filter instance responsible to extract data
         from the main_object
         '''
         return self.__filter_object(self.main_object, self)
         
     def __getitem__(self, name:str)->t.Self:
         try:
+            if isinstance(name, int):
+                name = f'n{name}'
             res = parse('$.'+name).find(self.main_object)[0].value
             if isinstance(res, list) or isinstance(res, dict):
-                return self.__class__(res)
+                return self.__class__(res, maintain=True)
             return res
     
         except IndexError:
             raise IndexError(f"path <<{name}>> not found in  the main_object")
 
     def __setitem__(self, name:str, value:t.Any):
+        if isinstance(name, int):
+            name = f'n{name}'
         path = parse('$.'+name)
         path.update_or_create(self.main_object, value)
 
     def get_all_paths(self, **kwargs)->t.Iterable:
         '''
         return an iterable that
         runs across the entire main_object, returning
```

### Comparing `prodot-0.3.6/prodot/json_tools/_filter/__main__.py` & `prodot-0.3.7/prodot/json_tools/_filter/__main__.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.6/prodot/json_tools/_filter/_filter_byPath.py` & `prodot-0.3.7/prodot/json_tools/_filter/_filter_byPath.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.6/prodot/json_tools/_filter/_filter_byValue.py` & `prodot-0.3.7/prodot/json_tools/_filter/_filter_byValue.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.6/prodot/json_tools/_filter/_filtered_object.py` & `prodot-0.3.7/prodot/json_tools/_filter/_filtered_object.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.6/prodot/json_tools/_get_all_paths.py` & `prodot-0.3.7/prodot/json_tools/_get_all_paths.py`

 * *Files identical despite different names*

### Comparing `prodot-0.3.6/PKG-INFO` & `prodot-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodot
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 License: GNU GENERAL PUBLIC LICENSE
 Author: Matheus Menezes Almeida
 Author-email: mrotame@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

