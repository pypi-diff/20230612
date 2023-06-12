# Comparing `tmp/SAMYOL-1.0.7.tar.gz` & `tmp/SAMYOL-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMYOL-1.0.7.tar", last modified: Mon Jun 12 10:48:04 2023, max compression
+gzip compressed data, was "SAMYOL-1.0.8.tar", last modified: Mon Jun 12 13:56:28 2023, max compression
```

## Comparing `SAMYOL-1.0.7.tar` & `SAMYOL-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:48:04.788470 SAMYOL-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-12 10:48:04.788470 SAMYOL-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:48:04.784470 SAMYOL-1.0.7/SAMYOL/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/SAMYOL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/SAMYOL/prediction_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/SAMYOL/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/SAMYOL/sam_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/SAMYOL/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/SAMYOL/yolo_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/SAMYOL/yolo_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/SAMYOL/yolo_preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:48:04.788470 SAMYOL-1.0.7/SAMYOL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-12 10:48:04.000000 SAMYOL-1.0.7/SAMYOL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 10:48:04.000000 SAMYOL-1.0.7/SAMYOL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:48:04.000000 SAMYOL-1.0.7/SAMYOL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 10:48:04.000000 SAMYOL-1.0.7/SAMYOL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 10:48:04.000000 SAMYOL-1.0.7/SAMYOL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 10:48:04.788470 SAMYOL-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-12 10:47:50.000000 SAMYOL-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:56:28.523151 SAMYOL-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-12 13:56:28.523151 SAMYOL-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:56:28.519151 SAMYOL-1.0.8/SAMYOL/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/prediction_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/sam_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/yolo_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/yolo_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/yolo_preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:56:28.523151 SAMYOL-1.0.8/SAMYOL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:56:28.523151 SAMYOL-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/setup.py
```

### Comparing `SAMYOL-1.0.7/LICENSE` & `SAMYOL-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.7/PKG-INFO` & `SAMYOL-1.0.8/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: SAMYOL
-Version: 1.0.7
-Summary: Combines YOLO models and SAM
-Author: Jawher Ben Abdallah
-Author-email: jawher.b.abdallah@gmail.com
-Maintainer: Rim Sleimi
-Maintainer-email: sleimi.rim1996@gmail.com
-License: Apache License 2.0
-Project-URL: Source, https://github.com/Jawher-Ben-Abdallah/SAMYOL
-Keywords: YOLOv6,YOLOv7,YOLOv8,YOLO-NAS SAM,Object_Detection,Segmentation
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 =======
 SAMYOL
 =======
 .. image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
    :target: https://opensource.org/licenses/Apache-2.0
    :alt: License: Apache 2.0
 
@@ -65,26 +48,18 @@
 
 ⏳ Quick Installation
 ---------------------
 SAMYOL is installed using pip. 
 
 This python library requires python>=3.11, as well as pytorch>=1.7.0 and torchvision>=0.8.1. Installing both PyTorch and TorchVision with CUDA support is strongly recommended. We will also need the models checkpoints. These will be installed automatically if they are not already installed.
 
-.. code:: python
 
-  # Install SAMYOL:
-  pip install SAMYOL
-  # or
-  conda install SAMYOL -c conda-forge
-  # or 
-  pip install git+https://github.com/Jawher-Ben-Abdallah/SAMYOL.git 
-  # or clone the repository locally and install 
-  git clone git@github.com:Jawher-Ben-Abdallah/SAMYOL.git
-  cd SAMYOL
-  pip install .
+.. code-block:: shell
+
+   pip install SAMYOL
 
 
 🚀 Getting Started
 -------------------
 
 The following notebook has detailed examples and usage instructions for each YOLO model:
```

### Comparing `SAMYOL-1.0.7/SAMYOL/prediction_results.py` & `SAMYOL-1.0.8/SAMYOL/prediction_results.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.7/SAMYOL/predictor.py` & `SAMYOL-1.0.8/SAMYOL/predictor.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.7/SAMYOL/sam_inference.py` & `SAMYOL-1.0.8/SAMYOL/sam_inference.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.7/SAMYOL/utils.py` & `SAMYOL-1.0.8/SAMYOL/utils.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.7/SAMYOL/yolo_inference.py` & `SAMYOL-1.0.8/SAMYOL/yolo_inference.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.7/SAMYOL/yolo_postprocessing.py` & `SAMYOL-1.0.8/SAMYOL/yolo_postprocessing.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.7/SAMYOL/yolo_preprocessing.py` & `SAMYOL-1.0.8/SAMYOL/yolo_preprocessing.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.7/setup.py` & `SAMYOL-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from setuptools import setup, find_packages
 
-with open("README.rst", "r", encoding="utf-8") as f:
-    long_description = f.read()
-
+long_description = 'SAMYOL is a Python library that combines an object detection model (YOLOv6, YOLOv7, YOLOv8, or YOLO-NAS) and the Segment Anything Model (SAM).'
 setup(
   name="SAMYOL",
-  version="1.0.7",
+  version="1.0.8",
   description="Combines YOLO models and SAM",
   packages=find_packages(),
   long_description=long_description,
-  long_description_content_type="text/markdown",
+  long_description_content_type="text/x-rst",
   project_urls={
         'Source': 'https://github.com/Jawher-Ben-Abdallah/SAMYOL',
     },
   author="Jawher Ben Abdallah",
   author_email="jawher.b.abdallah@gmail.com",
   maintainer="Rim Sleimi",
   maintainer_email="sleimi.rim1996@gmail.com",
@@ -29,13 +27,13 @@
         "Pillow>=7.1.2",
         "PyYAML>=5.3.1",
         "requests>=2.23.0",
         "scipy>=1.4.1",
         "torch>=1.7.0",
         "torchvision>=0.8.1",
         "tqdm>=4.64.0", 
-        "onnxruntime"
+        "onnxruntime",
     ],
     
     extras_require={"dev" : "twine>=4.0.2"},
     python_requires=">=3.10",
-)
+)
```

