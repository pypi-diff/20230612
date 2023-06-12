# Comparing `tmp/hot-fair-utilities-1.0.49.tar.gz` & `tmp/hot-fair-utilities-1.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hot-fair-utilities-1.0.49.tar", last modified: Mon Jan 30 11:58:11 2023, max compression
+gzip compressed data, was "hot-fair-utilities-1.0.50.tar", last modified: Mon Jun 12 13:19:02 2023, max compression
```

## Comparing `hot-fair-utilities-1.0.49.tar` & `hot-fair-utilities-1.0.50.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-01-30 11:58:11.711308 hot-fair-utilities-1.0.49/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    34523 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/LICENSE
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       91 2023-01-30 11:58:06.000000 hot-fair-utilities-1.0.49/MANIFEST.in
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    43175 2023-01-30 11:58:11.711308 hot-fair-utilities-1.0.49/PKG-INFO
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2801 2022-12-28 10:39:39.000000 hot-fair-utilities-1.0.49/README.md
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-01-30 11:58:11.691308 hot-fair-utilities-1.0.49/hot_fair_utilities/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      188 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1720 2023-01-04 15:35:16.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/georeferencing.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-01-30 11:58:11.701308 hot-fair-utilities-1.0.49/hot_fair_utilities/inference/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       29 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/inference/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1984 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/inference/predict.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      775 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/inference/utils.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-01-30 11:58:11.701308 hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       68 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2715 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/building_footprint.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      969 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/get_polygons.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2448 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/merge_polygons.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1640 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/polygonize.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     8440 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/utils.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2086 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/vectorize.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-01-30 11:58:11.711308 hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       35 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     4532 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/clip_labels.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1123 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/fix_labels.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2917 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/preprocess.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      629 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/reproject_labels.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-01-30 11:58:11.711308 hot-fair-utilities-1.0.49/hot_fair_utilities/training/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       25 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/training/__init__.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1967 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/training/cleanup.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     3628 2023-01-27 13:05:24.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/training/prepare_data.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     4105 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/training/ramp_config_base.json
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    11435 2023-01-30 11:51:24.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/training/run_training.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2269 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/training/train.py
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2255 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/hot_fair_utilities/utils.py
-drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-01-30 11:58:11.701308 hot-fair-utilities-1.0.49/hot_fair_utilities.egg-info/
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)    43175 2023-01-30 11:58:11.000000 hot-fair-utilities-1.0.49/hot_fair_utilities.egg-info/PKG-INFO
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1313 2023-01-30 11:58:11.000000 hot-fair-utilities-1.0.49/hot_fair_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)        1 2023-01-30 11:58:11.000000 hot-fair-utilities-1.0.49/hot_fair_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)      193 2023-01-30 11:58:11.000000 hot-fair-utilities-1.0.49/hot_fair_utilities.egg-info/requires.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       19 2023-01-30 11:58:11.000000 hot-fair-utilities-1.0.49/hot_fair_utilities.egg-info/top_level.txt
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1579 2023-01-30 11:57:47.000000 hot-fair-utilities-1.0.49/pyproject.toml
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       38 2023-01-30 11:58:11.711308 hot-fair-utilities-1.0.49/setup.cfg
--rw-r--r--   0 kshitij   (1000) kshitij   (1000)       38 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.49/setup.py
+drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)    34523 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/LICENSE
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)       91 2023-01-30 11:58:06.000000 hot-fair-utilities-1.0.50/MANIFEST.in
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)    43175 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/PKG-INFO
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2801 2022-12-28 10:39:39.000000 hot-fair-utilities-1.0.50/README.md
+drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.811496 hot-fair-utilities-1.0.50/hot_fair_utilities/
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)      188 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/__init__.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1720 2023-01-04 15:35:16.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/georeferencing.py
+drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.811496 hot-fair-utilities-1.0.50/hot_fair_utilities/inference/
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)       29 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/inference/__init__.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2648 2023-06-12 06:44:41.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/inference/predict.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)      775 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/inference/utils.py
+drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)       68 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/__init__.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2715 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/building_footprint.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)      991 2023-06-12 06:44:41.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/get_polygons.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2470 2023-06-12 06:44:41.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/merge_polygons.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1640 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/polygonize.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     8440 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/utils.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2452 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/vectorize.py
+drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)       35 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/__init__.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     4532 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/clip_labels.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1248 2023-06-12 06:44:41.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/fix_labels.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2917 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/preprocess.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)      629 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/reproject_labels.py
+drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/hot_fair_utilities/training/
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)       25 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/__init__.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1967 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/cleanup.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     3629 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/prepare_data.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     4105 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/ramp_config_base.json
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)    11507 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/run_training.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2269 2023-06-12 13:16:01.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/training/train.py
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     2255 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/hot_fair_utilities/utils.py
+drwxr-xr-x   0 kshitij   (1000) kshitij   (1000)        0 2023-06-12 13:19:02.811496 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)    43175 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1313 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)        1 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)      207 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/requires.txt
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)       19 2023-06-12 13:19:02.000000 hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/top_level.txt
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)     1595 2023-06-12 13:18:10.000000 hot-fair-utilities-1.0.50/pyproject.toml
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)       38 2023-06-12 13:19:02.821496 hot-fair-utilities-1.0.50/setup.cfg
+-rw-r--r--   0 kshitij   (1000) kshitij   (1000)       38 2022-12-19 17:00:58.000000 hot-fair-utilities-1.0.50/setup.py
```

### Comparing `hot-fair-utilities-1.0.49/LICENSE` & `hot-fair-utilities-1.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/PKG-INFO` & `hot-fair-utilities-1.0.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.0.49
+Version: 1.0.50
 Summary: Utilities for AI - Assisted Mapping fAIr
 Author-email: Omdena <project@omdena.com>, Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hot-fair-utilities-1.0.49/README.md` & `hot-fair-utilities-1.0.50/README.md`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/georeferencing.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/georeferencing.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/inference/predict.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/inference/predict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,81 @@
+# Standard library imports
 import os
+import time
 from glob import glob
 from pathlib import Path
 
+# Third party imports
 import numpy as np
 from tensorflow import keras
 
 from ..georeferencing import georeference
 from ..utils import remove_files
 from .utils import open_images, save_mask
 
 BATCH_SIZE = 8
 IMAGE_SIZE = 256
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 
 
-def predict(checkpoint_path: str, input_path: str, prediction_path: str) -> None:
+def predict(
+    checkpoint_path: str, input_path: str, prediction_path: str, confidence: float = 0.5
+) -> None:
     """Predict building footprints for aerial images given a model checkpoint.
 
     This function reads the model weights from the checkpoint path and outputs
     predictions in GeoTIF format. The input images have to be in PNG format.
 
     The predicted masks will be georeferenced with EPSG:3857 as CRS.
 
     Args:
         checkpoint_path: Path where the weights of the model can be found.
         input_path: Path of the directory where the images are stored.
         prediction_path: Path of the directory where the predicted images will go.
+        confidence: Threshold probability for filtering out low-confidence predictions.
 
     Example::
 
         predict(
             "model_1_checkpt.tf",
             "data/inputs_v2/4",
             "data/predictions/4"
         )
     """
+    start = time.time()
+    print(f"Using : {checkpoint_path}")
     model = keras.models.load_model(checkpoint_path)
+    print(f"It took {round(time.time()-start)} sec to load model")
+    start = time.time()
 
     os.makedirs(prediction_path, exist_ok=True)
     image_paths = glob(f"{input_path}/*.png")
 
     for i in range((len(image_paths) + BATCH_SIZE - 1) // BATCH_SIZE):
         image_batch = image_paths[BATCH_SIZE * i : BATCH_SIZE * (i + 1)]
         images = open_images(image_batch)
         images = images.reshape(-1, IMAGE_SIZE, IMAGE_SIZE, 3)
 
         preds = model.predict(images)
         preds = np.argmax(preds, axis=-1)
         preds = np.expand_dims(preds, axis=-1)
-        preds = np.where(preds > 0.5, 1, 0)
+        preds = np.where(
+            preds > confidence, 1, 0
+        )  # Filter out low confidence predictions
 
         for idx, path in enumerate(image_batch):
             save_mask(
                 preds[idx],
                 str(f"{prediction_path}/{Path(path).stem}.png"),
             )
+    print(
+        f"It took {round(time.time()-start)} sec to predict with {confidence} Confidence Threshold"
+    )
+    keras.backend.clear_session()
+    del model
+    start = time.time()
 
     georeference(prediction_path, prediction_path, is_mask=True)
+    print(f"It took {round(time.time()-start)} sec to georeference")
+
     remove_files(f"{prediction_path}/*.xml")
     remove_files(f"{prediction_path}/*.png")
```

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/inference/utils.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/inference/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/building_footprint.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/building_footprint.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/get_polygons.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/get_polygons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Third party imports
 import numpy as np
 from PIL import Image
 from tqdm import tqdm
 
 from .building_footprint import BuildingExtract
 from .utils import tiles_from_directory
