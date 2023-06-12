# Comparing `tmp/KTensors-0.0.9.tar.gz` & `tmp/KTensors-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KTensors-0.0.9.tar", last modified: Mon Jun 12 00:03:53 2023, max compression
+gzip compressed data, was "KTensors-0.1.0.tar", last modified: Mon Jun 12 00:06:15 2023, max compression
```

## Comparing `KTensors-0.0.9.tar` & `KTensors-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 00:03:53.331279 KTensors-0.0.9/
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 00:03:53.330925 KTensors-0.0.9/KTensors.egg-info/
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2838 2023-06-12 00:03:53.000000 KTensors-0.0.9/KTensors.egg-info/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)      158 2023-06-12 00:03:53.000000 KTensors-0.0.9/KTensors.egg-info/SOURCES.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-12 00:03:53.000000 KTensors-0.0.9/KTensors.egg-info/dependency_links.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        9 2023-06-12 00:03:53.000000 KTensors-0.0.9/KTensors.egg-info/top_level.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2731 2023-06-11 03:25:28.000000 KTensors-0.0.9/KTensors.py
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2838 2023-06-12 00:03:53.331134 KTensors-0.0.9/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-11 18:31:00.000000 KTensors-0.0.9/README.md
--rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-12 00:03:53.331328 KTensors-0.0.9/setup.cfg
--rw-r--r--   0 hanchaozhang   (501) staff       (20)      922 2023-06-12 00:03:31.000000 KTensors-0.0.9/setup.py
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 00:06:15.140084 KTensors-0.1.0/
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 00:06:15.139737 KTensors-0.1.0/KTensors.egg-info/
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2838 2023-06-12 00:06:15.000000 KTensors-0.1.0/KTensors.egg-info/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      158 2023-06-12 00:06:15.000000 KTensors-0.1.0/KTensors.egg-info/SOURCES.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-12 00:06:15.000000 KTensors-0.1.0/KTensors.egg-info/dependency_links.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        9 2023-06-12 00:06:15.000000 KTensors-0.1.0/KTensors.egg-info/top_level.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2751 2023-06-12 00:05:43.000000 KTensors-0.1.0/KTensors.py
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2838 2023-06-12 00:06:15.139939 KTensors-0.1.0/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-11 18:31:00.000000 KTensors-0.1.0/README.md
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-12 00:06:15.140129 KTensors-0.1.0/setup.cfg
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      922 2023-06-12 00:05:57.000000 KTensors-0.1.0/setup.py
```

### Comparing `KTensors-0.0.9/KTensors.egg-info/PKG-INFO` & `KTensors-0.1.0/KTensors.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.0.9
+Version: 0.1.0
 Home-page: https://github.com/Hanchao-Zhang/KTensors
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: BSD
 Keywords: Clustering Positive Semi-Denfinite Matrices
 Requires: numpy
```

### Comparing `KTensors-0.0.9/KTensors.py` & `KTensors-0.1.0/KTensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as np
+
 """
 Perform K-Tensors Clustering Algorithm for Positive Semi-Denfinite Matrices
 
 Parameters:
     Psis (3D np.array): The input matrices to be clustered with shape (n, p, p)
     K (int): The number of clusters
     max_iter (int): The maximum number of iterations
```

### Comparing `KTensors-0.0.9/PKG-INFO` & `KTensors-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.0.9
+Version: 0.1.0
 Home-page: https://github.com/Hanchao-Zhang/KTensors
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: BSD
 Keywords: Clustering Positive Semi-Denfinite Matrices
 Requires: numpy
```

### Comparing `KTensors-0.0.9/README.md` & `KTensors-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `KTensors-0.0.9/setup.py` & `KTensors-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "KTensors",
-    version = "0.0.9",
+    version = "0.1.0",
     author = "Hanchao Zhang",
     author_email = "hz1641@nyu.edu",
     license = "BSD",
     keywords = "Clustering Positive Semi-Denfinite Matrices",
     url = "https://github.com/Hanchao-Zhang/KTensors",
     packages=find_packages("KTensors"),
     py_modules=["KTensors"],
```

