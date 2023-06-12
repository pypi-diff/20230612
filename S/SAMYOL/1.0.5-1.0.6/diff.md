# Comparing `tmp/SAMYOL-1.0.5.tar.gz` & `tmp/SAMYOL-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMYOL-1.0.5.tar", last modified: Mon Jun 12 10:17:11 2023, max compression
+gzip compressed data, was "SAMYOL-1.0.6.tar", last modified: Mon Jun 12 10:21:50 2023, max compression
```

## Comparing `SAMYOL-1.0.5.tar` & `SAMYOL-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:17:11.883236 SAMYOL-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-12 10:17:11.883236 SAMYOL-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:17:11.883236 SAMYOL-1.0.5/SAMYOL/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/SAMYOL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/SAMYOL/prediction_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/SAMYOL/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/SAMYOL/sam_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/SAMYOL/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/SAMYOL/yolo_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/SAMYOL/yolo_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/SAMYOL/yolo_preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:17:11.883236 SAMYOL-1.0.5/SAMYOL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-12 10:17:11.000000 SAMYOL-1.0.5/SAMYOL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 10:17:11.000000 SAMYOL-1.0.5/SAMYOL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:17:11.000000 SAMYOL-1.0.5/SAMYOL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 10:17:11.000000 SAMYOL-1.0.5/SAMYOL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 10:17:11.000000 SAMYOL-1.0.5/SAMYOL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 10:17:11.883236 SAMYOL-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-12 10:16:57.000000 SAMYOL-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:21:50.519127 SAMYOL-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-12 10:21:50.519127 SAMYOL-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:21:50.519127 SAMYOL-1.0.6/SAMYOL/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/SAMYOL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/SAMYOL/prediction_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/SAMYOL/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/SAMYOL/sam_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/SAMYOL/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/SAMYOL/yolo_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/SAMYOL/yolo_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/SAMYOL/yolo_preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:21:50.519127 SAMYOL-1.0.6/SAMYOL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-12 10:21:50.000000 SAMYOL-1.0.6/SAMYOL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 10:21:50.000000 SAMYOL-1.0.6/SAMYOL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:21:50.000000 SAMYOL-1.0.6/SAMYOL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 10:21:50.000000 SAMYOL-1.0.6/SAMYOL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 10:21:50.000000 SAMYOL-1.0.6/SAMYOL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 10:21:50.519127 SAMYOL-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-12 10:21:40.000000 SAMYOL-1.0.6/setup.py
```

### Comparing `SAMYOL-1.0.5/LICENSE` & `SAMYOL-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.5/PKG-INFO` & `SAMYOL-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SAMYOL
-Version: 1.0.5
+Version: 1.0.6
 Summary: Combines YOLO models and SAM
-Author: Jawher Ben Abdallah - Rim Sleimi
+Author: Jawher Ben Abdallah, Rim Sleimi
 Author-email: jawher.b.abdallah@gmail.com, sleimi.rim1996@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/Jawher-Ben-Abdallah/SAMYOL
 Keywords: YOLOv6,YOLOv7,YOLOv8,YOLO-NAS SAM,Object_Detection,Segmentation
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `SAMYOL-1.0.5/README.rst` & `SAMYOL-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.5/SAMYOL/prediction_results.py` & `SAMYOL-1.0.6/SAMYOL/prediction_results.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.5/SAMYOL/predictor.py` & `SAMYOL-1.0.6/SAMYOL/predictor.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.5/SAMYOL/sam_inference.py` & `SAMYOL-1.0.6/SAMYOL/sam_inference.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.5/SAMYOL/utils.py` & `SAMYOL-1.0.6/SAMYOL/utils.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.5/SAMYOL/yolo_inference.py` & `SAMYOL-1.0.6/SAMYOL/yolo_inference.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.5/SAMYOL/yolo_postprocessing.py` & `SAMYOL-1.0.6/SAMYOL/yolo_postprocessing.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.5/SAMYOL/yolo_preprocessing.py` & `SAMYOL-1.0.6/SAMYOL/yolo_preprocessing.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.5/SAMYOL.egg-info/PKG-INFO` & `SAMYOL-1.0.6/SAMYOL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SAMYOL
-Version: 1.0.5
+Version: 1.0.6
 Summary: Combines YOLO models and SAM
-Author: Jawher Ben Abdallah - Rim Sleimi
+Author: Jawher Ben Abdallah, Rim Sleimi
 Author-email: jawher.b.abdallah@gmail.com, sleimi.rim1996@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/Jawher-Ben-Abdallah/SAMYOL
 Keywords: YOLOv6,YOLOv7,YOLOv8,YOLO-NAS SAM,Object_Detection,Segmentation
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `SAMYOL-1.0.5/setup.py` & `SAMYOL-1.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
   name="SAMYOL",
-  version="1.0.5",
+  version="1.0.6",
   description="Combines YOLO models and SAM",
   packages=find_packages(),
   long_description=long_description,
   long_description_content_type="text/markdown",
   project_urls={
         'Source': 'https://github.com/Jawher-Ben-Abdallah/SAMYOL',
     },
-  author="Jawher Ben Abdallah - Rim Sleimi",
+  author="Jawher Ben Abdallah, Rim Sleimi",
   author_email="jawher.b.abdallah@gmail.com, sleimi.rim1996@gmail.com",
   license='Apache License 2.0',
   classifiers=[
       "Programming Language :: Python :: 3.10",
     ],
     keywords="YOLOv6, YOLOv7, YOLOv8, YOLO-NAS SAM, Object_Detection, Segmentation",
     install_requires=[
```

