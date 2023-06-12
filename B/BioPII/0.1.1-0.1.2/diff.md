# Comparing `tmp/BioPII-0.1.1.tar.gz` & `tmp/BioPII-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioPII-0.1.1.tar", last modified: Mon Jun 12 04:43:25 2023, max compression
+gzip compressed data, was "BioPII-0.1.2.tar", last modified: Mon Jun 12 04:49:05 2023, max compression
```

## Comparing `BioPII-0.1.1.tar` & `BioPII-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:43:25.721450 BioPII-0.1.1/
-drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:43:25.721450 BioPII-0.1.1/BioPII.egg-info/
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      726 2023-06-12 04:43:25.000000 BioPII-0.1.1/BioPII.egg-info/PKG-INFO
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      182 2023-06-12 04:43:25.000000 BioPII-0.1.1/BioPII.egg-info/SOURCES.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        1 2023-06-12 04:43:25.000000 BioPII-0.1.1/BioPII.egg-info/dependency_links.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       40 2023-06-12 04:43:25.000000 BioPII-0.1.1/BioPII.egg-info/requires.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        1 2023-06-12 04:43:25.000000 BioPII-0.1.1/BioPII.egg-info/top_level.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      726 2023-06-12 04:43:25.721450 BioPII-0.1.1/PKG-INFO
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     2339 2023-06-11 00:53:51.000000 BioPII-0.1.1/README.md
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      581 2023-06-12 04:43:01.000000 BioPII-0.1.1/pyproject.toml
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       38 2023-06-12 04:43:25.721450 BioPII-0.1.1/setup.cfg
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      956 2023-06-12 04:43:09.000000 BioPII-0.1.1/setup.py
+drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:49:05.311740 BioPII-0.1.2/
+drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:49:05.311740 BioPII-0.1.2/BioPII.egg-info/
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      726 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/PKG-INFO
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      192 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/SOURCES.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        1 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/dependency_links.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       40 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/requires.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        7 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/top_level.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)    23892 2023-05-30 21:16:53.000000 BioPII-0.1.2/BioPII.py
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      726 2023-06-12 04:49:05.311740 BioPII-0.1.2/PKG-INFO
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     2339 2023-06-11 00:53:51.000000 BioPII-0.1.2/README.md
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      581 2023-06-12 04:48:08.000000 BioPII-0.1.2/pyproject.toml
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       38 2023-06-12 04:49:05.311740 BioPII-0.1.2/setup.cfg
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      983 2023-06-12 04:48:55.000000 BioPII-0.1.2/setup.py
```

### Comparing `BioPII-0.1.1/BioPII.egg-info/PKG-INFO` & `BioPII-0.1.2/BioPII.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BioPII
-Version: 0.1.1
+Version: 0.1.2
 Summary: BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images.
 Home-page: https://github.com/OckermanSethGVSU/Bio-PII
 Author: Seth Ockerman
 Author-email: ockermas@mail.gvsu.edu
 Keywords: Biology,Integral Image,Sliding Window,HPC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

### Comparing `BioPII-0.1.1/PKG-INFO` & `BioPII-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BioPII
-Version: 0.1.1
+Version: 0.1.2
 Summary: BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images.
 Home-page: https://github.com/OckermanSethGVSU/Bio-PII
 Author: Seth Ockerman
 Author-email: ockermas@mail.gvsu.edu
 Keywords: Biology,Integral Image,Sliding Window,HPC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

### Comparing `BioPII-0.1.1/README.md` & `BioPII-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `BioPII-0.1.1/pyproject.toml` & `BioPII-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "BioPII"
-version = "0.1.1"
+version = "0.1.2"
 authors = ["Seth Ockerman <ockermas@mail.gvsu.edu>"]
 description = "BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images."
 homepage = "https://github.com/OckermanSethGVSU/Bio-PII"
 keywords = ["Biology", "Integral Image", "Sliding Window", "HPC"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `BioPII-0.1.1/setup.py` & `BioPII-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='BioPII',
-    version='0.1.1',
+    version='0.1.2',
     author='Seth Ockerman',
     author_email='ockermas@mail.gvsu.edu',
     description='BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images.',
     url='https://github.com/OckermanSethGVSU/Bio-PII',
     packages=find_packages(),
+    py_modules=['BioPII'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Environment :: GPU :: NVIDIA CUDA',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

