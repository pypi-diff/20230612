# Comparing `tmp/jinja2_async_environment-0.1.6.tar.gz` & `tmp/jinja2_async_environment-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_async_environment-0.1.6.tar", last modified: Sun Jun 11 23:02:13 2023, max compression
+gzip compressed data, was "jinja2_async_environment-0.1.7.tar", last modified: Sun Jun 11 23:37:59 2023, max compression
```

## Comparing `jinja2_async_environment-0.1.6.tar` & `jinja2_async_environment-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.1.6/LICENSE
--rw-r--r--   0        0        0      255 2023-06-11 17:54:31.705304 jinja2_async_environment-0.1.6/README.md
--rw-r--r--   0        0        0      497 2023-06-08 14:36:19.764543 jinja2_async_environment-0.1.6/jinja2_async_environment/__init__.py
--rw-r--r--   0        0        0     1395 2023-06-11 20:52:38.004790 jinja2_async_environment-0.1.6/jinja2_async_environment/bccache.py
--rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 jinja2_async_environment-0.1.6/jinja2_async_environment/compiler.py
--rw-r--r--   0        0        0     1545 2023-06-11 17:38:28.289761 jinja2_async_environment-0.1.6/jinja2_async_environment/environment.py
--rw-r--r--   0        0        0     9734 2023-06-11 21:49:07.502050 jinja2_async_environment-0.1.6/jinja2_async_environment/loaders.py
--rw-r--r--   0        0        0      963 2023-06-11 23:02:13.530593 jinja2_async_environment-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 jinja2_async_environment-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.1.7/LICENSE
+-rw-r--r--   0        0        0      255 2023-06-11 17:54:31.705304 jinja2_async_environment-0.1.7/README.md
+-rw-r--r--   0        0        0      497 2023-06-08 14:36:19.764543 jinja2_async_environment-0.1.7/jinja2_async_environment/__init__.py
+-rw-r--r--   0        0        0     1395 2023-06-11 20:52:38.004790 jinja2_async_environment-0.1.7/jinja2_async_environment/bccache.py
+-rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 jinja2_async_environment-0.1.7/jinja2_async_environment/compiler.py
+-rw-r--r--   0        0        0     1545 2023-06-11 17:38:28.289761 jinja2_async_environment-0.1.7/jinja2_async_environment/environment.py
+-rw-r--r--   0        0        0     9734 2023-06-11 21:49:07.502050 jinja2_async_environment-0.1.7/jinja2_async_environment/loaders.py
+-rw-r--r--   0        0        0      963 2023-06-11 23:37:59.612161 jinja2_async_environment-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 jinja2_async_environment-0.1.7/PKG-INFO
```

### Comparing `jinja2_async_environment-0.1.6/LICENSE` & `jinja2_async_environment-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.6/jinja2_async_environment/bccache.py` & `jinja2_async_environment-0.1.7/jinja2_async_environment/bccache.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.6/jinja2_async_environment/compiler.py` & `jinja2_async_environment-0.1.7/jinja2_async_environment/compiler.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.6/jinja2_async_environment/environment.py` & `jinja2_async_environment-0.1.7/jinja2_async_environment/environment.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.6/jinja2_async_environment/loaders.py` & `jinja2_async_environment-0.1.7/jinja2_async_environment/loaders.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.1.6/pyproject.toml` & `jinja2_async_environment-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "jinja2-async-environment"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 dependencies = [
     "jinja2>=3.1.2",
     "redis>=4.5.5",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
```

### Comparing `jinja2_async_environment-0.1.6/PKG-INFO` & `jinja2_async_environment-0.1.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-async-environment
-Version: 0.1.6
+Version: 0.1.7
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Requires-Python: >=3.11
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: redis>=4.5.5
 Description-Content-Type: text/markdown
```

