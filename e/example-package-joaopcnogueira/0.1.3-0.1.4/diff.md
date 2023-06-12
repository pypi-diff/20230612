# Comparing `tmp/example_package_joaopcnogueira-0.1.3.tar.gz` & `tmp/example_package_joaopcnogueira-0.1.4.tar.gz`

## Comparing `example_package_joaopcnogueira-0.1.3.tar` & `example_package_joaopcnogueira-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/.DS_Store
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/example_package_joaopcnogueira/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/example_package_joaopcnogueira/example.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/notebooks/test_example.ipynb
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/tests/test_example.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/.gitignore
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/README.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/.DS_Store
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/example_package_joaopcnogueira/__init__.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/example_package_joaopcnogueira/__main__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/example_package_joaopcnogueira/example.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/notebooks/test_example.ipynb
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/tests/test_example.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.4/PKG-INFO
```

### Comparing `example_package_joaopcnogueira-0.1.3/.DS_Store` & `example_package_joaopcnogueira-0.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.3/notebooks/test_example.ipynb` & `example_package_joaopcnogueira-0.1.4/notebooks/test_example.ipynb`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.3/.gitignore` & `example_package_joaopcnogueira-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.3/README.md` & `example_package_joaopcnogueira-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 # Usage
 ```python
 from example_package_joaopcnogueira import example
 
 example.add_one(10)
 ```
 
+for the CLI interface, just go:
+```bash
+$ python -m example_package_joaopcnogueira --add-two 20
+```
+
 # Package Structure
 
 > `example_package_joaopcnogueira/`
 - The package folder, within it there is the python modules.
 
 > `example_package_joaopcnogueira/__init__.py`
 - File that indicates that the folder `example_package_joaopcnogueira` is a package
```

### Comparing `example_package_joaopcnogueira-0.1.3/pyproject.toml` & `example_package_joaopcnogueira-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "example_package_joaopcnogueira"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="João Nogueira", email="joaopcnogueira@gmail.com" },
   { name="Denise Vitoriano", email="denisevitoriano@gmail.com"}
 ]
 description = "A small example package"
 readme = "README.md"
 license = "MIT"
@@ -26,9 +26,12 @@
 [project.optional-dependencies]
 dev = [
     'pytest',
     'twine',
     'build',
 ]
 
+[project.scripts]
+example_cli_command = "example_package_joaopcnogueira.__main__:main"
+
 [project.urls]
 "Homepage" = "https://github.com/joaopcnogueira/packaging_tutorial"
```

### Comparing `example_package_joaopcnogueira-0.1.3/PKG-INFO` & `example_package_joaopcnogueira-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_joaopcnogueira
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small example package
 Project-URL: Homepage, https://github.com/joaopcnogueira/packaging_tutorial
 Author-email: João Nogueira <joaopcnogueira@gmail.com>, Denise Vitoriano <denisevitoriano@gmail.com>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -54,14 +54,19 @@
 # Usage
 ```python
 from example_package_joaopcnogueira import example
 
 example.add_one(10)
 ```
 
+for the CLI interface, just go:
+```bash
+$ python -m example_package_joaopcnogueira --add-two 20
+```
+
 # Package Structure
 
 > `example_package_joaopcnogueira/`
 - The package folder, within it there is the python modules.
 
 > `example_package_joaopcnogueira/__init__.py`
 - File that indicates that the folder `example_package_joaopcnogueira` is a package
```

