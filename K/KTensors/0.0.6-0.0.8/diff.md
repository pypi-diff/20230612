# Comparing `tmp/KTensors-0.0.6.tar.gz` & `tmp/KTensors-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KTensors-0.0.6.tar", last modified: Sun Jun 11 23:15:36 2023, max compression
+gzip compressed data, was "KTensors-0.0.8.tar", last modified: Sun Jun 11 23:50:21 2023, max compression
```

## Comparing `KTensors-0.0.6.tar` & `KTensors-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-11 23:15:36.156087 KTensors-0.0.6/
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-11 23:15:36.155802 KTensors-0.0.6/KTensors.egg-info/
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2769 2023-06-11 23:15:36.000000 KTensors-0.0.6/KTensors.egg-info/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)      146 2023-06-11 23:15:36.000000 KTensors-0.0.6/KTensors.egg-info/SOURCES.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-11 23:15:36.000000 KTensors-0.0.6/KTensors.egg-info/dependency_links.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-11 23:15:36.000000 KTensors-0.0.6/KTensors.egg-info/top_level.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2769 2023-06-11 23:15:36.155972 KTensors-0.0.6/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-11 18:31:00.000000 KTensors-0.0.6/README.md
--rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-11 23:15:36.156128 KTensors-0.0.6/setup.cfg
--rw-r--r--   0 hanchaozhang   (501) staff       (20)      873 2023-06-11 23:14:45.000000 KTensors-0.0.6/setup.py
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-11 23:50:21.650658 KTensors-0.0.8/
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-11 23:50:21.650244 KTensors-0.0.8/KTensors.egg-info/
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2769 2023-06-11 23:50:21.000000 KTensors-0.0.8/KTensors.egg-info/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      158 2023-06-11 23:50:21.000000 KTensors-0.0.8/KTensors.egg-info/SOURCES.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-11 23:50:21.000000 KTensors-0.0.8/KTensors.egg-info/dependency_links.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        9 2023-06-11 23:50:21.000000 KTensors-0.0.8/KTensors.egg-info/top_level.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2731 2023-06-11 03:25:28.000000 KTensors-0.0.8/KTensors.py
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2769 2023-06-11 23:50:21.650497 KTensors-0.0.8/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-11 18:31:00.000000 KTensors-0.0.8/README.md
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-11 23:50:21.650715 KTensors-0.0.8/setup.cfg
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      896 2023-06-11 23:50:08.000000 KTensors-0.0.8/setup.py
```

### Comparing `KTensors-0.0.6/KTensors.egg-info/PKG-INFO` & `KTensors-0.0.8/KTensors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.0.6
+Version: 0.0.8
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: BSD
 Keywords: Clustering Positive Semi-Denfinite Matrices
 
 K-Tensors: Clustering Positive Semi-Definite Matrices<img src="./ktensorlogo.png" align="right" width="150" />
 ========================================================================================================================
```

### Comparing `KTensors-0.0.6/PKG-INFO` & `KTensors-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.0.6
+Version: 0.0.8
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: BSD
 Keywords: Clustering Positive Semi-Denfinite Matrices
 
 K-Tensors: Clustering Positive Semi-Definite Matrices<img src="./ktensorlogo.png" align="right" width="150" />
 ========================================================================================================================
```

### Comparing `KTensors-0.0.6/README.md` & `KTensors-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `KTensors-0.0.6/setup.py` & `KTensors-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "KTensors",
-    version = "0.0.6",
+    version = "0.0.8",
     author = "Hanchao Zhang",
     author_email = "hz1641@nyu.edu",
     license = "BSD",
     keywords = "Clustering Positive Semi-Denfinite Matrices",
     # url = "https://github.com/Hanchao-Zhang/KTensors",
-    packages=find_packages(where="KTensors"),
+    packages=find_packages("KTensors"),
+    py_modules=["KTensors"],
     long_description=read('README.md'),
     # classifiers=[
     #     "Development Status :: 3 - Alpha",
     #     "Topic :: Utilities",
     #     "License :: OSI Approved :: BSD License",
     # ],
 )
```

