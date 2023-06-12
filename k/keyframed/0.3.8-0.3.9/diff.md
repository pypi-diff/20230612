# Comparing `tmp/keyframed-0.3.8.tar.gz` & `tmp/keyframed-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyframed-0.3.8.tar", last modified: Thu Mar  2 01:29:27 2023, max compression
+gzip compressed data, was "keyframed-0.3.9.tar", last modified: Fri Mar  3 03:27:02 2023, max compression
```

## Comparing `keyframed-0.3.8.tar` & `keyframed-0.3.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 01:29:27.598588 keyframed-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    19562 2023-03-02 01:29:27.598588 keyframed-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19416 2023-03-02 01:29:18.000000 keyframed-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 01:29:27.598588 keyframed-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-02 01:29:18.000000 keyframed-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 01:29:27.594588 keyframed-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 01:29:27.594588 keyframed-0.3.8/src/keyframed/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-02 01:29:18.000000 keyframed-0.3.8/src/keyframed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29482 2023-03-02 01:29:18.000000 keyframed-0.3.8/src/keyframed/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-02 01:29:18.000000 keyframed-0.3.8/src/keyframed/dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-02 01:29:18.000000 keyframed-0.3.8/src/keyframed/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-02 01:29:18.000000 keyframed-0.3.8/src/keyframed/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-03-02 01:29:18.000000 keyframed-0.3.8/src/keyframed/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-02 01:29:18.000000 keyframed-0.3.8/src/keyframed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 01:29:27.598588 keyframed-0.3.8/src/keyframed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19562 2023-03-02 01:29:27.000000 keyframed-0.3.8/src/keyframed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-02 01:29:27.000000 keyframed-0.3.8/src/keyframed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 01:29:27.000000 keyframed-0.3.8/src/keyframed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-02 01:29:27.000000 keyframed-0.3.8/src/keyframed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-02 01:29:27.000000 keyframed-0.3.8/src/keyframed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 01:29:27.598588 keyframed-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_append.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_curve_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_hawkes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_pgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_sinusoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-02 01:29:18.000000 keyframed-0.3.8/tests/test_slicing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 03:27:02.269149 keyframed-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-03-03 03:27:02.269149 keyframed-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20085 2023-03-03 03:26:52.000000 keyframed-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 03:27:02.269149 keyframed-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-03 03:26:52.000000 keyframed-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 03:27:02.265148 keyframed-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 03:27:02.265148 keyframed-0.3.9/src/keyframed/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-03 03:26:52.000000 keyframed-0.3.9/src/keyframed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29482 2023-03-03 03:26:52.000000 keyframed-0.3.9/src/keyframed/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-03 03:26:52.000000 keyframed-0.3.9/src/keyframed/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-03 03:26:52.000000 keyframed-0.3.9/src/keyframed/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-03 03:26:52.000000 keyframed-0.3.9/src/keyframed/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-03-03 03:26:52.000000 keyframed-0.3.9/src/keyframed/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-03 03:26:52.000000 keyframed-0.3.9/src/keyframed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 03:27:02.265148 keyframed-0.3.9/src/keyframed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-03-03 03:27:02.000000 keyframed-0.3.9/src/keyframed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-03 03:27:02.000000 keyframed-0.3.9/src/keyframed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 03:27:02.000000 keyframed-0.3.9/src/keyframed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-03 03:27:02.000000 keyframed-0.3.9/src/keyframed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-03 03:27:02.000000 keyframed-0.3.9/src/keyframed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 03:27:02.269149 keyframed-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_curve_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_hawkes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_pgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_sinusoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-03 03:26:52.000000 keyframed-0.3.9/tests/test_slicing.py
```

### Comparing `keyframed-0.3.8/PKG-INFO` & `keyframed-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: keyframed
-Version: 0.3.8
-Author: David Marx
-License: MIT
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 
 # <p align=center> Keyframed
 
  <p align=center><img alt="a colorful plot demonstrating something the library can achieve" src="static/images/fancy.png"/>
 
 ## <p align=center>Simple, Expressive Datatypes <br>For Manipulating Parameter Curves
 
