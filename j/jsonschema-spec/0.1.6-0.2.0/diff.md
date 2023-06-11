# Comparing `tmp/jsonschema_spec-0.1.6.tar.gz` & `tmp/jsonschema_spec-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_spec-0.1.6.tar", max compression
+gzip compressed data, was "jsonschema_spec-0.2.0.tar", max compression
```

## Comparing `jsonschema_spec-0.1.6.tar` & `jsonschema_spec-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/LICENSE
--rw-r--r--   0        0        0     3123 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/README.rst
--rw-r--r--   0        0        0      301 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/__init__.py
--rw-r--r--   0        0        0     1362 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/accessors.py
--rw-r--r--   0        0        0      761 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/__init__.py
--rw-r--r--   0        0        0     1557 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/file.py
--rw-r--r--   0        0        0      395 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/protocols.py
--rw-r--r--   0        0        0      747 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/requests.py
--rw-r--r--   0        0        0      587 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/urllib.py
--rw-r--r--   0        0        0      361 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/handlers/utils.py
--rw-r--r--   0        0        0     1392 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/loaders.py
--rw-r--r--   0        0        0     1559 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/paths.py
--rw-r--r--   0        0        0        0 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/py.typed
--rw-r--r--   0        0        0     1082 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/readers.py
--rw-r--r--   0        0        0      247 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/jsonschema_spec/utils.py
--rw-r--r--   0        0        0     2030 2023-06-11 08:09:37.852126 jsonschema_spec-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4384 1970-01-01 00:00:00.000000 jsonschema_spec-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3121 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/README.rst
+-rw-r--r--   0        0        0      360 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/__init__.py
+-rw-r--r--   0        0        0     2477 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/accessors.py
+-rw-r--r--   0        0        0      761 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/__init__.py
+-rw-r--r--   0        0        0     1557 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/file.py
+-rw-r--r--   0        0        0      210 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/protocols.py
+-rw-r--r--   0        0        0      747 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/requests.py
+-rw-r--r--   0        0        0      587 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/urllib.py
+-rw-r--r--   0        0        0      361 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/handlers/utils.py
+-rw-r--r--   0        0        0     1392 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/loaders.py
+-rw-r--r--   0        0        0     3271 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/paths.py
+-rw-r--r--   0        0        0        0 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/py.typed
+-rw-r--r--   0        0        0     1116 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/readers.py
+-rw-r--r--   0        0        0     1551 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/retrievers.py
+-rw-r--r--   0        0        0      148 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/typing.py
+-rw-r--r--   0        0        0      247 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/jsonschema_spec/utils.py
+-rw-r--r--   0        0        0     1897 2023-06-11 22:24:46.259956 jsonschema_spec-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 jsonschema_spec-0.2.0/PKG-INFO
```

### Comparing `jsonschema_spec-0.1.6/LICENSE` & `jsonschema_spec-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.6/README.rst` & `jsonschema_spec-0.2.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,21 @@
      :target: https://pypi.python.org/pypi/jsonschema-spec
 .. image:: https://img.shields.io/pypi/status/jsonschema-spec.svg
      :target: https://pypi.python.org/pypi/jsonschema-spec
 
 About
 #####
 
-JSONSchema Spec with object-oriented paths
+Object-oriented JSONSchema
 
 Key features
 ############
 
-* Traverse elements like paths
-* Access spec on demand with separate dereferencing accessor layer
+* Traverse schema like paths
+* Access schema on demand with separate dereferencing accessor layer
 
 Installation
 ############
 
 .. code-block:: console
 
    pip install jsonschema-spec
@@ -41,15 +41,15 @@
 
 
 Usage
 #####
 
 .. code-block:: python
 
-   >>> from jsonschema_spec import Spec
+   >>> from jsonschema_spec import SchemaPath
    
    >>> d = {
    ...     "properties": {
    ...        "info": {
    ...            "$ref": "#/$defs/Info",
    ...        },
    ...     },
@@ -64,33 +64,33 @@
    ...                     "default": "1.0",
    ...                 },
    ...             },
    ...         },
    ...     },
    ... }
    
-   >>> spec = Spec.from_dict(d)
+   >>> path = SchemaPath.from_dict(d)
    
    >>> # Stat keys
-   >>> "properties" in spec
+   >>> "properties" in path
    True
    
    >>> # Concatenate paths with /
-   >>> info_spec = spec / "properties" / "info"
+   >>> info_path = path / "properties" / "info"
    
    >>> # Stat keys with implicit dereferencing
-   >>> "properties" in info_spec
+   >>> "properties" in info_path
    True
    
    >>> # Concatenate paths with implicit dereferencing
-   >>> version_spec = info_spec / "properties" / "version"
+   >>> version_path = info_path / "properties" / "version"
    
    >>> # Open content with implicit dereferencing
-   >>> with version_spec.open() as version:
-   ...     print(version)
+   >>> with version_path.open() as contents:
+   ...     print(contents)
    {'type': 'string', 'default': '1.0'}
 
 
 Related projects
 ################
 
 * `openapi-core <https://github.com/p1c2u/openapi-core>`__
