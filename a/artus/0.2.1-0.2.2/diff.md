# Comparing `tmp/artus-0.2.1.tar.gz` & `tmp/artus-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artus-0.2.1.tar", last modified: Fri Jun  9 11:49:39 2023, max compression
+gzip compressed data, was "artus-0.2.2.tar", last modified: Mon Jun 12 14:42:56 2023, max compression
```

## Comparing `artus-0.2.1.tar` & `artus-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/
--rw-rw-r--   0 justine   (1000) justine   (1000)    11357 2023-06-08 12:27:48.000000 artus-0.2.1/LICENSE
--rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-09 11:49:39.847981 artus-0.2.1/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)     2514 2023-06-08 12:28:48.000000 artus-0.2.1/README.md
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.2.1/artus/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/evaluate_model/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/evaluate_model/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.2.1/artus/evaluate_model/coco_stats.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.2.1/artus/evaluate_model/evaluate.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-09 07:01:26.000000 artus-0.2.1/artus/evaluate_model/write_eval_results.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/inference/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/inference/__init__.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.2.1/artus/inference/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.2.1/artus/inference/deploy_unlabeled_dataset.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)    10522 2023-06-06 07:13:05.000000 artus-0.2.1/artus/inference/predict.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/prepare/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/prepare/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.2.1/artus/prepare/coco_splitting.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.2.1/artus/prepare/crs_settings.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.2.1/artus/prepare/tile.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.2.1/artus/prepare/transform_geojson_to_coco.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/spatialize/
--rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.2.1/artus/spatialize/GeoCOCOExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     7851 2023-06-07 12:07:22.000000 artus-0.2.1/artus/spatialize/GeoFiftyoneExporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)     1218 2023-06-07 12:07:12.000000 artus-0.2.1/artus/spatialize/LocationImporter.py
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/spatialize/__init__.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus/train/
--rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.1/artus/train/__init__.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.2.1/artus/train/build_trainer.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.2.1/artus/train/config.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.2.1/artus/train/data_augmentation.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.2.1/artus/train/train.py
--rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.2.1/artus/train/validation_hook.py
-drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-09 11:49:39.847981 artus-0.2.1/artus.egg-info/
--rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/PKG-INFO
--rw-rw-r--   0 justine   (1000) justine   (1000)      918 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/SOURCES.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/dependency_links.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)      426 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/requires.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-09 11:49:39.000000 artus-0.2.1/artus.egg-info/top_level.txt
--rw-rw-r--   0 justine   (1000) justine   (1000)     1356 2023-06-09 11:49:12.000000 artus-0.2.1/pyproject.toml
--rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-09 11:49:39.847981 artus-0.2.1/setup.cfg
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-12 14:42:56.598438 artus-0.2.2/
+-rw-rw-r--   0 justine   (1000) justine   (1000)    11357 2023-06-08 12:27:48.000000 artus-0.2.2/LICENSE
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-12 14:42:56.598438 artus-0.2.2/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2514 2023-06-08 12:28:48.000000 artus-0.2.2/README.md
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-12 14:42:56.598438 artus-0.2.2/artus/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-03-16 05:56:31.000000 artus-0.2.2/artus/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-12 14:42:56.598438 artus-0.2.2/artus/evaluate_model/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.2/artus/evaluate_model/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     5126 2023-06-06 13:00:06.000000 artus-0.2.2/artus/evaluate_model/coco_stats.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3269 2023-06-02 10:53:58.000000 artus-0.2.2/artus/evaluate_model/evaluate.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6076 2023-06-09 07:01:26.000000 artus-0.2.2/artus/evaluate_model/write_eval_results.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-12 14:42:56.598438 artus-0.2.2/artus/inference/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.2/artus/inference/__init__.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     2036 2023-06-02 10:56:11.000000 artus-0.2.2/artus/inference/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3004 2023-06-05 05:47:10.000000 artus-0.2.2/artus/inference/deploy_unlabeled_dataset.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)    10460 2023-06-12 14:40:44.000000 artus-0.2.2/artus/inference/predict.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-12 14:42:56.598438 artus-0.2.2/artus/prepare/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.2/artus/prepare/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     6361 2023-06-06 07:14:45.000000 artus-0.2.2/artus/prepare/coco_splitting.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)      567 2023-06-05 06:10:35.000000 artus-0.2.2/artus/prepare/crs_settings.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     5748 2023-06-05 06:43:00.000000 artus-0.2.2/artus/prepare/tile.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1167 2023-06-05 06:50:00.000000 artus-0.2.2/artus/prepare/transform_geojson_to_coco.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-12 14:42:56.598438 artus-0.2.2/artus/spatialize/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     4947 2023-06-05 07:14:37.000000 artus-0.2.2/artus/spatialize/GeoCOCOExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     7851 2023-06-07 12:07:22.000000 artus-0.2.2/artus/spatialize/GeoFiftyoneExporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1218 2023-06-07 12:07:12.000000 artus-0.2.2/artus/spatialize/LocationImporter.py
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.2/artus/spatialize/__init__.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-12 14:42:56.598438 artus-0.2.2/artus/train/
+-rw-rw-r--   0 justine   (1000) justine   (1000)        0 2023-04-18 14:15:29.000000 artus-0.2.2/artus/train/__init__.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2460 2023-06-06 06:41:04.000000 artus-0.2.2/artus/train/build_trainer.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2799 2023-06-06 06:50:12.000000 artus-0.2.2/artus/train/config.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     1566 2023-06-06 06:53:08.000000 artus-0.2.2/artus/train/data_augmentation.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     2993 2023-06-06 06:56:30.000000 artus-0.2.2/artus/train/train.py
+-rwxrwxr-x   0 justine   (1000) justine   (1000)     3286 2023-06-06 07:01:54.000000 artus-0.2.2/artus/train/validation_hook.py
+drwxrwxr-x   0 justine   (1000) justine   (1000)        0 2023-06-12 14:42:56.598438 artus-0.2.2/artus.egg-info/
+-rw-rw-r--   0 justine   (1000) justine   (1000)     3168 2023-06-12 14:42:56.000000 artus-0.2.2/artus.egg-info/PKG-INFO
+-rw-rw-r--   0 justine   (1000) justine   (1000)      918 2023-06-12 14:42:56.000000 artus-0.2.2/artus.egg-info/SOURCES.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        1 2023-06-12 14:42:56.000000 artus-0.2.2/artus.egg-info/dependency_links.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)      426 2023-06-12 14:42:56.000000 artus-0.2.2/artus.egg-info/requires.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)        6 2023-06-12 14:42:56.000000 artus-0.2.2/artus.egg-info/top_level.txt
+-rw-rw-r--   0 justine   (1000) justine   (1000)     1356 2023-06-12 14:40:10.000000 artus-0.2.2/pyproject.toml
+-rw-rw-r--   0 justine   (1000) justine   (1000)       38 2023-06-12 14:42:56.598438 artus-0.2.2/setup.cfg
```

### Comparing `artus-0.2.1/LICENSE` & `artus-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/PKG-INFO` & `artus-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.2.1
+Version: 0.2.2
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
 Project-URL: Tutorials, https://github.com/6tronl/artus-examples
 Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `artus-0.2.1/README.md` & `artus-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/evaluate_model/coco_stats.py` & `artus-0.2.2/artus/evaluate_model/coco_stats.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/evaluate_model/evaluate.py` & `artus-0.2.2/artus/evaluate_model/evaluate.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/evaluate_model/write_eval_results.py` & `artus-0.2.2/artus/evaluate_model/write_eval_results.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/inference/config.py` & `artus-0.2.2/artus/inference/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/inference/deploy_unlabeled_dataset.py` & `artus-0.2.2/artus/inference/deploy_unlabeled_dataset.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/inference/predict.py` & `artus-0.2.2/artus/inference/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """
 
 from detectron2.engine import DefaultPredictor
 from detectron2.structures import Boxes, Instances
 from torchvision.transforms import functional as func
 import numpy as np
 import cv2
-from PIL import Image
 import fiftyone as fo
 import fiftyone.utils.labels as foul
 from fiftyone import ViewField as F
 import os
 import cv2
 from torchvision.ops import nms
 import fiftyone as fo
@@ -107,17 +106,17 @@
         nms_threshold (float): the non-maximum-suppression threshold.
         classes (list): a list of the classes that can be predicted by the AI model.
         type_of_preds (str): indicate if semgentation masks "segm" expected or bounding boxes "bbox"
 
     Returns:
         a fiftyone field :class:``fiftyone.core.detections`` containing predictions for the sample
     """
-    image = Image.open(sample_filepath)
-    image = func.to_tensor(image).to(device)
-    c, h, w = image.shape
+    
+    image = cv2.imread(sample_filepath)
+    h, w, c = image.shape
 
     preds = predict(predictor, sample_filepath)
 
     preds = apply_nms(preds, nms_threshold, type_of_preds)
     
     labels = preds['instances'].pred_classes.cpu().detach().numpy()
     scores = preds['instances'].scores.cpu().detach().numpy()
```

