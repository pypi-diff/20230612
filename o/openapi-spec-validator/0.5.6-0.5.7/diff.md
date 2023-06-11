# Comparing `tmp/openapi_spec_validator-0.5.6.tar.gz` & `tmp/openapi_spec_validator-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_spec_validator-0.5.6.tar", max compression
+gzip compressed data, was "openapi_spec_validator-0.5.7.tar", max compression
```

## Comparing `openapi_spec_validator-0.5.6.tar` & `openapi_spec_validator-0.5.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/LICENSE
--rw-r--r--   0        0        0     3745 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/README.rst
--rw-r--r--   0        0        0      845 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/__init__.py
--rw-r--r--   0        0        0     3041 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/__main__.py
--rw-r--r--   0        0        0       53 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/py.typed
--rw-r--r--   0        0        0      670 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/readers.py
--rw-r--r--   0        0        0    40203 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/resources/schemas/v2.0/schema.json
--rw-r--r--   0        0        0    35440 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/resources/schemas/v3.0/schema.json
--rw-r--r--   0        0        0    37211 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/resources/schemas/v3.0.0/schema.json
--rw-r--r--   0        0        0    30377 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/resources/schemas/v3.1/schema.json
--rw-r--r--   0        0        0      612 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/schemas/__init__.py
--rw-r--r--   0        0        0      924 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/schemas/utils.py
--rw-r--r--   0        0        0      756 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/shortcuts.py
--rw-r--r--   0        0        0     2523 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/validation/__init__.py
--rw-r--r--   0        0        0      922 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/validation/decorators.py
--rw-r--r--   0        0        0      529 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/validation/exceptions.py
--rw-r--r--   0        0        0      829 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/validation/protocols.py
--rw-r--r--   0        0        0     1537 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/validation/proxies.py
--rw-r--r--   0        0        0    11732 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/openapi_spec_validator/validation/validators.py
--rw-r--r--   0        0        0     2619 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     1401 2023-03-17 08:40:24.299854 openapi_spec_validator-0.5.6/tests/integration/conftest.py
--rw-r--r--   0        0        0        2 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/empty.yaml
--rw-r--r--   0        0        0       14 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v2.0/empty.yaml
--rw-r--r--   0        0        0     2137 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v2.0/missing-reference.yaml
--rw-r--r--   0        0        0     2145 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v2.0/petstore.yaml
--rw-r--r--   0        0        0       16 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/empty.yaml
--rw-r--r--   0        0        0      267 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/missing-description.yaml
--rw-r--r--   0        0        0      306 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/parent-reference/common.yaml
--rw-r--r--   0        0        0      938 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/parent-reference/openapi.yaml
--rw-r--r--   0        0        0       94 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/parent-reference/recursive.yaml
--rw-r--r--   0        0        0      159 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/parent-reference/recursive2.yaml
--rw-r--r--   0        0        0      198 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/parent-reference/spec/components.yaml
--rw-r--r--   0        0        0      127 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/petstore-separate/common/schemas/Error.yaml
--rw-r--r--   0        0        0     2037 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml
--rw-r--r--   0        0        0      128 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pet.yaml
--rw-r--r--   0        0        0       37 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pets.yaml
--rw-r--r--   0        0        0     2571 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/petstore.yaml
--rw-r--r--   0        0        0      279 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/property-missing-reference.yaml
--rw-r--r--   0        0        0      295 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.0/property-recursive.yaml
--rw-r--r--   0        0        0     2599 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/data/v3.1/petstore.yaml
--rw-r--r--   0        0        0     3576 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/test_main.py
--rw-r--r--   0        0        0     4647 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/test_shortcuts.py
--rw-r--r--   0        0        0    16360 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/validation/test_exceptions.py
--rw-r--r--   0        0        0     5867 2023-03-17 08:40:24.303854 openapi_spec_validator-0.5.6/tests/integration/validation/test_validators.py
--rw-r--r--   0        0        0     5647 1970-01-01 00:00:00.000000 openapi_spec_validator-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/LICENSE
+-rw-r--r--   0        0        0     3936 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/README.rst
+-rw-r--r--   0        0        0      845 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/__init__.py
+-rw-r--r--   0        0        0     3041 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/__main__.py
+-rw-r--r--   0        0        0       53 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/py.typed
+-rw-r--r--   0        0        0      670 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/readers.py
+-rw-r--r--   0        0        0    40203 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v2.0/schema.json
+-rw-r--r--   0        0        0    35816 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.0/schema.json
+-rw-r--r--   0        0        0    37211 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.0.0/schema.json
+-rw-r--r--   0        0        0    34260 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.1/schema.json
+-rw-r--r--   0        0        0      612 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/schemas/utils.py
+-rw-r--r--   0        0        0      756 2023-06-11 23:13:13.965076 openapi_spec_validator-0.5.7/openapi_spec_validator/shortcuts.py
+-rw-r--r--   0        0        0     2523 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/__init__.py
+-rw-r--r--   0        0        0      922 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/decorators.py
+-rw-r--r--   0        0        0      529 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/exceptions.py
+-rw-r--r--   0        0        0      796 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/protocols.py
+-rw-r--r--   0        0        0     1537 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/proxies.py
+-rw-r--r--   0        0        0    11732 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/openapi_spec_validator/validation/validators.py
+-rw-r--r--   0        0        0     2577 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1401 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/conftest.py
+-rw-r--r--   0        0        0        2 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/empty.yaml
+-rw-r--r--   0        0        0       14 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v2.0/empty.yaml
+-rw-r--r--   0        0        0     2137 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v2.0/missing-reference.yaml
+-rw-r--r--   0        0        0     2145 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v2.0/petstore.yaml
+-rw-r--r--   0        0        0       16 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/empty.yaml
+-rw-r--r--   0        0        0      267 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/missing-description.yaml
+-rw-r--r--   0        0        0      306 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/common.yaml
+-rw-r--r--   0        0        0      938 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/openapi.yaml
+-rw-r--r--   0        0        0       94 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/recursive.yaml
+-rw-r--r--   0        0        0      159 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/recursive2.yaml
+-rw-r--r--   0        0        0      198 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/spec/components.yaml
+-rw-r--r--   0        0        0      127 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/common/schemas/Error.yaml
+-rw-r--r--   0        0        0     2037 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml
+-rw-r--r--   0        0        0      128 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pet.yaml
+-rw-r--r--   0        0        0       37 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/spec/schemas/Pets.yaml
+-rw-r--r--   0        0        0     2571 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore.yaml
+-rw-r--r--   0        0        0      279 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/property-missing-reference.yaml
+-rw-r--r--   0        0        0      295 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.0/property-recursive.yaml
+-rw-r--r--   0        0        0     2718 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/data/v3.1/petstore.yaml
+-rw-r--r--   0        0        0     3576 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/test_main.py
+-rw-r--r--   0        0        0     4647 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/test_shortcuts.py
+-rw-r--r--   0        0        0    16360 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/validation/test_exceptions.py
+-rw-r--r--   0        0        0     5867 2023-06-11 23:13:13.969076 openapi_spec_validator-0.5.7/tests/integration/validation/test_validators.py
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 openapi_spec_validator-0.5.7/PKG-INFO
```

### Comparing `openapi_spec_validator-0.5.6/LICENSE` & `openapi_spec_validator-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/README.rst` & `openapi_spec_validator-0.5.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 **********************
 OpenAPI Spec validator
 **********************
 
