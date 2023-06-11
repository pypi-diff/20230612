# Comparing `tmp/physionet-0.1.0.tar.gz` & `tmp/physionet-0.1.1.tar.gz`

## Comparing `physionet-0.1.0.tar` & `physionet-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 physionet-0.1.0/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 physionet-0.1.0/requirements.txt
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 physionet-0.1.0/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 physionet-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 physionet-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 physionet-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 physionet-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 physionet-0.1.0/physionet/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 physionet-0.1.0/physionet/dataset.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 physionet-0.1.0/physionet/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 physionet-0.1.0/physionet/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 physionet-0.1.0/physionet/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 physionet-0.1.0/physionet/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 physionet-0.1.0/tests/test_dataset.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 physionet-0.1.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 physionet-0.1.0/LICENSE
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 physionet-0.1.0/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 physionet-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 physionet-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 physionet-0.1.1/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 physionet-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 physionet-0.1.1/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 physionet-0.1.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 physionet-0.1.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 physionet-0.1.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 physionet-0.1.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 physionet-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 physionet-0.1.1/physionet/__init__.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 physionet-0.1.1/physionet/mlhc.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 physionet-0.1.1/physionet/project.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 physionet-0.1.1/physionet/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 physionet-0.1.1/physionet/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 physionet-0.1.1/physionet/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 physionet-0.1.1/physionet/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 physionet-0.1.1/tests/test_dataset.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 physionet-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 physionet-0.1.1/LICENSE
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 physionet-0.1.1/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 physionet-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 physionet-0.1.1/PKG-INFO
```

### Comparing `physionet-0.1.0/.github/workflows/run-tests.yml` & `physionet-0.1.1/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `physionet-0.1.0/.gitignore` & `physionet-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `physionet-0.1.0/LICENSE` & `physionet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `physionet-0.1.0/pyproject.toml` & `physionet-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "physionet"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Tom Pollard", email="tpollard@mit.edu" },
 ]
 license = {file = "LICENSE"}
 description = "A collection of tools for working with the PhysioNet repository."
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `physionet-0.1.0/PKG-INFO` & `physionet-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physionet
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of tools for working with the PhysioNet repository.
 Project-URL: homepage, https://github.com/MIT-LCP/physionet
 Project-URL: repository, https://github.com/MIT-LCP/physionet
 Author-email: Tom Pollard <tpollard@mit.edu>
 License: The MIT License (MIT)
         
         Copyright (c) Tom Pollard
```