### Comparing `artus-0.2.1/artus/prepare/coco_splitting.py` & `artus-0.2.2/artus/prepare/coco_splitting.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/prepare/crs_settings.py` & `artus-0.2.2/artus/prepare/crs_settings.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/prepare/tile.py` & `artus-0.2.2/artus/prepare/tile.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/prepare/transform_geojson_to_coco.py` & `artus-0.2.2/artus/prepare/transform_geojson_to_coco.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/spatialize/GeoCOCOExporter.py` & `artus-0.2.2/artus/spatialize/GeoCOCOExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/spatialize/GeoFiftyoneExporter.py` & `artus-0.2.2/artus/spatialize/GeoFiftyoneExporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/spatialize/LocationImporter.py` & `artus-0.2.2/artus/spatialize/LocationImporter.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/train/build_trainer.py` & `artus-0.2.2/artus/train/build_trainer.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/train/config.py` & `artus-0.2.2/artus/train/config.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/train/data_augmentation.py` & `artus-0.2.2/artus/train/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/train/train.py` & `artus-0.2.2/artus/train/train.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus/train/validation_hook.py` & `artus-0.2.2/artus/train/validation_hook.py`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/artus.egg-info/PKG-INFO` & `artus-0.2.2/artus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artus
-Version: 0.2.1
+Version: 0.2.2
 Summary: A geoAI package to train and predict spatial occurences on rasters or georeferenced images.
 Author-email: Justine Talpaert Daudon <justine.daudon@protonmail.com>
 Project-URL: Homepage, https://github.com/6tronl/artus
 Project-URL: Bug Tracker, https://github.com/6tronl/artus/issues
 Project-URL: Tutorials, https://github.com/6tronl/artus-examples
 Project-URL: Documentation, https://artus.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `artus-0.2.1/artus.egg-info/SOURCES.txt` & `artus-0.2.2/artus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artus-0.2.1/pyproject.toml` & `artus-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "artus"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Justine Talpaert Daudon", email="justine.daudon@protonmail.com" },
 ]
 description = "A geoAI package to train and predict spatial occurences on rasters or georeferenced images."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