@@ -515,16 +507,36 @@
       - 0.3
     loop: true
 """.strip()
 
 curves = serialization.from_yaml(txt)
 ```
 
-For most users, yaml serialization will probably be more useful. The yaml serialization machinery is built around an intermediary `dict` structure 
-that might be more appropriate for certain use cases, such as users who want to serialize keyframed objects to JSON.
+Breaking down the yaml syntax:
+
+```yaml
+curve:
+- - <time0>
+  - <value0>
+  - <interpolation method>
+  - <interpolator arguments>
+- - <time1>
+  - <value1>
+  - <another interpolation method, this one doesn't take arguments >
+- - <time2>
+  - <value2>
+  # because no interpolator is specified, time2 falls back to the most recent keyframe where an interpolator was 
+  # specified and re-uses the interpolation method from time1. To include redundant information like an 
+  # interpolator that is implied by a previous frame (because it's the same), set `simplify=False` when calling
+  # the serialization method (usually `to_yaml`).
+```
+
+Yaml serialization as just demonstrated will probably be the preferred approach for most use cases.
+The yaml serialization machinery is built around an intermediary `dict` structure 
+that might be more appropriate for certain situations, such as users who want to serialize keyframed objects to JSON.
 
 ```python
 d = curves.to_dict(simplify=True, for_yaml=False)
 ## returned dict looks like this:
 # {'parameters': {'foo': {'curve': {0: {'value': 0.0001,
 #      'interpolation_method': 'eased_lerp'},
 #     49: {'value': 0.3},
```

### Comparing `keyframed-0.3.8/README.md` & `keyframed-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: keyframed
+Version: 0.3.9
+Author: David Marx
+License: MIT
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 
 # <p align=center> Keyframed
 
  <p align=center><img alt="a colorful plot demonstrating something the library can achieve" src="static/images/fancy.png"/>
 
 ## <p align=center>Simple, Expressive Datatypes <br>For Manipulating Parameter Curves
 
@@ -507,16 +515,36 @@
       - 0.3
     loop: true
 """.strip()
 
 curves = serialization.from_yaml(txt)
 ```
 
-For most users, yaml serialization will probably be more useful. The yaml serialization machinery is built around an intermediary `dict` structure 
-that might be more appropriate for certain use cases, such as users who want to serialize keyframed objects to JSON.
+Breaking down the yaml syntax:
+
+```yaml
+curve:
+- - <time0>
+  - <value0>
+  - <interpolation method>
+  - <interpolator arguments>
+- - <time1>
+  - <value1>
+  - <another interpolation method, this one doesn't take arguments >
+- - <time2>
+  - <value2>
+  # because no interpolator is specified, time2 falls back to the most recent keyframe where an interpolator was 
+  # specified and re-uses the interpolation method from time1. To include redundant information like an 
+  # interpolator that is implied by a previous frame (because it's the same), set `simplify=False` when calling
+  # the serialization method (usually `to_yaml`).
+```
+
+Yaml serialization as just demonstrated will probably be the preferred approach for most use cases.
+The yaml serialization machinery is built around an intermediary `dict` structure 
+that might be more appropriate for certain situations, such as users who want to serialize keyframed objects to JSON.
 
 ```python
 d = curves.to_dict(simplify=True, for_yaml=False)
 ## returned dict looks like this:
 # {'parameters': {'foo': {'curve': {0: {'value': 0.0001,
 #      'interpolation_method': 'eased_lerp'},
 #     49: {'value': 0.3},
