# Comparing `tmp/onnx-predict-yolov8-1.0.5.tar.gz` & `tmp/onnx-predict-yolov8-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-predict-yolov8-1.0.5.tar", last modified: Thu May 25 08:18:31 2023, max compression
+gzip compressed data, was "onnx-predict-yolov8-1.0.6.tar", last modified: Mon Jun 12 12:55:29 2023, max compression
```

## Comparing `onnx-predict-yolov8-1.0.5.tar` & `onnx-predict-yolov8-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 08:18:31.970624 onnx-predict-yolov8-1.0.5/
--rw-rw-rw-   0        0        0     1096 2023-05-23 12:24:50.000000 onnx-predict-yolov8-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2467 2023-05-25 08:18:31.969594 onnx-predict-yolov8-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-05-24 08:47:57.000000 onnx-predict-yolov8-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 08:18:31.965144 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/
--rw-rw-rw-   0        0        0     2467 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-25 08:18:31.000000 onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 08:18:31.968652 onnx-predict-yolov8-1.0.5/opyv8/
--rw-rw-rw-   0        0        0       61 2023-05-23 09:27:35.000000 onnx-predict-yolov8-1.0.5/opyv8/__init__.py
--rw-rw-rw-   0        0        0     1185 2023-05-24 09:41:37.000000 onnx-predict-yolov8-1.0.5/opyv8/model.py
--rw-rw-rw-   0        0        0     2501 2023-05-24 09:57:12.000000 onnx-predict-yolov8-1.0.5/opyv8/predictor.py
--rw-rw-rw-   0        0        0     2362 2023-05-24 09:57:28.000000 onnx-predict-yolov8-1.0.5/opyv8/utils.py
--rw-rw-rw-   0        0        0      629 2023-05-25 08:17:31.000000 onnx-predict-yolov8-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 08:18:31.970624 onnx-predict-yolov8-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 12:55:29.404477 onnx-predict-yolov8-1.0.6/
+-rw-rw-rw-   0        0        0     1096 2023-05-23 12:24:50.000000 onnx-predict-yolov8-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2467 2023-06-12 12:55:29.403464 onnx-predict-yolov8-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-05-24 08:47:57.000000 onnx-predict-yolov8-1.0.6/README.md
+-rw-rw-rw-   0        0        0      780 2023-06-12 12:53:45.000000 onnx-predict-yolov8-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:55:29.404477 onnx-predict-yolov8-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 12:55:29.367397 onnx-predict-yolov8-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 12:55:29.392456 onnx-predict-yolov8-1.0.6/src/onnx_predict_yolov8.egg-info/
+-rw-rw-rw-   0        0        0     2467 2023-06-12 12:55:29.000000 onnx-predict-yolov8-1.0.6/src/onnx_predict_yolov8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-06-12 12:55:29.000000 onnx-predict-yolov8-1.0.6/src/onnx_predict_yolov8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:55:29.000000 onnx-predict-yolov8-1.0.6/src/onnx_predict_yolov8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-12 12:55:29.000000 onnx-predict-yolov8-1.0.6/src/onnx_predict_yolov8.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 12:55:29.000000 onnx-predict-yolov8-1.0.6/src/onnx_predict_yolov8.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 12:55:29.402463 onnx-predict-yolov8-1.0.6/src/opyv8/
+-rw-rw-rw-   0        0        0       61 2023-05-23 09:27:35.000000 onnx-predict-yolov8-1.0.6/src/opyv8/__init__.py
+-rw-rw-rw-   0        0        0     1185 2023-05-24 09:41:37.000000 onnx-predict-yolov8-1.0.6/src/opyv8/model.py
+-rw-rw-rw-   0        0        0     2501 2023-06-12 12:31:38.000000 onnx-predict-yolov8-1.0.6/src/opyv8/predictor.py
+-rw-rw-rw-   0        0        0     2366 2023-06-12 12:30:17.000000 onnx-predict-yolov8-1.0.6/src/opyv8/utils.py
```

### Comparing `onnx-predict-yolov8-1.0.5/LICENSE` & `onnx-predict-yolov8-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-predict-yolov8-1.0.5/PKG-INFO` & `onnx-predict-yolov8-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-predict-yolov8
-Version: 1.0.5
+Version: 1.0.6
 Author-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>, Kristian Torp <torp@cs.aau.dk>
 Maintainer-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>
 License: MIT License
         
         Copyright (c) 2023 Aalborg University
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnx-predict-yolov8-1.0.5/README.md` & `onnx-predict-yolov8-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `onnx-predict-yolov8-1.0.5/onnx_predict_yolov8.egg-info/PKG-INFO` & `onnx-predict-yolov8-1.0.6/src/onnx_predict_yolov8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-predict-yolov8
-Version: 1.0.5
+Version: 1.0.6
 Author-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>, Kristian Torp <torp@cs.aau.dk>
 Maintainer-email: Kasper Fromm Pedersen <kasperf@cs.aau.dk>
 License: MIT License
         
         Copyright (c) 2023 Aalborg University
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnx-predict-yolov8-1.0.5/opyv8/model.py` & `onnx-predict-yolov8-1.0.6/src/opyv8/model.py`

 * *Files identical despite different names*

### Comparing `onnx-predict-yolov8-1.0.5/opyv8/predictor.py` & `onnx-predict-yolov8-1.0.6/src/opyv8/predictor.py`

 * *Files identical despite different names*

### Comparing `onnx-predict-yolov8-1.0.5/opyv8/utils.py` & `onnx-predict-yolov8-1.0.6/src/opyv8/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,18 @@
         sorted_indices = sorted_indices[keep_indices + 1]
 
     return keep_boxes
 
 
 def image_to_tensor(img: Image, model: PInferenceSession) -> ImageTensor:
     _, _, width, height = model.get_inputs()[0].shape
-    original_size = img.size
+
     img = ImageOps.exif_transpose(img)
+    original_size = img.size
+
     img = ImageOps.contain(img, (width, height), Resampling.BILINEAR)
     scale_size = img.size
 
     img = ImageOps.pad(
         img, (width, height), Resampling.BILINEAR, (114, 114, 114), (0, 0)
     )
     data = numpy.array(img)
```

### Comparing `onnx-predict-yolov8-1.0.5/pyproject.toml` & `onnx-predict-yolov8-1.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "onnx-predict-yolov8"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 readme = "README.md"
 authors = [
     {name = "Kasper Fromm Pedersen", email = "kasperf@cs.aau.dk"},
     {name = "Kristian Torp", email = "torp@cs.aau.dk"}
 ]
 maintainers = [
@@ -14,10 +14,19 @@
 keywords = ["ONNX", "YOLOv8", "onnxruntime", "vision"]
 requires-python = ">=3.8,<3.12"
 dependencies = [
     "numpy>=1.20",
     "Pillow>=9.1.0",
 ]
 
+[tool.pdm.dev-dependencies]
+test = [
+    "onnxruntime~=1.15.0",
+    "typer[all]~=0.9.0"
+]
+
 [project.urls]
 homepage = "https://www.cs.aau.dk/"
-repository = "https://github.com/fromm1990/onnx-predict-yolov8"
+repository = "https://github.com/fromm1990/onnx-predict-yolov8"
+
+[tool.pdm.scripts]
+predict = "python cli/main.py"
```

