# Comparing `tmp/corgy-9.1.2.tar.gz` & `tmp/corgy-9.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-9.1.2.tar", max compression
+gzip compressed data, was "corgy-9.1.3.tar", max compression
```

## Comparing `corgy-9.1.2.tar` & `corgy-9.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    32262 2023-06-11 23:23:51.214913 corgy-9.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1077 2023-06-11 23:23:51.214913 corgy-9.1.2/LICENSE
--rw-r--r--   0        0        0     4020 2023-06-11 23:23:51.214913 corgy-9.1.2/README.md
--rw-r--r--   0        0        0      468 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_annotations.py
--rw-r--r--   0        0        0    53646 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_corgy.py
--rw-r--r--   0        0        0     3202 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_corgychecker.py
--rw-r--r--   0        0        0     6237 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_corgyparser.py
--rw-r--r--   0        0        0    37670 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_helpfmt.py
--rw-r--r--   0        0        0    19746 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-06-11 23:24:33.410706 corgy-9.1.2/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/py.typed
--rw-r--r--   0        0        0     1598 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/__init__.py
--rw-r--r--   0        0        0     2382 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_expand.py
--rw-r--r--   0        0        0     3750 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-06-11 23:23:51.214913 corgy-9.1.2/corgy/types/_subclass.py
--rw-r--r--   0        0        0    36201 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/corgy.md
--rw-r--r--   0        0        0    11884 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/index.md
--rw-r--r--   0        0        0       82 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/www/usage/corgy.md
--rw-r--r--   0        0        0      389 2023-06-11 23:23:51.214913 corgy-9.1.2/docs/www/usage/corgy.types.md
--rw-r--r--   0        0        0     2801 2023-06-11 23:24:33.410706 corgy-9.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/__init__.py
--rw-r--r--   0        0        0    94529 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/test_corgy.py
--rw-r--r--   0        0        0     4753 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/test_corgychecker.py
--rw-r--r--   0        0        0    20305 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/test_corgyparser.py
--rw-r--r--   0        0        0      800 2023-06-11 23:23:51.214913 corgy-9.1.2/tests/test_doctests.py
--rw-r--r--   0        0        0    49021 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/_test_file.py
--rw-r--r--   0        0        0     2678 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5122 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-06-11 23:23:51.218912 corgy-9.1.2/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 corgy-9.1.2/PKG-INFO
+-rw-r--r--   0        0        0    32353 2023-06-11 23:27:32.480168 corgy-9.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1077 2023-06-11 23:27:32.480168 corgy-9.1.3/LICENSE
+-rw-r--r--   0        0        0     4020 2023-06-11 23:27:32.480168 corgy-9.1.3/README.md
+-rw-r--r--   0        0        0      468 2023-06-11 23:27:32.480168 corgy-9.1.3/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-11 23:27:32.480168 corgy-9.1.3/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-06-11 23:27:32.480168 corgy-9.1.3/corgy/_annotations.py
+-rw-r--r--   0        0        0    53646 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/_corgy.py
+-rw-r--r--   0        0        0     3202 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/_corgychecker.py
+-rw-r--r--   0        0        0     6237 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    37670 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    19746 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-06-11 23:28:07.912755 corgy-9.1.3/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3750 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-06-11 23:27:32.484168 corgy-9.1.3/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    36201 2023-06-11 23:27:32.484168 corgy-9.1.3/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-06-11 23:27:32.484168 corgy-9.1.3/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-06-11 23:27:32.484168 corgy-9.1.3/docs/index.md
+-rw-r--r--   0        0        0       82 2023-06-11 23:27:32.484168 corgy-9.1.3/docs/www/usage/corgy.md
+-rw-r--r--   0        0        0      389 2023-06-11 23:27:32.484168 corgy-9.1.3/docs/www/usage/corgy.types.md
+-rw-r--r--   0        0        0     2801 2023-06-11 23:28:07.912755 corgy-9.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/__init__.py
+-rw-r--r--   0        0        0    94529 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/test_corgy.py
+-rw-r--r--   0        0        0     4753 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/test_corgychecker.py
+-rw-r--r--   0        0        0    20305 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      800 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/test_doctests.py
+-rw-r--r--   0        0        0    49021 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-06-11 23:27:32.484168 corgy-9.1.3/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 corgy-9.1.3/PKG-INFO
```

### Comparing `corgy-9.1.2/CHANGELOG.md` & `corgy-9.1.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [9.1.3](https://github.com/jayanthkoushik/corgy/compare/v9.1.2...v9.1.3) (2023-06-11)
+
 ### [9.1.2](https://github.com/jayanthkoushik/corgy/compare/v9.1.1...v9.1.2) (2023-06-11)
 
 ### [9.1.1](https://github.com/jayanthkoushik/corgy/compare/v9.1.0...v9.1.1) (2023-06-01)
 
 
 ### Bug Fixes
```

### Comparing `corgy-9.1.2/LICENSE` & `corgy-9.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/README.md` & `corgy-9.1.3/README.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/_actions.py` & `corgy-9.1.3/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/_corgy.py` & `corgy-9.1.3/corgy/_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/_corgychecker.py` & `corgy-9.1.3/corgy/_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/_corgyparser.py` & `corgy-9.1.3/corgy/_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/_helpfmt.py` & `corgy-9.1.3/corgy/_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/_meta.py` & `corgy-9.1.3/corgy/_meta.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/types/__init__.py` & `corgy-9.1.3/corgy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/types/_expand.py` & `corgy-9.1.3/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/types/_initargs.py` & `corgy-9.1.3/corgy/types/_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/types/_inputfile.py` & `corgy-9.1.3/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/types/_keyvaluepairs.py` & `corgy-9.1.3/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/types/_outputfile.py` & `corgy-9.1.3/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/corgy/types/_subclass.py` & `corgy-9.1.3/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/docs/corgy.md` & `corgy-9.1.3/docs/corgy.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/docs/corgy.types.md` & `corgy-9.1.3/docs/corgy.types.md`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/pyproject.toml` & `corgy-9.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "9.1.2"  # managed by `poetry-dynamic-versioning`
+version = "9.1.3"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
```

### Comparing `corgy-9.1.2/tests/test_corgy.py` & `corgy-9.1.3/tests/test_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/test_corgychecker.py` & `corgy-9.1.3/tests/test_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/test_corgyparser.py` & `corgy-9.1.3/tests/test_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/test_doctests.py` & `corgy-9.1.3/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/test_helpfmt.py` & `corgy-9.1.3/tests/test_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/types/_specialtmps.py` & `corgy-9.1.3/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/types/_test_file.py` & `corgy-9.1.3/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/types/test_initargs.py` & `corgy-9.1.3/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/types/test_inputfiles.py` & `corgy-9.1.3/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/types/test_keyvaluepairs.py` & `corgy-9.1.3/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/types/test_outputfiles.py` & `corgy-9.1.3/tests/types/test_outputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/tests/types/test_subclass.py` & `corgy-9.1.3/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-9.1.2/PKG-INFO` & `corgy-9.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 9.1.2
+Version: 9.1.3
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
```

