# Comparing `tmp/moosez-2.0.6.tar.gz` & `tmp/moosez-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.0.6.tar", last modified: Sun Jun 11 20:09:25 2023, max compression
+gzip compressed data, was "moosez-2.0.7.tar", last modified: Mon Jun 12 16:14:39 2023, max compression
```

## Comparing `moosez-2.0.6.tar` & `moosez-2.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:09:25.104988 moosez-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 20:09:12.000000 moosez-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-11 20:09:25.104988 moosez-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-06-11 20:09:12.000000 moosez-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:09:25.104988 moosez-2.0.6/moosez/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/moosez.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-11 20:09:12.000000 moosez-2.0.6/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 20:09:25.104988 moosez-2.0.6/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-11 20:09:25.000000 moosez-2.0.6/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-11 20:09:25.000000 moosez-2.0.6/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 20:09:25.000000 moosez-2.0.6/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-11 20:09:25.000000 moosez-2.0.6/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 20:09:25.000000 moosez-2.0.6/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 20:09:25.000000 moosez-2.0.6/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 20:09:25.104988 moosez-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-11 20:09:12.000000 moosez-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:14:39.984008 moosez-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 16:14:27.000000 moosez-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 16:14:39.984008 moosez-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19071 2023-06-12 16:14:27.000000 moosez-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:14:39.984008 moosez-2.0.7/moosez/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/moosez.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-12 16:14:27.000000 moosez-2.0.7/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:14:39.984008 moosez-2.0.7/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 16:14:39.000000 moosez-2.0.7/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-12 16:14:39.000000 moosez-2.0.7/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:14:39.000000 moosez-2.0.7/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 16:14:39.000000 moosez-2.0.7/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-12 16:14:39.000000 moosez-2.0.7/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 16:14:39.000000 moosez-2.0.7/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:14:39.984008 moosez-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 16:14:27.000000 moosez-2.0.7/setup.py
```

### Comparing `moosez-2.0.6/LICENSE` & `moosez-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/PKG-INFO` & `moosez-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.6
+Version: 2.0.7
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.0.6/README.md` & `moosez-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez/constants.py` & `moosez-2.0.7/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez/display.py` & `moosez-2.0.7/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez/download.py` & `moosez-2.0.7/moosez/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import logging
 import os
+from rich.progress import Progress
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Author: Lalith Kumar Shiyam Sundar
 # Institution: Medical University of Vienna
 # Research Group: Quantitative Imaging and Medical Physics (QIMP) Team
 # Date: 13.02.2023
 # Version: 2.0.0
@@ -35,49 +36,52 @@
     print("Binary to download: " + binary_name)
     response = requests.get(url + binary_name)
 
     with open(binary_name, "wb") as f:
         f.write(response.content)
 
 
+
 def model(model_name, model_path):
     """
     Downloads the model for the current system.
     :param model_name: The name of the model to download.
     :param model_path: The path to store the model.
     """
     model_info = resources.MODELS[model_name]
     url = model_info["url"]
     filename = os.path.join(model_path, model_info["filename"])
     directory = os.path.join(model_path, model_info["directory"])
 
     if not os.path.exists(directory):
         logging.info(f" Downloading {directory}")
-        # show progress using tqdm
-        with tqdm(unit="B", unit_scale=True, leave=False, desc=f" Downloading {os.path.basename(directory)}") as pbar:
-            response = requests.get(url, stream=True)
-            total_size = int(response.headers.get("Content-Length", 0))
-            pbar.total = total_size
-            chunk_size = 1024 * 10
+        # show progress using rich
+        response = requests.get(url, stream=True)
+        total_size = int(response.headers.get("Content-Length", 0))
+        chunk_size = 1024 * 10
+
+        with Progress() as progress:
+            task = progress.add_task("[cyan] Downloading...", total=total_size)
             for chunk in response.iter_content(chunk_size=chunk_size):
                 open(filename, "ab").write(chunk)
-                pbar.update(chunk_size)
-        # Unzip the model
+                progress.update(task, advance=chunk_size)
+
         # Unzip the model
         import zipfile
-        with tqdm(unit="B", unit_scale=True, leave=False, desc=f" Extracting {os.path.basename(directory)}") as pbar:
+        with Progress() as progress:
             with zipfile.ZipFile(filename, 'r') as zip_ref:
                 total_size = sum((file.file_size for file in zip_ref.infolist()))
-                pbar.total = total_size
+                task = progress.add_task("[cyan] Extracting...", total=total_size)
                 # Get the parent directory of 'directory'
                 parent_directory = os.path.dirname(directory)
                 for file in zip_ref.infolist():
                     zip_ref.extract(file, parent_directory)
                     extracted_size = file.file_size
-                    pbar.update(extracted_size)
+                    progress.update(task, advance=extracted_size)
+
         logging.info(f" {os.path.basename(directory)} extracted.")
 
         # Delete the zip file
         os.remove(filename)
         print(f"{constants.ANSI_GREEN} {os.path.basename(directory)} - download complete. {constants.ANSI_RESET}")
         logging.info(f" {os.path.basename(directory)} - download complete.")
     else:
```

### Comparing `moosez-2.0.6/moosez/file_utilities.py` & `moosez-2.0.7/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez/image_conversion.py` & `moosez-2.0.7/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez/image_processing.py` & `moosez-2.0.7/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez/input_validation.py` & `moosez-2.0.7/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez/moosez.py` & `moosez-2.0.7/moosez/moosez.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez/predict.py` & `moosez-2.0.7/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez/resources.py` & `moosez-2.0.7/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.0.6/moosez.egg-info/PKG-INFO` & `moosez-2.0.7/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.0.6
+Version: 2.0.7
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/QIMP-Team/mooseZ
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: Apache 2.0
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.0.6/setup.py` & `moosez-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='moosez',
-    version='2.0.6',
+    version='2.0.7',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.9',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
@@ -43,15 +43,16 @@
         'numpy~=1.22.3',
         'mpire~=2.3.3',
         'openpyxl~=3.0.9',
         'matplotlib',
         'pyfiglet~=0.8.post1',
         'natsort~=8.1.0',
         'pillow>=9.2.0',
-        'colorama~=0.4.6'
+        'colorama~=0.4.6',
+        'rich'
     ],
     entry_points={
         'console_scripts': [
             'moosez=moosez.moosez:main',
         ],
     },
 )
```