+.. image:: https://img.shields.io/docker/v/p1c2u/openapi-spec-validator.svg?color=%23086DD7&label=docker%20hub&sort=semver
+     :target: https://hub.docker.com/r/p1c2u/openapi-spec-validator
 .. image:: https://img.shields.io/pypi/v/openapi-spec-validator.svg
      :target: https://pypi.python.org/pypi/openapi-spec-validator
 .. image:: https://travis-ci.org/python-openapi/openapi-spec-validator.svg?branch=master
      :target: https://travis-ci.org/python-openapi/openapi-spec-validator
 .. image:: https://img.shields.io/codecov/c/github/python-openapi/openapi-spec-validator/master.svg?style=flat
      :target: https://codecov.io/github/python-openapi/openapi-spec-validator?branch=master
 .. image:: https://img.shields.io/pypi/pyversions/openapi-spec-validator.svg
```

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/__init__.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from openapi_spec_validator.validation import openapi_v2_spec_validator
 from openapi_spec_validator.validation import openapi_v3_spec_validator
 from openapi_spec_validator.validation import openapi_v30_spec_validator
 from openapi_spec_validator.validation import openapi_v31_spec_validator
 
 __author__ = "Artur Maciag"
 __email__ = "maciag.artur@gmail.com"
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 __url__ = "https://github.com/python-openapi/openapi-spec-validator"
 __license__ = "Apache License, Version 2.0"
 
 __all__ = [
     "openapi_v2_spec_validator",
     "openapi_v3_spec_validator",
     "openapi_v30_spec_validator",
```

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/__main__.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/readers.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/readers.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/resources/schemas/v2.0/schema.json` & `openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/resources/schemas/v3.0/schema.json` & `openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.0/schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7497478187321938%*

 * *Differences: {"'definitions'": "{'HTTPSecurityScheme': {'oneOf': {0: {'properties': {'scheme': {replace: "*

 * *                  "OrderedDict([('type', 'string'), ('pattern', "*

 * *                  "'^[Bb][Ee][Aa][Rr][Ee][Rr]$')])}}}, 1: {'properties': {'scheme': {'not': "*

 * *                  "{replace: OrderedDict([('type', 'string'), ('pattern', "*

 * *                  "'^[Bb][Ee][Aa][Rr][Ee][Rr]$')])}}}}}}, 'PasswordOAuthFlow': {'required': "*

 * *                  "{insert: [(1, 'scopes')]}}, 'ClientCredentialsFlow': {'required': {in […]*

```diff
@@ -59,15 +59,16 @@
                 "tokenUrl": {
                     "format": "uri-reference",
                     "type": "string"
                 }
             },
             "required": [
                 "authorizationUrl",
-                "tokenUrl"
+                "tokenUrl",
+                "scopes"
             ],
             "type": "object"
         },
         "Callback": {
             "additionalProperties": {
                 "$ref": "#/definitions/PathItem"
             },
@@ -94,15 +95,16 @@
                 },
                 "tokenUrl": {
                     "format": "uri-reference",
                     "type": "string"
                 }
             },
             "required": [
-                "tokenUrl"
+                "tokenUrl",
+                "scopes"
             ],
             "type": "object"
         },
         "Components": {
             "additionalProperties": false,
             "patternProperties": {
                 "^x-": {}
@@ -281,28 +283,38 @@
             "required": [
                 "propertyName"
             ],
             "type": "object"
         },
         "Encoding": {
             "additionalProperties": false,
+            "patternProperties": {
+                "^x-": {}
+            },
             "properties": {
                 "allowReserved": {
                     "default": false,
                     "type": "boolean"
                 },
                 "contentType": {
                     "type": "string"
                 },
                 "explode": {
                     "type": "boolean"
                 },
                 "headers": {
                     "additionalProperties": {
-                        "$ref": "#/definitions/Header"
+                        "oneOf": [
+                            {
+                                "$ref": "#/definitions/Header"
+                            },
+                            {
+                                "$ref": "#/definitions/Reference"
+                            }
+                        ]
                     },
                     "type": "object"
                 },
                 "style": {
                     "enum": [
                         "form",
                         "spaceDelimited",
@@ -365,33 +377,31 @@
         "HTTPSecurityScheme": {
             "additionalProperties": false,
             "oneOf": [
                 {
                     "description": "Bearer",
                     "properties": {
                         "scheme": {
-                            "enum": [
-                                "bearer"
-                            ]
+                            "pattern": "^[Bb][Ee][Aa][Rr][Ee][Rr]$",
+                            "type": "string"
                         }
                     }
                 },
                 {
                     "description": "Non Bearer",
                     "not": {
                         "required": [
                             "bearerFormat"
                         ]
                     },
                     "properties": {
                         "scheme": {
                             "not": {
-                                "enum": [
-                                    "bearer"
-                                ]
+                                "pattern": "^[Bb][Ee][Aa][Rr][Ee][Rr]$",
+                                "type": "string"
                             }
                         }
                     }
                 }
             ],
             "patternProperties": {
                 "^x-": {}
@@ -998,15 +1008,16 @@
                 },
                 "tokenUrl": {
                     "format": "uri-reference",
                     "type": "string"
                 }
             },
             "required": [
-                "tokenUrl"
+                "tokenUrl",
+                "scopes"
             ],
             "type": "object"
         },
         "PathItem": {
             "additionalProperties": false,
             "patternProperties": {
                 "^(get|put|post|delete|options|head|patch|trace)$": {
@@ -1558,15 +1569,16 @@
                     "default": false,
                     "type": "boolean"
                 }
             },
             "type": "object"
         }
     },
-    "description": "Validation schema for OpenAPI Specification 3.0.X.",
+    "description": "The description of OpenAPI v3.0.x documents, as defined by https://spec.openapis.org/oas/v3.0.3",
+    "id": "https://spec.openapis.org/oas/3.0/schema/2021-09-28",
     "patternProperties": {
         "^x-": {}
     },
     "properties": {
         "components": {
             "$ref": "#/definitions/Components"
         },
@@ -1604,10 +1616,9 @@
         }
     },
     "required": [
         "openapi",
         "info",
         "paths"
     ],
-    "title": "A JSON Schema for OpenAPI 3.0.X.",
     "type": "object"
 }
```

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/resources/schemas/v3.0.0/schema.json` & `openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.0.0/schema.json`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/resources/schemas/v3.1/schema.json` & `openapi_spec_validator-0.5.7/openapi_spec_validator/resources/schemas/v3.1/schema.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8442811522245115%*

 * *Differences: {"'$defs'": "{'info': {'properties': {'termsOfService': {'format': 'uri'}}, '$comment': "*

 * *            "'https://spec.openapis.org/oas/v3.1.0#info-object'}, 'contact': {'properties': "*

 * *            "{'url': {'format': 'uri'}, 'email': {'format': 'email'}}, '$comment': "*

 * *            "'https://spec.openapis.org/oas/v3.1.0#contact-object'}, 'license': {'$comment': "*

 * *            "'https://spec.openapis.org/oas/v3.1.0#license-object', 'dependentSchemas': "*

 * *            "OrderedDict([('identifier', OrderedDict([('no […]*

```diff
@@ -1,30 +1,33 @@
 {
     "$defs": {
         "callbacks": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#callback-object",
             "$ref": "#/$defs/specification-extensions",
             "additionalProperties": {
                 "$ref": "#/$defs/path-item-or-reference"
             },
             "type": "object"
         },
         "callbacks-or-reference": {
             "else": {
                 "$ref": "#/$defs/callbacks"
             },
             "if": {
                 "required": [
                     "$ref"
-                ]
+                ],
+                "type": "object"
             },
             "then": {
                 "$ref": "#/$defs/reference"
             }
         },
         "components": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#components-object",
             "$ref": "#/$defs/specification-extensions",
             "patternProperties": {
                 "^(schemas|responses|parameters|examples|requestBodies|headers|securitySchemes|links|callbacks|pathItems)$": {
                     "$comment": "Enumerating all of the property names in the regex above is necessary for unevaluatedProperties to work as expected",
                     "propertyNames": {
                         "pattern": "^[a-zA-Z0-9._-]+$"
                     }
@@ -92,39 +95,44 @@
                     "type": "object"
                 }
             },
             "type": "object",
             "unevaluatedProperties": false
         },
         "contact": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#contact-object",
             "$ref": "#/$defs/specification-extensions",
             "properties": {
                 "email": {
+                    "format": "email",
                     "type": "string"
                 },
                 "name": {
                     "type": "string"
                 },
                 "url": {
+                    "format": "uri",
                     "type": "string"
                 }
             },
             "type": "object",
             "unevaluatedProperties": false
         },
         "content": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#fixed-fields-10",
             "additionalProperties": {
                 "$ref": "#/$defs/media-type"
             },
             "propertyNames": {
                 "format": "media-range"
             },
             "type": "object"
         },
         "encoding": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#encoding-object",
             "$defs": {
                 "explode-default": {
                     "else": {
                         "properties": {
                             "explode": {
                                 "default": false
                             }
@@ -185,15 +193,22 @@
                     ]
                 }
             },
             "type": "object",
             "unevaluatedProperties": false
         },
         "example": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#example-object",
             "$ref": "#/$defs/specification-extensions",
