# Comparing `tmp/BioPII-0.1.3.tar.gz` & `tmp/BioPII-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioPII-0.1.3.tar", last modified: Mon Jun 12 04:59:11 2023, max compression
+gzip compressed data, was "BioPII-0.1.4.tar", last modified: Mon Jun 12 05:15:21 2023, max compression
```

## Comparing `BioPII-0.1.3.tar` & `BioPII-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:59:11.079607 BioPII-0.1.3/
-drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:59:11.079607 BioPII-0.1.3/BioPII.egg-info/
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      725 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/PKG-INFO
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      192 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/SOURCES.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        1 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/dependency_links.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       40 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/requires.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        7 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/top_level.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)    23350 2023-06-12 04:56:01.000000 BioPII-0.1.3/BioPII.py
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      725 2023-06-12 04:59:11.079607 BioPII-0.1.3/PKG-INFO
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     2339 2023-06-11 00:53:51.000000 BioPII-0.1.3/README.md
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      580 2023-06-12 04:58:44.000000 BioPII-0.1.3/pyproject.toml
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       38 2023-06-12 04:59:11.079607 BioPII-0.1.3/setup.cfg
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      982 2023-06-12 04:58:42.000000 BioPII-0.1.3/setup.py
+drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 05:15:21.115792 BioPII-0.1.4/
+drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 05:15:21.115792 BioPII-0.1.4/BioPII.egg-info/
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     3140 2023-06-12 05:15:21.000000 BioPII-0.1.4/BioPII.egg-info/PKG-INFO
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      192 2023-06-12 05:15:21.000000 BioPII-0.1.4/BioPII.egg-info/SOURCES.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        1 2023-06-12 05:15:21.000000 BioPII-0.1.4/BioPII.egg-info/dependency_links.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       40 2023-06-12 05:15:21.000000 BioPII-0.1.4/BioPII.egg-info/requires.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        7 2023-06-12 05:15:21.000000 BioPII-0.1.4/BioPII.egg-info/top_level.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)    23350 2023-06-12 04:56:01.000000 BioPII-0.1.4/BioPII.py
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     3140 2023-06-12 05:15:21.115792 BioPII-0.1.4/PKG-INFO
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     2374 2023-06-12 05:11:01.000000 BioPII-0.1.4/README.md
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      580 2023-06-12 05:14:36.000000 BioPII-0.1.4/pyproject.toml
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       38 2023-06-12 05:15:21.115792 BioPII-0.1.4/setup.cfg
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     1139 2023-06-12 05:15:12.000000 BioPII-0.1.4/setup.py
```

### Comparing `BioPII-0.1.3/BioPII.py` & `BioPII-0.1.4/BioPII.py`

 * *Files identical despite different names*

### Comparing `BioPII-0.1.3/README.md` & `BioPII-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# Bio_PII
+# BioPII
 
-Bio_PII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images. This package makes use of the integral image technique to drastically speedup SWA, enabling SWA analysis of images that would have been too large for previous SWA implementations. 
+BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images. This package makes use of the integral image technique to drastically speedup SWA, enabling SWA analysis of images that would have been too large for previous SWA implementations. 
 
-To use the package include the following statement at the top of your file: `from Bio_PII import PII`
+To use the package include the following statement at the top of your file: `from BioPII import PII`
 
 To cite this package, cite our [IEEE CIBCB 2023 short paper](TODO). 
 
 
 This code and package is under the MIT License - copyright (c) Seth Ockerman
 
-The package name is prounounced bio-pie-squared :)
+The package name is prounounced bio-pie :)
 
 ## Performance Numbers
-We tested our methods to determine its performance relative to past methods. We created a C++ SWA (refered to as DP-Naive) script which used dynamic programming to reduce the number of additions needed to be performed. DP-Naive SWA was already 400x faster than a naive approach (a simple 4 for loop approach) on small images and is used as the baseline for comparision to our bio-PII methods. 
+We tested our methods to determine its performance relative to past methods. We created a C++ SWA (referred to as DP-Naive) script which used dynamic programming to reduce the number of additions needed to be performed. DP-Naive SWA was already 400x faster than a naive approach (a simple four for loop approach) on small images and is used as the baseline for comparison to our integral-image-based methods. 
 
 |                   | 30k by 30k | 30k by 30k Speedup | 40k by 50k | 40k by 50k Speedup | 60k by 60k | 60k by 60k Speedup |
 |-------------------|------------|--------------------|------------|--------------------|------------|--------------------|
 | **DP-Naive**      | 211,381,433| N/A                | 491,374,150| N/A                | 943,858,845     | N/A                |
-| **II**            | 56,693     | 3728x              | 253,082    | 1942x               | 319,666    | 2953x               |
-| **PII**           | 20,137     | 10,497x             | 46,532     | 10,559x             | 86,583    | 10,901x            |
+| **Integral Image**            | 56,693     | 3728x              | 253,082    | 1942x               | 319,666    | 2953x               |
+| **Parallel Integral Image**           | 20,137     | 10,497x             | 46,532     | 10,559x             | 86,583    | 10,901x            |
 
 *Note: SWA runtime in milliseconds on different image sizes; speedups relative to DP-Naive Solution*
 
 
 ## Features
 
 - Efficient computation for various biological image analysis tasks.
 - Supports different types of SWA (Sliding Window Analysis) algorithms.
 - Flexible window size selection for analyzing different cellular features.
 - GPU acceleration option for faster computations.
 - Works with numpy arrays for easy integration into existing workflows.
 
 ## Installation
 
-You can install bio PII using pip:
+You can install BioPII using pip:
 
-``` pip3 install Bio_PII ```
+``` pip3 install BioPII ```
 
 ## Documentation
 Documentation can be found internally within our code and in the [documentation file](./documentation.md).
```

### Comparing `BioPII-0.1.3/pyproject.toml` & `BioPII-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "BioPII"
-version = "0.1.3"
+version = "0.1.4"
 authors = ["Seth Ockerman <ockermas@mail.gvsu.edu>"]
 description = "BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images."
 homepage = "https://github.com/OckermanSethGVSU/BioPII"
 keywords = ["Biology", "Integral Image", "Sliding Window", "HPC"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

