# Comparing `tmp/BioPII-0.1.5.tar.gz` & `tmp/BioPII-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioPII-0.1.5.tar", last modified: Mon Jun 12 05:19:26 2023, max compression
+gzip compressed data, was "BioPII-0.1.6.tar", last modified: Mon Jun 12 05:22:02 2023, max compression
```

## Comparing `BioPII-0.1.5.tar` & `BioPII-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 05:19:26.737580 BioPII-0.1.5/
-drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 05:19:26.737580 BioPII-0.1.5/BioPII.egg-info/
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     3150 2023-06-12 05:19:26.000000 BioPII-0.1.5/BioPII.egg-info/PKG-INFO
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      192 2023-06-12 05:19:26.000000 BioPII-0.1.5/BioPII.egg-info/SOURCES.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        1 2023-06-12 05:19:26.000000 BioPII-0.1.5/BioPII.egg-info/dependency_links.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       40 2023-06-12 05:19:26.000000 BioPII-0.1.5/BioPII.egg-info/requires.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        7 2023-06-12 05:19:26.000000 BioPII-0.1.5/BioPII.egg-info/top_level.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)    23350 2023-06-12 04:56:01.000000 BioPII-0.1.5/BioPII.py
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     3150 2023-06-12 05:19:26.737580 BioPII-0.1.5/PKG-INFO
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     2384 2023-06-12 05:19:01.000000 BioPII-0.1.5/README.md
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      580 2023-06-12 05:18:40.000000 BioPII-0.1.5/pyproject.toml
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       38 2023-06-12 05:19:26.737580 BioPII-0.1.5/setup.cfg
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     1139 2023-06-12 05:18:32.000000 BioPII-0.1.5/setup.py
+drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 05:22:02.973062 BioPII-0.1.6/
+drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 05:22:02.973062 BioPII-0.1.6/BioPII.egg-info/
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     3151 2023-06-12 05:22:02.000000 BioPII-0.1.6/BioPII.egg-info/PKG-INFO
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      192 2023-06-12 05:22:02.000000 BioPII-0.1.6/BioPII.egg-info/SOURCES.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        1 2023-06-12 05:22:02.000000 BioPII-0.1.6/BioPII.egg-info/dependency_links.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       40 2023-06-12 05:22:02.000000 BioPII-0.1.6/BioPII.egg-info/requires.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        7 2023-06-12 05:22:02.000000 BioPII-0.1.6/BioPII.egg-info/top_level.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)    23350 2023-06-12 04:56:01.000000 BioPII-0.1.6/BioPII.py
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     3151 2023-06-12 05:22:02.973062 BioPII-0.1.6/PKG-INFO
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     2385 2023-06-12 05:21:27.000000 BioPII-0.1.6/README.md
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      580 2023-06-12 05:18:40.000000 BioPII-0.1.6/pyproject.toml
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       38 2023-06-12 05:22:02.973062 BioPII-0.1.6/setup.cfg
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     1139 2023-06-12 05:21:50.000000 BioPII-0.1.6/setup.py
```

### Comparing `BioPII-0.1.5/BioPII.egg-info/PKG-INFO` & `BioPII-0.1.6/BioPII.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BioPII
-Version: 0.1.5
+Version: 0.1.6
 Summary: BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images.
 Home-page: https://github.com/OckermanSethGVSU/BioPII
 Author: Seth Ockerman
 Author-email: ockermas@mail.gvsu.edu
 Keywords: Biology,Integral Image,Sliding Window,HPC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -18,20 +18,20 @@
 
 # BioPII
 
 BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images. This package makes use of the integral image technique to drastically speedup SWA, enabling SWA analysis of images that would have been too large for previous SWA implementations. 
 
 To use the package include the following statement at the top of your file: `from BioPII import PII`
 
-To cite this package, cite our [IEEE CIBCB 2023 short paper](TODO). 
+ <!--  To cite this package, cite our [IEEE CIBCB 2023 short paper](TODO).  -->
 
 
 This code and package is under the MIT License - copyright (c) Seth Ockerman
 