+            "not": {
+                "required": [
+                    "value",
+                    "externalValue"
+                ]
+            },
             "properties": {
                 "description": {
                     "type": "string"
                 },
                 "externalValue": {
                     "format": "uri",
                     "type": "string"
@@ -209,15 +224,16 @@
         "example-or-reference": {
             "else": {
                 "$ref": "#/$defs/example"
             },
             "if": {
                 "required": [
                     "$ref"
-                ]
+                ],
+                "type": "object"
             },
             "then": {
                 "$ref": "#/$defs/reference"
             }
         },
         "examples": {
             "properties": {
@@ -227,14 +243,15 @@
                         "$ref": "#/$defs/example-or-reference"
                     },
                     "type": "object"
                 }
             }
         },
         "external-documentation": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#external-documentation-object",
             "$ref": "#/$defs/specification-extensions",
             "properties": {
                 "description": {
                     "type": "string"
                 },
                 "url": {
                     "format": "uri",
@@ -244,80 +261,83 @@
             "required": [
                 "url"
             ],
             "type": "object",
             "unevaluatedProperties": false
         },
         "header": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#header-object",
             "$ref": "#/$defs/specification-extensions",
             "dependentSchemas": {
-                "content": {
-                    "properties": {
-                        "content": {
-                            "$ref": "#/$defs/content"
-                        }
-                    }
-                },
                 "schema": {
                     "$ref": "#/$defs/examples",
                     "properties": {
-                        "allowReserved": {
-                            "default": false,
-                            "type": "boolean"
-                        },
                         "explode": {
                             "default": false,
                             "type": "boolean"
                         },
-                        "schema": {
-                            "$dynamicRef": "#meta"
-                        },
                         "style": {
-                            "default": "simple",
-                            "enum": [
-                                "simple"
-                            ]
+                            "const": "simple",
+                            "default": "simple"
                         }
                     }
                 }
             },
+            "oneOf": [
+                {
+                    "required": [
+                        "schema"
+                    ]
+                },
+                {
+                    "required": [
+                        "content"
+                    ]
+                }
+            ],
             "properties": {
-                "allowEmptyValue": {
-                    "default": false,
-                    "type": "boolean"
+                "content": {
+                    "$ref": "#/$defs/content",
+                    "maxProperties": 1,
+                    "minProperties": 1
                 },
                 "deprecated": {
                     "default": false,
                     "type": "boolean"
                 },
                 "description": {
                     "type": "string"
                 },
                 "required": {
                     "default": false,
                     "type": "boolean"
+                },
+                "schema": {
+                    "$dynamicRef": "#meta"
                 }
             },
             "type": "object",
             "unevaluatedProperties": false
         },
         "header-or-reference": {
             "else": {
                 "$ref": "#/$defs/header"
             },
             "if": {
                 "required": [
                     "$ref"
-                ]
+                ],
+                "type": "object"
             },
             "then": {
                 "$ref": "#/$defs/reference"
             }
         },
         "info": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#info-object",
             "$ref": "#/$defs/specification-extensions",
             "properties": {
                 "contact": {
                     "$ref": "#/$defs/contact"
                 },
                 "description": {
                     "type": "string"
@@ -325,14 +345,15 @@
                 "license": {
                     "$ref": "#/$defs/license"
                 },
                 "summary": {
                     "type": "string"
                 },
                 "termsOfService": {
+                    "format": "uri",
                     "type": "string"
                 },
                 "title": {
                     "type": "string"
                 },
                 "version": {
                     "type": "string"
@@ -342,27 +363,25 @@
                 "title",
                 "version"
             ],
             "type": "object",
             "unevaluatedProperties": false
         },
         "license": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#license-object",
             "$ref": "#/$defs/specification-extensions",
-            "oneOf": [
-                {
-                    "required": [
-                        "identifier"
-                    ]
-                },
-                {
-                    "required": [
-                        "url"
-                    ]
+            "dependentSchemas": {
+                "identifier": {
+                    "not": {
+                        "required": [
+                            "url"
+                        ]
+                    }
                 }
-            ],
+            },
             "properties": {
                 "identifier": {
                     "type": "string"
                 },
                 "name": {
                     "type": "string"
                 },
@@ -374,14 +393,15 @@
             "required": [
                 "name"
             ],
             "type": "object",
             "unevaluatedProperties": false
         },
         "link": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#link-object",
             "$ref": "#/$defs/specification-extensions",
             "oneOf": [
                 {
                     "required": [
                         "operationRef"
                     ]
                 },
@@ -394,15 +414,17 @@
             "properties": {
                 "body": {
                     "$ref": "#/$defs/server"
                 },
                 "description": {
                     "type": "string"
                 },
-                "operationId": true,
+                "operationId": {
+                    "type": "string"
+                },
                 "operationRef": {
                     "format": "uri-reference",
                     "type": "string"
                 },
                 "parameters": {
                     "$ref": "#/$defs/map-of-strings"
                 },
@@ -414,27 +436,29 @@
         "link-or-reference": {
             "else": {
                 "$ref": "#/$defs/link"
             },
             "if": {
                 "required": [
                     "$ref"
-                ]
+                ],
+                "type": "object"
             },
             "then": {
                 "$ref": "#/$defs/reference"
             }
         },
         "map-of-strings": {
             "additionalProperties": {
                 "type": "string"
             },
             "type": "object"
         },
         "media-type": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#media-type-object",
             "allOf": [
                 {
                     "$ref": "#/$defs/specification-extensions"
                 },
                 {
                     "$ref": "#/$defs/examples"
                 }
@@ -455,23 +479,26 @@
         },
         "oauth-flows": {
             "$defs": {
                 "authorization-code": {
                     "$ref": "#/$defs/specification-extensions",
                     "properties": {
                         "authorizationUrl": {
+                            "format": "uri",
                             "type": "string"
                         },
                         "refreshUrl": {
+                            "format": "uri",
                             "type": "string"
                         },
                         "scopes": {
                             "$ref": "#/$defs/map-of-strings"
                         },
                         "tokenUrl": {
+                            "format": "uri",
                             "type": "string"
                         }
                     },
                     "required": [
                         "authorizationUrl",
                         "tokenUrl",
                         "scopes"
@@ -479,37 +506,41 @@
                     "type": "object",
                     "unevaluatedProperties": false
                 },
                 "client-credentials": {
                     "$ref": "#/$defs/specification-extensions",
                     "properties": {
                         "refreshUrl": {
+                            "format": "uri",
                             "type": "string"
                         },
                         "scopes": {
                             "$ref": "#/$defs/map-of-strings"
                         },
                         "tokenUrl": {
+                            "format": "uri",
                             "type": "string"
                         }
                     },
                     "required": [
                         "tokenUrl",
                         "scopes"
                     ],
                     "type": "object",
                     "unevaluatedProperties": false
                 },
                 "implicit": {
                     "$ref": "#/$defs/specification-extensions",
                     "properties": {
                         "authorizationUrl": {
+                            "format": "uri",
                             "type": "string"
                         },
                         "refreshUrl": {
+                            "format": "uri",
                             "type": "string"
                         },
                         "scopes": {
                             "$ref": "#/$defs/map-of-strings"
                         }
                     },
                     "required": [
@@ -519,20 +550,22 @@
                     "type": "object",
                     "unevaluatedProperties": false
                 },
                 "password": {
                     "$ref": "#/$defs/specification-extensions",
                     "properties": {
                         "refreshUrl": {
+                            "format": "uri",
                             "type": "string"
                         },
                         "scopes": {
                             "$ref": "#/$defs/map-of-strings"
                         },
                         "tokenUrl": {
+                            "format": "uri",
                             "type": "string"
                         }
                     },
                     "required": [
                         "tokenUrl",
                         "scopes"
                     ],
@@ -555,14 +588,15 @@
                     "$ref": "#/$defs/oauth-flows/$defs/password"
                 }
             },
             "type": "object",
             "unevaluatedProperties": false
         },
         "operation": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#operation-object",
             "$ref": "#/$defs/specification-extensions",
             "properties": {
                 "callbacks": {
                     "additionalProperties": {
                         "$ref": "#/$defs/callbacks-or-reference"
                     },
                     "type": "object"
@@ -614,14 +648,15 @@
                     "type": "array"
                 }
             },
             "type": "object",
             "unevaluatedProperties": false
         },
         "parameter": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#parameter-object",
             "$ref": "#/$defs/specification-extensions",
             "dependentSchemas": {
                 "schema": {
                     "$defs": {
                         "styles-for-cookie": {
                             "if": {
                                 "properties": {
@@ -632,18 +667,16 @@
                                 "required": [
                                     "in"
                                 ]
                             },
                             "then": {
                                 "properties": {
                                     "style": {
-                                        "default": "form",
-                                        "enum": [
-                                            "form"
-                                        ]
+                                        "const": "form",
+                                        "default": "form"
                                     }
                                 }
                             }
                         },
                         "styles-for-form": {
                             "else": {
                                 "properties": {
@@ -680,18 +713,16 @@
                                 "required": [
                                     "in"
                                 ]
                             },
                             "then": {
                                 "properties": {
                                     "style": {
-                                        "default": "simple",
-                                        "enum": [
-                                            "simple"
-                                        ]
+                                        "const": "simple",
+                                        "default": "simple"
                                     }
                                 }
                             }
                         },
                         "styles-for-path": {
                             "if": {
                                 "properties": {
@@ -701,14 +732,17 @@
                                 },
                                 "required": [
                                     "in"
                                 ]
                             },
                             "then": {
                                 "properties": {
+                                    "name": {
+                                        "pattern": "[^/#?]+$"
+                                    },
                                     "required": {
                                         "const": true
                                     },
                                     "style": {
                                         "default": "simple",
                                         "enum": [
                                             "matrix",
@@ -731,14 +765,18 @@
                                 },
                                 "required": [
                                     "in"
                                 ]
                             },
                             "then": {
                                 "properties": {
+                                    "allowReserved": {
+                                        "default": false,
+                                        "type": "boolean"
+                                    },
                                     "style": {
                                         "default": "form",
                                         "enum": [
                                             "form",
                                             "spaceDelimited",
                                             "pipeDelimited",
                                             "deepObject"
@@ -765,46 +803,50 @@
                             "$ref": "#/$defs/parameter/dependentSchemas/schema/$defs/styles-for-cookie"
                         },
                         {
                             "$ref": "#/$defs/parameter/dependentSchemas/schema/$defs/styles-for-form"
                         }
                     ],
                     "properties": {
-                        "allowReserved": {
-                            "default": false,
-                            "type": "boolean"
-                        },
                         "explode": {
                             "type": "boolean"
                         },
                         "style": {
                             "type": "string"
                         }
                     }
                 }
             },
+            "if": {
+                "properties": {
+                    "in": {
+                        "const": "query"
+                    }
+                },
+                "required": [
+                    "in"
+                ]
+            },
             "oneOf": [
                 {
                     "required": [
                         "schema"
                     ]
                 },
                 {
                     "required": [
                         "content"
                     ]
                 }
             ],
             "properties": {
-                "allowEmptyValue": {
-                    "default": false,
-                    "type": "boolean"
-                },
                 "content": {
-                    "$ref": "#/$defs/content"
+                    "$ref": "#/$defs/content",
+                    "maxProperties": 1,
+                    "minProperties": 1
                 },
                 "deprecated": {
                     "default": false,
                     "type": "boolean"
                 },
                 "description": {
                     "type": "string"
@@ -825,86 +867,119 @@
                     "type": "boolean"
                 },
                 "schema": {
                     "$dynamicRef": "#meta"
                 }
             },
             "required": [
+                "name",
                 "in"
             ],
+            "then": {
+                "properties": {
+                    "allowEmptyValue": {
+                        "default": false,
+                        "type": "boolean"
+                    }
+                }
+            },
             "type": "object",
             "unevaluatedProperties": false
         },
         "parameter-or-reference": {
             "else": {
                 "$ref": "#/$defs/parameter"
             },
             "if": {
                 "required": [
                     "$ref"
-                ]
+                ],
+                "type": "object"
             },
             "then": {
                 "$ref": "#/$defs/reference"
             }
         },
         "path-item": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#path-item-object",
             "$ref": "#/$defs/specification-extensions",
-            "patternProperties": {
-                "^(get|put|post|delete|options|head|patch|trace)$": {
-                    "$ref": "#/$defs/operation"
-                }
-            },
             "properties": {
+                "delete": {
+                    "$ref": "#/$defs/operation"
+                },
                 "description": {
                     "type": "string"
                 },
+                "get": {
+                    "$ref": "#/$defs/operation"
+                },
+                "head": {
+                    "$ref": "#/$defs/operation"
+                },
+                "options": {
+                    "$ref": "#/$defs/operation"
+                },
                 "parameters": {
                     "items": {
                         "$ref": "#/$defs/parameter-or-reference"
                     },
                     "type": "array"
                 },
+                "patch": {
+                    "$ref": "#/$defs/operation"
+                },
+                "post": {
+                    "$ref": "#/$defs/operation"
+                },
+                "put": {
+                    "$ref": "#/$defs/operation"
+                },
                 "servers": {
                     "items": {
                         "$ref": "#/$defs/server"
                     },
                     "type": "array"
                 },
                 "summary": {
                     "type": "string"
+                },
+                "trace": {
+                    "$ref": "#/$defs/operation"
                 }
             },
             "type": "object",
             "unevaluatedProperties": false
         },
         "path-item-or-reference": {
             "else": {
                 "$ref": "#/$defs/path-item"
             },
             "if": {
                 "required": [
                     "$ref"
-                ]
+                ],
+                "type": "object"
             },
             "then": {
                 "$ref": "#/$defs/reference"
             }
         },
         "paths": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#paths-object",
             "$ref": "#/$defs/specification-extensions",
             "patternProperties": {
                 "^/": {
-                    "$ref": "#/$defs/path-item"
+                    "$ref": "#/$defs/path-item-or-reference"
                 }
             },
             "type": "object",
             "unevaluatedProperties": false
         },
         "reference": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#reference-object",
             "properties": {
                 "$ref": {
                     "format": "uri-reference",
                     "type": "string"
                 },
                 "description": {
                     "type": "string"
@@ -913,14 +988,15 @@
                     "type": "string"
                 }
             },
             "type": "object",
             "unevaluatedProperties": false
         },
         "request-body": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#request-body-object",
             "$ref": "#/$defs/specification-extensions",
             "properties": {
                 "content": {
                     "$ref": "#/$defs/content"
                 },
                 "description": {
                     "type": "string"
@@ -939,21 +1015,23 @@
         "request-body-or-reference": {
             "else": {
                 "$ref": "#/$defs/request-body"
             },
             "if": {
                 "required": [
                     "$ref"
-                ]
+                ],
+                "type": "object"
             },
             "then": {
                 "$ref": "#/$defs/reference"
             }
         },
         "response": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#response-object",
             "$ref": "#/$defs/specification-extensions",
             "properties": {
                 "content": {
                     "$ref": "#/$defs/content"
                 },
                 "description": {
                     "type": "string"
@@ -980,52 +1058,69 @@
         "response-or-reference": {
             "else": {
                 "$ref": "#/$defs/response"
             },
             "if": {
                 "required": [
                     "$ref"
-                ]
+                ],
+                "type": "object"
             },
             "then": {
                 "$ref": "#/$defs/reference"
             }
         },
         "responses": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#responses-object",
             "$ref": "#/$defs/specification-extensions",
+            "if": {
+                "$comment": "either default, or at least one response code property must exist",
+                "patternProperties": {
+                    "^[1-5](?:[0-9]{2}|XX)$": false
+                }
+            },
+            "minProperties": 1,
             "patternProperties": {
-                "^[1-5][0-9X]{2}$": {
+                "^[1-5](?:[0-9]{2}|XX)$": {
                     "$ref": "#/$defs/response-or-reference"
                 }
             },
             "properties": {
                 "default": {
                     "$ref": "#/$defs/response-or-reference"
                 }
             },
+            "then": {
+                "required": [
+                    "default"
+                ]
+            },
             "type": "object",
             "unevaluatedProperties": false
         },
         "schema": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#schema-object",
             "$dynamicAnchor": "meta",
             "type": [
                 "object",
                 "boolean"
             ]
         },
         "security-requirement": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#security-requirement-object",
             "additionalProperties": {
                 "items": {
                     "type": "string"
                 },
                 "type": "array"
             },
             "type": "object"
         },
         "security-scheme": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#security-scheme-object",
             "$defs": {
                 "type-apikey": {
                     "if": {
                         "properties": {
                             "type": {
                                 "const": "apiKey"
                             }
@@ -1075,15 +1170,16 @@
                         ]
                     }
                 },
                 "type-http-bearer": {
                     "if": {
                         "properties": {
                             "scheme": {
-                                "const": "bearer"
+                                "pattern": "^[Bb][Ee][Aa][Rr][Ee][Rr]$",
+                                "type": "string"
                             },
                             "type": {
                                 "const": "http"
                             }
                         },
                         "required": [
                             "type",
@@ -1091,18 +1187,15 @@
                         ]
                     },
                     "then": {
                         "properties": {
                             "bearerFormat": {
                                 "type": "string"
                             }
-                        },
-                        "required": [
-                            "scheme"
-                        ]
+                        }
                     }
                 },
                 "type-oauth2": {
                     "if": {
                         "properties": {
                             "type": {
                                 "const": "oauth2"
@@ -1190,21 +1283,23 @@
         "security-scheme-or-reference": {
             "else": {
                 "$ref": "#/$defs/security-scheme"
             },
             "if": {
                 "required": [
                     "$ref"
-                ]
+                ],
+                "type": "object"
             },
             "then": {
                 "$ref": "#/$defs/reference"
             }
         },
         "server": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#server-object",
             "$ref": "#/$defs/specification-extensions",
             "properties": {
                 "description": {
                     "type": "string"
                 },
                 "url": {
                     "format": "uri-reference",
@@ -1220,14 +1315,15 @@
             "required": [
                 "url"
             ],
             "type": "object",
             "unevaluatedProperties": false
         },
         "server-variable": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#server-variable-object",
             "$ref": "#/$defs/specification-extensions",
             "properties": {
                 "default": {
                     "type": "string"
                 },
                 "description": {
                     "type": "string"
@@ -1243,19 +1339,21 @@
             "required": [
                 "default"
             ],
             "type": "object",
             "unevaluatedProperties": false
         },
         "specification-extensions": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#specification-extensions",
             "patternProperties": {
                 "^x-": true
             }
         },
         "tag": {
+            "$comment": "https://spec.openapis.org/oas/v3.1.0#tag-object",
             "$ref": "#/$defs/specification-extensions",
             "properties": {
                 "description": {
                     "type": "string"
                 },
                 "externalDocs": {
                     "$ref": "#/$defs/external-documentation"
@@ -1267,15 +1365,15 @@
             "required": [
                 "name"
             ],
             "type": "object",
             "unevaluatedProperties": false
         }
     },
-    "$id": "https://spec.openapis.org/oas/3.1/schema/2021-05-20",
+    "$id": "https://spec.openapis.org/oas/3.1/schema/2022-10-07",
     "$ref": "#/$defs/specification-extensions",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "anyOf": [
         {
             "required": [
                 "paths"
             ]
@@ -1287,14 +1385,15 @@
         },
         {
             "required": [
                 "webhooks"
             ]
         }
     ],
+    "description": "The description of OpenAPI v3.1.x documents without schema validation, as defined by https://spec.openapis.org/oas/v3.1.0",
     "properties": {
         "components": {
             "$ref": "#/$defs/components"
         },
         "externalDocs": {
             "$ref": "#/$defs/external-documentation"
         },
@@ -1316,14 +1415,19 @@
         "security": {
             "items": {
                 "$ref": "#/$defs/security-requirement"
             },
             "type": "array"
         },
         "servers": {
+            "default": [
+                {
+                    "url": "/"
+                }
+            ],
             "items": {
                 "$ref": "#/$defs/server"
             },
             "type": "array"
         },
         "tags": {
             "items": {
```

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/schemas/__init__.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/schemas/utils.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/shortcuts.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/shortcuts.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/validation/__init__.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/validation/decorators.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/decorators.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/validation/exceptions.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/validation/protocols.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/protocols.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-from typing import TYPE_CHECKING
 from typing import Any
 from typing import Hashable
 from typing import Iterator
 from typing import Mapping
 
 if sys.version_info >= (3, 8):
     from typing import Protocol
```

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/validation/proxies.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/proxies.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/openapi_spec_validator/validation/validators.py` & `openapi_spec_validator-0.5.7/openapi_spec_validator/validation/validators.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/pyproject.toml` & `openapi_spec_validator-0.5.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [[tool.mypy.overrides]]
 module = "lazy_object_proxy.*"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "openapi-spec-validator"
-version = "0.5.6"
+version = "0.5.7"
 description = "OpenAPI 2.0 (aka Swagger) and OpenAPI 3 spec validator"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/python-openapi/openapi-spec-validator"
 keywords = ["openapi", "swagger", "schema"]
 classifiers = [
@@ -47,36 +47,35 @@
     {path = "tests", format = "sdist"},
 ]
 
 [tool.poetry.dependencies]
 jsonschema = ">=4.0.0,<4.18.0"
 openapi-schema-validator = "^0.4.2"
 python = "^3.7.0"
-requests = {version = "*", optional = true}
 importlib-resources = {version = "^5.8.0", python = "<3.9" }
+typing-extensions = {version = "^4.5.0", python = "<3.8" }
 jsonschema-spec = "^0.1.1"
 lazy-object-proxy = "^1.7.1"
-sphinx = {version = "^5.3.0", optional = true}
-sphinx-immaterial = {version = "^0.11.0", optional = true}
 
 [tool.poetry.extras]
 dev = ["pre-commit"]
 docs = ["sphinx", "sphinx-immaterial"]
 requests = ["requests"]
 
 [tool.poetry.dev-dependencies]
 pre-commit =  {version = "*", optional = true}
 pytest = "^6.2.5"
-pytest-flake8 = "=1.0.7"
-pytest-cov = "^3.0.0"
+pytest-flake8 = "=1.1.0"
+pytest-cov = "^4.1.0"
 tox = "*"
-mypy = "^0.971"
-isort = "^5.10.1"
-black = "^22.8.0"
-flynt = "^0.76"
+mypy = "^1.3"
+isort = "^5.11.5"
+black = "^23.3.0"
+flynt = "^0.78"
+deptry = { version = "^0.11.0", python = ">=3.8" }
 
 [tool.poetry.scripts]
 openapi-spec-validator = "openapi_spec_validator.__main__:main"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.3.0"
 sphinx-immaterial = "^0.11.0"
```

### Comparing `openapi_spec_validator-0.5.6/tests/integration/conftest.py` & `openapi_spec_validator-0.5.7/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/tests/integration/data/v2.0/missing-reference.yaml` & `openapi_spec_validator-0.5.7/tests/integration/data/v2.0/missing-reference.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/tests/integration/data/v2.0/petstore.yaml` & `openapi_spec_validator-0.5.7/tests/integration/data/v2.0/petstore.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/tests/integration/data/v3.0/parent-reference/openapi.yaml` & `openapi_spec_validator-0.5.7/tests/integration/data/v3.0/parent-reference/openapi.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml` & `openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore-separate/spec/openapi.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/tests/integration/data/v3.0/petstore.yaml` & `openapi_spec_validator-0.5.7/tests/integration/data/v3.0/petstore.yaml`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/tests/integration/data/v3.1/petstore.yaml` & `openapi_spec_validator-0.5.7/tests/integration/data/v3.1/petstore.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -51,39 +51,15 @@
         default:
           description: unexpected error
           content:
             application/json:
               schema:
                 $ref: "#/components/schemas/Error"
   /pets/{petId}:
-    get:
-      summary: Info for a specific pet
-      operationId: showPetById
-      tags:
-        - pets
-      parameters:
-        - name: petId
-          in: path
-          required: true
-          description: The id of the pet to retrieve
-          schema:
-            type: string
-      responses:
-        '200':
-          description: Expected response to a valid request
-          content:
-            application/json:
-              schema:
-                $ref: "#/components/schemas/Pets"
-        default:
-          description: unexpected error
-          content:
-            application/json:
-              schema:
-                $ref: "#/components/schemas/Error"
+    $ref: "#/components/pathItems/PetPath"
 components:
   schemas:
     Pet:
       required:
         - id
         - name
       properties:
@@ -105,8 +81,35 @@
         - code
         - message
       properties:
         code:
           type: integer
           format: int32
         message:
-          type: string
+          type: string
+  pathItems:
+    PetPath:
+      get:
+        summary: Info for a specific pet
+        operationId: showPetById
+        tags:
+          - pets
+        parameters:
+          - name: petId
+            in: path
+            required: true
+            description: The id of the pet to retrieve
+            schema:
+              type: string
+        responses:
+          '200':
+            description: Expected response to a valid request
+            content:
+              application/json:
+                schema:
+                  $ref: "#/components/schemas/Pets"
+          default:
+            description: unexpected error
+            content:
+              application/json:
+                schema:
+                  $ref: "#/components/schemas/Error"
```

### Comparing `openapi_spec_validator-0.5.6/tests/integration/test_main.py` & `openapi_spec_validator-0.5.7/tests/integration/test_main.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/tests/integration/test_shortcuts.py` & `openapi_spec_validator-0.5.7/tests/integration/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/tests/integration/validation/test_exceptions.py` & `openapi_spec_validator-0.5.7/tests/integration/validation/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/tests/integration/validation/test_validators.py` & `openapi_spec_validator-0.5.7/tests/integration/validation/test_validators.py`

 * *Files identical despite different names*

### Comparing `openapi_spec_validator-0.5.6/PKG-INFO` & `openapi_spec_validator-0.5.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-spec-validator
-Version: 0.5.6
+Version: 0.5.7
 Summary: OpenAPI 2.0 (aka Swagger) and OpenAPI 3 spec validator
 Home-page: https://github.com/python-openapi/openapi-spec-validator
 License: Apache-2.0
 Keywords: openapi,swagger,schema
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -14,40 +14,34 @@
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
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: requests
 Requires-Dist: importlib-resources (>=5.8.0,<6.0.0) ; python_version < "3.9"
 Requires-Dist: jsonschema (>=4.0.0,<4.18.0)
 Requires-Dist: jsonschema-spec (>=0.1.1,<0.2.0)
 Requires-Dist: lazy-object-proxy (>=1.7.1,<2.0.0)
 Requires-Dist: openapi-schema-validator (>=0.4.2,<0.5.0)
-Requires-Dist: requests ; extra == "requests"
-Requires-Dist: sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
-Requires-Dist: sphinx-immaterial (>=0.11.0,<0.12.0) ; extra == "docs"
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.8"
 Project-URL: Repository, https://github.com/python-openapi/openapi-spec-validator
 Description-Content-Type: text/x-rst
 
 **********************
 OpenAPI Spec validator
 **********************
 
+.. image:: https://img.shields.io/docker/v/p1c2u/openapi-spec-validator.svg?color=%23086DD7&label=docker%20hub&sort=semver
+     :target: https://hub.docker.com/r/p1c2u/openapi-spec-validator
 .. image:: https://img.shields.io/pypi/v/openapi-spec-validator.svg
      :target: https://pypi.python.org/pypi/openapi-spec-validator
 .. image:: https://travis-ci.org/python-openapi/openapi-spec-validator.svg?branch=master
      :target: https://travis-ci.org/python-openapi/openapi-spec-validator
 .. image:: https://img.shields.io/codecov/c/github/python-openapi/openapi-spec-validator/master.svg?style=flat
      :target: https://codecov.io/github/python-openapi/openapi-spec-validator?branch=master
 .. image:: https://img.shields.io/pypi/pyversions/openapi-spec-validator.svg
```

