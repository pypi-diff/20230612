# Comparing `tmp/spPersist-0.3.3.tar.gz` & `tmp/spPersist-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.3.3.tar", last modified: Thu Jun  8 09:23:38 2023, max compression
+gzip compressed data, was "spPersist-0.4.0.tar", last modified: Sun Jun 11 03:33:48 2023, max compression
```

## Comparing `spPersist-0.3.3.tar` & `spPersist-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:38.186333 spPersist-0.3.3/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-08 09:16:42.000000 spPersist-0.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-08 09:23:38.186333 spPersist-0.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1096 2023-06-08 09:16:42.000000 spPersist-0.3.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 09:23:38.187333 spPersist-0.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 09:22:44.000000 spPersist-0.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:38.183333 spPersist-0.3.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:38.185333 spPersist-0.3.3/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 09:14:01.000000 spPersist-0.3.3/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-08 09:14:02.000000 spPersist-0.3.3/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-08 09:14:02.000000 spPersist-0.3.3/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-08 09:14:01.000000 spPersist-0.3.3/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 09:14:02.000000 spPersist-0.3.3/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-08 09:14:01.000000 spPersist-0.3.3/src/spPersist/ph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:38.186333 spPersist-0.3.3/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 03:33:48.214777 spPersist-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-11 03:32:23.000000 spPersist-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-11 03:33:48.214777 spPersist-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-11 03:32:23.000000 spPersist-0.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 03:33:48.214777 spPersist-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-06-11 03:32:50.000000 spPersist-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 03:33:48.211777 spPersist-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 03:33:48.213777 spPersist-0.4.0/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-11 03:30:46.000000 spPersist-0.4.0/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-11 03:31:23.000000 spPersist-0.4.0/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-11 03:30:46.000000 spPersist-0.4.0/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-11 03:30:46.000000 spPersist-0.4.0/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-11 03:30:46.000000 spPersist-0.4.0/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-11 03:30:47.000000 spPersist-0.4.0/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-11 03:31:01.000000 spPersist-0.4.0/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 03:33:48.214777 spPersist-0.4.0/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-11 03:33:48.000000 spPersist-0.4.0/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-11 03:33:48.000000 spPersist-0.4.0/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 03:33:48.000000 spPersist-0.4.0/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-11 03:33:48.000000 spPersist-0.4.0/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-11 03:33:48.000000 spPersist-0.4.0/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.3.3/LICENSE` & `spPersist-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.3/PKG-INFO` & `spPersist-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.3.3
+Version: 0.4.0
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spatial transcriptomics with Persistent Homology
 
 This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
-the theory of Persistent Homology and persistence diagram. The package so far
+the theory of Persistent Homology and persistence diagram. The package 
 contains a data processing module, called dp, allowing users to load either the
 standard datasets from Visium and MERFISH, or published datasets into desired
 annotated data format for the analysis performed in this package. The format is
 compatible with the package Squidpy.
 
 The package also includes a pre-processing module, a 
 persistent homology module and a homological classification module, respectively
 named pp, ph and hc.
 
+The pre-processing module contains quality control metrics, deconvolution
+methods and cell type identifications.
+
 The persistent homology module contains functions for computing simplicial 
 complexes of point clouds (See data structures in the gudhi package.) and their
 topological measures. It also includes plotting features of the persistence 
 diagram.
 
 The homological classification module computes the number of holes and connected
 components as a dictionary.
```

### Comparing `spPersist-0.3.3/README.md` & `spPersist-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Spatial transcriptomics with Persistent Homology
 
 This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
-the theory of Persistent Homology and persistence diagram. The package so far
+the theory of Persistent Homology and persistence diagram. The package 
 contains a data processing module, called dp, allowing users to load either the
 standard datasets from Visium and MERFISH, or published datasets into desired
 annotated data format for the analysis performed in this package. The format is
 compatible with the package Squidpy.
 
 The package also includes a pre-processing module, a 
 persistent homology module and a homological classification module, respectively
 named pp, ph and hc.
 
+The pre-processing module contains quality control metrics, deconvolution
+methods and cell type identifications.
+
 The persistent homology module contains functions for computing simplicial 
 complexes of point clouds (See data structures in the gudhi package.) and their
 topological measures. It also includes plotting features of the persistence 
 diagram.
 
 The homological classification module computes the number of holes and connected
 components as a dictionary.
```

### Comparing `spPersist-0.3.3/setup.py` & `spPersist-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="spPersist",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.3.3",  # Required
+    version="0.4.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.3.3/src/spPersist/DTM_filtrations.py` & `spPersist-0.4.0/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.3/src/spPersist/dp.py` & `spPersist-0.4.0/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.3/src/spPersist/hc.py` & `spPersist-0.4.0/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.3/src/spPersist/persistence_statistics.py` & `spPersist-0.4.0/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.3/src/spPersist/ph.py` & `spPersist-0.4.0/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.3/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.4.0/src/spPersist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.3.3
+Version: 0.4.0
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spatial transcriptomics with Persistent Homology
 
 This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
-the theory of Persistent Homology and persistence diagram. The package so far
+the theory of Persistent Homology and persistence diagram. The package 
 contains a data processing module, called dp, allowing users to load either the
 standard datasets from Visium and MERFISH, or published datasets into desired
 annotated data format for the analysis performed in this package. The format is
 compatible with the package Squidpy.
 
 The package also includes a pre-processing module, a 
 persistent homology module and a homological classification module, respectively
 named pp, ph and hc.
 
+The pre-processing module contains quality control metrics, deconvolution
+methods and cell type identifications.
+
 The persistent homology module contains functions for computing simplicial 
 complexes of point clouds (See data structures in the gudhi package.) and their
 topological measures. It also includes plotting features of the persistence 
 diagram.
 
 The homological classification module computes the number of holes and connected
 components as a dictionary.
```

