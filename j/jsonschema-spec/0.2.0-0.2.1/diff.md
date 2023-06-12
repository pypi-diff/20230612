# Comparing `tmp/jsonschema_spec-0.2.0.tar.gz` & `tmp/jsonschema_spec-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_spec-0.2.0.tar", max compression
+gzip compressed data, was "jsonschema_spec-0.2.1.tar", max compression
```

## Comparing `jsonschema_spec-0.2.0.tar` & `jsonschema_spec-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/LICENSE
--rw-r--r--   0        0        0     3121 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/README.rst
--rw-r--r--   0        0        0      360 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/__init__.py
--rw-r--r--   0        0        0     2477 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/accessors.py
--rw-r--r--   0        0        0      761 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/__init__.py
--rw-r--r--   0        0        0     1557 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/file.py
--rw-r--r--   0        0        0      210 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/protocols.py
--rw-r--r--   0        0        0      747 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/requests.py
--rw-r--r--   0        0        0      587 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/urllib.py
--rw-r--r--   0        0        0      361 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/utils.py
--rw-r--r--   0        0        0     1392 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/loaders.py
--rw-r--r--   0        0        0     3271 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/paths.py
--rw-r--r--   0        0        0        0 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/py.typed
--rw-r--r--   0        0        0     1116 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/readers.py
--rw-r--r--   0        0        0     1551 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/retrievers.py
--rw-r--r--   0        0        0      148 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/typing.py
--rw-r--r--   0        0        0      247 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/utils.py
--rw-r--r--   0        0        0     1897 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 jsonschema_spec-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-12 17:39:03.948618 jsonschema_spec-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3121 2023-06-12 17:39:03.948618 jsonschema_spec-0.2.1/README.rst
+-rw-r--r--   0        0        0      360 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/__init__.py
+-rw-r--r--   0        0        0     2477 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/accessors.py
+-rw-r--r--   0        0        0      761 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/__init__.py
+-rw-r--r--   0        0        0     1557 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/file.py
+-rw-r--r--   0        0        0      210 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/protocols.py
+-rw-r--r--   0        0        0      747 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/requests.py
+-rw-r--r--   0        0        0      587 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/urllib.py
+-rw-r--r--   0        0        0      361 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/handlers/utils.py
+-rw-r--r--   0        0        0     1392 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/loaders.py
+-rw-r--r--   0        0        0     3271 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/paths.py
+-rw-r--r--   0        0        0        0 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/py.typed
+-rw-r--r--   0        0        0     1116 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/readers.py
+-rw-r--r--   0        0        0     1551 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/retrievers.py
+-rw-r--r--   0        0        0      148 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/typing.py
+-rw-r--r--   0        0        0      247 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/jsonschema_spec/utils.py
+-rw-r--r--   0        0        0     1906 2023-06-12 17:39:03.952618 jsonschema_spec-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 jsonschema_spec-0.2.1/PKG-INFO
```

### Comparing `jsonschema_spec-0.2.0/LICENSE` & `jsonschema_spec-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/README.rst` & `jsonschema_spec-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/jsonschema_spec/accessors.py` & `jsonschema_spec-0.2.1/jsonschema_spec/accessors.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/jsonschema_spec/handlers/__init__.py` & `jsonschema_spec-0.2.1/jsonschema_spec/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/jsonschema_spec/handlers/file.py` & `jsonschema_spec-0.2.1/jsonschema_spec/handlers/file.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/jsonschema_spec/handlers/requests.py` & `jsonschema_spec-0.2.1/jsonschema_spec/handlers/requests.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/jsonschema_spec/handlers/urllib.py` & `jsonschema_spec-0.2.1/jsonschema_spec/handlers/urllib.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/jsonschema_spec/loaders.py` & `jsonschema_spec-0.2.1/jsonschema_spec/loaders.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/jsonschema_spec/paths.py` & `jsonschema_spec-0.2.1/jsonschema_spec/paths.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/jsonschema_spec/readers.py` & `jsonschema_spec-0.2.1/jsonschema_spec/readers.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/jsonschema_spec/retrievers.py` & `jsonschema_spec-0.2.1/jsonschema_spec/retrievers.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.2.0/pyproject.toml` & `jsonschema_spec-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [[tool.mypy.overrides]]
 module = "jsonschema_specifications"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "jsonschema-spec"
-version = "0.2.0"
+version = "0.2.1"
 description = "JSONSchema Spec with object-oriented paths"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/p1c2u/jsonschema-spec"
 keywords = ["jsonschema", "swagger", "spec"]
 classifiers = [
@@ -40,16 +40,16 @@
 ]
 
 [tool.poetry.dependencies]
 pathable = "^0.4.1"
 python = "^3.8.0"
 PyYAML = ">=5.1"
 requests = {version = "^2.31.0", optional = true}
-referencing = "^0.24.4"
-jsonschema-specifications = "^2023.3.4"
+referencing = ">=0.28.0,<0.30.0"
+jsonschema-specifications = "^2023.5.1"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "*"
 pytest = "^7.3.1"
 pytest-flake8 = "=1.1.0"
 pytest-cov = "^4.1.0"
 isort = "^5.0.0"
```

### Comparing `jsonschema_spec-0.2.0/PKG-INFO` & `jsonschema_spec-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-spec
-Version: 0.2.0
+Version: 0.2.1
 Summary: JSONSchema Spec with object-oriented paths
 Home-page: https://github.com/p1c2u/jsonschema-spec
 License: Apache-2.0
 Keywords: jsonschema,swagger,spec
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=5.1)
-Requires-Dist: jsonschema-specifications (>=2023.3.4,<2024.0.0)
+Requires-Dist: jsonschema-specifications (>=2023.5.1,<2024.0.0)
 Requires-Dist: pathable (>=0.4.1,<0.5.0)
-Requires-Dist: referencing (>=0.24.4,<0.25.0)
+Requires-Dist: referencing (>=0.28.0,<0.30.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/p1c2u/jsonschema-spec
 Description-Content-Type: text/x-rst
 
 ***************
 JSONSchema Spec
 ***************
```

