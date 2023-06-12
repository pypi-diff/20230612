# Comparing `tmp/BioPII-0.1.2.tar.gz` & `tmp/BioPII-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioPII-0.1.2.tar", last modified: Mon Jun 12 04:49:05 2023, max compression
+gzip compressed data, was "BioPII-0.1.3.tar", last modified: Mon Jun 12 04:59:11 2023, max compression
```

## Comparing `BioPII-0.1.2.tar` & `BioPII-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:49:05.311740 BioPII-0.1.2/
-drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:49:05.311740 BioPII-0.1.2/BioPII.egg-info/
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      726 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/PKG-INFO
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      192 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/SOURCES.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        1 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/dependency_links.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       40 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/requires.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        7 2023-06-12 04:49:05.000000 BioPII-0.1.2/BioPII.egg-info/top_level.txt
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)    23892 2023-05-30 21:16:53.000000 BioPII-0.1.2/BioPII.py
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      726 2023-06-12 04:49:05.311740 BioPII-0.1.2/PKG-INFO
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     2339 2023-06-11 00:53:51.000000 BioPII-0.1.2/README.md
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      581 2023-06-12 04:48:08.000000 BioPII-0.1.2/pyproject.toml
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       38 2023-06-12 04:49:05.311740 BioPII-0.1.2/setup.cfg
--rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      983 2023-06-12 04:48:55.000000 BioPII-0.1.2/setup.py
+drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:59:11.079607 BioPII-0.1.3/
+drwxrwxr-x   0 ockermans  (1000) ockermans  (1000)        0 2023-06-12 04:59:11.079607 BioPII-0.1.3/BioPII.egg-info/
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      725 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/PKG-INFO
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      192 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/SOURCES.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        1 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/dependency_links.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       40 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/requires.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)        7 2023-06-12 04:59:11.000000 BioPII-0.1.3/BioPII.egg-info/top_level.txt
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)    23350 2023-06-12 04:56:01.000000 BioPII-0.1.3/BioPII.py
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      725 2023-06-12 04:59:11.079607 BioPII-0.1.3/PKG-INFO
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)     2339 2023-06-11 00:53:51.000000 BioPII-0.1.3/README.md
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      580 2023-06-12 04:58:44.000000 BioPII-0.1.3/pyproject.toml
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)       38 2023-06-12 04:59:11.079607 BioPII-0.1.3/setup.cfg
+-rw-rw-r--   0 ockermans  (1000) ockermans  (1000)      982 2023-06-12 04:58:42.000000 BioPII-0.1.3/setup.py
```

### Comparing `BioPII-0.1.2/BioPII.egg-info/PKG-INFO` & `BioPII-0.1.3/BioPII.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: BioPII
-Version: 0.1.2
+Version: 0.1.3
 Summary: BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images.
-Home-page: https://github.com/OckermanSethGVSU/Bio-PII
+Home-page: https://github.com/OckermanSethGVSU/BioPII
 Author: Seth Ockerman
 Author-email: ockermas@mail.gvsu.edu
 Keywords: Biology,Integral Image,Sliding Window,HPC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BioPII-0.1.2/BioPII.py` & `BioPII-0.1.3/BioPII.py`

 * *Files 5% similar despite different names*

```diff
@@ -506,31 +506,8 @@
             case "sum":
                 return [PII.process_split_image("sum", windowSize,chunks,GPU=GPU),max_i,max_j]
             case "avg":
                 return [PII.process_split_image("avg", windowSize,chunks,GPU=GPU),max_i,max_j]
             case "std":
                 return [PII.process_split_image("std",windowSize,chunks,GPU=GPU), max_i,max_j]
             case _:
-                raise ValueError("Please provide a valid analysis type \nOptions: 'sum','avg','std'")
-    
-
-            
-            
-            
-
-# chunkSize = int(input("Enter chunk size: "))
-# windowSize = int(input("Enter window size: "))
-# cv_image = cv2.imread("../capstone/images/40x40.png")
-# image = cv_image[:, :, 0]
-# r1 = PII.SWA(image,windowSize,"std")
-# # np.set_printoptions(threshold=np.inf)
-
-# print(r1)
-
-
-# chunks,rows,cols = PII.SWA(image,windowSize,"std",subImageSize=chunkSize)
-# r2 = PII.reconstruct_image(chunks,rows,cols)
-# print(r2)
-
-# print(r1 == r2)
-
-# PII.save_split_image(chunks,rows,cols,"out/",reconstruct=True)
+                raise ValueError("Please provide a valid analysis type \nOptions: 'sum','avg','std'")
```

### Comparing `BioPII-0.1.2/PKG-INFO` & `BioPII-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: BioPII
-Version: 0.1.2
+Version: 0.1.3
 Summary: BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images.
-Home-page: https://github.com/OckermanSethGVSU/Bio-PII
+Home-page: https://github.com/OckermanSethGVSU/BioPII
 Author: Seth Ockerman
 Author-email: ockermas@mail.gvsu.edu
 Keywords: Biology,Integral Image,Sliding Window,HPC
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BioPII-0.1.2/README.md` & `BioPII-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `BioPII-0.1.2/pyproject.toml` & `BioPII-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "BioPII"
-version = "0.1.2"
+version = "0.1.3"
 authors = ["Seth Ockerman <ockermas@mail.gvsu.edu>"]
 description = "BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images."
-homepage = "https://github.com/OckermanSethGVSU/Bio-PII"
+homepage = "https://github.com/OckermanSethGVSU/BioPII"
 keywords = ["Biology", "Integral Image", "Sliding Window", "HPC"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 numpy = "*"
 opencv-python = "*"
```

### Comparing `BioPII-0.1.2/setup.py` & `BioPII-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='BioPII',
-    version='0.1.2',
+    version='0.1.3',
     author='Seth Ockerman',
     author_email='ockermas@mail.gvsu.edu',
     description='BioPII (Biology Parallel Integral Image) is a Python package for performing sliding window analysis (SWA) on biological images.',
-    url='https://github.com/OckermanSethGVSU/Bio-PII',
+    url='https://github.com/OckermanSethGVSU/BioPII',
     packages=find_packages(),
     py_modules=['BioPII'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Environment :: GPU :: NVIDIA CUDA',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3',
```