```

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/merge_polygons.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/merge_polygons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Third party imports
 from geopandas import GeoSeries, read_file
 from shapely.geometry import MultiPolygon, Polygon
 from shapely.validation import make_valid
 from tqdm import tqdm
 
 from .utils import UndirectedGraph, make_index, project, union
```

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/polygonize.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/polygonize.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/utils.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/postprocessing/vectorize.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/postprocessing/vectorize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+# Standard library imports
 from glob import glob
 from pathlib import Path
 
+# Third party imports
+import geopandas as gpd
 import numpy as np
 import rasterio as rio
-from geopandas import GeoSeries
 from rasterio.features import shapes
 from rasterio.merge import merge
 from shapely.geometry import Polygon, shape
 from tqdm import tqdm
 
-TOLERANCE = 1
+TOLERANCE = 0.5
 AREA_THRESHOLD = 0.1
 MAX_RATIO = 10
 
 
 def vectorize(input_path: str, output_path: str) -> None:
     """Polygonize raster tiles from the input path.
 
@@ -27,45 +29,53 @@
     Example::
 
         vectorize("data/masks_v2/4", "labels.geojson")
     """
     base_path = Path(output_path).parents[0]
     base_path.mkdir(exist_ok=True, parents=True)
 
-    rasters = []
-    for path in glob(f"{input_path}/*.tif"):
-        raster = rio.open(path)
-        rasters.append(raster)
+    raster_paths = glob(f"{input_path}/*.tif")
+    with rio.open(raster_paths[0]) as src:
+        kwargs = src.meta.copy()
 
