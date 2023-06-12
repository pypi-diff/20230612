# Comparing `tmp/openapi_schema_validator-0.4.4.tar.gz` & `tmp/openapi_schema_validator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_schema_validator-0.4.4.tar", max compression
+gzip compressed data, was "openapi_schema_validator-0.5.0.tar", max compression
```

## Comparing `openapi_schema_validator-0.4.4.tar` & `openapi_schema_validator-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1509 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/LICENSE
--rw-r--r--   0        0        0     4076 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/README.rst
--rw-r--r--   0        0        0      829 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/openapi_schema_validator/__init__.py
--rw-r--r--   0        0        0     1717 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/openapi_schema_validator/_format.py
--rw-r--r--   0        0        0      697 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/openapi_schema_validator/_types.py
--rw-r--r--   0        0        0     8135 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/openapi_schema_validator/_validators.py
--rw-r--r--   0        0        0        0 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/openapi_schema_validator/py.typed
--rw-r--r--   0        0        0      590 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/openapi_schema_validator/shortcuts.py
--rw-r--r--   0        0        0     5040 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/openapi_schema_validator/validators.py
--rw-r--r--   0        0        0     2167 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    26828 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/tests/integration/test_validators.py
--rw-r--r--   0        0        0      615 2023-03-17 08:33:02.124249 openapi_schema_validator-0.4.4/tests/unit/test_shortcut.py
--rw-r--r--   0        0        0     5666 1970-01-01 00:00:00.000000 openapi_schema_validator-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1509 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4076 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/README.rst
+-rw-r--r--   0        0        0      829 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/__init__.py
+-rw-r--r--   0        0        0     2483 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/_format.py
+-rw-r--r--   0        0        0      697 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/_types.py
+-rw-r--r--   0        0        0     8135 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/_validators.py
+-rw-r--r--   0        0        0        0 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/py.typed
+-rw-r--r--   0        0        0      590 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/shortcuts.py
+-rw-r--r--   0        0        0     5040 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/validators.py
+-rw-r--r--   0        0        0     2211 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    28846 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/tests/integration/test_validators.py
+-rw-r--r--   0        0        0      615 2023-06-12 09:36:24.513618 openapi_schema_validator-0.5.0/tests/unit/test_shortcut.py
+-rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 openapi_schema_validator-0.5.0/PKG-INFO
```

### Comparing `openapi_schema_validator-0.4.4/LICENSE` & `openapi_schema_validator-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.4.4/README.rst` & `openapi_schema_validator-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.4.4/openapi_schema_validator/__init__.py` & `openapi_schema_validator-0.5.0/openapi_schema_validator/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from openapi_schema_validator.validators import OAS30ReadValidator
 from openapi_schema_validator.validators import OAS30Validator
 from openapi_schema_validator.validators import OAS30WriteValidator
 from openapi_schema_validator.validators import OAS31Validator
 
 __author__ = "Artur Maciag"
 __email__ = "maciag.artur@gmail.com"
