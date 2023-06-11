# Comparing `tmp/crackerjack-0.2.7.tar.gz` & `tmp/crackerjack-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.2.7.tar", last modified: Sun Jun 11 22:07:10 2023, max compression
+gzip compressed data, was "crackerjack-0.2.8.tar", last modified: Sun Jun 11 22:09:49 2023, max compression
```

## Comparing `crackerjack-0.2.7.tar` & `crackerjack-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.7/LICENSE
--rw-r--r--   0        0        0     3208 2023-06-02 09:59:18.505246 crackerjack-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-06-11 22:06:40.546998 crackerjack-0.2.7/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      163 2023-06-11 22:06:40.502864 crackerjack-0.2.7/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-06-11 22:06:40.532706 crackerjack-0.2.7/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     1723 2023-06-11 22:06:40.517794 crackerjack-0.2.7/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.7/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.7/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.7/crackerjack/__init__.py
--rw-r--r--   0        0        0     1413 2023-06-10 14:55:58.374530 crackerjack-0.2.7/crackerjack/__main__.py
--rw-r--r--   0        0        0     5385 2023-06-11 22:03:26.544834 crackerjack-0.2.7/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1595 2023-06-11 22:06:41.292877 crackerjack-0.2.7/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     1595 2023-06-11 22:07:10.112891 crackerjack-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 crackerjack-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3208 2023-06-02 09:59:18.505246 crackerjack-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 22:09:20.352667 crackerjack-0.2.8/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      163 2023-06-11 22:09:20.309862 crackerjack-0.2.8/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-06-11 22:09:20.338943 crackerjack-0.2.8/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     1723 2023-06-11 22:09:20.324823 crackerjack-0.2.8/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.8/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.8/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.8/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1413 2023-06-10 14:55:58.374530 crackerjack-0.2.8/crackerjack/__main__.py
+-rw-r--r--   0        0        0     5385 2023-06-11 22:08:22.602288 crackerjack-0.2.8/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1595 2023-06-11 22:09:21.088264 crackerjack-0.2.8/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     1595 2023-06-11 22:09:49.451160 crackerjack-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 crackerjack-0.2.8/PKG-INFO
```

### Comparing `crackerjack-0.2.7/LICENSE` & `crackerjack-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.7/README.md` & `crackerjack-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.7/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.2.8/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.7/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.2.8/crackerjack/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.7/crackerjack/__main__.py` & `crackerjack-0.2.8/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.7/crackerjack/crackerjack.py` & `crackerjack-0.2.8/crackerjack/crackerjack.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,12 +131,12 @@
         check_all = call(["pre-commit", "run", "--all-files"])
         if check_all > 0:
             call(["pre-commit", "run", "--all-files"])
         if options.publish:
             run(["pdm", "publish"])
         if options.commit:
             commit_msg = input("Commit message: ")
-            call(["git", "commit", "-m", f"'{commit_msg}'", "--", ".", "--no-verify"])
+            call(["git", "commit", "-m", f"'{commit_msg}'", "--no-verify", "--", "."])
             call(["git", "push", "origin", "main"])
 
 
 crackerjack_it = Crakerjack().process
```

### Comparing `crackerjack-0.2.7/crackerjack/pyproject.toml` & `crackerjack-0.2.8/crackerjack/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.2.7"
+version = "0.2.8"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.2.7/pyproject.toml` & `crackerjack-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.2.7"
+version = "0.2.8"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.2.7/PKG-INFO` & `crackerjack-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.2.7
+Version: 0.2.8
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
```

