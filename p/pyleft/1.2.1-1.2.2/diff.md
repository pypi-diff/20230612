# Comparing `tmp/pyleft-1.2.1.tar.gz` & `tmp/pyleft-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyleft-1.2.1.tar", max compression
+gzip compressed data, was "pyleft-1.2.2.tar", max compression
```

## Comparing `pyleft-1.2.1.tar` & `pyleft-1.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-24 04:09:47.529989 pyleft-1.2.1/LICENSE
--rw-r--r--   0        0        0     4274 2023-05-24 04:09:47.529989 pyleft-1.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-24 04:09:47.529989 pyleft-1.2.1/pyleft/__init__.py
--rw-r--r--   0        0        0       37 2023-05-24 04:09:47.529989 pyleft-1.2.1/pyleft/__main__.py
--rw-r--r--   0        0        0     6228 2023-05-24 04:09:47.529989 pyleft-1.2.1/pyleft/api.py
--rw-r--r--   0        0        0      539 2023-05-24 04:09:47.529989 pyleft-1.2.1/pyleft/console.py
--rw-r--r--   0        0        0      276 2023-05-24 04:09:47.529989 pyleft-1.2.1/pyleft/models.py
--rw-r--r--   0        0        0     1880 2023-05-24 04:09:47.529989 pyleft-1.2.1/pyleft/path_utils.py
--rw-r--r--   0        0        0      474 2023-05-24 04:09:47.529989 pyleft-1.2.1/pyleft/printing.py
--rw-r--r--   0        0        0     8758 2023-05-24 04:09:47.529989 pyleft-1.2.1/pyleft/settings.py
--rw-r--r--   0        0        0     1353 2023-05-24 04:09:47.529989 pyleft-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 pyleft-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-12 21:49:27.879779 pyleft-1.2.2/LICENSE
+-rw-r--r--   0        0        0     4264 2023-06-12 21:49:27.879779 pyleft-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 21:49:27.879779 pyleft-1.2.2/pyleft/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-12 21:49:27.879779 pyleft-1.2.2/pyleft/__main__.py
+-rw-r--r--   0        0        0     6228 2023-06-12 21:49:27.879779 pyleft-1.2.2/pyleft/api.py
+-rw-r--r--   0        0        0      539 2023-06-12 21:49:27.879779 pyleft-1.2.2/pyleft/console.py
+-rw-r--r--   0        0        0      276 2023-06-12 21:49:27.883779 pyleft-1.2.2/pyleft/models.py
+-rw-r--r--   0        0        0     1880 2023-06-12 21:49:27.883779 pyleft-1.2.2/pyleft/path_utils.py
+-rw-r--r--   0        0        0      474 2023-06-12 21:49:27.883779 pyleft-1.2.2/pyleft/printing.py
+-rw-r--r--   0        0        0     8706 2023-06-12 21:49:27.883779 pyleft-1.2.2/pyleft/settings.py
+-rw-r--r--   0        0        0     1353 2023-06-12 21:49:27.883779 pyleft-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 pyleft-1.2.2/PKG-INFO
```

### Comparing `pyleft-1.2.1/LICENSE` & `pyleft-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyleft-1.2.1/README.md` & `pyleft-1.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 `pip install pyleft`
 
 ## Usage
 
 PyLeft is a Python module that can be run via `python -m`. Just provide the directories
 or files to recursively check.
 
-`python -m pyleft .`
+`pyleft .`
 
 The module will exit with an exit code of 0 if all type hints are present, or 1
 if there are any issues.
 
 ### Example
 
 ```bash
```

### Comparing `pyleft-1.2.1/pyleft/api.py` & `pyleft-1.2.2/pyleft/api.py`

 * *Files identical despite different names*

### Comparing `pyleft-1.2.1/pyleft/console.py` & `pyleft-1.2.2/pyleft/console.py`

 * *Files identical despite different names*

### Comparing `pyleft-1.2.1/pyleft/path_utils.py` & `pyleft-1.2.2/pyleft/path_utils.py`

 * *Files identical despite different names*

### Comparing `pyleft-1.2.1/pyleft/settings.py` & `pyleft-1.2.2/pyleft/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,25 +78,24 @@
                 all_files.add(raw_path_obj)
 
             # if it's a directory, find all python files inside
             if raw_path_obj.is_dir():
                 all_files.update(raw_path_obj.glob("**/*.py"))
                 all_files.update(raw_path_obj.glob("**/*.pyi"))
 
-        # make all paths absolute
-        all_files = set(a.absolute() for a in all_files)
+        # make all paths absolute and remove directories
+        all_files = {a.absolute() for a in all_files if a.is_file()}
 
         # if a .pyi file exists alongside a .py file, remove the .py file
         all_files = {
             f
             for f in all_files
             if f.name.endswith(".pyi")
-            or (
-                f.name.endswith(".py") and Path(f.parent, f.name + "i") not in all_files
-            )
+            or f.name.endswith(".py")
+            and Path(f.parent, f"{f.name}i") not in all_files
         }
 
         return all_files
 
     @property
     def files(self) -> Set[Path]:
         """
@@ -104,21 +103,17 @@
         have been applied.
         """
         exclusions = self.load_exclusions()
         all_files = self.load_files()
 
         # iterate through all of the files
         # if no matches found, add it to final output
-        return set(
-            [
-                f
-                for f in all_files
-                if not check_if_file_matches_exclusions(f, exclusions)
-            ]
-        )
+        return {
+            f for f in all_files if not check_if_file_matches_exclusions(f, exclusions)
+        }
 
     @property
     def no_gitignore(self) -> bool:
         return self._no_gitignore
 
     @property
     def ignore_if_has_default(self) -> bool:
```

### Comparing `pyleft-1.2.1/pyproject.toml` & `pyleft-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "pyleft"
-    version = "1.2.1"
+    version = "1.2.2"
     description = "Python type annotation existence checker"
     license = "MIT"
     readme = "README.md"
     homepage = "https://github.com/NathanVaughn/pyleft"
     repository = "https://github.com/NathanVaughn/pyleft.git"
     authors = ["Nathan Vaughn <nvaughn51@gmail.com>"]
     classifiers = [
```

### Comparing `pyleft-1.2.1/PKG-INFO` & `pyleft-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyleft
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python type annotation existence checker
 Home-page: https://github.com/NathanVaughn/pyleft
 License: MIT
 Author: Nathan Vaughn
 Author-email: nvaughn51@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -49,15 +49,15 @@
 `pip install pyleft`
 
 ## Usage
 
 PyLeft is a Python module that can be run via `python -m`. Just provide the directories
 or files to recursively check.
 
-`python -m pyleft .`
+`pyleft .`
 
 The module will exit with an exit code of 0 if all type hints are present, or 1
 if there are any issues.
 
 ### Example
 
 ```bash
```

