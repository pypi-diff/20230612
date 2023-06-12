# Comparing `tmp/cognitive-service-vision-model-customization-python-samples-0.0.4.tar.gz` & `tmp/cognitive-service-vision-model-customization-python-samples-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognitive-service-vision-model-customization-python-samples-0.0.4.tar", last modified: Tue May 23 03:12:41 2023, max compression
+gzip compressed data, was "cognitive-service-vision-model-customization-python-samples-0.0.5.tar", last modified: Mon Jun 12 17:15:47 2023, max compression
```

## Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4.tar` & `cognitive-service-vision-model-customization-python-samples-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.955618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.963618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/prediction_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/training_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.963618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/training_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.955618 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 03:12:41.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:41.967618 cognitive-service-vision-model-customization-python-samples-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_coco_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-23 03:12:30.000000 cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/prediction_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/training_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/training_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_coco_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_e2e.py
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/LICENSE` & `cognitive-service-vision-model-customization-python-samples-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/LICENSE.md` & `cognitive-service-vision-model-customization-python-samples-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/PKG-INFO` & `cognitive-service-vision-model-customization-python-samples-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitive-service-vision-model-customization-python-samples
-Version: 0.0.4
+Version: 0.0.5
 Summary: A sample code repo for model customization using Python for Cognitive Service for Vision.
 Home-page: 
 Author: Ping Jin
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/README.md` & `cognitive-service-vision-model-customization-python-samples-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/__init__.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/__init__.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     def request_post(self, path, params=None, data=None, content_type=None):
         assert data is None or content_type
 
         params = params or {}
         headers = dict(self._headers, **{'Content-Type': content_type}) if content_type else self._headers
         r = requests.post(self._construct_url(path), data=data, params=dict(self._params, **params), headers=headers)
 
-        if r.get(headers['Content-Type'], None) == 'image/jpeg':
+        if r.headers.get('Content-Type', None) == 'image/jpeg':
             return r.content
 
         return self._get_json_response(r)
 
     def request_patch(self, path, json):
         r = requests.patch(self._construct_url(path), json=json, params=self._params, headers=self._headers)
         return self._get_json_response(r)
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/clients/training_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/training_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/__init__.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/models/training_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/training_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitive-service-vision-model-customization-python-samples
-Version: 0.0.4
+Version: 0.0.5
 Summary: A sample code repo for model customization using Python for Cognitive Service for Vision.
 Home-page: 
 Author: Ping Jin
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt` & `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/setup.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 from os import path
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), 'r') as f:
     long_description = f.read()
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_clients.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_clients.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_coco_check.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_coco_check.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.4/test/test_e2e.py` & `cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_e2e.py`

 * *Files identical despite different names*

