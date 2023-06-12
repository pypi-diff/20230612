# Comparing `tmp/processors-0.0.1.tar.gz` & `tmp/processors-0.0.2.tar.gz`

## Comparing `processors-0.0.1.tar` & `processors-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 processors-0.0.1/src/processors/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 processors-0.0.1/src/processors/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 processors-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 processors-0.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 processors-0.0.1/LICENSE
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 processors-0.0.1/README.md
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 processors-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 processors-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 processors-0.0.2/src/processors/__about__.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 processors-0.0.2/src/processors/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 processors-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 processors-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 processors-0.0.2/LICENSE
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 processors-0.0.2/README.md
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 processors-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 processors-0.0.2/PKG-INFO
```

### Comparing `processors-0.0.1/.gitignore` & `processors-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `processors-0.0.1/LICENSE` & `processors-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `processors-0.0.1/README.md` & `processors-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `processors-0.0.1/pyproject.toml` & `processors-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dynamic = ["version"]
 description = 'Data processors'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
-  { name = "fenke meijer", email = "fenke@live.com" },
+  { name = "fenke meijer", email = "fenkemeijer@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
```

### Comparing `processors-0.0.1/PKG-INFO` & `processors-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: processors
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data processors
 Project-URL: Documentation, https://github.com/fenke/processors#readme
 Project-URL: Issues, https://github.com/fenke/processors/issues
 Project-URL: Source, https://github.com/fenke/processors
-Author-email: fenke meijer <fenke@live.com>
+Author-email: fenke meijer <fenkemeijer@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