+    rasters = [rio.open(path) for path in raster_paths]
     mosaic, output = merge(rasters)
+
+    # Close raster files after merging
+    for raster in rasters:
+        raster.close()
+
     polygons = [shape(s) for s, _ in shapes(mosaic, transform=output)]
 
     areas = [poly.area for poly in polygons]
     max_area, median_area = np.max(areas), np.median(areas)
     polygons = [
         Polygon(poly.exterior.coords)
         for poly in polygons
-        if poly.area != max_area and poly.area / median_area > AREA_THRESHOLD
+        if poly.area != max_area
+        and poly.area / median_area > AREA_THRESHOLD
+        and poly.area > 3
     ]
 
-    gs = GeoSeries(polygons).set_crs("EPSG:3857").simplify(TOLERANCE)
+    gs = gpd.GeoSeries(polygons, crs=kwargs["crs"]).simplify(TOLERANCE)
     gs = remove_overlapping_polygons(gs)
+    if gs.empty:
+        raise ValueError("No Features Found")
     gs.to_crs("EPSG:4326").to_file(output_path)
 
 
-def remove_overlapping_polygons(gs: GeoSeries) -> GeoSeries:
-    """Remove overlapping polygons.
-
-    Args:
-        gs: List of polygons to be fixed.
-    """
+def remove_overlapping_polygons(gs: gpd.GeoSeries) -> gpd.GeoSeries:
     to_remove = set()
-    for i in tqdm(range(len(gs))):
-        for j in range(i + 1, len(gs)):
-            p, q = gs.iloc[i], gs.iloc[j]
+    gs_sindex = gs.sindex
+
+    for i, p in tqdm(gs.items()):
+        possible_matches_index = list(gs_sindex.intersection(p.bounds))
+        possible_matches = gs.iloc[possible_matches_index]
+        precise_matches = possible_matches[possible_matches.overlaps(p)]
 
-            if GeoSeries(p).overlaps(q).bool():
+        for j, q in precise_matches.items():
+            if i != j:
                 ratio = max(p.area, q.area) / min(p.area, q.area)
                 if ratio > MAX_RATIO:
                     to_remove.add(i if p.area < q.area else j)
 
     return gs.drop(list(to_remove))
```

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/clip_labels.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/clip_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/fix_labels.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/fix_labels.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Third party imports
 import geopandas
 from shapely.validation import explain_validity, make_valid
 
 
 def remove_self_intersection(row):
     """Fix self-intersections in the polygons.
 
@@ -25,9 +26,11 @@
     """Fix GeoJSON file so that it doesn't have any self-intersecting polygons.
 
     Args:
         input_path: Path to the GeoJSON file where the input data are stored.
         output_path: Path to the GeoJSON file where the output data will go.
     """
     gdf = geopandas.read_file(input_path)
+    if gdf.empty:
+        raise ValueError("Error: gdf is empty, No Labels found : Check your labels")
     gdf["geometry"] = gdf.apply(remove_self_intersection, axis=1)
     gdf.to_file(output_path)
```

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/preprocess.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/preprocessing/reproject_labels.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/preprocessing/reproject_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/training/cleanup.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/training/cleanup.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/training/prepare_data.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/training/prepare_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 "0.85",
                 "-val",
                 "0.15",
             ],
             stderr=subprocess.PIPE,
         )
     except subprocess.CalledProcessError as ex:
