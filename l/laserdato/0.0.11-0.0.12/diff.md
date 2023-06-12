# Comparing `tmp/laserdato-0.0.11.tar.gz` & `tmp/laserdato-0.0.12.tar.gz`

## Comparing `laserdato-0.0.11.tar` & `laserdato-0.0.12.tar`

### file list

```diff
@@ -1,18 +1,13 @@
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 laserdato-0.0.11/main.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.0.11/laserdato/__init__.py
--rw-r--r--   0        0        0    20534 2020-02-02 00:00:00.000000 laserdato-0.0.11/laserdato/embed.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 laserdato-0.0.11/laserdato/get_model.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 laserdato-0.0.11/laserdato/laser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.0.11/laserdato/lib/__init__.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 laserdato-0.0.11/laserdato/lib/text_processing.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.0.11/settings.json/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.0.11/src/laserdato/__init__.py
--rw-r--r--   0        0        0    20564 2020-02-02 00:00:00.000000 laserdato-0.0.11/src/laserdato/embed.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 laserdato-0.0.11/src/laserdato/get_model.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 laserdato-0.0.11/src/laserdato/laser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.0.11/src/laserdato/lib/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 laserdato-0.0.11/src/laserdato/lib/text_processing.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.0.11/LICENSE
--rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 laserdato-0.0.11/README.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 laserdato-0.0.11/pyproject.toml
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 laserdato-0.0.11/PKG-INFO
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 laserdato-0.0.12/main.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/__init__.py
+-rw-r--r--   0        0        0    20534 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/embed.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/get_model.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/laser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/lib/__init__.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/lib/constants.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 laserdato-0.0.12/laserdato/lib/text_processing.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 laserdato-0.0.12/settings.json/settings.json
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 laserdato-0.0.12/LICENSE
+-rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 laserdato-0.0.12/README.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 laserdato-0.0.12/pyproject.toml
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 laserdato-0.0.12/PKG-INFO
```

### Comparing `laserdato-0.0.11/laserdato/embed.py` & `laserdato-0.0.12/laserdato/embed.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.11/laserdato/get_model.py` & `laserdato-0.0.12/laserdato/get_model.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.11/laserdato/lib/text_processing.py` & `laserdato-0.0.12/laserdato/lib/text_processing.py`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.11/LICENSE` & `laserdato-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.11/README.md` & `laserdato-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `laserdato-0.0.11/pyproject.toml` & `laserdato-0.0.12/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "laserdato"
-version = "0.0.11"
+version = "0.0.12"
 authors = [
   { name="Lingua Custodia", email="" },
 ]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-requires-python = ">=3.7,<3.11"
+requires-python = ">=3.7"
 dependencies = [
   "torch~=2.0.1",
   "sentencepiece",
   "numpy",
   "requests",
   "ftfy",
   "mosestokenizer",
```

### Comparing `laserdato-0.0.11/PKG-INFO` & `laserdato-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: laserdato
-Version: 0.0.11
+Version: 0.0.12
 Summary: A small example package
 Author: Lingua Custodia
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Requires-Dist: fairseq
 Requires-Dist: ftfy
 Requires-Dist: mosestokenizer
 Requires-Dist: numpy
 Requires-Dist: requests
 Requires-Dist: sentencepiece
 Requires-Dist: torch~=2.0.1
```