```

### Comparing `jsonschema_spec-0.1.6/jsonschema_spec/handlers/__init__.py` & `jsonschema_spec-0.2.0/jsonschema_spec/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.6/jsonschema_spec/handlers/file.py` & `jsonschema_spec-0.2.0/jsonschema_spec/handlers/file.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.6/jsonschema_spec/handlers/requests.py` & `jsonschema_spec-0.2.0/jsonschema_spec/handlers/requests.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.6/jsonschema_spec/handlers/urllib.py` & `jsonschema_spec-0.2.0/jsonschema_spec/handlers/urllib.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.6/jsonschema_spec/loaders.py` & `jsonschema_spec-0.2.0/jsonschema_spec/loaders.py`

 * *Files identical despite different names*

### Comparing `jsonschema_spec-0.1.6/pyproject.toml` & `jsonschema_spec-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,60 +10,60 @@
 output = "reports/coverage.xml"
 
 [tool.mypy]
 files = "jsonschema_spec"
 strict = true
 
 [[tool.mypy.overrides]]
-module = "jsonschema.validators"
+module = "jsonschema_specifications"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "jsonschema-spec"
-version = "0.1.6"
+version = "0.2.0"
 description = "JSONSchema Spec with object-oriented paths"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/p1c2u/jsonschema-spec"
 keywords = ["jsonschema", "swagger", "spec"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries",
 ]
 
 [tool.poetry.dependencies]
-jsonschema = ">=4.0.0,<4.18.0"
 pathable = "^0.4.1"
-python = "^3.7.0"
+python = "^3.8.0"
 PyYAML = ">=5.1"
-typing-extensions = {version = "<4.6.0", python = "<3.8"} # See https://github.com/p1c2u/jsonschema-spec/issues/14
 requests = {version = "^2.31.0", optional = true}
+referencing = "^0.24.4"
+jsonschema-specifications = "^2023.3.4"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "*"
 pytest = "^7.3.1"
 pytest-flake8 = "=1.1.0"
 pytest-cov = "^4.1.0"
 isort = "^5.0.0"
 black = "^23.3.0"
 flynt = "0.76"
 mypy = "^0.971"
 types-PyYAML = "^6.0.11"
 types-requests = "^2.28.9"
-deptry = { version = "^0.11.0", python = ">=3.8" }
+responses = "^0.23.1"
+deptry = "^0.11.0"
 
 [tool.pytest.ini_options]
 addopts = """
 --capture=no
 --verbose
 --showlocals
 --junitxml=reports/junit.xml
```

### Comparing `jsonschema_spec-0.1.6/PKG-INFO` & `jsonschema_spec-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: jsonschema-spec
-Version: 0.1.6
+Version: 0.2.0
 Summary: JSONSchema Spec with object-oriented paths
 Home-page: https://github.com/p1c2u/jsonschema-spec
 License: Apache-2.0
 Keywords: jsonschema,swagger,spec
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=5.1)
-Requires-Dist: jsonschema (>=4.0.0,<4.18.0)
+Requires-Dist: jsonschema-specifications (>=2023.3.4,<2024.0.0)
 Requires-Dist: pathable (>=0.4.1,<0.5.0)
+Requires-Dist: referencing (>=0.24.4,<0.25.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: typing-extensions (<4.6.0) ; python_version < "3.8"
 Project-URL: Repository, https://github.com/p1c2u/jsonschema-spec
 Description-Content-Type: text/x-rst
 
 ***************
 JSONSchema Spec
 ***************
 
@@ -44,21 +43,21 @@
      :target: https://pypi.python.org/pypi/jsonschema-spec
 .. image:: https://img.shields.io/pypi/status/jsonschema-spec.svg
      :target: https://pypi.python.org/pypi/jsonschema-spec
 
 About
 #####
 
-JSONSchema Spec with object-oriented paths
+Object-oriented JSONSchema
 
 Key features
 ############
 
-* Traverse elements like paths
-* Access spec on demand with separate dereferencing accessor layer
+* Traverse schema like paths
+* Access schema on demand with separate dereferencing accessor layer
 
 Installation
 ############
 
 .. code-block:: console
 
    pip install jsonschema-spec
@@ -71,15 +70,15 @@
 
 
 Usage
 #####
 
 .. code-block:: python
 
-   >>> from jsonschema_spec import Spec
+   >>> from jsonschema_spec import SchemaPath
    
    >>> d = {
    ...     "properties": {
    ...        "info": {
    ...            "$ref": "#/$defs/Info",
    ...        },
    ...     },
@@ -94,33 +93,33 @@
    ...                     "default": "1.0",
    ...                 },
    ...             },
    ...         },
    ...     },
    ... }
    
-   >>> spec = Spec.from_dict(d)
+   >>> path = SchemaPath.from_dict(d)
    
    >>> # Stat keys
-   >>> "properties" in spec
+   >>> "properties" in path
    True
    
    >>> # Concatenate paths with /
-   >>> info_spec = spec / "properties" / "info"
+   >>> info_path = path / "properties" / "info"
    
    >>> # Stat keys with implicit dereferencing
-   >>> "properties" in info_spec
+   >>> "properties" in info_path
    True
    
    >>> # Concatenate paths with implicit dereferencing
-   >>> version_spec = info_spec / "properties" / "version"
+   >>> version_path = info_path / "properties" / "version"
    
    >>> # Open content with implicit dereferencing
-   >>> with version_spec.open() as version:
-   ...     print(version)
+   >>> with version_path.open() as contents:
+   ...     print(contents)
    {'type': 'string', 'default': '1.0'}
 
 
 Related projects
 ################
 
 * `openapi-core <https://github.com/p1c2u/openapi-core>`__
```

