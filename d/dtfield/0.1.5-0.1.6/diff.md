# Comparing `tmp/dtfield-0.1.5.tar.gz` & `tmp/dtfield-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.1.5.tar", max compression
+gzip compressed data, was "dtfield-0.1.6.tar", max compression
```

## Comparing `dtfield-0.1.5.tar` & `dtfield-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.5/dtfield/__init__.py
--rw-r--r--   0        0        0     1918 2023-06-12 03:58:10.452251 dtfield-0.1.5/dtfield/_imports.py
--rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.5/dtfield/base_enum.py
--rw-r--r--   0        0        0    19428 2023-06-12 03:22:00.100166 dtfield-0.1.5/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.5/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.5/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.5/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.5/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.5/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.5/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.5/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.5/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.5/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11825 2023-06-11 21:21:41.254529 dtfield-0.1.5/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.5/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.5/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.5/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.5/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.5/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.5/dtfield/parse/string.py
--rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.1.5/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      387 2023-06-12 04:07:43.880730 dtfield-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      715 2023-06-12 04:07:50.737050 dtfield-0.1.5/setup.py
--rw-r--r--   0        0        0      503 2023-06-12 04:07:50.737393 dtfield-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.6/dtfield/__init__.py
+-rw-r--r--   0        0        0     1918 2023-06-12 03:58:10.452251 dtfield-0.1.6/dtfield/_imports.py
+-rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.6/dtfield/base_enum.py
+-rw-r--r--   0        0        0    19467 2023-06-12 04:58:08.747657 dtfield-0.1.6/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.6/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.6/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.6/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.6/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.6/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.6/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.6/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.6/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.6/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11825 2023-06-11 21:21:41.254529 dtfield-0.1.6/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.6/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.6/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.6/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.6/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.6/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.6/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.1.6/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      387 2023-06-12 04:58:37.467436 dtfield-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      715 2023-06-12 04:58:40.680323 dtfield-0.1.6/setup.py
+-rw-r--r--   0        0        0      503 2023-06-12 04:58:40.680547 dtfield-0.1.6/PKG-INFO
```

### Comparing `dtfield-0.1.5/dtfield/_imports.py` & `dtfield-0.1.6/dtfield/_imports.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/base_enum.py` & `dtfield-0.1.6/dtfield/base_enum.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/engine.py` & `dtfield-0.1.6/dtfield/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,16 +541,17 @@
     def validate_predicate(self, instance, value):
         if self.predicate:
             if self.predicate(value) is False:
                 raise ValueError(f'{self.name} não passou no teste de predicativo com o valor "{value}".')
     
     def validate(self, instance, value):
         self.validate_null(instance, value)
-        self.validate_type(instance, value)
-        self.validate_other(instance, value)
+        if not is_null(value):
+            self.validate_type(instance, value)
+            self.validate_other(instance, value)
 
 
 class Descriptor(BaseDescriptor):
     pass
 
 
 class Validator(BaseValidator):
```

### Comparing `dtfield-0.1.5/dtfield/functions.py` & `dtfield-0.1.6/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.1.6/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.1.6/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.1.6/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.1.6/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.1.6/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtfield-0.1.6/dtfield/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/dates.py` & `dtfield-0.1.6/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/json_encoder.py` & `dtfield-0.1.6/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/number.py` & `dtfield-0.1.6/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/string.py` & `dtfield-0.1.6/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/dtfield/parse/type_hint.py` & `dtfield-0.1.6/dtfield/parse/type_hint.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.5/setup.py` & `dtfield-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'anyio>=3.7.0,<4.0.0',
  'dtbase>=0.0.4,<0.0.5',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

