# Comparing `tmp/example_package_joaopcnogueira-0.1.1.tar.gz` & `tmp/example_package_joaopcnogueira-0.1.2.tar.gz`

## Comparing `example_package_joaopcnogueira-0.1.1.tar` & `example_package_joaopcnogueira-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/.DS_Store
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/example_package_joaopcnogueira/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/example_package_joaopcnogueira/example.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/notebooks/test_example.ipynb
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/tests/test_example.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/.gitignore
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/README.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/.DS_Store
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/example_package_joaopcnogueira/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/example_package_joaopcnogueira/example.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/notebooks/test_example.ipynb
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/tests/test_example.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/README.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/PKG-INFO
```

### Comparing `example_package_joaopcnogueira-0.1.1/.DS_Store` & `example_package_joaopcnogueira-0.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.1/notebooks/test_example.ipynb` & `example_package_joaopcnogueira-0.1.2/notebooks/test_example.ipynb`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.1/.gitignore` & `example_package_joaopcnogueira-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.1/README.md` & `example_package_joaopcnogueira-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.1/pyproject.toml` & `example_package_joaopcnogueira-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "example_package_joaopcnogueira"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="João Nogueira", email="joaopcnogueira@gmail.com" },
   { name="Denise Vitoriano", email="denisevitoriano@gmail.com"}
 ]
 description = "A small example package"
 readme = "README.md"
 license = "MIT"
```

### Comparing `example_package_joaopcnogueira-0.1.1/PKG-INFO` & `example_package_joaopcnogueira-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_joaopcnogueira
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small example package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: João Nogueira <joaopcnogueira@gmail.com>, Denise Vitoriano <denisevitoriano@gmail.com>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

