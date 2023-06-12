# Comparing `tmp/reasoner_validator-3.5.6.tar.gz` & `tmp/reasoner_validator-3.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.5.6.tar", max compression
+gzip compressed data, was "reasoner_validator-3.5.7.tar", max compression
```

## Comparing `reasoner_validator-3.5.6.tar` & `reasoner_validator-3.5.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1153 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/LICENSE
--rw-r--r--   0        0        0    12431 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/README.md
--rw-r--r--   0        0        0      131 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/Makefile
--rw-r--r--   0        0        0     2288 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/conf.py
--rw-r--r--   0        0        0    18216 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/index.rst
--rw-r--r--   0        0        0      795 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/make.bat
--rw-r--r--   0        0        0      136 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36025 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2093 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/pyproject.toml
--rw-r--r--   0        0        0    20545 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    61249 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39243 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    26862 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4350 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     9718 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    13781 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     9922 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/versioning.py
--rw-r--r--   0        0        0        0 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/conftest.py
--rw-r--r--   0        0        0   111722 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    42178 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_data/sample_trapi_schema.yaml
--rw-r--r--   0        0        0    31899 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_response_validator.py
--rw-r--r--   0        0        0     4533 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_semver.py
--rw-r--r--   0        0        0     1746 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26543 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_validate.py
--rw-r--r--   0        0        0    19013 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_validation_report.py
--rw-r--r--   0        0        0     2061 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_workflows.py
--rw-r--r--   0        0        0    14470 1970-01-01 00:00:00.000000 reasoner_validator-3.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/LICENSE
+-rw-r--r--   0        0        0    12606 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/README.md
+-rw-r--r--   0        0        0      131 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/conf.py
+-rw-r--r--   0        0        0    19034 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-12 21:28:39.063953 reasoner_validator-3.5.7/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36025 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2093 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/pyproject.toml
+-rw-r--r--   0        0        0    20545 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    61511 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39243 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    26862 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4350 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     9718 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    13781 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0     9922 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:28:39.067953 reasoner_validator-3.5.7/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/conftest.py
+-rw-r--r--   0        0        0   112361 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    42178 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_data/sample_trapi_schema.yaml
+-rw-r--r--   0        0        0    31899 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_response_validator.py
+-rw-r--r--   0        0        0     4533 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_semver.py
+-rw-r--r--   0        0        0     1746 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26543 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_validate.py
+-rw-r--r--   0        0        0    19013 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2061 2023-06-12 21:28:39.071953 reasoner_validator-3.5.7/tests/test_workflows.py
+-rw-r--r--   0        0        0    14645 1970-01-01 00:00:00.000000 reasoner_validator-3.5.7/PKG-INFO
```

### Comparing `reasoner_validator-3.5.6/LICENSE` & `reasoner_validator-3.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/README.md` & `reasoner_validator-3.5.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,14 @@
 
 For script usage, type:
 
 ```bash
 ./trapi_validator.py --help
 ```
 
-The script allows
-
 (*) Thank you Eric Deutsch for the prototype code for this script
 
 ## Running tests
 
 To run the test locally install with the `dev` dependencies group if not already done:
 
 ```bash
@@ -77,18 +75,33 @@
 
 Run the tests with coverage report:
 
 ```bash
 poetry run pytest --cov
 ```
 
+Note that [poetry automatically uses any existing virtual environment](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment), but you can otherwise also enter the one that is created by poetry by default:
+
+```shell
+poetry shell
+# run your commands, e.g. the web service module
+exit  # exit the poetry shell
+```
+
+The use of the Poetry shell command allows for running of the tests without the `poetry run` prefix. We will continue in this manner.
+
+```bash
+% poetry shell
+(reasoner-validator-py3.9) % pytest --cov
+```
+
 Run the tests with detailed coverage report in a HTML page:
 
 ```bash
-poetry run pytest --cov --cov-report html
+pytest --cov --cov-report html
 ```
 
 Serve the report on http://localhost:3000:
 
 ```bash
 python -m http.server 3000 --directory ./htmlcov
 ```
@@ -159,22 +172,14 @@
 
 The service may be run directly as a Python module. The web services module may be directly run, as follows. 
 
 ```shell
 python -m api.main
 ```
 
-Note that [poetry automatically uses any existing virtual environment](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment), but you can otherwise also enter the one that is created by poetry by default:
-
-```shell
-poetry shell
-# run your commands, e.g. the web service module
-exit  # exit the poetry shell
-```
-
 Go to  http://localhost/docs to see the service documentation and to use the simple UI to input TRAPI messages for validation.
 
 ### Typical Output
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
```

