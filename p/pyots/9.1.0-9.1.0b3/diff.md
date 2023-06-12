# Comparing `tmp/pyots-9.1.0.tar.gz` & `tmp/pyots-9.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyots-9.1.0.tar", last modified: Mon Jun 12 19:36:49 2023, max compression
+gzip compressed data, was "pyots-9.1.0b3.tar", last modified: Mon Jun 12 19:22:12 2023, max compression
```

## Comparing `pyots-9.1.0.tar` & `pyots-9.1.0b3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:36:49.853398 pyots-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 19:33:20.000000 pyots-9.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:36:49.849398 pyots-9.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:36:49.853398 pyots-9.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-12 19:33:20.000000 pyots-9.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 19:33:20.000000 pyots-9.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:36:49.853398 pyots-9.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-12 19:33:20.000000 pyots-9.1.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-12 19:33:20.000000 pyots-9.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-12 19:33:20.000000 pyots-9.1.0/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-12 19:33:20.000000 pyots-9.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-12 19:33:20.000000 pyots-9.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-12 19:36:49.853398 pyots-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-12 19:33:20.000000 pyots-9.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-12 19:33:20.000000 pyots-9.1.0/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-12 19:33:20.000000 pyots-9.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 19:33:20.000000 pyots-9.1.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 19:33:20.000000 pyots-9.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 19:36:49.853398 pyots-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-12 19:33:20.000000 pyots-9.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:36:49.849398 pyots-9.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:36:49.853398 pyots-9.1.0/src/_pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-12 19:33:20.000000 pyots-9.1.0/src/_pyots/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-12 19:33:20.000000 pyots-9.1.0/src/_pyots/pyots-context.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:36:49.853398 pyots-9.1.0/src/pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-12 19:33:20.000000 pyots-9.1.0/src/pyots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:36:49.853398 pyots-9.1.0/src/pyots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-12 19:36:49.000000 pyots-9.1.0/src/pyots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-12 19:36:49.000000 pyots-9.1.0/src/pyots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:36:49.000000 pyots-9.1.0/src/pyots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:36:49.000000 pyots-9.1.0/src/pyots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 19:36:49.000000 pyots-9.1.0/src/pyots.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:36:49.853398 pyots-9.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-12 19:33:20.000000 pyots-9.1.0/tests/test_compare_ots_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-12 19:33:20.000000 pyots-9.1.0/tests/test_ots_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.134186 pyots-9.1.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-12 19:18:42.000000 pyots-9.1.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-12 19:18:42.000000 pyots-9.1.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-12 19:22:12.134186 pyots-9.1.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-12 19:18:42.000000 pyots-9.1.0b3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-12 19:18:42.000000 pyots-9.1.0b3/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-12 19:18:42.000000 pyots-9.1.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 19:18:42.000000 pyots-9.1.0b3/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 19:18:42.000000 pyots-9.1.0b3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 19:22:12.134186 pyots-9.1.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-12 19:18:42.000000 pyots-9.1.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/src/_pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-12 19:18:42.000000 pyots-9.1.0b3/src/_pyots/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-12 19:18:42.000000 pyots-9.1.0b3/src/_pyots/pyots-context.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.130186 pyots-9.1.0b3/src/pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-12 19:18:42.000000 pyots-9.1.0b3/src/pyots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.134186 pyots-9.1.0b3/src/pyots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-12 19:22:11.000000 pyots-9.1.0b3/src/pyots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-12 19:22:12.000000 pyots-9.1.0b3/src/pyots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:22:11.000000 pyots-9.1.0b3/src/pyots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:22:11.000000 pyots-9.1.0b3/src/pyots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 19:22:11.000000 pyots-9.1.0b3/src/pyots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:22:12.134186 pyots-9.1.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-12 19:18:42.000000 pyots-9.1.0b3/tests/test_compare_ots_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-12 19:18:42.000000 pyots-9.1.0b3/tests/test_ots_suite.py
```

### Comparing `pyots-9.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `pyots-9.1.0b3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pyots-9.1.0b3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/.github/workflows/codeql.yml` & `pyots-9.1.0b3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/.github/workflows/release.yml` & `pyots-9.1.0b3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/.github/workflows/run_tests.yml` & `pyots-9.1.0b3/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/.gitignore` & `pyots-9.1.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/LICENSE` & `pyots-9.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/PKG-INFO` & `pyots-9.1.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0
+Version: 9.1.0b3
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyots-9.1.0/README.md` & `pyots-9.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/build.py` & `pyots-9.1.0b3/build.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/setup.py` & `pyots-9.1.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/src/_pyots/bindings.cpp` & `pyots-9.1.0b3/src/_pyots/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/src/_pyots/pyots-context.h` & `pyots-9.1.0b3/src/_pyots/pyots-context.h`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/src/pyots/__init__.py` & `pyots-9.1.0b3/src/pyots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/src/pyots.egg-info/PKG-INFO` & `pyots-9.1.0b3/src/pyots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0
+Version: 9.1.0b3
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyots-9.1.0/src/pyots.egg-info/SOURCES.txt` & `pyots-9.1.0b3/src/pyots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/tests/test_compare_ots_python.py` & `pyots-9.1.0b3/tests/test_compare_ots_python.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0/tests/test_ots_suite.py` & `pyots-9.1.0b3/tests/test_ots_suite.py`

 * *Files identical despite different names*

