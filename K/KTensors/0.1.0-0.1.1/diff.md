# Comparing `tmp/KTensors-0.1.0.tar.gz` & `tmp/KTensors-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KTensors-0.1.0.tar", last modified: Mon Jun 12 00:06:15 2023, max compression
+gzip compressed data, was "KTensors-0.1.1.tar", last modified: Mon Jun 12 00:10:54 2023, max compression
```

## Comparing `KTensors-0.1.0.tar` & `KTensors-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 00:06:15.140084 KTensors-0.1.0/
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 00:06:15.139737 KTensors-0.1.0/KTensors.egg-info/
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2838 2023-06-12 00:06:15.000000 KTensors-0.1.0/KTensors.egg-info/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)      158 2023-06-12 00:06:15.000000 KTensors-0.1.0/KTensors.egg-info/SOURCES.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-12 00:06:15.000000 KTensors-0.1.0/KTensors.egg-info/dependency_links.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        9 2023-06-12 00:06:15.000000 KTensors-0.1.0/KTensors.egg-info/top_level.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2751 2023-06-12 00:05:43.000000 KTensors-0.1.0/KTensors.py
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2838 2023-06-12 00:06:15.139939 KTensors-0.1.0/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-11 18:31:00.000000 KTensors-0.1.0/README.md
--rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-12 00:06:15.140129 KTensors-0.1.0/setup.cfg
--rw-r--r--   0 hanchaozhang   (501) staff       (20)      922 2023-06-12 00:05:57.000000 KTensors-0.1.0/setup.py
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 00:10:54.283243 KTensors-0.1.1/
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 00:10:54.282827 KTensors-0.1.1/KTensors.egg-info/
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2838 2023-06-12 00:10:54.000000 KTensors-0.1.1/KTensors.egg-info/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      189 2023-06-12 00:10:54.000000 KTensors-0.1.1/KTensors.egg-info/SOURCES.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-12 00:10:54.000000 KTensors-0.1.1/KTensors.egg-info/dependency_links.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        6 2023-06-12 00:10:54.000000 KTensors-0.1.1/KTensors.egg-info/requires.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        9 2023-06-12 00:10:54.000000 KTensors-0.1.1/KTensors.egg-info/top_level.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2750 2023-06-12 00:09:37.000000 KTensors-0.1.1/KTensors.py
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2838 2023-06-12 00:10:54.283083 KTensors-0.1.1/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-11 18:31:00.000000 KTensors-0.1.1/README.md
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-12 00:10:54.283287 KTensors-0.1.1/setup.cfg
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      986 2023-06-12 00:10:41.000000 KTensors-0.1.1/setup.py
```

### Comparing `KTensors-0.1.0/KTensors.egg-info/PKG-INFO` & `KTensors-0.1.1/KTensors.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/Hanchao-Zhang/KTensors
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: BSD
 Keywords: Clustering Positive Semi-Denfinite Matrices
 Requires: numpy
```

### Comparing `KTensors-0.1.0/KTensors.py` & `KTensors-0.1.1/KTensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-
 """
 Perform K-Tensors Clustering Algorithm for Positive Semi-Denfinite Matrices
 
 Parameters:
     Psis (3D np.array): The input matrices to be clustered with shape (n, p, p)
     K (int): The number of clusters
     max_iter (int): The maximum number of iterations
@@ -14,14 +12,15 @@
     F (np.array): The orthonormal transformation of the input matrices to the
         common principal components
     diagF (np.array): The diagonal matrices of the orthonormal transformation
         of the input matrices to the common principal components
     centers0 (np.array): The centers of the clusters
     mse_vec (list): The mean squared error of the clusters at each iteration
 """
+import numpy as np
 class KTensors:
     def __init__(self, Psis, K, max_iter=1000):
         self.Psis = Psis
         self.K = K
         self.n = Psis.shape[0]
         self.p = Psis.shape[1]
         self.max_iter = max_iter
```

### Comparing `KTensors-0.1.0/PKG-INFO` & `KTensors-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/Hanchao-Zhang/KTensors
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: BSD
 Keywords: Clustering Positive Semi-Denfinite Matrices
 Requires: numpy
```

### Comparing `KTensors-0.1.0/README.md` & `KTensors-0.1.1/README.md`

 * *Files identical despite different names*