### Comparing `reasoner_validator-3.5.6/docs/Makefile` & `reasoner_validator-3.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/docs/conf.py` & `reasoner_validator-3.5.7/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import sys
 sys.path.insert(0, os.path.abspath('..'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'Reasoner Validator'
-copyright = '2022, Richard Bruskiewich;  2020-21, Patrick Wang'
+copyright = '2022-23, Richard Bruskiewich;  2020-21, Patrick Wang'
 author = 'Richard Bruskiewich and Patrick Wang'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `reasoner_validator-3.5.6/docs/index.rst` & `reasoner_validator-3.5.7/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 Checkout then setup dependencies and the standard virtual environment using poetry, as follows:
 
 .. code-block:: bash
 
     git checkout https://github.com/NCATSTranslator/reasoner-validator.git
     cd reasoner-validator
     poetry install
+    poetry shell
+
+These operations install the software and creates a virtual operation for running the software in a simple fashion.
 
 You can optionally, `use a tool like pyenv to set your local shell Python version to a 3.9 release <https://python-poetry.org/docs/managing-environments/>`_  prior to the poetry installation.
 
 Basic Programmatic Usage
 ========================
 
 Unlike earlier release of the reasoner-validator package, the current (major release 3.*.*) wraps validation in a general Python class object, 'ValidatorReporter' which is subclassed into various validator types (TRAPI Schema, Biolink, etc.).
@@ -199,14 +202,31 @@
    Validation Codes Dictionary <reasoner_validator.validation_codes>
    Validation Codes <validation_codes_dictionary>
    SemVer Version Utilities <reasoner_validator.versioning>
 
 Refer to the `reasoner_validator package unit tests <https://github
 .com/NCATSTranslator/reasoner-validator/blob/master/tests>`_ for additional guidance on how to use the Python API.
 
+
+Running Validation against an ARS UUID Result(*) or using a Local TRAPI Request Query
+=====================================================================================
+
+A local script trapi_validator.py is available to run TRAPI Response validation against either a PK (UUID)
+indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS), a local JSON Response
+text file or a locally triggered _ad hoc_ query Request against an directly specified TRAPI endpoint.
+
+Note that it is best run within a **`poetry shell`** created by **`poetry install`**.
+
+For script usage, type:
+
+.. code-block:: bash
+
+    ./trapi_validator.py --help
+
+
 Validation Run as a Web Service
 ===============================
 
 The Reasoner Validator is available wrapped as a simple web service.  The service may be run directly or as a Docker container.
 
 Web Service API
 ---------------
@@ -256,14 +276,15 @@
 --------------------------------
 
 The service may be run directly as a Python module after certain dependencies are installed using poetry, as follows:
 
 .. code-block:: bash
 
     poetry install
+    poetry shell
 
 The module may afterwards be run, as follows:
 
 .. code-block:: bash
 
     python -m api.main
```

### Comparing `reasoner_validator-3.5.6/docs/make.bat` & `reasoner_validator-3.5.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/docs/validation_codes_dictionary.md` & `reasoner_validator-3.5.7/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/pyproject.toml` & `reasoner_validator-3.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.5.6"
+version = "3.5.7"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.5.6/reasoner_validator/__init__.py` & `reasoner_validator-3.5.7/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.5.7/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1052,16 +1052,28 @@
         :param edge: basic dictionary of a templated input edge - S-P-O including concept Biolink Model categories
         :type edge: Dict[str,str]
         """
         # data fields to be validated...
         subject_category_curie = edge['subject_category'] if 'subject_category' in edge else None
         object_category_curie = edge['object_category'] if 'object_category' in edge else None
         predicate = edge['predicate'] if 'predicate' in edge else None
-        subject_curie = edge['subject'] if 'subject' in edge else None
-        object_curie = edge['object'] if 'object' in edge else None
+
+        if 'subject_id' in edge:
+            subject_curie = edge['subject_id']
+        elif 'subject' in edge:
+            subject_curie = edge['subject']
+        else:
+            subject_curie = None
+
+        if 'object_id' in edge:
+            object_curie = edge['object_id']
+        elif 'object' in edge:
+            object_curie = edge['object']
+        else:
+            object_curie = None
 
         edge_id = f"{str(subject_curie)}--{predicate}->{str(object_curie)}"
 
         self.validate_input_edge_node(
             context='Subject',
             node_id=subject_curie,
             category_name=subject_category_curie
```

### Comparing `reasoner_validator-3.5.6/reasoner_validator/codes.yaml` & `reasoner_validator-3.5.7/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/reasoner_validator/report.py` & `reasoner_validator-3.5.7/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/reasoner_validator/sri/util.py` & `reasoner_validator-3.5.7/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.5.7/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.5.7/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/reasoner_validator/validation_codes.py` & `reasoner_validator-3.5.7/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/reasoner_validator/versioning.py` & `reasoner_validator-3.5.7/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.5.7/tests/test_biolink_compliance_validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,217 +94,228 @@
     [
         (   # Query 0 - Valid edge object
             LATEST_BIOLINK_MODEL_VERSION,  # Biolink Model Version
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:subclass_of',
-                'subject': 'UBERON:0005453',
-                'object': 'UBERON:0035769'
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'UBERON:0035769'
             },
             ""
         ),
-        (   # Query 1 - Missing subject category
-            LATEST_BIOLINK_MODEL_VERSION,
+        (   # Query 1 - Valid edge object, using original 'subject' and 'object' JSON tags
+            LATEST_BIOLINK_MODEL_VERSION,  # Biolink Model Version
             {
+                'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:subclass_of',
                 'subject': 'UBERON:0005453',
                 'object': 'UBERON:0035769'
             },
+            ""  # should still no generate an error message
+        ),
+        (   # Query 2 - Missing subject category
+            LATEST_BIOLINK_MODEL_VERSION,
+            {
+                'object_category': 'biolink:AnatomicalEntity',
+                'predicate': 'biolink:subclass_of',
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'UBERON:0035769'
+            },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Subject has a missing Biolink category!"
             "error.input_edge.node.category.missing"
         ),
-        (   # Query 2 - Invalid subject category
+        (   # Query 3 - Invalid subject category
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:NotACategory',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:subclass_of',
-                'subject': 'UBERON:0005453',
-                'object': 'UBERON:0035769'
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'UBERON:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Subject element 'biolink:NotACategory' is unknown!"
             "error.input_edge.node.category.unknown"
         ),
-        (   # Query 3 - Missing object category
+        (   # Query 4 - Missing object category
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:subclass_of',
-                'subject': 'UBERON:0005453',
-                'object': 'UBERON:0035769'
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'UBERON:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Object has a missing Biolink category!"
             "error.input_edge.node.category.missing"
         ),
-        (   # Query 4 - Invalid object category
+        (   # Query 5 - Invalid object category
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:NotACategory',
                 'predicate': 'biolink:subclass_of',
-                'subject': 'UBERON:0005453',
-                'object': 'UBERON:0035769'
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'UBERON:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Object element 'biolink:NotACategory' is unknown!"
             "error.input_edge.node.category.unknown"
         ),
-        (   # Query 5 - Missing predicate
+        (   # Query 6 - Missing predicate
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
-                'subject': 'UBERON:0005453',
-                'object': 'UBERON:0035769'
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'UBERON:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Predicate is missing or empty!"
             "error.input_edge.predicate.missing"
         ),
-        (   # Query 6 - Empty predicate
+        (   # Query 7- Empty predicate
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': '',
-                'subject': 'UBERON:0005453',
-                'object': 'UBERON:0035769'
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'UBERON:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Predicate is missing or empty!"
             "error.input_edge.predicate.missing"
         ),
-        (   # Query 7 - Predicate is deprecated
+        (   # Query 8 - Predicate is deprecated
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:Drug',
                 'object_category': 'biolink:Protein',
                 'predicate': 'biolink:increases_amount_or_activity_of',
-                'subject': 'NDC:0002-8215-01',  # a form of insulin
-                'object': 'MONDO:0005148'  # type 2 diabetes?
+                'subject_id': 'NDC:0002-8215-01',  # a form of insulin
+                'object_id': 'MONDO:0005148'  # type 2 diabetes?
             },
             # f"{INPUT_EDGE_PREFIX}: WARNING - Predicate element " +
             # "'binds' is deprecated?"  # in Biolink 3.1.1
             "warning.input_edge.predicate.deprecated"
         ),
-        (   # Query 8 - Predicate is abstract
+        (   # Query 9 - Predicate is abstract
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:InformationContentEntity',
                 'object_category': 'biolink:Agent',
                 'predicate': 'biolink:contributor',
-                'subject': 'PMID:1234',
-                'object': 'ORCID:56789'
+                'subject_id': 'PMID:1234',
+                'object_id': 'ORCID:56789'
             },
             # f"{INPUT_EDGE_PREFIX}: INFO - Predicate element 'biolink:contributor' is abstract."
             "info.input_edge.predicate.abstract"
         ),
-        (   # Query 9 - Predicate is a mixin
+        (   # Query 10 - Predicate is a mixin
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:Drug',
                 'object_category': 'biolink:BiologicalProcess',
                 'predicate': 'biolink:decreases_amount_or_activity_of',
-                'subject': 'NDC:50090‑0766',  # Metformin
-                'object': 'GO:0006094'  # Gluconeogenesis
+                'subject_id': 'NDC:50090‑0766',  # Metformin
+                'object_id': 'GO:0006094'  # Gluconeogenesis
             },
             # f"{INPUT_EDGE_PREFIX}: INFO - Predicate element 'biolink:decreases_amount_or_activity_of' is a mixin."
             "info.input_edge.predicate.mixin"
         ),
-        (   # Query 10 - Unknown predicate element
+        (   # Query 11 - Unknown predicate element
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:not_a_predicate',
-                'subject': 'UBERON:0005453',
-                'object': 'UBERON:0035769'
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'UBERON:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Predicate element 'biolink:not_a_predicate' is unknown!"
             "error.input_edge.predicate.unknown"
         ),
-        (   # Query 11 - Invalid or unknown predicate
+        (   # Query 12 - Invalid or unknown predicate
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:has_unit',
-                'subject': 'UBERON:0005453',
-                'object': 'UBERON:0035769'
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'UBERON:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Predicate element 'biolink:has_unit' is invalid!"
             "error.input_edge.predicate.invalid"
         ),
-        (   # Query 12 - Non-canonical directed predicate
+        (   # Query 13 - Non-canonical directed predicate
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:SmallMolecule',
                 'object_category': 'biolink:Disease',
                 'predicate': 'biolink:affected_by',
-                'subject': 'DRUGBANK:DB00331',
-                'object': 'MONDO:0005148'
+                'subject_id': 'DRUGBANK:DB00331',
+                'object_id': 'MONDO:0005148'
             },
             # f"{INPUT_EDGE_PREFIX}: WARNING - Edge predicate 'biolink:affected_by' is non-canonical?"
             "warning.input_edge.predicate.non_canonical"
         ),
-        (   # Query 13 - Missing subject
+        (   # Query 14 - Missing subject
             LATEST_BIOLINK_MODEL_VERSION,  # Biolink Model Version
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:subclass_of',
-                'object': 'UBERON:0035769'
+                'object_id': 'UBERON:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Subject node identifier is missing!"
             "error.input_edge.node.id.missing"
         ),
-        (   # Query 14 - Unmappable subject namespace
+        (   # Query 15 - Unmappable subject namespace
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:subclass_of',
-                'subject': 'FOO:0005453',
-                'object': 'UBERON:0035769'
+                'subject_id': 'FOO:0005453',
+                'object_id': 'UBERON:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: WARNING - Subject node identifier 'FOO:0005453' " +
             # "is unmapped to 'biolink:AnatomicalEntity'?"
             "warning.input_edge.node.id.unmapped_to_category"
         ),
-        (   # Query 15 - missing object
+        (   # Query 16 - missing object
             LATEST_BIOLINK_MODEL_VERSION,  # Biolink Model Version
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:subclass_of',
-                'subject': "UBERON:0005453"
+                'subject_id': "UBERON:0005453"
             },
             # f"{INPUT_EDGE_PREFIX}: ERROR - Object node identifier is missing!"
             "error.input_edge.node.id.missing"
         ),
-        (   # Query 16 - Unmappable object namespace
+        (   # Query 17 - Unmappable object namespace
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AnatomicalEntity',
                 'object_category': 'biolink:AnatomicalEntity',
                 'predicate': 'biolink:subclass_of',
-                'subject': 'UBERON:0005453',
-                'object': 'BAR:0035769'
+                'subject_id': 'UBERON:0005453',
+                'object_id': 'BAR:0035769'
             },
             # f"{INPUT_EDGE_PREFIX}: WARNING - Object node identifier 'BAR:0035769' " +
             # "is unmapped to 'biolink:AnatomicalEntity'?"
             "warning.input_edge.node.id.unmapped_to_category"
         ),
-        (   # Query 17 - Valid other model
+        (   # Query 18 - Valid other model
             "1.8.2",
             {
                 'subject_category': 'biolink:ChemicalSubstance',
                 'object_category': 'biolink:Protein',
                 'predicate': 'biolink:entity_negatively_regulates_entity',
-                'subject': 'DRUGBANK:DB00945',
-                'object': 'UniProtKB:P23219'
+                'subject_id': 'DRUGBANK:DB00945',
+                'object_id': 'UniProtKB:P23219'
             },
             ""
         ),
         # (   # Query xx - Deprecated node category - no example of this in BIolink 3.1.1
         #     LATEST_BIOLINK_MODEL,
         #     {
         #         'subject_category': 'biolink:Nutrient',
@@ -312,33 +323,33 @@
         #         'predicate': 'biolink:physically_interacts_with',
         #         'subject': 'CHEBI:27300',
         #         'object': 'Orphanet:120464'
         #     },
         #     # f"{INPUT_EDGE_PREFIX}: WARNING - Subject 'biolink:Nutrient' is deprecated?"
         #     "warning.input_edge.node.category.deprecated"
         # ),
-        (   # Query 18 - Issue a warning for input_edge data with a category that is a mixin?
+        (   # Query 19 - Issue a warning for input_edge data with a category that is a mixin?
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:GeneOrGeneProduct',
                 'object_category': 'biolink:Protein',
                 'predicate': 'biolink:related_to',
-                'subject': 'HGNC:9604',
-                'object': 'UniProtKB:P23219'
+                'subject_id': 'HGNC:9604',
+                'object_id': 'UniProtKB:P23219'
             },
             "warning.input_edge.node.category.not_concrete"
         ),
-        (   # Query 19 - Issue a warning for input_edge data with a category that is abstract?
+        (   # Query 20 - Issue a warning for input_edge data with a category that is abstract?
             LATEST_BIOLINK_MODEL_VERSION,
             {
                 'subject_category': 'biolink:AdministrativeEntity',
                 'object_category': 'biolink:Agent',
                 'predicate': 'biolink:related_to',
-                'subject': 'isbn:1234',
-                'object': 'ORCID:1234'
+                'subject_id': 'isbn:1234',
+                'object_id': 'ORCID:1234'
             },
             "warning.input_edge.node.category.not_concrete"
         )
     ]
 )
 def test_check_biolink_model_compliance_of_input_edge(query: Tuple):
     validator: BiolinkValidator = check_biolink_model_compliance_of_input_edge(edge=query[1], biolink_version=query[0])
```

### Comparing `reasoner_validator-3.5.6/tests/test_data/sample_trapi_schema.yaml` & `reasoner_validator-3.5.7/tests/test_data/sample_trapi_schema.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/tests/test_response_validator.py` & `reasoner_validator-3.5.7/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/tests/test_semver.py` & `reasoner_validator-3.5.7/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/tests/test_trapi_versioning.py` & `reasoner_validator-3.5.7/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/tests/test_validate.py` & `reasoner_validator-3.5.7/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/tests/test_validation_report.py` & `reasoner_validator-3.5.7/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/tests/test_workflows.py` & `reasoner_validator-3.5.7/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.6/PKG-INFO` & `reasoner_validator-3.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.5.6
+Version: 3.5.7
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -102,16 +102,14 @@
 
 For script usage, type:
 
 ```bash
 ./trapi_validator.py --help
 ```
 
-The script allows
-
 (*) Thank you Eric Deutsch for the prototype code for this script
 
 ## Running tests
 
 To run the test locally install with the `dev` dependencies group if not already done:
 
 ```bash
@@ -120,18 +118,33 @@
 
 Run the tests with coverage report:
 
 ```bash
 poetry run pytest --cov
 ```
 
+Note that [poetry automatically uses any existing virtual environment](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment), but you can otherwise also enter the one that is created by poetry by default:
+
+```shell
+poetry shell
+# run your commands, e.g. the web service module
+exit  # exit the poetry shell
+```
+
+The use of the Poetry shell command allows for running of the tests without the `poetry run` prefix. We will continue in this manner.
+
+```bash
+% poetry shell
+(reasoner-validator-py3.9) % pytest --cov
+```
+
 Run the tests with detailed coverage report in a HTML page:
 
 ```bash
-poetry run pytest --cov --cov-report html
+pytest --cov --cov-report html
 ```
 
 Serve the report on http://localhost:3000:
 
 ```bash
 python -m http.server 3000 --directory ./htmlcov
 ```
@@ -202,22 +215,14 @@
 
 The service may be run directly as a Python module. The web services module may be directly run, as follows. 
 
 ```shell
 python -m api.main
 ```
 
-Note that [poetry automatically uses any existing virtual environment](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment), but you can otherwise also enter the one that is created by poetry by default:
-
-```shell
-poetry shell
-# run your commands, e.g. the web service module
-exit  # exit the poetry shell
-```
-
 Go to  http://localhost/docs to see the service documentation and to use the simple UI to input TRAPI messages for validation.
 
 ### Typical Output
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
```

