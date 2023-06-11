# Comparing `tmp/corgy-9.1.5.tar.gz` & `tmp/corgy-9.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-9.1.5.tar", max compression
+gzip compressed data, was "corgy-9.1.6.tar", max compression
```

## Comparing `corgy-9.1.5.tar` & `corgy-9.1.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    32535 2023-06-11 23:34:28.979814 corgy-9.1.5/CHANGELOG.md
--rw-r--r--   0        0        0     1077 2023-06-11 23:34:28.979814 corgy-9.1.5/LICENSE
--rw-r--r--   0        0        0     4020 2023-06-11 23:34:28.979814 corgy-9.1.5/README.md
--rw-r--r--   0        0        0      468 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/_annotations.py
--rw-r--r--   0        0        0    53646 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/_corgy.py
--rw-r--r--   0        0        0     3202 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/_corgychecker.py
--rw-r--r--   0        0        0     6237 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/_corgyparser.py
--rw-r--r--   0        0        0    37670 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/_helpfmt.py
--rw-r--r--   0        0        0    19746 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-06-11 23:35:06.295934 corgy-9.1.5/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/py.typed
--rw-r--r--   0        0        0     1598 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/types/__init__.py
--rw-r--r--   0        0        0     2382 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/types/_expand.py
--rw-r--r--   0        0        0     3750 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-06-11 23:34:28.979814 corgy-9.1.5/corgy/types/_subclass.py
--rw-r--r--   0        0        0    36201 2023-06-11 23:34:28.979814 corgy-9.1.5/docs/corgy.md
--rw-r--r--   0        0        0    11884 2023-06-11 23:34:28.979814 corgy-9.1.5/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-06-11 23:34:28.979814 corgy-9.1.5/docs/index.md
--rw-r--r--   0        0        0       82 2023-06-11 23:34:28.979814 corgy-9.1.5/docs/www/usage/corgy.md
--rw-r--r--   0        0        0      389 2023-06-11 23:34:28.979814 corgy-9.1.5/docs/www/usage/corgy.types.md
--rw-r--r--   0        0        0     2843 2023-06-11 23:35:06.295934 corgy-9.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/__init__.py
--rw-r--r--   0        0        0    94529 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/test_corgy.py
--rw-r--r--   0        0        0     4753 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/test_corgychecker.py
--rw-r--r--   0        0        0    20305 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/test_corgyparser.py
--rw-r--r--   0        0        0      800 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/test_doctests.py
--rw-r--r--   0        0        0    49021 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/types/_test_file.py
--rw-r--r--   0        0        0     2678 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5122 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-06-11 23:34:28.983814 corgy-9.1.5/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 corgy-9.1.5/PKG-INFO
+-rw-r--r--   0        0        0    32626 2023-06-11 23:39:07.119833 corgy-9.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1077 2023-06-11 23:39:07.119833 corgy-9.1.6/LICENSE
+-rw-r--r--   0        0        0     4020 2023-06-11 23:39:07.119833 corgy-9.1.6/README.md
+-rw-r--r--   0        0        0      468 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/_annotations.py
+-rw-r--r--   0        0        0    53646 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/_corgy.py
+-rw-r--r--   0        0        0     3202 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/_corgychecker.py
+-rw-r--r--   0        0        0     6237 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    37670 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    19746 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-06-11 23:39:49.457402 corgy-9.1.6/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-06-11 23:39:07.119833 corgy-9.1.6/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-11 23:39:07.123833 corgy-9.1.6/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3750 2023-06-11 23:39:07.123833 corgy-9.1.6/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-06-11 23:39:07.123833 corgy-9.1.6/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-06-11 23:39:07.123833 corgy-9.1.6/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-06-11 23:39:07.123833 corgy-9.1.6/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-06-11 23:39:07.123833 corgy-9.1.6/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    36201 2023-06-11 23:39:07.123833 corgy-9.1.6/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-06-11 23:39:07.123833 corgy-9.1.6/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-06-11 23:39:07.123833 corgy-9.1.6/docs/index.md
+-rw-r--r--   0        0        0       82 2023-06-11 23:39:07.123833 corgy-9.1.6/docs/www/usage/corgy.md
+-rw-r--r--   0        0        0      389 2023-06-11 23:39:07.123833 corgy-9.1.6/docs/www/usage/corgy.types.md
+-rw-r--r--   0        0        0     2843 2023-06-11 23:39:49.453402 corgy-9.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/__init__.py
+-rw-r--r--   0        0        0    94529 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/test_corgy.py
+-rw-r--r--   0        0        0     4753 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/test_corgychecker.py
+-rw-r--r--   0        0        0    20305 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      800 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/test_doctests.py
+-rw-r--r--   0        0        0    49021 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-06-11 23:39:07.123833 corgy-9.1.6/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 corgy-9.1.6/PKG-INFO
```

### Comparing `corgy-9.1.5/CHANGELOG.md` & `corgy-9.1.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [9.1.6](https://github.com/jayanthkoushik/corgy/compare/v9.1.5...v9.1.6) (2023-06-11)
+
 ### [9.1.5](https://github.com/jayanthkoushik/corgy/compare/v9.1.4...v9.1.5) (2023-06-11)
 
 ### [9.1.4](https://github.com/jayanthkoushik/corgy/compare/v9.1.3...v9.1.4) (2023-06-11)
 
 ### [9.1.3](https://github.com/jayanthkoushik/corgy/compare/v9.1.2...v9.1.3) (2023-06-11)
 
 ### [9.1.2](https://github.com/jayanthkoushik/corgy/compare/v9.1.1...v9.1.2) (2023-06-11)
```

### Comparing `corgy-9.1.5/LICENSE` & `corgy-9.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/README.md` & `corgy-9.1.6/README.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/_actions.py` & `corgy-9.1.6/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/_corgy.py` & `corgy-9.1.6/corgy/_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/_corgychecker.py` & `corgy-9.1.6/corgy/_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/_corgyparser.py` & `corgy-9.1.6/corgy/_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/_helpfmt.py` & `corgy-9.1.6/corgy/_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/_meta.py` & `corgy-9.1.6/corgy/_meta.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/types/__init__.py` & `corgy-9.1.6/corgy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/types/_expand.py` & `corgy-9.1.6/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/types/_initargs.py` & `corgy-9.1.6/corgy/types/_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/types/_inputfile.py` & `corgy-9.1.6/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/types/_keyvaluepairs.py` & `corgy-9.1.6/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/types/_outputfile.py` & `corgy-9.1.6/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/corgy/types/_subclass.py` & `corgy-9.1.6/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/docs/corgy.md` & `corgy-9.1.6/docs/corgy.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/docs/corgy.types.md` & `corgy-9.1.6/docs/corgy.types.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/pyproject.toml` & `corgy-9.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "9.1.5"  # managed by `poetry-dynamic-versioning`
+version = "9.1.6"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
```

### Comparing `corgy-9.1.5/tests/test_corgy.py` & `corgy-9.1.6/tests/test_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/test_corgychecker.py` & `corgy-9.1.6/tests/test_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/test_corgyparser.py` & `corgy-9.1.6/tests/test_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/test_doctests.py` & `corgy-9.1.6/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/test_helpfmt.py` & `corgy-9.1.6/tests/test_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/types/_specialtmps.py` & `corgy-9.1.6/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/types/_test_file.py` & `corgy-9.1.6/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/types/test_initargs.py` & `corgy-9.1.6/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/types/test_inputfiles.py` & `corgy-9.1.6/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/types/test_keyvaluepairs.py` & `corgy-9.1.6/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/types/test_outputfiles.py` & `corgy-9.1.6/tests/types/test_outputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/tests/types/test_subclass.py` & `corgy-9.1.6/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.5/PKG-INFO` & `corgy-9.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 9.1.5
+Version: 9.1.6
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
```

