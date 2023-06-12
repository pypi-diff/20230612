# Comparing `tmp/mwiszenko-med-1.0.0.tar.gz` & `tmp/mwiszenko-med-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwiszenko-med-1.0.0.tar", last modified: Mon Jun 12 16:52:55 2023, max compression
+gzip compressed data, was "mwiszenko-med-1.0.1.tar", last modified: Mon Jun 12 17:09:42 2023, max compression
```

## Comparing `mwiszenko-med-1.0.0.tar` & `mwiszenko-med-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:52:55.341723 mwiszenko-med-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-12 16:52:55.341723 mwiszenko-med-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:52:55.341723 mwiszenko-med-1.0.0/med/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/med/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/med/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/med/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/med/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/med/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/med/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:52:55.341723 mwiszenko-med-1.0.0/mwiszenko_med.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-12 16:52:55.000000 mwiszenko-med-1.0.0/mwiszenko_med.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 16:52:55.000000 mwiszenko-med-1.0.0/mwiszenko_med.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:52:55.000000 mwiszenko-med-1.0.0/mwiszenko_med.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 16:52:55.000000 mwiszenko-med-1.0.0/mwiszenko_med.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 16:52:55.000000 mwiszenko-med-1.0.0/mwiszenko_med.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 16:52:55.000000 mwiszenko-med-1.0.0/mwiszenko_med.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:52:55.341723 mwiszenko-med-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:52:55.341723 mwiszenko-med-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:52:55.341723 mwiszenko-med-1.0.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/tests/data/empty.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 16:52:45.000000 mwiszenko-med-1.0.0/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:09:42.090967 mwiszenko-med-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-12 17:09:42.090967 mwiszenko-med-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:09:42.090967 mwiszenko-med-1.0.1/med/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/med/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/med/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/med/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/med/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/med/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/med/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:09:42.090967 mwiszenko-med-1.0.1/mwiszenko_med.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-12 17:09:42.000000 mwiszenko-med-1.0.1/mwiszenko_med.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 17:09:42.000000 mwiszenko-med-1.0.1/mwiszenko_med.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:09:42.000000 mwiszenko-med-1.0.1/mwiszenko_med.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 17:09:42.000000 mwiszenko-med-1.0.1/mwiszenko_med.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 17:09:42.000000 mwiszenko-med-1.0.1/mwiszenko_med.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 17:09:42.000000 mwiszenko-med-1.0.1/mwiszenko_med.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:09:42.090967 mwiszenko-med-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:09:42.090967 mwiszenko-med-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:09:42.090967 mwiszenko-med-1.0.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/tests/data/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 17:09:30.000000 mwiszenko-med-1.0.1/tests/test_constants.py
```

### Comparing `mwiszenko-med-1.0.0/HISTORY.md` & `mwiszenko-med-1.0.1/HISTORY.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Merge pull request #8 from mwiszenko/hotfix. [Michał Wiszenko]
+
+  Fix error handling on loading data
+- Fix error handling on loading data. [Michał Wiszenko]
+
+
+1.0.0 (2023-06-12)
+------------------
+- Release: version 1.0.0 🚀 [Michał Wiszenko]
 - Merge pull request #7 from mwiszenko/hotfix. [Michał Wiszenko]
 
   Fix imports, reformat
 - Fix imports. [Michał Wiszenko]
 - Merge pull request #6 from mwiszenko/research. [Michał Wiszenko]
 
   Add test mode for averaging time of execution
```

### Comparing `mwiszenko-med-1.0.0/LICENSE` & `mwiszenko-med-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mwiszenko-med-1.0.0/PKG-INFO` & `mwiszenko-med-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwiszenko-med
-Version: 1.0.0
+Version: 1.0.1
 Summary: Awesome med created by mwiszenko
 Home-page: https://github.com/mwiszenko/MED/
 Author: mwiszenko
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `mwiszenko-med-1.0.0/README.md` & `mwiszenko-med-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mwiszenko-med-1.0.0/med/base.py` & `mwiszenko-med-1.0.1/med/base.py`

 * *Files identical despite different names*

### Comparing `mwiszenko-med-1.0.0/med/cli.py` & `mwiszenko-med-1.0.1/med/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 class ModeMapper:
     def __init__(self) -> None:
         pass
 
     @staticmethod
     def run(args):
         ds: DataSet = read_sequence_file(filename=args.input)
+        if len(ds) == 0:
+            print("Data could not be loaded properly.")
+            exit(1)
 
         min_sup: float
         if args.min_sup is not None:
             min_sup = args.min_sup
         else:
             min_sup = args.min_sup_percentage * len(ds)
         res: dict[Sequence, int] = prefix_span(
@@ -73,14 +76,17 @@
         else:
             print(number_of_found_sequences)
             print(found_sequences)
 
     @staticmethod
     def test(args):
         ds: DataSet = read_sequence_file(filename=args.input)
+        if len(ds) == 0:
+            print("Data could not be loaded properly.")
+            exit(1)
 
         min_sup: float
         if args.min_sup is not None:
             min_sup = args.min_sup
         else:
             min_sup = args.min_sup_percentage * len(ds)
```

### Comparing `mwiszenko-med-1.0.0/mwiszenko_med.egg-info/PKG-INFO` & `mwiszenko-med-1.0.1/mwiszenko_med.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwiszenko-med
-Version: 1.0.0
+Version: 1.0.1
 Summary: Awesome med created by mwiszenko
 Home-page: https://github.com/mwiszenko/MED/
 Author: mwiszenko
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `mwiszenko-med-1.0.0/setup.py` & `mwiszenko-med-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `mwiszenko-med-1.0.0/tests/test_cli.py` & `mwiszenko-med-1.0.1/tests/test_cli.py`

 * *Files identical despite different names*

