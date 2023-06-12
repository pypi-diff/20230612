# Comparing `tmp/mapperr-0.1.0.tar.gz` & `tmp/mapperr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapperr-0.1.0.tar", last modified: Fri May 19 20:26:47 2023, max compression
+gzip compressed data, was "mapperr-0.1.1.tar", last modified: Mon Jun 12 04:25:22 2023, max compression
```

## Comparing `mapperr-0.1.0.tar` & `mapperr-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-19 20:26:47.987399 mapperr-0.1.0/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.1.0/LICENSE
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2684 2023-05-19 20:26:47.987256 mapperr-0.1.0/PKG-INFO
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     2314 2023-05-19 20:22:50.000000 mapperr-0.1.0/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-19 20:26:47.985823 mapperr-0.1.0/mapperr/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      959 2023-05-15 14:38:18.000000 mapperr-0.1.0/mapperr/__init__.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     2346 2023-05-15 14:38:18.000000 mapperr-0.1.0/mapperr/mapr.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-19 20:26:47.986522 mapperr-0.1.0/mapperr.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2684 2023-05-19 20:26:47.000000 mapperr-0.1.0/mapperr.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      268 2023-05-19 20:26:47.000000 mapperr-0.1.0/mapperr.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-05-19 20:26:47.000000 mapperr-0.1.0/mapperr.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-05-19 20:26:47.000000 mapperr-0.1.0/mapperr.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-05-19 20:26:47.987449 mapperr-0.1.0/setup.cfg
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-05-19 20:23:41.000000 mapperr-0.1.0/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-19 20:26:47.987028 mapperr-0.1.0/test/
--rw-rw-r--   0 mujdecisy   (501) staff       (20)     1741 2023-05-15 14:38:02.000000 mapperr-0.1.0/test/test_nested_objects.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.1.0/test/test_op_required.py
--rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-05-15 14:38:02.000000 mapperr-0.1.0/test/test_unmatched_types.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-06-12 04:25:22.093165 mapperr-0.1.1/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-05-15 14:31:09.000000 mapperr-0.1.1/LICENSE
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2684 2023-06-12 04:25:22.092992 mapperr-0.1.1/PKG-INFO
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2314 2023-05-19 20:22:50.000000 mapperr-0.1.1/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-06-12 04:25:22.091496 mapperr-0.1.1/mapperr/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      959 2023-05-19 20:57:17.000000 mapperr-0.1.1/mapperr/__init__.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2364 2023-06-12 04:18:50.000000 mapperr-0.1.1/mapperr/mapr.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-06-12 04:25:22.092173 mapperr-0.1.1/mapperr.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2684 2023-06-12 04:25:22.000000 mapperr-0.1.1/mapperr.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      268 2023-06-12 04:25:22.000000 mapperr-0.1.1/mapperr.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-06-12 04:25:22.000000 mapperr-0.1.1/mapperr.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        8 2023-06-12 04:25:22.000000 mapperr-0.1.1/mapperr.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-06-12 04:25:22.093213 mapperr-0.1.1/setup.cfg
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      697 2023-06-12 04:23:31.000000 mapperr-0.1.1/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-06-12 04:25:22.092740 mapperr-0.1.1/test/
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)     2064 2023-06-12 04:22:42.000000 mapperr-0.1.1/test/test_nested_objects.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      711 2023-05-19 20:18:23.000000 mapperr-0.1.1/test/test_op_required.py
+-rw-rw-r--   0 mujdecisy   (501) staff       (20)      763 2023-05-15 14:38:02.000000 mapperr-0.1.1/test/test_unmatched_types.py
```

### Comparing `mapperr-0.1.0/LICENSE` & `mapperr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mapperr-0.1.0/PKG-INFO` & `mapperr-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapperr
-Version: 0.1.0
+Version: 0.1.1
 Summary: mapperr for mapping across dict and object, recursively
 Home-page: https://github.com/mujdecisy/mapperr
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,mapper,recursive mapping
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mapperr-0.1.0/README.md` & `mapperr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mapperr-0.1.0/mapperr/__init__.py` & `mapperr-0.1.1/mapperr/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from mapperr.mapr import _maprit
 
+def to_dict( src: object ) -> dict:
+    des = {}
+    return _maprit(src, des, src.__class__)
+
 def to_obj( src: dict, root_class: type) -> object:
     des: object = root_class()
     required_variables = getattr(des, 'op_required', [])
 
     res = _maprit(src, des, root_class)
 
     res.__setattr__('op_required', required_variables)
     __check_required(res, root_class)
     return res
 
-def to_dict( src: object ) -> dict:
-    des = {}
-    return _maprit(src, des, src.__class__)
-
 def obj_to_obj( src: object, dest_class: type ) -> object:
     d = to_dict(src)
     return to_obj(d, dest_class)
 
 def __check_required(o: object, root_class: type) -> bool:
     required_variables: list = getattr(o, 'op_required', [])
     annot_keys = root_class.__annotations__.keys()
```

### Comparing `mapperr-0.1.0/mapperr/mapr.py` & `mapperr-0.1.1/mapperr/mapr.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,16 @@
 }
 
 __prm = {
     str: "str",
     int: "int",
     float: "float",
     dict: "dict",
-    list: "list"
+    list: "list",
+    bool: "bool"
 }
 
 def __simport(module_and_class: str):
     cstr = module_and_class.split(".")[-1]
     mstr = module_and_class.replace(f".{cstr}", "")
     m = importlib.import_module(mstr)
     c = getattr(m, cstr)
```

### Comparing `mapperr-0.1.0/mapperr.egg-info/PKG-INFO` & `mapperr-0.1.1/mapperr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapperr
-Version: 0.1.0
+Version: 0.1.1
 Summary: mapperr for mapping across dict and object, recursively
 Home-page: https://github.com/mujdecisy/mapperr
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,mapper,recursive mapping
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mapperr-0.1.0/setup.py` & `mapperr-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="mapperr",
-    version="0.1.0",
+    version="0.1.1",
     description="mapperr for mapping across dict and object, recursively",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/mapperr",
     keywords=["python", "mapper", "recursive mapping"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
```

### Comparing `mapperr-0.1.0/test/test_op_required.py` & `mapperr-0.1.1/test/test_op_required.py`

 * *Files identical despite different names*

### Comparing `mapperr-0.1.0/test/test_unmatched_types.py` & `mapperr-0.1.1/test/test_unmatched_types.py`

 * *Files identical despite different names*