```

### Comparing `keyframed-0.3.8/setup.py` & `keyframed-0.3.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 st = """
 Simple, expressive, pythonic datatypes for manipulating curves parameterized by keyframes and interpolators. The motivation for this library is to facilitate object-oriented parameterization of generative animations.
 """.strip()
         
 setup(
     name='keyframed',
-    version='0.3.8',
+    version='0.3.9',
     author='David Marx',
     long_description=README,
     long_description_content_type='text/markdown',
     short_description=st,
     install_requires=[
         'sortedcontainers',
         'omegaconf',
```

### Comparing `keyframed-0.3.8/src/keyframed/__init__.py` & `keyframed-0.3.9/src/keyframed/__init__.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/src/keyframed/curve.py` & `keyframed-0.3.9/src/keyframed/curve.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/src/keyframed/dsl.py` & `keyframed-0.3.9/src/keyframed/dsl.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/src/keyframed/interpolation.py` & `keyframed-0.3.9/src/keyframed/interpolation.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/src/keyframed/misc.py` & `keyframed-0.3.9/src/keyframed/misc.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/src/keyframed/serialization.py` & `keyframed-0.3.9/src/keyframed/serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .curve import Keyframe, Curve, CurveBase, ParameterGroup, Composition
 
+from numbers import Number
+
 # can probably use a simpler yaml library
 from omegaconf import OmegaConf
 
 #from loguru import logger
 
 def _test_type_by_keys(d:dict, keys):
     assert isinstance(d, dict)
@@ -77,15 +79,21 @@
         if d.get('label') is not None:
             d_['label'] = d['label']
         if d.get('weight') is not None:
             d_['weight'] = from_dict(d['weight'])
 
         curves = {}
         for k,v in d['parameters'].items():
-            curves[k] = from_dict(v)
+            if isinstance(v, Number):
+                param = v
+            elif isinstance(v, dict):
+                param = from_dict(v)
+            else:
+                raise NotImplementedError(f"expected number of dict, got {v} of type {type(v)}")
+            curves[k] = param
         d_['parameters'] = curves
 
         if not _is_comp(d):
             return ParameterGroup(**d_)
         else:
             d_['reduction'] = d['reduction']
             return Composition(**d_)
```

### Comparing `keyframed-0.3.8/src/keyframed/utils.py` & `keyframed-0.3.9/src/keyframed/utils.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/src/keyframed.egg-info/PKG-INFO` & `keyframed-0.3.9/src/keyframed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyframed
-Version: 0.3.8
+Version: 0.3.9
 Author: David Marx
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 
 # <p align=center> Keyframed
@@ -515,16 +515,36 @@
       - 0.3
     loop: true
 """.strip()
 
 curves = serialization.from_yaml(txt)
 ```
 
-For most users, yaml serialization will probably be more useful. The yaml serialization machinery is built around an intermediary `dict` structure 
-that might be more appropriate for certain use cases, such as users who want to serialize keyframed objects to JSON.
+Breaking down the yaml syntax:
+
+```yaml
+curve:
+- - <time0>
+  - <value0>
+  - <interpolation method>
+  - <interpolator arguments>
+- - <time1>
+  - <value1>
+  - <another interpolation method, this one doesn't take arguments >
+- - <time2>
+  - <value2>
+  # because no interpolator is specified, time2 falls back to the most recent keyframe where an interpolator was 
+  # specified and re-uses the interpolation method from time1. To include redundant information like an 
+  # interpolator that is implied by a previous frame (because it's the same), set `simplify=False` when calling
+  # the serialization method (usually `to_yaml`).
+```
+
+Yaml serialization as just demonstrated will probably be the preferred approach for most use cases.
+The yaml serialization machinery is built around an intermediary `dict` structure 
+that might be more appropriate for certain situations, such as users who want to serialize keyframed objects to JSON.
 
 ```python
 d = curves.to_dict(simplify=True, for_yaml=False)
 ## returned dict looks like this:
 # {'parameters': {'foo': {'curve': {0: {'value': 0.0001,
 #      'interpolation_method': 'eased_lerp'},
 #     49: {'value': 0.3},
```

### Comparing `keyframed-0.3.8/src/keyframed.egg-info/SOURCES.txt` & `keyframed-0.3.9/src/keyframed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/tests/test_arithmetic.py` & `keyframed-0.3.9/tests/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/tests/test_composition.py` & `keyframed-0.3.9/tests/test_composition.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/tests/test_curve.py` & `keyframed-0.3.9/tests/test_curve.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/tests/test_curve_to_dict.py` & `keyframed-0.3.9/tests/test_curve_to_dict.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/tests/test_hawkes.py` & `keyframed-0.3.9/tests/test_hawkes.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/tests/test_interpolation.py` & `keyframed-0.3.9/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/tests/test_pgroup.py` & `keyframed-0.3.9/tests/test_pgroup.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/tests/test_serialization.py` & `keyframed-0.3.9/tests/test_serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -396,8 +396,28 @@
     print(txt1)
     c2 = from_yaml(txt1)
     txt2 = to_yaml(c2, simplify=True)
     assert txt1 == txt2
 
 ###########################
 
+def test_pgroup_from_ultra_simple_yaml():
+    txt1 = """
+parameters:
+  a: 0
+  b: 1    
+  bar:
+    curve:
+    - - 0
+      - 0.3
+      - eased_lerp
+    - - 49
+      - 0.0001
+    - - 99
+      - 0.3
+    loop: true
+""".strip()
+    pg = from_yaml(txt1)
+    assert pg[1] == {'a':0,'b':1, 'bar':0.2996919116429129}
+###########################
+
 # to do: test loop and bounce serialization
```

### Comparing `keyframed-0.3.8/tests/test_sinusoid.py` & `keyframed-0.3.9/tests/test_sinusoid.py`

 * *Files identical despite different names*

### Comparing `keyframed-0.3.8/tests/test_slicing.py` & `keyframed-0.3.9/tests/test_slicing.py`

 * *Files identical despite different names*