- <!-- The package name is prounounced bio-pie :) -->
+The package name is prounounced bio-pie :)
 
 ## Performance Numbers
 We tested our methods to determine its performance relative to past methods. We created a C++ SWA (referred to as DP-Naive) script which used dynamic programming to reduce the number of additions needed to be performed. DP-Naive SWA was already 400x faster than a naive approach (a simple four for loop approach) on small images and is used as the baseline for comparison to our integral-image-based methods. 
 
 |                   | 30k by 30k | 30k by 30k Speedup | 40k by 50k | 40k by 50k Speedup | 60k by 60k | 60k by 60k Speedup |
 |-------------------|------------|--------------------|------------|--------------------|------------|--------------------|
 | **DP-Naive**      | 211,381,433| N/A                | 491,374,150| N/A                | 943,858,845     | N/A                |
```

### Comparing `BioPII-0.1.5/BioPII.py` & `BioPII-0.1.6/BioPII.py`

 * *Files identical despite different names*

### Comparing `BioPII-0.1.5/PKG-INFO` & `BioPII-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BioPII
-Version: 0.1.5
+Version: 0.1.6
 Summary: BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images.
 Home-page: https://github.com/OckermanSethGVSU/BioPII
 Author: Seth Ockerman
 Author-email: ockermas@mail.gvsu.edu
 Keywords: Biology,Integral Image,Sliding Window,HPC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -18,20 +18,20 @@
 
 # BioPII
 
 BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images. This package makes use of the integral image technique to drastically speedup SWA, enabling SWA analysis of images that would have been too large for previous SWA implementations. 
 
 To use the package include the following statement at the top of your file: `from BioPII import PII`
 
-To cite this package, cite our [IEEE CIBCB 2023 short paper](TODO). 
+ <!--  To cite this package, cite our [IEEE CIBCB 2023 short paper](TODO).  -->
 
 
 This code and package is under the MIT License - copyright (c) Seth Ockerman
 
- <!-- The package name is prounounced bio-pie :) -->
+The package name is prounounced bio-pie :)
 
 ## Performance Numbers
 We tested our methods to determine its performance relative to past methods. We created a C++ SWA (referred to as DP-Naive) script which used dynamic programming to reduce the number of additions needed to be performed. DP-Naive SWA was already 400x faster than a naive approach (a simple four for loop approach) on small images and is used as the baseline for comparison to our integral-image-based methods. 
 
 |                   | 30k by 30k | 30k by 30k Speedup | 40k by 50k | 40k by 50k Speedup | 60k by 60k | 60k by 60k Speedup |
 |-------------------|------------|--------------------|------------|--------------------|------------|--------------------|
 | **DP-Naive**      | 211,381,433| N/A                | 491,374,150| N/A                | 943,858,845     | N/A                |
```

### Comparing `BioPII-0.1.5/README.md` & `BioPII-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # BioPII
 
 BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images. This package makes use of the integral image technique to drastically speedup SWA, enabling SWA analysis of images that would have been too large for previous SWA implementations. 
 
 To use the package include the following statement at the top of your file: `from BioPII import PII`
 
-To cite this package, cite our [IEEE CIBCB 2023 short paper](TODO). 
+ <!--  To cite this package, cite our [IEEE CIBCB 2023 short paper](TODO).  -->
 
 
 This code and package is under the MIT License - copyright (c) Seth Ockerman
 
- <!-- The package name is prounounced bio-pie :) -->
+The package name is prounounced bio-pie :)
 
 ## Performance Numbers
 We tested our methods to determine its performance relative to past methods. We created a C++ SWA (referred to as DP-Naive) script which used dynamic programming to reduce the number of additions needed to be performed. DP-Naive SWA was already 400x faster than a naive approach (a simple four for loop approach) on small images and is used as the baseline for comparison to our integral-image-based methods. 
 
 |                   | 30k by 30k | 30k by 30k Speedup | 40k by 50k | 40k by 50k Speedup | 60k by 60k | 60k by 60k Speedup |
 |-------------------|------------|--------------------|------------|--------------------|------------|--------------------|
 | **DP-Naive**      | 211,381,433| N/A                | 491,374,150| N/A                | 943,858,845     | N/A                |
```

### Comparing `BioPII-0.1.5/pyproject.toml` & `BioPII-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `BioPII-0.1.5/setup.py` & `BioPII-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='BioPII',
-    version='0.1.5',
+    version='0.1.6',
     author='Seth Ockerman',
     author_email='ockermas@mail.gvsu.edu',
     description='BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/OckermanSethGVSU/BioPII',
     packages=find_packages(),
```