-__version__ = "0.4.4"
+__version__ = "0.5.0"
 __url__ = "https://github.com/python-openapi/openapi-schema-validator"
 __license__ = "3-clause BSD License"
 
 __all__ = [
     "validate",
     "OAS30ReadValidator",
     "OAS30WriteValidator",
```

### Comparing `openapi_schema_validator-0.4.4/openapi_schema_validator/_types.py` & `openapi_schema_validator-0.5.0/openapi_schema_validator/_types.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.4.4/openapi_schema_validator/_validators.py` & `openapi_schema_validator-0.5.0/openapi_schema_validator/_validators.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.4.4/openapi_schema_validator/shortcuts.py` & `openapi_schema_validator-0.5.0/openapi_schema_validator/shortcuts.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.4.4/openapi_schema_validator/validators.py` & `openapi_schema_validator-0.5.0/openapi_schema_validator/validators.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.4.4/pyproject.toml` & `openapi_schema_validator-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 [tool.coverage.run]
 branch = true
 source =["openapi_schema_validator"]
 
 [tool.coverage.xml]
 output = "reports/coverage.xml"
 
+[tool.deptry]
+ignore_unused = ["rfc3339-validator"]
+
 [tool.mypy]
 files = "openapi_schema_validator"
 strict = true
 
 [[tool.mypy.overrides]]
 module = "jsonschema.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "rfc3339_validator"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "openapi-schema-validator"
-version = "0.4.4"
+version = "0.5.0"
 description = "OpenAPI schema validation for Python"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 repository = "https://github.com/python-openapi/openapi-schema-validator"
 keywords = ["openapi", "swagger", "schema"]
 classifiers = [
@@ -46,30 +49,29 @@
 include = [
     {path = "tests", format = "sdist"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
 jsonschema = ">=4.0.0,<4.18.0"
-rfc3339-validator = "*"
-sphinx = {version = "^5.3.0", optional = true}
-sphinx-immaterial = {version = "^0.11.0", optional = true}
+rfc3339-validator = "*" # requred by jsonschema for date-time checker
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-immaterial"]
 
 [tool.poetry.dev-dependencies]
-black = "^22.0.0"
+black = "^23.3.0"
 isort = "^5.9.1"
 pre-commit = "*"
-pytest = "^6"
+pytest = "^7"
 pytest-flake8 = "*"
 pytest-cov = "*"
 mypy = "^0.910"
-flynt = "^0.76"
+flynt = "^0.78"
+deptry = { version = "^0.11.0", python = ">=3.8" }
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.3.0"
 sphinx-immaterial = "^0.11.0"
 
 [tool.pytest.ini_options]
 addopts = """
```

### Comparing `openapi_schema_validator-0.4.4/tests/integration/test_validators.py` & `openapi_schema_validator-0.5.0/tests/integration/test_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,61 @@
         }
         assert required_formats_set.issubset(
             set(format_checker.checkers.keys())
         )
 
 
 class BaseTestOASValidatorValidate:
+    @pytest.mark.parametrize(
+        "format,value",
+        [
+            ("int32", "test"),
+            ("int32", True),
+            ("int32", 3.12),
+            ("int32", ["test"]),
+            ("int64", "test"),
+            ("int64", True),
+            ("int64", 3.12),
+            ("int64", ["test"]),
+            ("float", "test"),
+            ("float", 3),
+            ("float", True),
+            ("float", ["test"]),
+            ("double", "test"),
+            ("double", 3),
+            ("double", True),
+            ("double", ["test"]),
+            ("password", 3.12),
+            ("password", True),
+            ("password", 3),
+            ("password", ["test"]),
+        ],
+    )
+    def test_formats_ignored(
+        self, format, value, validator_class, format_checker
+    ):
+        schema = {"format": format}
+        validator = validator_class(schema, format_checker=format_checker)
+
+        result = validator.validate(value)
+
+        assert result is None
+
+    @pytest.mark.parametrize("format", ["float", "double"])
+    @pytest.mark.parametrize("value", [3, 3.14, 1.0])
+    def test_number_float_and_double_valid(
+        self, format, value, validator_class, format_checker
+    ):
+        schema = {"type": "number", "format": format}
+        validator = validator_class(schema, format_checker=format_checker)
+
+        result = validator.validate(value)
+
+        assert result is None
+
     @pytest.mark.parametrize("value", ["test"])
     def test_string(self, validator_class, value):
         schema = {"type": "string"}
         validator = validator_class(schema)
 
         result = validator.validate(value)
 
@@ -57,14 +104,37 @@
     def validator_class(self):
         return OAS30Validator
 
     @pytest.fixture
     def format_checker(self):
         return oas30_format_checker
 
+    @pytest.mark.parametrize(
+        "format,value",
+        [
+            ("binary", True),
+            ("binary", 3),
+            ("binary", 3.12),
+            ("binary", ["test"]),
+            ("byte", True),
+            ("byte", 3),
+            ("byte", 3.12),
+            ("byte", ["test"]),
+        ],
+    )
+    def test_oas30_formats_ignored(
+        self, format, value, validator_class, format_checker
+    ):
+        schema = {"format": format}
+        validator = validator_class(schema, format_checker=format_checker)
+
+        result = validator.validate(value)
+
+        assert result is None
+
     @pytest.mark.xfail(reason="OAS 3.0 string type checker allows byte")
     @pytest.mark.parametrize("value", [b"test"])
     def test_string_disallow_binary(self, validator_class, value):
         schema = {"type": "string"}
         validator = validator_class(schema)
 
         with pytest.raises(ValidationError):
```

### Comparing `openapi_schema_validator-0.4.4/tests/unit/test_shortcut.py` & `openapi_schema_validator-0.5.0/tests/unit/test_shortcut.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.4.4/PKG-INFO` & `openapi_schema_validator-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-schema-validator
-Version: 0.4.4
+Version: 0.5.0
 Summary: OpenAPI schema validation for Python
 Home-page: https://github.com/python-openapi/openapi-schema-validator
 License: BSD-3-Clause
 Keywords: openapi,swagger,schema
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -14,27 +14,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Requires-Dist: jsonschema (>=4.0.0,<4.18.0)
 Requires-Dist: rfc3339-validator
-Requires-Dist: sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
-Requires-Dist: sphinx-immaterial (>=0.11.0,<0.12.0) ; extra == "docs"
 Project-URL: Repository, https://github.com/python-openapi/openapi-schema-validator
 Description-Content-Type: text/x-rst
 
 ************************
 openapi-schema-validator
 ************************
```

