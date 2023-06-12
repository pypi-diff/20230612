# Comparing `tmp/dtfield-0.1.0.tar.gz` & `tmp/dtfield-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.1.0.tar", max compression
+gzip compressed data, was "dtfield-0.1.1.tar", max compression
```

## Comparing `dtfield-0.1.0.tar` & `dtfield-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       91 2023-06-11 22:49:23.831378 dtfield-0.1.0/dtfield/__init__.py
--rw-r--r--   0        0        0     1888 2023-06-12 01:48:15.527391 dtfield-0.1.0/dtfield/_imports.py
--rw-r--r--   0        0        0     1094 2023-06-11 22:23:16.619926 dtfield-0.1.0/dtfield/base_enum.py
--rw-r--r--   0        0        0    19429 2023-06-12 02:42:22.853221 dtfield-0.1.0/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.0/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.0/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.0/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.0/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.0/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.0/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.0/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.0/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.0/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11825 2023-06-11 21:21:41.254529 dtfield-0.1.0/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.0/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.0/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.0/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.0/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.0/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.0/dtfield/parse/string.py
--rw-r--r--   0        0        0    10904 2023-06-11 21:21:40.293530 dtfield-0.1.0/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      387 2023-06-12 00:13:48.708220 dtfield-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      715 2023-06-12 03:06:17.353448 dtfield-0.1.0/setup.py
--rw-r--r--   0        0        0      503 2023-06-12 03:06:17.353823 dtfield-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2023-06-11 22:49:23.831378 dtfield-0.1.1/dtfield/__init__.py
+-rw-r--r--   0        0        0     1888 2023-06-12 01:48:15.527391 dtfield-0.1.1/dtfield/_imports.py
+-rw-r--r--   0        0        0     1094 2023-06-11 22:23:16.619926 dtfield-0.1.1/dtfield/base_enum.py
+-rw-r--r--   0        0        0    19428 2023-06-12 03:22:00.100166 dtfield-0.1.1/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.1/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.1/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.1/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.1/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.1/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.1/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.1/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.1/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.1/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11825 2023-06-11 21:21:41.254529 dtfield-0.1.1/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.1/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.1/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.1/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.1/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.1/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.1/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10904 2023-06-11 21:21:40.293530 dtfield-0.1.1/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      387 2023-06-12 03:22:10.729165 dtfield-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      715 2023-06-12 03:22:19.443166 dtfield-0.1.1/setup.py
+-rw-r--r--   0        0        0      503 2023-06-12 03:22:19.443372 dtfield-0.1.1/PKG-INFO
```

### Comparing `dtfield-0.1.0/dtfield/_imports.py` & `dtfield-0.1.1/dtfield/_imports.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/base_enum.py` & `dtfield-0.1.1/dtfield/base_enum.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/engine.py` & `dtfield-0.1.1/dtfield/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,11 +549,11 @@
         self.validate_other(instance, value)
 
 
 class Descriptor(BaseDescriptor):
     pass
 
 
-class Validator(BaseDescriptor):
+class Validator(BaseValidator):
     pass
```

### Comparing `dtfield-0.1.0/dtfield/functions.py` & `dtfield-0.1.1/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.1.1/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.1.1/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.1.1/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.1.1/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.1.1/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtfield-0.1.1/dtfield/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/dates.py` & `dtfield-0.1.1/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/json_encoder.py` & `dtfield-0.1.1/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/number.py` & `dtfield-0.1.1/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/string.py` & `dtfield-0.1.1/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/dtfield/parse/type_hint.py` & `dtfield-0.1.1/dtfield/parse/type_hint.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.0/setup.py` & `dtfield-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'anyio>=3.7.0,<4.0.0',
  'dtbase>=0.0.4,<0.0.5',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

