# Comparing `tmp/example_package_joaopcnogueira-0.1.2.tar.gz` & `tmp/example_package_joaopcnogueira-0.1.3.tar.gz`

## Comparing `example_package_joaopcnogueira-0.1.2.tar` & `example_package_joaopcnogueira-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/.DS_Store
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/example_package_joaopcnogueira/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/example_package_joaopcnogueira/example.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/notebooks/test_example.ipynb
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/tests/test_example.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/.gitignore
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/README.md
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/.DS_Store
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/example_package_joaopcnogueira/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/example_package_joaopcnogueira/example.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/notebooks/test_example.ipynb
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/tests/test_example.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/README.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 example_package_joaopcnogueira-0.1.3/PKG-INFO
```

### Comparing `example_package_joaopcnogueira-0.1.2/.DS_Store` & `example_package_joaopcnogueira-0.1.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.2/notebooks/test_example.ipynb` & `example_package_joaopcnogueira-0.1.3/notebooks/test_example.ipynb`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.2/.gitignore` & `example_package_joaopcnogueira-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.2/README.md` & `example_package_joaopcnogueira-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `example_package_joaopcnogueira-0.1.2/pyproject.toml` & `example_package_joaopcnogueira-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "example_package_joaopcnogueira"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="João Nogueira", email="joaopcnogueira@gmail.com" },
   { name="Denise Vitoriano", email="denisevitoriano@gmail.com"}
 ]
 description = "A small example package"
 readme = "README.md"
 license = "MIT"
@@ -19,10 +19,16 @@
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[project.optional-dependencies]
+dev = [
+    'pytest',
+    'twine',
+    'build',
+]
+
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Homepage" = "https://github.com/joaopcnogueira/packaging_tutorial"
```

### Comparing `example_package_joaopcnogueira-0.1.2/PKG-INFO` & `example_package_joaopcnogueira-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: example_package_joaopcnogueira
-Version: 0.1.2
+Version: 0.1.3
 Summary: A small example package
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/joaopcnogueira/packaging_tutorial
 Author-email: João Nogueira <joaopcnogueira@gmail.com>, Denise Vitoriano <denisevitoriano@gmail.com>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy
 Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Example Package
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
```