-        raise RaiseError(ex.output.decode())
+        raise RaiseError(ex.stderr.decode())
 
     # move all the VALIDATION chips, labels and masks to their new locations
     try:
         subprocess.check_output(
             [
                 python_exec,
                 f"{RAMP_HOME}/ramp-code/scripts/move_chips_from_csv.py",
@@ -76,15 +76,16 @@
                 "-csv",
                 f"{dst_path}/fair_split_val.csv",
                 "-mv",
             ],
             stderr=subprocess.PIPE,
         )
     except subprocess.CalledProcessError as ex:
-        raise RaiseError(ex.output.decode())
+        raise RaiseError(ex.stderr.decode())
+
     try:
         subprocess.check_output(
             [
                 python_exec,
                 f"{RAMP_HOME}/ramp-code/scripts/move_chips_from_csv.py",
                 "-sd",
                 f"{dst_path}/labels",
@@ -93,15 +94,15 @@
                 "-csv",
                 f"{dst_path}/fair_split_val.csv",
                 "-mv",
             ],
             stderr=subprocess.PIPE,
         )
     except subprocess.CalledProcessError as ex:
-        raise RaiseError(ex.output.decode())
+        raise RaiseError(ex.stderr.decode())
 
     try:
         subprocess.check_output(
             [
                 python_exec,
                 f"{RAMP_HOME}/ramp-code/scripts/move_chips_from_csv.py",
                 "-sd",
@@ -111,8 +112,8 @@
                 "-csv",
                 f"{dst_path}/fair_split_val.csv",
                 "-mv",
             ],
             stderr=subprocess.PIPE,
         )
     except subprocess.CalledProcessError as ex:
-        raise RaiseError(ex.output.decode())
+        raise RaiseError(ex.stderr.decode())
```

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/training/ramp_config_base.json` & `hot-fair-utilities-1.0.50/hot_fair_utilities/training/ramp_config_base.json`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/training/run_training.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/training/run_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,17 @@
 
     ## Main training block ##
     n_epochs = cfg["num_epochs"]
     print(
         f"Starting Training with {n_epochs} epochs , {batch_size} batch size , {steps_per_epoch} steps per epoch , {validation_steps} validation steps......"
     )
     if validation_steps <= 0:
-        raise RaiseError("Not enough data for training")
+        raise RaiseError(
+            "Not enough data for training, Increase image or Try reducing batchsize/ephochs"
+        )
     # FIXME : Make checkpoint
     start = perf_counter()
     history = the_model.fit(
         train_batches,
         epochs=n_epochs,
         steps_per_epoch=steps_per_epoch,
         validation_data=val_batches,
```

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/training/train.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/training/train.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities/utils.py` & `hot-fair-utilities-1.0.50/hot_fair_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities.egg-info/PKG-INFO` & `hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.0.49
+Version: 1.0.50
 Summary: Utilities for AI - Assisted Mapping fAIr
 Author-email: Omdena <project@omdena.com>, Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hot-fair-utilities-1.0.49/hot_fair_utilities.egg-info/SOURCES.txt` & `hot-fair-utilities-1.0.50/hot_fair_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.49/pyproject.toml` & `hot-fair-utilities-1.0.50/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hot-fair-utilities"
-version = "1.0.49"
+version = "1.0.50"
 description = "Utilities for AI - Assisted Mapping fAIr"
 readme = "README.md"
 authors = [{ name = "Omdena", email = "project@omdena.com" },{ name = "Hot Tech Team", email = "sysadmin@hotosm.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
 ]
 keywords = [
     "preprocessing", "inference", 
     "postprocessing", "stitching","training"
 ]
 dependencies = [
     "shapely==1.8.0", "GDAL", "numpy", 
-    "Pillow==9.0.1", "geopandas==0.10.2", 
+    "Pillow==9.0.1", "geopandas==0.10.2","pandas==1.5.3", 
     "rasterio", "mercantile==1.2.1", "tqdm==4.62.3", 
     "rtree", "opencv-python==4.5.5.64","ramp-fair==0.1.2"
 ]
 requires-python = ">=3.7"
 
     [project.optional-dependencies]
     build = ["build", "twine"]
```

