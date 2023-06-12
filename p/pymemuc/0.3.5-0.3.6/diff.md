# Comparing `tmp/pymemuc-0.3.5.tar.gz` & `tmp/pymemuc-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.3.5.tar", max compression
+gzip compressed data, was "pymemuc-0.3.6.tar", max compression
```

## Comparing `pymemuc-0.3.5.tar` & `pymemuc-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-06-08 18:30:14.192958 pymemuc-0.3.5/LICENSE
--rw-r--r--   0        0        0     1586 2023-06-08 18:30:14.192958 pymemuc-0.3.5/README.md
--rw-r--r--   0        0        0      386 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/__init__.py
--rw-r--r--   0        0        0    22761 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_constants.py
--rw-r--r--   0        0        0     4984 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_control.py
--rw-r--r--   0        0        0     1214 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_decorators.py
--rw-r--r--   0        0        0    13670 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_manage.py
--rw-r--r--   0        0        0     4134 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2899 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1665 2023-06-08 18:30:40.189348 pymemuc-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-06-12 04:30:57.265317 pymemuc-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1586 2023-06-12 04:30:57.265317 pymemuc-0.3.6/README.md
+-rw-r--r--   0        0        0      386 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/__init__.py
+-rw-r--r--   0        0        0    22761 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_constants.py
+-rw-r--r--   0        0        0     4984 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_control.py
+-rw-r--r--   0        0        0     1214 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    13670 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_manage.py
+-rw-r--r--   0        0        0     4134 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2941 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-06-12 04:30:57.269317 pymemuc-0.3.6/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-06-12 04:31:16.737548 pymemuc-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.6/PKG-INFO
```

### Comparing `pymemuc-0.3.5/LICENSE` & `pymemuc-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.5/README.md` & `pymemuc-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.5/pymemuc/_command.py` & `pymemuc-0.3.6/pymemuc/_command.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.5/pymemuc/_control.py` & `pymemuc-0.3.6/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.5/pymemuc/_decorators.py` & `pymemuc-0.3.6/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.5/pymemuc/_manage.py` & `pymemuc-0.3.6/pymemuc/_manage.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.5/pymemuc/_memuc.py` & `pymemuc-0.3.6/pymemuc/_memuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.5/pymemuc/exceptions.py` & `pymemuc-0.3.6/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.5/pymemuc/pymemuc.py` & `pymemuc-0.3.6/pymemuc/pymemuc.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     def _configure_logger(self):
         """Configure the logger for the class"""
         logger = logging.getLogger(__name__)
         logger.setLevel(logging.DEBUG if self.debug else logging.INFO)
 
         # Create a handler for console output
         console_handler = logging.StreamHandler()
+        console_handler.propagate = False
         console_handler.setLevel(logging.DEBUG)
         formatter = logging.Formatter(
             "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
         )
         console_handler.setFormatter(formatter)
 
         # Add the handler to the logger
```

### Comparing `pymemuc-0.3.5/pyproject.toml` & `pymemuc-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.3.5"
+version = "v0.3.6"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.3.5/PKG-INFO` & `pymemuc-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```

