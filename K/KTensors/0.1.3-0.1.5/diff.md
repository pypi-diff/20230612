# Comparing `tmp/KTensors-0.1.3.tar.gz` & `tmp/KTensors-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KTensors-0.1.3.tar", last modified: Mon Jun 12 04:03:48 2023, max compression
+gzip compressed data, was "KTensors-0.1.5.tar", last modified: Mon Jun 12 04:06:31 2023, max compression
```

## Comparing `KTensors-0.1.3.tar` & `KTensors-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 04:03:48.923010 KTensors-0.1.3/
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 04:03:48.922696 KTensors-0.1.3/KTensors.egg-info/
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2951 2023-06-12 04:03:48.000000 KTensors-0.1.3/KTensors.egg-info/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)      189 2023-06-12 04:03:48.000000 KTensors-0.1.3/KTensors.egg-info/SOURCES.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-12 04:03:48.000000 KTensors-0.1.3/KTensors.egg-info/dependency_links.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        6 2023-06-12 04:03:48.000000 KTensors-0.1.3/KTensors.egg-info/requires.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        9 2023-06-12 04:03:48.000000 KTensors-0.1.3/KTensors.egg-info/top_level.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2751 2023-06-12 00:12:19.000000 KTensors-0.1.3/KTensors.py
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2951 2023-06-12 04:03:48.922879 KTensors-0.1.3/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-12 04:00:49.000000 KTensors-0.1.3/README.md
--rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-12 04:03:48.923054 KTensors-0.1.3/setup.cfg
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     1269 2023-06-12 04:03:16.000000 KTensors-0.1.3/setup.py
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 04:06:31.489947 KTensors-0.1.5/
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 04:06:31.489599 KTensors-0.1.5/KTensors.egg-info/
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2907 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      189 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/SOURCES.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/dependency_links.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        6 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/requires.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        9 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/top_level.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2751 2023-06-12 00:12:19.000000 KTensors-0.1.5/KTensors.py
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2907 2023-06-12 04:06:31.489805 KTensors-0.1.5/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-12 04:05:32.000000 KTensors-0.1.5/README.md
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-12 04:06:31.489991 KTensors-0.1.5/setup.cfg
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     1225 2023-06-12 04:05:44.000000 KTensors-0.1.5/setup.py
```

### Comparing `KTensors-0.1.3/KTensors.egg-info/PKG-INFO` & `KTensors-0.1.5/KTensors.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.1.3
-Summary: K-Tensors: Clustering Positive Semi-Definite Matrices
+Version: 0.1.5
+Summary: K-Tensors
 Home-page: https://github.com/Hanchao-Zhang/KTensors
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: MIT
 Keywords: KTensors: Clustering Positive Semi-Denfinite Matrices
 Requires: numpy
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 
 [![Project Status:
 Active](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active) [![Build
 Status](https://travis-ci.org/stephenslab/clusteringCPC.svg?branch=master)](https://travis-ci.org/stephenslab/clusteringCPC) [![codecov](https://codecov.io/gh/stephenslab/clusteringCPC/branch/master/graph/badge.svg)](https://codecov.io/gh/stephenslab/clusteringCPC) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC) [![CRAN\_Download\_Badge](http://cranlogs.r-pkg.org/badges/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC)
 
 ## Install the Package from PyPI
-+ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install KTensors` or `pip3 install KTensors==0.1.2` for a specific version
++ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install KTensors` or `pip3 install KTensors==0.1.5` for a specific version
 
 ## install the Package from GitHub
 
 + Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install git+https://github.com/Hanchao-Zhang/KTensors.git`
 + Open a python console, copy and paste: `from KTensors import KTensors`
```

### Comparing `KTensors-0.1.3/KTensors.py` & `KTensors-0.1.5/KTensors.py`

 * *Files identical despite different names*

### Comparing `KTensors-0.1.3/PKG-INFO` & `KTensors-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.1.3
-Summary: K-Tensors: Clustering Positive Semi-Definite Matrices
+Version: 0.1.5
+Summary: K-Tensors
 Home-page: https://github.com/Hanchao-Zhang/KTensors
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: MIT
 Keywords: KTensors: Clustering Positive Semi-Denfinite Matrices
 Requires: numpy
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 
 [![Project Status:
 Active](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active) [![Build
 Status](https://travis-ci.org/stephenslab/clusteringCPC.svg?branch=master)](https://travis-ci.org/stephenslab/clusteringCPC) [![codecov](https://codecov.io/gh/stephenslab/clusteringCPC/branch/master/graph/badge.svg)](https://codecov.io/gh/stephenslab/clusteringCPC) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC) [![CRAN\_Download\_Badge](http://cranlogs.r-pkg.org/badges/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC)
 
 ## Install the Package from PyPI
-+ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install KTensors` or `pip3 install KTensors==0.1.2` for a specific version
++ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install KTensors` or `pip3 install KTensors==0.1.5` for a specific version
 
 ## install the Package from GitHub
 
 + Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install git+https://github.com/Hanchao-Zhang/KTensors.git`
 + Open a python console, copy and paste: `from KTensors import KTensors`
```

### Comparing `KTensors-0.1.3/README.md` & `KTensors-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 [![Project Status:
 Active](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active) [![Build
 Status](https://travis-ci.org/stephenslab/clusteringCPC.svg?branch=master)](https://travis-ci.org/stephenslab/clusteringCPC) [![codecov](https://codecov.io/gh/stephenslab/clusteringCPC/branch/master/graph/badge.svg)](https://codecov.io/gh/stephenslab/clusteringCPC) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC) [![CRAN\_Download\_Badge](http://cranlogs.r-pkg.org/badges/clusteringCPC)](https://cran.r-project.org/package=clusteringCPC)
 
 ## Install the Package from PyPI
-+ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install KTensors` or `pip3 install KTensors==0.1.2` for a specific version
++ Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install KTensors` or `pip3 install KTensors==0.1.5` for a specific version
 
 ## install the Package from GitHub
 
 + Go to the terminal (mac) or command line (windows), copy and paste:`pip3 install git+https://github.com/Hanchao-Zhang/KTensors.git`
 + Open a python console, copy and paste: `from KTensors import KTensors`
```

### Comparing `KTensors-0.1.3/setup.py` & `KTensors-0.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "KTensors",
-    description="K-Tensors: Clustering Positive Semi-Definite Matrices",
+    description="K-Tensors",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version = "0.1.3",
+    version = "0.1.5",
     author = "Hanchao Zhang",
     author_email = "hz1641@nyu.edu",
     license = "MIT",
     keywords = "KTensors: Clustering Positive Semi-Denfinite Matrices",
     url = "https://github.com/Hanchao-Zhang/KTensors",
     packages=find_packages("KTensors"),
     py_modules=["KTensors"],
```

