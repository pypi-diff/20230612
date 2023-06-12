# Comparing `tmp/waffle_hub-0.2.2.tar.gz` & `tmp/waffle_hub-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.2.2.tar", last modified: Fri Jun  2 11:05:31 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.3.tar", last modified: Mon Jun 12 07:52:06 2023, max compression
```

## Comparing `waffle_hub-0.2.2.tar` & `waffle_hub-0.2.3.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/
--rw-r--r--   0 zero      (1000) zero      (1000)    35149 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/LICENSE
--rw-r--r--   0 zero      (1000) zero      (1000)      138 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/MANIFEST.in
--rw-r--r--   0 zero      (1000) zero      (1000)     1962 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/PKG-INFO
--rw-r--r--   0 zero      (1000) zero      (1000)      881 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/README.md
--rw-r--r--   0 zero      (1000) zero      (1000)      385 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/requirements.txt
--rw-r--r--   0 zero      (1000) zero      (1000)       38 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/setup.cfg
--rw-r--r--   0 zero      (1000) zero      (1000)     2670 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/setup.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.875476 waffle_hub-0.2.2/tests/
--rw-r--r--   0 zero      (1000) zero      (1000)     8047 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/tests/test_cli.py
--rw-r--r--   0 zero      (1000) zero      (1000)    12185 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/tests/test_dataset.py
--rw-r--r--   0 zero      (1000) zero      (1000)    10733 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/tests/test_hub.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.875476 waffle_hub-0.2.2/waffle_hub/
--rw-r--r--   0 zero      (1000) zero      (1000)     3723 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/__init__.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.875476 waffle_hub-0.2.2/waffle_hub/dataset/
--rw-r--r--   0 zero      (1000) zero      (1000)       53 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/__init__.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/dataset/adapter/
--rw-r--r--   0 zero      (1000) zero      (1000)      168 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/adapter/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     2992 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/adapter/coco.py
--rw-r--r--   0 zero      (1000) zero      (1000)     4780 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/adapter/huggingface.py
--rw-r--r--   0 zero      (1000) zero      (1000)     7223 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/adapter/yolo.py
--rw-r--r--   0 zero      (1000) zero      (1000)    51612 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/dataset/dataset.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/experimental/
--rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/experimental/__init__.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/experimental/auto_label/
--rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/experimental/auto_label/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     7920 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-r--r--   0 zero      (1000) zero      (1000)     2986 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/experimental/serve.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/
--rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/__init__.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/
--rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/__init__.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/
--rw-r--r--   0 zero      (1000) zero      (1000)       75 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     9319 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
--rw-r--r--   0 zero      (1000) zero      (1000)     2409 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/config.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/
--rw-r--r--   0 zero      (1000) zero      (1000)      129 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     1913 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
--rw-r--r--   0 zero      (1000) zero      (1000)     3660 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/
--rw-r--r--   0 zero      (1000) zero      (1000)       75 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     2406 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/config.py
--rw-r--r--   0 zero      (1000) zero      (1000)    10318 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
--rw-r--r--   0 zero      (1000) zero      (1000)     8490 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/train_input_helper.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/
--rw-r--r--   0 zero      (1000) zero      (1000)       74 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     4252 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/config.py
--rw-r--r--   0 zero      (1000) zero      (1000)    12302 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-r--r--   0 zero      (1000) zero      (1000)    37067 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/base_hub.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/hub/model/
--rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/model/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)    12854 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/hub/model/wrapper.py
--rw-r--r--   0 zero      (1000) zero      (1000)    12811 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/run.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/schema/
--rw-r--r--   0 zero      (1000) zero      (1000)      345 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     1169 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/base_schema.py
--rw-r--r--   0 zero      (1000) zero      (1000)     1699 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/configs.py
--rw-r--r--   0 zero      (1000) zero      (1000)      785 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/data.py
--rw-r--r--   0 zero      (1000) zero      (1000)      304 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/evaluate.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/schema/fields/
--rw-r--r--   0 zero      (1000) zero      (1000)      138 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)    17217 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/annotation.py
--rw-r--r--   0 zero      (1000) zero      (1000)     1455 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/base_field.py
--rw-r--r--   0 zero      (1000) zero      (1000)     7241 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/category.py
--rw-r--r--   0 zero      (1000) zero      (1000)     2599 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/fields/image.py
--rw-r--r--   0 zero      (1000) zero      (1000)      496 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/schema/result.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.885476 waffle_hub-0.2.2/waffle_hub/utils/
--rw-r--r--   0 zero      (1000) zero      (1000)        0 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/__init__.py
--rw-r--r--   0 zero      (1000) zero      (1000)     3694 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/callback.py
--rw-r--r--   0 zero      (1000) zero      (1000)     1686 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/conversion.py
--rw-r--r--   0 zero      (1000) zero      (1000)     5650 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/data.py
--rw-r--r--   0 zero      (1000) zero      (1000)     3218 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/draw.py
--rw-r--r--   0 zero      (1000) zero      (1000)     3706 2023-06-02 10:53:30.000000 waffle_hub-0.2.2/waffle_hub/utils/evaluate.py
-drwxr-xr-x   0 zero      (1000) zero      (1000)        0 2023-06-02 11:05:31.875476 waffle_hub-0.2.2/waffle_hub.egg-info/
--rw-r--r--   0 zero      (1000) zero      (1000)     1962 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/PKG-INFO
--rw-r--r--   0 zero      (1000) zero      (1000)     2098 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/SOURCES.txt
--rw-r--r--   0 zero      (1000) zero      (1000)        1 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/dependency_links.txt
--rw-r--r--   0 zero      (1000) zero      (1000)       68 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/entry_points.txt
--rw-r--r--   0 zero      (1000) zero      (1000)      302 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/requires.txt
--rw-r--r--   0 zero      (1000) zero      (1000)       11 2023-06-02 11:05:31.000000 waffle_hub-0.2.2/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      881 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      385 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2670 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8049 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/tests/test_cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    14730 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/tests/test_dataset.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3082 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/tests/test_ddp.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10674 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1581 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/dataset/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/dataset/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/dataset/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      239 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3423 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/autocare_dlt.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2992 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/coco.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4785 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/transformers.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7223 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/dataset/adapter/yolo.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    59466 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/dataset/dataset.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/experimental/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/experimental/auto_label/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/experimental/auto_label/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2078 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10097 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4377 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/config.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5865 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       77 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2406 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8490 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/train_input_helper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10319 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/transformers_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4252 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    12534 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    40833 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/base_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    13840 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/hub/model/wrapper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    12819 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      378 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/schema/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/schema/fields/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    17217 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/annotation.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/base_field.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/category.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/fields/image.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/schema/result.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/utils/conversion.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-06-12 07:00:05.000000 waffle_hub-0.2.3/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4200 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/utils/draw.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4420 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/utils/evaluate.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      631 2023-06-12 07:51:09.000000 waffle_hub-0.2.3/waffle_hub/utils/process.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:52:06.172147 waffle_hub-0.2.3/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2188 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       68 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      302 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-06-12 07:52:06.000000 waffle_hub-0.2.3/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.2.2/LICENSE` & `waffle_hub-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/PKG-INFO` & `waffle_hub-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.2.2
+Version: 0.2.3
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.2 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.3 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.2/README.md` & `waffle_hub-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/setup.py` & `waffle_hub-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/tests/test_cli.py` & `waffle_hub-0.2.3/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,22 +59,22 @@
         --yaml-path {yolo_dir / 'data.yaml'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "from_yolo").exists()
 
 
-def test_dataset_from_huggingface(test_dir: Path):
+def test_dataset_from_transformers(test_dir: Path):
     url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist_huggingface_classification.zip"
     hf_dir = test_dir / "datasets" / "mnist_hf"
 
     get_file_from_url(url, str(test_dir), True)
     unzip(str(test_dir / "mnist_huggingface_classification.zip"), hf_dir)
 
-    cmd = f"python -m waffle_hub.run dataset from_huggingface \
+    cmd = f"python -m waffle_hub.run dataset from_transformers \
         --name from_hf \
         --root-dir {test_dir / 'datasets'} \
         --task classification \
         --dataset-dir {hf_dir} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
```

### Comparing `waffle_hub-0.2.2/tests/test_dataset.py` & `waffle_hub-0.2.3/tests/test_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,14 +72,21 @@
         annotation_id=1,
         image_id=1,
         category_id=1,
         keypoints=keypoints,
         num_keypoints=3,
     )
 
+    # text recognition
+    a = Annotation.text_recognition(
+        annotation_id=1,
+        image_id=1,
+        caption="1",
+    )
+
 
 def test_image():
 
     image = Image.new(
         image_id=1,
         file_name="test.jpg",
         width=100,
@@ -121,14 +128,21 @@
         category_id=1,
         name="test",
         supercategory="object",
         keypoints=["a", "b", "c"],
         skeleton=[[1, 2], [2, 3]],
     )
 
+    # text recognition
+    category = Category.text_recognition(
+        category_id=1,
+        name="test",
+        supercategory="object",
+    )
+
 
 def test_dataset(tmpdir):
 
     dataset: Dataset = Dataset.new(name="test_new", task=TaskType.OBJECT_DETECTION, root_dir=tmpdir)
     assert Path(dataset.dataset_dir).exists()
 
     dataset.delete()
@@ -183,15 +197,55 @@
     dataset.split(0.05)
 
     if task in [TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION, TaskType.CLASSIFICATION]:
         dataset.export("coco")
     if task in [TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION, TaskType.CLASSIFICATION]:
         dataset.export("yolo")
     if task in [TaskType.OBJECT_DETECTION, TaskType.CLASSIFICATION]:
-        dataset.export("huggingface")
+        dataset.export("transformers")
+    if task in [TaskType.OBJECT_DETECTION, TaskType.TEXT_RECOGNITION, TaskType.CLASSIFICATION]:
+        dataset.export("autocare_dlt")
+
+
+# test dummy
+def _dummy(dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir):
+    dataset = Dataset.dummy(
+        name=dataset_name,
+        task=task,
+        image_num=image_num,
+        category_num=category_num,
+        unlabeld_image_num=unlabeled_image_num,
+        root_dir=root_dir,
+    )
+    assert len(dataset.images) == image_num
+    assert len(dataset.categories) == category_num
+    assert len(dataset.unlabeled_images) == unlabeled_image_num
+
+
+def _total_dummy(
+    dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir
+):
+    _dummy(dataset_name, task, image_num, category_num, unlabeled_image_num, root_dir)
+    _load(dataset_name, root_dir)
+    _clone(dataset_name, root_dir)
+    _split(dataset_name, root_dir)
+    _export(dataset_name, task, root_dir)
+
+
+def test_dummy(tmpdir):
+    for task in [
+        TaskType.CLASSIFICATION,
+        TaskType.OBJECT_DETECTION,
+        TaskType.INSTANCE_SEGMENTATION,
+        TaskType.TEXT_RECOGNITION,
+    ]:
+        _total_dummy(f"dummy_{task}", task, 100, 5, 10, tmpdir)
+
+    with pytest.raises(ValueError):
+        _total_dummy("dummy", TaskType.CLASSIFICATION, 3, 3, 0, tmpdir)
 
 
 # test dummy
 def _dummy(dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir):
     dataset = Dataset.dummy(
         name=dataset_name,
         task=task,
@@ -265,50 +319,79 @@
     _from_coco(dataset_name, task, coco_path, root_dir)
     _load(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, task, root_dir)
 
 
-def test_coco(coco_path, tmpdir):
-    for task in [TaskType.CLASSIFICATION, TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION]:
-        _total_coco(f"coco_{task}", task, coco_path, tmpdir)
+@pytest.mark.parametrize(
+    "task", [TaskType.CLASSIFICATION, TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION]
+)
+def test_coco(coco_path, tmpdir, task):
+    _total_coco(f"coco_{task}", task, coco_path, tmpdir)
+
+
+# test autocare_dlt
+def _from_autocare_dlt(dataset_name, task: TaskType, coco_path, root_dir):
+    dataset = Dataset.from_autocare_dlt(
+        name=dataset_name,
+        task=task,
+        coco_file=coco_path / "coco.json",
+        coco_root_dir=coco_path / "images",
+        root_dir=root_dir,
+    )
+    assert dataset.dataset_info_file.exists()
+
+
+def _total_autocare_dlt(dataset_name, task: TaskType, coco_path, root_dir):
+    _from_autocare_dlt(dataset_name, task, coco_path, root_dir)
+    _load(dataset_name, root_dir)
+    _clone(dataset_name, root_dir)
+    _split(dataset_name, root_dir)
+    _export(dataset_name, task, root_dir)
+
+
+@pytest.mark.parametrize(
+    "task", [TaskType.CLASSIFICATION, TaskType.OBJECT_DETECTION, TaskType.TEXT_RECOGNITION]
+)
+def test_autocare_dlt(coco_path, tmpdir, task):
+    _total_autocare_dlt(f"autocare_dlt_{task}", task, coco_path, tmpdir)
 
 
-# test huggingface
-def _from_huggingface(dataset_name, task: TaskType, huggingface_path, root_dir):
-    dataset = Dataset.from_huggingface(
+# test transformers
+def _from_transformers(dataset_name, task: TaskType, transformers_path, root_dir):
+    dataset = Dataset.from_transformers(
         name=dataset_name,
         task=task,
-        dataset_dir=huggingface_path,
+        dataset_dir=transformers_path,
         root_dir=root_dir,
     )
     assert dataset.dataset_info_file.exists()
 
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) == 80
     assert len(dataset.images) == 100
 
 
-def _total_huggingface(dataset_name, task: TaskType, huggingface_path, root_dir):
-    _from_huggingface(dataset_name, task, huggingface_path, root_dir)
+def _total_transformers(dataset_name, task: TaskType, transformers_path, root_dir):
+    _from_transformers(dataset_name, task, transformers_path, root_dir)
     _load(dataset_name, root_dir)
     _clone(dataset_name, root_dir)
     _split(dataset_name, root_dir)
     _export(dataset_name, task, root_dir)
 
 
-def test_huggingface(huggingface_detection_path, huggingface_classification_path, tmpdir):
-    _total_huggingface(
-        "huggingface_object_detection", TaskType.OBJECT_DETECTION, huggingface_detection_path, tmpdir
+def test_transformers(transformers_detection_path, transformers_classification_path, tmpdir):
+    _total_transformers(
+        "transformers_object_detection", TaskType.OBJECT_DETECTION, transformers_detection_path, tmpdir
     )
-    _total_huggingface(
-        "huggingface_classification",
+    _total_transformers(
+        "transformers_classification",
         TaskType.CLASSIFICATION,
-        huggingface_classification_path,
+        transformers_classification_path,
         tmpdir,
     )
 
 
 # dataloader
 def test_image_dataloader(coco_path, tmpdir):
```

### Comparing `waffle_hub-0.2.2/tests/test_hub.py` & `waffle_hub-0.2.3/tests/test_hub.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,26 @@
 import time
 from pathlib import Path
 
-import pytest
 import torch
 
 from waffle_hub import TaskType
 from waffle_hub.dataset import Dataset
+from waffle_hub.hub import get_hub, load_hub
 from waffle_hub.hub.adapter.autocare_dlt import AutocareDLTHub
-from waffle_hub.hub.adapter.hugging_face import HuggingFaceHub
+from waffle_hub.hub.adapter.transformers import TransformersHub
 from waffle_hub.hub.adapter.ultralytics import UltralyticsHub
 from waffle_hub.schema.result import (
     EvaluateResult,
     ExportResult,
     InferenceResult,
     TrainResult,
 )
 
 
-@pytest.fixture
-def instance_segmentation_dataset(coco_path: Path, tmpdir: Path):
-    dataset: Dataset = Dataset.from_coco(
-        name="seg",
-        task=TaskType.INSTANCE_SEGMENTATION,
-        coco_file=coco_path / "coco.json",
-        coco_root_dir=coco_path / "images",
-        root_dir=tmpdir,
-    )
-    dataset.split(0.2, 0.2, 0.6)
-
-    return dataset
-
-
-@pytest.fixture
-def object_detection_dataset(coco_path: Path, tmpdir: Path):
-    dataset: Dataset = Dataset.from_coco(
-        name="od",
-        task=TaskType.OBJECT_DETECTION,
-        coco_file=coco_path / "coco.json",
-        coco_root_dir=coco_path / "images",
-        root_dir=tmpdir,
-    )
-    dataset.split(0.2, 0.2, 0.6)
-
-    return dataset
-
-
-@pytest.fixture
-def classification_dataset(coco_path: Path, tmpdir: Path):
-    dataset: Dataset = Dataset.from_coco(
-        name="cls",
-        task=TaskType.CLASSIFICATION,
-        coco_file=coco_path / "coco.json",
-        coco_root_dir=coco_path / "images",
-        root_dir=tmpdir,
-    )
-    dataset.split(0.2, 0.2, 0.6)
-
-    return dataset
-
-
 def _train(hub, dataset: Dataset, image_size: int, hold: bool = True):
     result: TrainResult = hub.train(
         dataset_path=dataset.export(hub.backend),
         epochs=1,
         image_size=image_size,
         batch_size=4,
         pretrained_model=None,
@@ -166,23 +124,36 @@
     assert len(feature_maps) == 1
 
 
 def _benchmark(hub, image_size):
     hub.benchmark(device="cpu", half=False, image_size=image_size)
 
 
+def _util(hub):
+    name = hub.name
+    backend = hub.backend
+    root_dir = hub.root_dir
+
+    hub_class = get_hub(backend)
+    assert hub_class == type(hub)
+
+    hub_loaded = load_hub(name, root_dir)
+    assert isinstance(hub_loaded, type(hub))
+
+
 def _total(hub, dataset: Dataset, image_size: int, hold: bool = True):
 
     _train(hub, dataset, image_size, hold=hold)
     _evaluate(hub, dataset, hold=hold)
     _inference(hub, dataset.raw_image_dir, hold=hold)
     _export(hub, half=False, hold=hold)
     # _export(hub, half=True, hold=hold)  # cpu cannot be half
     _feature_extraction(hub, image_size)
     _benchmark(hub, image_size)
+    _util(hub)
 
 
 def test_ultralytics_segmentation(instance_segmentation_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = instance_segmentation_dataset
 
     # test hub
@@ -249,56 +220,56 @@
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
-def test_huggingface_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
+def test_transformers_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = object_detection_dataset
 
     # test hub
     name = "test_det"
-    hub = HuggingFaceHub.new(
+    hub = TransformersHub.new(
         name=name,
         task=TaskType.OBJECT_DETECTION,
         model_type="YOLOS",
         model_size="tiny",
         categories=object_detection_dataset.category_names,
         root_dir=tmpdir,
     )
-    hub = HuggingFaceHub.load(name=name, root_dir=tmpdir)
-    hub: HuggingFaceHub = HuggingFaceHub.from_model_config(
+    hub = TransformersHub.load(name=name, root_dir=tmpdir)
+    hub: TransformersHub = TransformersHub.from_model_config(
         name=name,
-        model_config_file=tmpdir / name / HuggingFaceHub.MODEL_CONFIG_FILE,
+        model_config_file=tmpdir / name / TransformersHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
-def test_huggingface_classification(classification_dataset: Dataset, tmpdir: Path):
+def test_transformers_classification(classification_dataset: Dataset, tmpdir: Path):
     image_size = 224
     dataset = classification_dataset
 
     # test hub
     name = "test_cls"
-    hub = HuggingFaceHub.new(
+    hub = TransformersHub.new(
         name=name,
         task=TaskType.CLASSIFICATION,
         model_type="ViT",
         model_size="tiny",
         categories=classification_dataset.category_names,
         root_dir=tmpdir,
     )
-    hub = HuggingFaceHub.load(name=name, root_dir=tmpdir)
-    hub: HuggingFaceHub = HuggingFaceHub.from_model_config(
+    hub = TransformersHub.load(name=name, root_dir=tmpdir)
+    hub: TransformersHub = TransformersHub.from_model_config(
         name=name,
-        model_config_file=tmpdir / name / HuggingFaceHub.MODEL_CONFIG_FILE,
+        model_config_file=tmpdir / name / TransformersHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
 def test_non_hold(classification_dataset: Dataset, tmpdir: Path):
@@ -376,10 +347,34 @@
         root_dir=tmpdir,
     )
     hub = AutocareDLTHub.load(name=name, root_dir=tmpdir)
     hub: AutocareDLTHub = AutocareDLTHub.from_model_config(
         name=name,
         model_config_file=tmpdir / name / AutocareDLTHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
+    )
+
+    _total(hub, dataset, image_size)
+
+
+def test_autocare_dlt_text_recognition(text_recognition_dataset: Dataset, tmpdir: Path):
+    image_size = 32
+    dataset = text_recognition_dataset
+
+    # test hub
+    name = "test_ocr"
+    hub = AutocareDLTHub.new(
+        name=name,
+        task=TaskType.TEXT_RECOGNITION,
+        model_type="TextRecognition",
+        model_size="s",
+        categories=dataset.category_names,
+        root_dir=tmpdir,
+    )
+    hub = AutocareDLTHub.load(name=name, root_dir=tmpdir)
+    hub: AutocareDLTHub = AutocareDLTHub.from_model_config(
+        name=name,
+        model_config_file=tmpdir / name / AutocareDLTHub.MODEL_CONFIG_FILE,
+        root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
```

### Comparing `waffle_hub-0.2.2/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.2.3/waffle_hub/dataset/adapter/coco.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/dataset/adapter/huggingface.py` & `waffle_hub-0.2.3/waffle_hub/dataset/adapter/transformers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     Sequence,
     Value,
 )
 from waffle_hub import TaskType
 from waffle_hub.schema.fields import Image
 
 
-def _export_huggingface_classification(
+def _export_transformers_classification(
     self,
     export_dir: Path,
     train_ids: list,
     val_ids: list,
     test_ids: list,
     unlabeled_ids: list,
 ):
-    """Export dataset to Hugging Face format for classification task
+    """Export dataset to Transformers format for classification task
 
     Args:
         export_dir (Path): Path to export directory
         train_ids (list): List of train ids
         val_ids (list): List of validation ids
         test_ids (list): List of test ids
         unlabeled_ids (list): List of unlabeled ids
@@ -61,23 +61,23 @@
             lambda: _export(self.get_images(image_ids)), features=features
         )
 
     dataset = DatasetDict(dataset)
     dataset.save_to_disk(export_dir)
 
 
-def _export_huggingface_detection(
+def _export_transformers_detection(
     self,
     export_dir: Path,
     train_ids: list,
     val_ids: list,
     test_ids: list,
     unlabeled_ids: list,
 ):
-    """Export dataset to Hugging Face format for detection task
+    """Export dataset to Transformers format for detection task
 
     Args:
         export_dir (Path): Path to export directory
         train_ids (list): List of train ids
         val_ids (list): List of validation ids
         test_ids (list): List of test ids
         unlabeled_ids (list): List of unlabeled ids
@@ -137,28 +137,28 @@
             lambda: _export(self.get_images(image_ids)), features=features
         )
 
     dataset = DatasetDict(dataset)
     dataset.save_to_disk(export_dir)
 
 
-def export_huggingface(self, export_dir: Union[str, Path]) -> str:
-    """Export dataset to Hugging Face format
+def export_transformers(self, export_dir: Union[str, Path]) -> str:
+    """Export dataset to Transformers format
 
     Args:
         export_dir (str): Path to export directory
 
     Returns:
         str: Path to export directory
     """
     export_dir = Path(export_dir)
 
     train_ids, val_ids, test_ids, _ = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
-        _export_huggingface_classification(self, export_dir, train_ids, val_ids, test_ids, [])
+        _export_transformers_classification(self, export_dir, train_ids, val_ids, test_ids, [])
     elif self.task == TaskType.OBJECT_DETECTION:
-        _export_huggingface_detection(self, export_dir, train_ids, val_ids, test_ids, [])
+        _export_transformers_detection(self, export_dir, train_ids, val_ids, test_ids, [])
     else:
         raise ValueError(f"Unsupported task type: {self.task}")
 
     return str(export_dir)
```

### Comparing `waffle_hub-0.2.2/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.3/waffle_hub/dataset/adapter/yolo.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.3/waffle_hub/dataset/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 from waffle_utils.log import datetime_now
 from waffle_utils.utils import type_validator
 
 from datasets import Dataset as HFDataset
 from datasets import DatasetDict, load_from_disk
 from waffle_hub import DataType, SplitMethod, TaskType
 from waffle_hub.dataset.adapter import (
+    export_autocare_dlt,
     export_coco,
-    export_huggingface,
+    export_transformers,
     export_yolo,
 )
 from waffle_hub.schema import Annotation, Category, DatasetInfo, Image
 
 logger = logging.getLogger(__name__)
 
 
@@ -213,19 +214,31 @@
             self._category_to_annotations = dict(category_to_annotations)
         return self._category_to_annotations
 
     @cached_property
     def category_to_images(self) -> dict[int, list[Image]]:
         if not hasattr(self, "_category_to_images"):
             category_to_images = {category_id: [] for category_id in self.categories.keys()}
+            category_name_to_id = {
+                category.name: category.category_id for category in self.categories.values()
+            }
             for image_id, annotations in tqdm.tqdm(
                 self.image_to_annotations.items(), desc="Building category to image index"
             ):
-                category_count = Counter(map(lambda a: a.category_id, annotations))
-                category_to_images[category_count.most_common(1)[0][0]].append(self.images[image_id])
+                if self.task == TaskType.TEXT_RECOGNITION:
+                    texts = map(lambda a: a.caption, annotations)
+                    character_count = Counter("".join(texts))
+                    for k in character_count:
+                        category_to_images[category_name_to_id[k]].append(self.images[image_id])
+                else:
+                    category_ids = map(lambda a: a.category_id, annotations)
+                    category_count = Counter(category_ids)
+                    category_to_images[category_count.most_common(1)[0][0]].append(
+                        self.images[image_id]
+                    )
             self._category_to_images = dict(category_to_images)
         return self._category_to_images
 
     @cached_property
     def num_images_per_category(self) -> dict[int, int]:
         if not hasattr(self, "_num_images_per_category"):
             self._num_images_per_category = {
@@ -370,14 +383,20 @@
                     )
                 elif task == TaskType.INSTANCE_SEGMENTATION:
                     category = Category.instance_segmentation(
                         category_id=category_id,
                         name=f"category_{category_id}",
                         supercategory="object",
                     )
+                elif task == TaskType.TEXT_RECOGNITION:
+                    category = Category.text_recognition(
+                        category_id=category_id,
+                        name=chr(64 + category_id),
+                        supercategory="object",
+                    )
 
                 ds.add_categories([category])
 
             annotation_id = 1
             for image_id in range(1, image_num + 1):
                 file_name = f"image_{image_id}.jpg"
                 ds.add_images([Image(image_id=image_id, file_name=file_name, width=100, height=100)])
@@ -418,15 +437,22 @@
                                 random.randint(0, 100),
                                 random.randint(0, 100),
                             ],
                             segmentation=[[random.randint(0, 100) for _ in range(10)]],
                         )
                         for i in range(random.randint(1, 5))
                     ]
-
+                elif task == TaskType.TEXT_RECOGNITION:
+                    annotations = [
+                        Annotation.text_recognition(
+                            annotation_id=annotation_id,
+                            image_id=image_id,
+                            caption=chr(64 + random.randint(1, category_num)),
+                        )
+                    ]
                 ds.add_annotations(annotations)
                 annotation_id += len(annotations)
 
             if unlabeld_image_num > 0:
                 for image_id in range(image_num + 1, image_num + unlabeld_image_num + 1):
                     file_name = f"image_{image_id}.jpg"
                     ds.add_images(
@@ -730,14 +756,164 @@
 
         # TODO: add unlabeled set
         io.save_json([], ds.unlabeled_set_file, create_directory=True)
 
         return ds
 
     @classmethod
+    def from_autocare_dlt(
+        cls,
+        name: str,
+        task: str,
+        coco_file: Union[str, list[str]],
+        coco_root_dir: Union[str, list[str]],
+        root_dir: str = None,
+    ) -> "Dataset":
+        """
+        Import dataset from autocare dlt format.
+        This method is used for importing dataset from autocare dlt format.
+
+        Args:
+            name (str): name of dataset.
+            task (str): task of dataset.
+            coco_file (Union[str, list[str]]): coco annotation file path.
+            coco_root_dir (Union[str, list[str]]): root directory of coco dataset.
+            root_dir (str, optional): root directory of dataset. Defaults to None.
+
+        Raises:
+            FileExistsError: if new dataset name already exist.
+
+        Examples:
+            # Import one coco json file.
+            >>> ds = Dataset.from_coco("my_dataset", "object_detection", "path/to/coco.json", "path/to/coco_root")
+            >>> ds.images
+            {1: <Image: 1>, 2: <Image: 2>, 3: <Image: 3>, 4: <Image: 4>, 5: <Image: 5>}
+            >>> ds.annotations
+            {1: <Annotation: 1>, 2: <Annotation: 2>, 3: <Annotation: 3>, 4: <Annotation: 4>, 5: <Annotation: 5>}
+            >>> ds.categories
+            {1: <Category: 1>, 2: <Category: 2>, 3: <Category: 3>, 4: <Category: 4>, 5: <Category: 5>}
+            >>> ds.category_names
+            ['person', 'bicycle', 'car', 'motorcycle', 'airplane']
+
+
+        Returns:
+            Dataset: Dataset Class.
+        """
+        ds = Dataset.new(name, task, root_dir)
+        ds.initialize()
+
+        if isinstance(coco_file, list) and isinstance(coco_root_dir, list):
+            if len(coco_file) != len(coco_root_dir):
+                raise ValueError("coco_file and coco_root_dir should have same length.")
+        if not isinstance(coco_file, list) and isinstance(coco_root_dir, list):
+            raise ValueError(
+                "ambiguous input. The number of coco_file should be same or greater than coco_root_dir."
+            )
+        if not isinstance(coco_file, list):
+            coco_file = [coco_file]
+        if not isinstance(coco_root_dir, list):
+            coco_root_dir = [coco_root_dir] * len(coco_file)
+
+        coco_files = coco_file
+        coco_root_dirs = coco_root_dir
+
+        if len(coco_files) == 1:
+            set_names = [None]
+        elif len(coco_files) == 2:
+            set_names = ["train", "val"]
+        elif len(coco_files) == 3:
+            set_names = ["train", "val", "test"]
+        else:
+            raise ValueError("coco_file should have 1, 2, or 3 files.")
+
+        cocos = [COCO(coco_file) for coco_file in coco_files]
+
+        # categories should be same between coco files
+        categories = cocos[0].loadCats(cocos[0].getCatIds())
+        for coco in cocos[1:]:
+            if categories != coco.loadCats(coco.getCatIds()):
+                raise ValueError("categories should be same between coco files.")
+
+        coco_cat_id_to_waffle_cat_id = {}
+        for i, category in enumerate(categories, start=1):
+            coco_category_id = category.pop("id")
+            coco_cat_id_to_waffle_cat_id[coco_category_id] = i
+            ds.add_categories([Category.from_dict({**category, "category_id": i}, task=ds.task)])
+
+        # import coco dataset
+        total_length = sum([len(coco.getImgIds()) for coco in cocos])
+        logging.info(f"Importing coco dataset. Total length: {total_length}")
+        pgbar = tqdm.tqdm(total=total_length, desc="Importing coco dataset")
+
+        image_id = 1
+        annotation_id = 1
+
+        # parse coco annotation file
+        for coco, coco_root_dir, set_name in tqdm.tqdm(zip(cocos, coco_root_dirs, set_names)):
+
+            image_ids = []
+            for coco_image_id, annotation_dicts in coco.imgToAnns.items():
+                if len(annotation_dicts) == 0:
+                    warnings.warn(f"image_id {coco_image_id} has no annotations.")
+                    continue
+
+                image_dict = coco.loadImgs(coco_image_id)[0]
+                image_dict.pop("id")
+
+                file_name = image_dict.pop("file_name")
+                image_path = Path(coco_root_dir) / file_name
+                if not image_path.exists():
+                    raise FileNotFoundError(f"{image_path} does not exist.")
+
+                if set_name:
+                    file_name = f"{set_name}/{file_name}"
+
+                ds.add_images(
+                    [Image.from_dict({**image_dict, "image_id": image_id, "file_name": file_name})]
+                )
+                io.copy_file(image_path, ds.raw_image_dir / file_name, create_directory=True)
+
+                for annotation_dict in annotation_dicts:
+                    annotation_dict.pop("id")
+                    ds.add_annotations(
+                        [
+                            Annotation.from_dict(
+                                {
+                                    **annotation_dict,
+                                    "image_id": image_id,
+                                    "annotation_id": annotation_id,
+                                    "category_id": coco_cat_id_to_waffle_cat_id[
+                                        annotation_dict["category_id"]
+                                    ],
+                                },
+                                task=ds.task,
+                            )
+                        ]
+                    )
+                    annotation_id += 1
+
+                image_ids.append(image_id)
+                image_id += 1
+                pgbar.update(1)
+
+            if set_name:
+                io.save_json(image_ids, ds.set_dir / f"{set_name}.json", create_directory=True)
+
+        pgbar.close()
+
+        if len(coco_files) == 2:
+            logging.info("copying val set to test set")
+            io.copy_file(ds.val_set_file, ds.test_set_file, create_directory=True)
+
+        # TODO: add unlabeled set
+        io.save_json([], ds.unlabeled_set_file, create_directory=True)
+
+        return ds
+
+    @classmethod
     def from_yolo(
         cls,
         name: str,
         task: str,
         yaml_path: str,
         root_dir: str = None,
     ) -> "Dataset":
@@ -898,37 +1074,37 @@
 
         # TODO: add unlabeled set
         io.save_json([], ds.unlabeled_set_file, create_directory=True)
 
         return ds
 
     @classmethod
-    def from_huggingface(
+    def from_transformers(
         cls,
         name: str,
         task: str,
         dataset_dir: str,
         root_dir=None,
     ) -> "Dataset":
         """
-        Import Dataset from huggingface datasets.
-        This method imports huggingface dataset from directory.
+        Import Dataset from transformers datasets.
+        This method imports transformers dataset from directory.
 
         Args:
             name (str): Dataset name.
-            dataset_dir (str): Hugging Face dataset directory.
+            dataset_dir (str): Transformers dataset directory.
             task (str): Task name.
             root_dir (str, optional): Dataset root directory. Defaults to None.
 
         Raises:
             FileExistsError: if dataset name already exists
             ValueError: if dataset is not Dataset or DatasetDict
 
         Examples:
-            >>> ds = Dataset.from_huggingface("huggingface", "object_detection", "path/to/huggingface/dataset")
+            >>> ds = Dataset.from_transformers("transformers", "object_detection", "path/to/transformers/dataset")
 
         Returns:
             Dataset: Dataset Class
         """
         ds = Dataset.new(name, task, root_dir)
         ds.initialize()
 
@@ -939,14 +1115,23 @@
         elif isinstance(dataset, HFDataset):
             is_splited = False
         else:
             raise ValueError("dataset should be Dataset or DatasetDict")
 
         def _import(dataset: HFDataset, task: str, image_ids: list[int]):
             if task == "object_detection":
+                categories = dataset.features["objects"].feature["category"].names
+                for category_id, category_name in enumerate(categories):
+                    category = Category.object_detection(
+                        category_id=category_id + 1,
+                        supercategory="object",
+                        name=category_name,
+                    )
+                    ds.add_categories([category])
+
                 for data in dataset:
                     data["image"].save(f"{ds.raw_image_dir}/{data['image_id']}.jpg")
                     image = Image.new(
                         image_id=data["image_id"],
                         file_name=f"{data['image_id']}.jpg",
                         width=data["width"],
                         height=data["height"],
@@ -966,24 +1151,24 @@
                             image_id=image.image_id,
                             category_id=category_id + 1,
                             area=area,
                             bbox=bbox,
                         )
                         ds.add_annotations([annotation])
 
-                categories = dataset.features["objects"].feature["category"].names
+            elif task == "classification":
+                categories = dataset.features["label"].names
                 for category_id, category_name in enumerate(categories):
-                    category = Category.object_detection(
+                    category = Category.classification(
                         category_id=category_id + 1,
                         supercategory="object",
                         name=category_name,
                     )
                     ds.add_categories([category])
 
-            elif task == "classification":
                 for image_id, data in zip(image_ids, dataset):
                     image_save_path = f"{ds.raw_image_dir}/{image_id}.jpg"
                     data["image"].save(image_save_path)
                     pil_image = PIL.Image.open(image_save_path)
                     width, height = pil_image.size
                     image = Image.new(
                         image_id=image_id,
@@ -996,22 +1181,14 @@
                     annotation = Annotation.classification(
                         annotation_id=image_id,
                         image_id=image.image_id,
                         category_id=data["label"] + 1,
                     )
                     ds.add_annotations([annotation])
 
-                categories = dataset.features["label"].names
-                for category_id, category_name in enumerate(categories):
-                    category = Category.classification(
-                        category_id=category_id + 1,
-                        supercategory="object",
-                        name=category_name,
-                    )
-                    ds.add_categories([category])
             else:
                 raise ValueError("task should be one of ['classification', 'object_detection']")
 
         if is_splited:
             start_num = 1
             for set_type, set in dataset.items():
                 image_ids = list(range(start_num, set.num_rows + start_num))
@@ -1036,24 +1213,28 @@
             name (str): Dataset name.
             task (str): Task name.
             root_dir (str, optional): Dataset root directory. Defaults to None.
 
         Returns:
             Dataset: Dataset Class
         """
-        if task not in [
-            TaskType.CLASSIFICATION,
-            TaskType.OBJECT_DETECTION,
-            TaskType.INSTANCE_SEGMENTATION,
-        ]:
-            raise NotImplementedError(f"not supported task: {task}")
 
+        temp_dir = Path(mkdtemp())
         try:
-            url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist.zip"
-            temp_dir = Path(mkdtemp())
+            if task in [
+                TaskType.CLASSIFICATION,
+                TaskType.OBJECT_DETECTION,
+                TaskType.INSTANCE_SEGMENTATION,
+            ]:
+                url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist.zip"
+            elif task == TaskType.TEXT_RECOGNITION:
+                url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/ocr_sample.zip"
+            else:
+                raise NotImplementedError(f"not supported task: {task}")
+
             network.get_file_from_url(url, temp_dir / "mnist.zip")
             io.unzip(temp_dir / "mnist.zip", temp_dir)
 
             ds = Dataset.from_coco(
                 name=name,
                 root_dir=root_dir,
                 task=task,
@@ -1236,14 +1417,18 @@
     def add_annotations(self, annotations: list[Annotation]):
         """Add "Annotation"s to dataset.
 
         Args:
             annotations (list[Annotation]): list of "Annotation"s
         """
         for item in annotations:
+            if self.task == TaskType.TEXT_RECOGNITION:
+                for char in item.caption:
+                    if char not in self.category_names:
+                        raise ValueError(f"Category '{char}' is not in dataset")
             item_path = self.annotation_dir / f"{item.image_id}" / f"{item.annotation_id}.json"
             io.save_json(item.to_dict(), item_path, create_directory=True)
 
     def add_predictions(self, predictions: list[Annotation]):
         """Add "Annotation"s to dataset.
 
         Args:
@@ -1397,23 +1582,24 @@
         """
 
         self.check_trainable()
 
         if data_type in [DataType.YOLO, DataType.ULTRALYTICS]:
             export_dir: Path = self.export_dir / str(DataType.YOLO)
             export_function = export_yolo
-        elif data_type in [
-            DataType.COCO,
-            DataType.AUTOCARE_DLT,
-        ]:
+        elif data_type in [DataType.COCO]:
             export_dir: Path = self.export_dir / str(DataType.COCO)
             export_function = export_coco
-        elif data_type in [DataType.HUGGINGFACE, DataType.TRANSFORMERS]:
-            export_dir: Path = self.export_dir / str(DataType.HUGGINGFACE)
-            export_function = export_huggingface
+        elif data_type in [DataType.AUTOCARE_DLT]:
+            export_dir: Path = self.export_dir / str(DataType.AUTOCARE_DLT)
+            export_function = export_autocare_dlt
+        elif data_type in [DataType.TRANSFORMERS]:
+            export_dir: Path = self.export_dir / str(DataType.TRANSFORMERS)
+            export_function = export_transformers
+
         else:
             raise ValueError(f"Invalid data_type: {data_type}")
 
         try:
             if export_dir.exists():
                 io.remove_directory(export_dir)
                 warnings.warn(f"{export_dir} already exists. Removing exist export and override.")
```

### Comparing `waffle_hub-0.2.2/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.3/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.3/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py` & `waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """
 Tx Model Hub
 See BaseHub documentation for more details about usage.
 """
 
-from waffle_hub import get_installed_backend_version
-
-BACKEND_NAME = "autocare_dlt"
-BACKEND_VERSION = get_installed_backend_version(BACKEND_NAME)
-
 import warnings
 from pathlib import Path
 from typing import Union
 
+import autocare_dlt
 import tbparse
 import torch
 from autocare_dlt.core.model import build_model
 from autocare_dlt.tools import train
 from box import Box
 from torchvision import transforms as T
 from waffle_utils.file import io
@@ -31,45 +27,48 @@
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
 from .config import DATA_TYPE_MAP, DEFAULT_PARAMAS, MODEL_TYPES, WEIGHT_PATH
 
 
 class AutocareDLTHub(BaseHub):
+    BACKEND_NAME = "autocare_dlt"
     MODEL_TYPES = MODEL_TYPES
+    MULTI_GPU_TRAIN = False
+    DEFAULT_PARAMAS = DEFAULT_PARAMAS
+
     DATA_TYPE_MAP = DATA_TYPE_MAP
     WEIGHT_PATH = WEIGHT_PATH
-    DEFAULT_PARAMAS = DEFAULT_PARAMAS
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
         backend: str = None,
         version: str = None,
     ):
-        """Create Tx Model Hub Class. Do not use this class directly. Use AutocareDLTHub.new() instead."""
-
-        if backend is not None and backend != BACKEND_NAME:
-            raise ValueError(f"you've loaded {backend}. backend must be {BACKEND_NAME}")
+        if backend is not None and AutocareDLTHub.BACKEND_NAME != backend:
+            raise ValueError(
+                f"Backend {backend} is not supported. Please use {AutocareDLTHub.BACKEND_NAME}"
+            )
 
-        if version is not None and version != BACKEND_VERSION:
+        if version is not None and autocare_dlt.__version__ != version:
             warnings.warn(
-                f"you've loaded a {BACKEND_NAME}=={version} version while {BACKEND_NAME}=={BACKEND_VERSION} version is installed."
-                "It will cause unexpected results."
+                f"You've loaded the Hub created with autocare_dlt=={version}, \n"
+                + f"but the installed version is {autocare_dlt.__version__}."
             )
 
         super().__init__(
             name=name,
-            backend=BACKEND_NAME,
-            version=BACKEND_VERSION,
+            backend=AutocareDLTHub.BACKEND_NAME,
+            version=autocare_dlt.__version__,
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
@@ -131,14 +130,23 @@
 
         elif self.task == TaskType.CLASSIFICATION:
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
+        elif self.task == TaskType.TEXT_RECOGNITION:
+            normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
+
+            def preprocess(x, *args, **kwargs):
+                return normalize(x)
+
+        else:
+            raise NotImplementedError(f"task {self.task} is not supported yet")
+
         return preprocess
 
     def get_postprocess(self, *args, **kwargs):
 
         if self.task == TaskType.OBJECT_DETECTION:
 
             def inner(x: torch.Tensor, *args, **kwargs):
@@ -150,14 +158,23 @@
 
         elif self.task == TaskType.CLASSIFICATION:
 
             def inner(x: torch.Tensor, *args, **kwargs):
                 x = [t.squeeze() for t in x]
                 return x
 
+        elif self.task == TaskType.TEXT_RECOGNITION:
+
+            def inner(x: torch.Tensor, *args, **kwargs):
+                scores, character_class_ids = x.max(dim=-1)
+                return character_class_ids, scores
+
+        else:
+            raise NotImplementedError(f"task {self.task} is not supported yet")
+
         return inner
 
     def get_metrics(self) -> list[dict]:
         """Get metrics from tensorboard log directory.
         Args:
             tbdir (Union[str, Path]): tensorboard log directory
         Returns:
@@ -196,14 +213,16 @@
             str(cfg.dataset_path / "train.json"),
             str(cfg.dataset_path / "images"),
             str(cfg.dataset_path / "val.json"),
             str(cfg.dataset_path / "images"),
             str(cfg.dataset_path / "test.json"),
             str(cfg.dataset_path / "images"),
         )
+        if self.model_type == "LicencePlateRecognition":
+            data_config["data"]["mode"] = "lpr"
 
         cfg.data_config = self.artifact_dir / "data.json"
         io.save_json(data_config, cfg.data_config, create_directory=True)
         categories = (
             self.categories
             if self._BaseHub__task == "classification"
             else [x["name"] for x in self.categories]
@@ -273,15 +292,18 @@
         preprocess = self.get_preprocess()
         postprocess = self.get_postprocess()
 
         # get model
         categories = [x["name"] for x in self.categories]
         cfg = io.load_json(self.artifact_dir / "model.json")
         cfg["ckpt"] = str(self.best_ckpt_file)
-        cfg["model"]["head"]["num_classes"] = len(categories)
+        if self.task == TaskType.TEXT_RECOGNITION:
+            cfg["model"]["Prediction"]["num_classes"] = len(categories) + 1
+        else:
+            cfg["model"]["head"]["num_classes"] = len(categories)
         cfg["num_classes"] = len(categories)
         model, categories = build_model(Box(cfg), strict=True)
 
         model = ModelWrapper(
             model=model.eval(),
             preprocess=preprocess,
             postprocess=postprocess,
```

### Comparing `waffle_hub-0.2.2/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py` & `waffle_hub-0.2.3/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/config.py` & `waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py` & `waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/transformers_hub.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 """
-Hugging Face Hub
+Transformers Hub
 See BaseHub documentation for more details about usage.
 """
 
-from waffle_hub import get_installed_backend_version
-
-BACKEND_NAME = "transformers"
-BACKEND_VERSION = get_installed_backend_version(BACKEND_NAME)
-
 import os
 import warnings
 from copy import deepcopy
 from functools import cached_property
 from pathlib import Path
 from typing import Callable, Union
 
 import torch
+import transformers
 from torchvision import transforms as T
 from transformers import (
     AutoImageProcessor,
     AutoModelForImageClassification,
     AutoModelForObjectDetection,
     Trainer,
     TrainerCallback,
     TrainingArguments,
 )
 from transformers.utils import ModelOutput
 from waffle_utils.file import io
 
 from datasets import load_from_disk
-
 from waffle_hub import TaskType
-from waffle_hub.hub.adapter.hugging_face.train_input_helper import (
+from waffle_hub.hub.adapter.transformers.train_input_helper import (
     ClassifierInputHelper,
     ObjectDetectionInputHelper,
 )
 from waffle_hub.hub.base_hub import BaseHub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
@@ -58,66 +53,67 @@
             self._trainer.evaluate(
                 eval_dataset=self._trainer.train_dataset,
                 metric_key_prefix="train",
             )
             return control_copy
 
 
-class HuggingFaceHub(BaseHub):
+class TransformersHub(BaseHub):
+    BACKEND_NAME = "transformers"
+    MODEL_TYPES = MODEL_TYPES
+    MULTI_GPU_TRAIN = False
+    DEFAULT_PARAMAS = DEFAULT_PARAMAS
 
     # Override
     LAST_CKPT_FILE = "weights/last_ckpt"
     BEST_CKPT_FILE = "weights/best_ckpt"
 
-    # Common
-    MODEL_TYPES = MODEL_TYPES
-    DEFAULT_PARAMAS = DEFAULT_PARAMAS
-
     def __init__(
         self,
         name: str,
         task: str,
         model_type: str,
         model_size: str,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
         backend: str = None,
         version: str = None,
     ):
+        if backend is not None and TransformersHub.BACKEND_NAME != backend:
+            raise ValueError(
+                f"Backend {backend} is not supported. Please use {TransformersHub.BACKEND_NAME}"
+            )
 
-        if backend is not None and backend != BACKEND_NAME:
-            raise ValueError(f"you've loaded {backend}. backend must be {BACKEND_NAME}")
-
-        if version is not None and version != BACKEND_VERSION:
+        if version is not None and transformers.__version__ != version:
             warnings.warn(
-                f"you've loaded a {BACKEND_NAME}=={version} version while {BACKEND_NAME}=={BACKEND_VERSION} version is installed."
-                "It will cause unexpected results."
+                f"You've loaded the Hub created with transformers=={version}, \n"
+                + f"but the installed version is {transformers.__version__}."
             )
 
         super().__init__(
             name=name,
-            backend=BACKEND_NAME,
-            version=BACKEND_VERSION,
+            backend=TransformersHub.BACKEND_NAME,
+            version=transformers.__version__,
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
     # Override
     @cached_property
     def best_ckpt_file(self) -> Path:
         """Best Checkpoint File"""
-        return self.hub_dir / HuggingFaceHub.BEST_CKPT_FILE
+        return self.hub_dir / TransformersHub.BEST_CKPT_FILE
 
     @cached_property
     def last_ckpt_file(self) -> Path:
         """Last Checkpoint File"""
-        return self.hub_dir / HuggingFaceHub.LAST_CKPT_FILE
+        return self.hub_dir / TransformersHub.LAST_CKPT_FILE
 
     @classmethod
     def new(
         cls,
         name: str,
         task: str = None,
         model_type: str = None,
```

### Comparing `waffle_hub-0.2.2/waffle_hub/hub/adapter/hugging_face/train_input_helper.py` & `waffle_hub-0.2.3/waffle_hub/hub/adapter/transformers/train_input_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     collator: Callable = None
     model: _BaseAutoModelClass = None
     compute_metrics: Callable = None
 
 
 class TrainInputHelper(ABC):
     """
-    This class is designed to assist with passing arguments to the Hugging Face's Trainer function.
+    This class is designed to assist with passing arguments to the Transformers's Trainer function.
     """
 
     def __init__(self, pretrained_model: str, image_size: Union[int, list[int]]) -> None:
         self.pretrained_model = pretrained_model
         self.image_size = image_size
 
         if isinstance(image_size, int):
```

### Comparing `waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/config.py` & `waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.3/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 """
 Ultralytics Hub
 See BaseHub documentation for more details about usage.
 """
 
-from waffle_hub import get_installed_backend_version
-
-BACKEND_NAME = "ultralytics"
-BACKEND_VERSION = get_installed_backend_version(BACKEND_NAME)
-
 import warnings
 from pathlib import Path
 from typing import Union
 
 import torch
+import ultralytics
 from torchvision import transforms as T
 from ultralytics import YOLO
 from waffle_utils.file import io
 
 from waffle_hub import TaskType
 from waffle_hub.hub.base_hub import BaseHub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
+from waffle_hub.utils.process import run_python_file
 
 from .config import DEFAULT_PARAMAS, MODEL_TYPES, TASK_MAP, TASK_SUFFIX
 
 
 class UltralyticsHub(BaseHub):
+    BACKEND_NAME = "ultralytics"
     MODEL_TYPES = MODEL_TYPES
+    MULTI_GPU_TRAIN = True
+    DEFAULT_PARAMAS = DEFAULT_PARAMAS
+
     TASK_MAP = TASK_MAP
     TASK_SUFFIX = TASK_SUFFIX
-    DEFAULT_PARAMAS = DEFAULT_PARAMAS
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
         backend: str = None,
         version: str = None,
     ):
-        """Create Ultralytics Hub Class. Do not use this class directly. Use UltralyticsHub.new() instead."""
-
-        if backend is not None and backend != BACKEND_NAME:
-            raise ValueError(f"you've loaded {backend}. backend must be {BACKEND_NAME}")
+        if backend is not None and UltralyticsHub.BACKEND_NAME != backend:
+            raise ValueError(
+                f"Backend {backend} is not supported. Please use {UltralyticsHub.BACKEND_NAME}"
+            )
 
-        if version is not None and version != BACKEND_VERSION:
+        if version is not None and ultralytics.__version__ != version:
             warnings.warn(
-                f"you've loaded a {BACKEND_NAME}=={version} version while {BACKEND_NAME}=={BACKEND_VERSION} version is installed."
-                "It will cause unexpected results."
+                f"You've loaded the Hub created with ultralytics=={version}, \n"
+                + f"but the installed version is {ultralytics.__version__}."
             )
 
         super().__init__(
             name=name,
-            backend=BACKEND_NAME,
-            version=BACKEND_VERSION,
+            backend=UltralyticsHub.BACKEND_NAME,
+            version=ultralytics.__version__,
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
@@ -258,31 +258,38 @@
             cfg.pretrained_model
             if cfg.pretrained_model
             else self.model_type + self.model_size + self.TASK_SUFFIX[self.backend_task_name] + ".pt"
         )
 
     def training(self, cfg: TrainConfig, callback: TrainCallback):
 
-        model = YOLO(cfg.pretrained_model, task=self.backend_task_name)
+        code = f"""if __name__ == "__main__":
+        from ultralytics import YOLO
+        model = YOLO("{cfg.pretrained_model}", task="{self.backend_task_name}")
         model.train(
-            data=cfg.dataset_path,
-            epochs=cfg.epochs,
-            batch=cfg.batch_size,
-            imgsz=cfg.image_size,
-            lr0=cfg.learning_rate,
-            lrf=cfg.learning_rate,
-            rect=cfg.letter_box,
-            device=cfg.device,
-            workers=cfg.workers,
-            seed=cfg.seed,
-            verbose=cfg.verbose,
-            project=self.hub_dir,
-            name=self.ARTIFACT_DIR,
-        )
-        del model
+            data="{cfg.dataset_path}",
+            epochs={cfg.epochs},
+            batch={cfg.batch_size},
+            imgsz={cfg.image_size},
+            lr0={cfg.learning_rate},
+            lrf={cfg.learning_rate},
+            rect={cfg.letter_box},
+            device="{cfg.device}",
+            workers={cfg.workers},
+            seed={cfg.seed},
+            verbose={cfg.verbose},
+            project="{self.hub_dir}",
+            name="{self.ARTIFACT_DIR}",
+        )"""
+
+        script_file = str((self.hub_dir / "train.py").absolute())
+        with open(script_file, "w") as f:
+            f.write(code)
+
+        run_python_file(script_file)
 
     def on_train_end(self, cfg: TrainConfig):
         io.copy_file(
             self.artifact_dir / "weights" / "best.pt",
             self.best_ckpt_file,
             create_directory=True,
         )
@@ -324,8 +331,8 @@
         # wrap model
         model = ModelWrapper(
             model=model,
             preprocess=preprocess,
             postprocess=postprocess,
         )
 
-        return model
+        return model
```

### Comparing `waffle_hub-0.2.2/waffle_hub/hub/base_hub.py` & `waffle_hub-0.2.3/waffle_hub/hub/base_hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Hub is a multi-backend compatible interface for model training, evaluation, inference, and export.
 
 .. note::
     Check out docstrings for more details.
 
 """
 import logging
+import os
 import threading
 import time
 import warnings
 from functools import cached_property
 from pathlib import Path
 from typing import Union
 
@@ -50,16 +51,19 @@
 from waffle_hub.utils.draw import draw_results
 from waffle_hub.utils.evaluate import evaluate_function
 
 logger = logging.getLogger(__name__)
 
 
 class BaseHub:
-
-    MODEL_TYPES = {}
+    # Hub Spec. must have
+    BACKEND_NAME = None
+    MODEL_TYPES = None
+    MULTI_GPU_TRAIN = None
+    DEFAULT_PARAMAS = None
 
     # directory settings
     DEFAULT_ROOT_DIR = Path("./hubs")
 
     ARTIFACT_DIR = Path("artifacts")
 
     INFERENCE_DIR = Path("inferences")
@@ -93,14 +97,26 @@
         version: str = None,
         task: Union[str, TaskType] = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
     ):
+        if self.BACKEND_NAME is None:
+            raise AttributeError("BACKEND_NAME must be specified.")
+
+        if self.MODEL_TYPES is None:
+            raise AttributeError("MODEL_TYPES must be specified.")
+
+        if self.MULTI_GPU_TRAIN is None:
+            raise AttributeError("MULTI_GPU_TRAIN must be specified.")
+
+        if self.DEFAULT_PARAMAS is None:
+            raise AttributeError("DEFAULT_PARAMAS must be specified.")
+
         self.name: str = name
         self.task: str = task
         self.model_type: str = model_type
         self.model_size: str = model_size
         self.categories: list[dict] = categories
         self.root_dir: Path = Path(root_dir) if root_dir else None
 
@@ -124,14 +140,43 @@
                 categories=self.categories,
             )
             model_config.save_yaml(self.model_config_file)
         except Exception as e:
             raise e
 
     @classmethod
+    def new(
+        cls,
+        name: str,
+        task: str = None,
+        model_type: str = None,
+        model_size: str = None,
+        categories: Union[list[dict], list] = None,
+        root_dir: str = None,
+    ):
+        """Create Hub.
+
+        Args:
+            name (str): Hub name
+            task (str, optional): Task Name. See Hub.TASKS. Defaults to None.
+            model_type (str, optional): Model Type. See Hub.MODEL_TYPES. Defaults to None.
+            model_size (str, optional): Model Size. See Hub.MODEL_SIZES. Defaults to None.
+            categories (Union[list[dict], list]): class dictionary or list. [{"supercategory": "name"}, ] or ["name",].
+            root_dir (str, optional): Root directory of hub repository. Defaults to None.
+        """
+        return cls(
+            name=name,
+            task=task,
+            model_type=model_type,
+            model_size=model_size,
+            categories=categories,
+            root_dir=root_dir,
+        )
+
+    @classmethod
     def load(cls, name: str, root_dir: str = None) -> "BaseHub":
         """Load Hub by name.
 
         Args:
             name (str): hub name.
             root_dir (str, optional): hub root directory. Defaults to None.
 
@@ -468,15 +513,57 @@
             image, image_info = transform(x)
             return image, image_info
 
         return inner
 
     # Train Hook
     def before_train(self, cfg: TrainConfig):
-        pass
+        # check device
+        device = cfg.device
+        if device == "cpu":
+            logger.info("CPU training")
+        elif device.isdigit():
+            if not torch.cuda.is_available():
+                raise ValueError("CUDA is not available.")
+            # if (
+            #     int(device) >= torch.cuda.device_count()  # TODO: torch.cuda.device_count() occurs unexpected errors
+            # ):
+            #     raise IndexError(
+            #         f"GPU[{device}] index is out of range. device id should be smaller than {torch.cuda.device_count()}\n"
+            #     )
+            logger.info(f"Single GPU training: {device}")
+        elif "," in device:
+            if not torch.cuda.is_available():
+                raise ValueError("CUDA is not available.")
+            if not self.MULTI_GPU_TRAIN:
+                raise ValueError(f"{self.backend} does not support MULTI_GPU_TRAIN.")
+            # if len(device.split(",")) > torch.cuda.device_count():  # TODO: torch.cuda.device_count() occurs unexpected errors
+            #     raise ValueError(
+            #         f"GPU number is not enough. {device}\n"
+            #         + f"Given device: {device}\n"
+            #         + f"Available device count: {torch.cuda.device_count()}"
+            #     )
+            # if not all([int(x) < torch.cuda.device_count() for x in device.split(",")]):
+            #     raise IndexError(
+            #         f"GPU index is out of range. device id should be smaller than {torch.cuda.device_count()}\n"
+            #     )
+            logger.info(f"Multi GPU training: {device}")
+        else:
+            raise ValueError(f"Invalid device: {device}\n" + "Please use 'cpu', '0', '0,1,2,3'")
+
+        # check if it is already trained
+        rank = os.getenv("RANK", -1)
+        if self.artifact_dir.exists() and rank in [
+            -1,
+            0,
+        ]:  # TODO: need to ensure that training is not already running
+            raise FileExistsError(
+                f"{self.artifact_dir}\n"
+                "Train artifacts already exist. Remove artifact to re-train (hub.delete_artifact())."
+            )
 
     def on_train_start(self, cfg: TrainConfig):
         pass
 
     def save_train_config(self, cfg: TrainConfig):
         cfg.save_yaml(self.train_config_file)
 
@@ -512,15 +599,16 @@
             dataset_path (str): dataset path
             epochs (int, optional): number of epochs. None to use default. Defaults to None.
             batch_size (int, optional): batch size. None to use default. Defaults to None.
             image_size (Union[int, list[int]], optional): image size. None to use default. Defaults to None.
             learning_rate (float, optional): learning rate. None to use default. Defaults to None.
             letter_box (bool, optional): letter box. None to use default. Defaults to None.
             pretrained_model (str, optional): pretrained model. None to use default. Defaults to None.
-            device (str, optional): device. "cpu" or "gpu_id". Defaults to "0".
+            device (str, optional):
+                "cpu" or "gpu_id" or comma seperated "gpu_ids". Defaults to "0".
             workers (int, optional): number of workers. Defaults to 2.
             seed (int, optional): random seed. Defaults to 0.
             verbose (bool, optional): verbose. Defaults to True.
             hold (bool, optional): hold process. Defaults to True.
 
         Raises:
             FileExistsError: if trained artifact exists.
@@ -532,33 +620,29 @@
             >>> train_result = hub.train(
                     dataset_path=dataset_path,
                     epochs=100,
                     batch_size=16,
                     image_size=640,
                     learning_rate=0.001,
                     letterbox=False,
-                    device="0",
+                    device="0",  # use gpu 0
+                    # device="0,1,2,3",  # use gpu 0,1,2,3
+                    # device="cpu",  # use cpu
                     workers=2,
                     seed=123
                 )
             >>> train_result.best_ckpt_file
             hubs/my_hub/weights/best_ckpt.pt
             >>> train_result.metrics
             [[{"tag": "epoch", "value": 1}, {"tag": "train/loss", "value": 0.1}, ...], ...]
 
         Returns:
             TrainResult: train result
         """
 
-        if self.artifact_dir.exists():
-            raise FileExistsError(
-                f"{self.artifact_dir}\n"
-                "Train artifacts already exist. Remove artifact to re-train (hub.delete_artifact())."
-            )
-
         def inner(callback: TrainCallback, result: TrainResult):
             try:
                 self.before_train(cfg)
                 self.on_train_start(cfg)
                 self.save_train_config(cfg)
                 self.training(cfg, callback)
                 self.on_train_end(cfg)
@@ -630,15 +714,15 @@
         dataloader = LabeledDataset(
             dataset,
             cfg.image_size,
             letter_box=cfg.letter_box,
             set_name=cfg.set_name,
         ).get_dataloader(cfg.batch_size, cfg.workers)
 
-        result_parser = get_parser(self.task)(**cfg.to_dict())
+        result_parser = get_parser(self.task)(**cfg.to_dict(), categories=self.categories)
 
         callback._total_steps = len(dataloader) + 1
 
         preds = []
         labels = []
         for i, (images, image_infos, annotations) in tqdm.tqdm(
             enumerate(dataloader, start=1), total=len(dataloader)
@@ -789,15 +873,15 @@
         device = cfg.device
 
         model = self.get_model().to(device)
         dataloader = ImageDataset(
             cfg.source, cfg.image_size, letter_box=cfg.letter_box
         ).get_dataloader(cfg.batch_size, cfg.workers)
 
-        result_parser = get_parser(self.task)(**cfg.to_dict())
+        result_parser = get_parser(self.task)(**cfg.to_dict(), categories=self.categories)
 
         results = []
         callback._total_steps = len(dataloader) + 1
         for i, (images, image_infos) in tqdm.tqdm(
             enumerate(dataloader, start=1), total=len(dataloader)
         ):
             result_batch = model(images.to(device))
@@ -959,14 +1043,16 @@
         input_name = ["inputs"]
         if self.task == "object_detection":
             output_names = ["bbox", "conf", "class_id"]
         elif self.task == "classification":
             output_names = ["predictions"]
         elif self.task == "instance_segmentation":
             output_names = ["bbox", "conf", "class_id", "masks"]
+        elif self.task == "text_recognition":
+            output_names = ["class_ids", "confs"]
         else:
             raise NotImplementedError(f"{self.task} does not support export yet.")
 
         dummy_input = torch.randn(
             cfg.batch_size, 3, *image_size, dtype=torch.float16 if cfg.half else torch.float32
         )
         dummy_input = dummy_input.to(cfg.device)
```

### Comparing `waffle_hub-0.2.2/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.2.3/waffle_hub/hub/model/wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,21 +186,52 @@
                         segmentation=segment,
                     )
                 )
             parseds.append(parsed)
         return parseds
 
 
+class TextRecognitionResultParser(ResultParser):
+    def __init__(self, categories, *args, **kwargs):
+        self.categories = categories
+        self.category_names = [""] + [d["name"] for d in self.categories]
+
+    def __call__(
+        self, results: list[torch.Tensor], image_infos: list[ImageInfo] = None, *args, **kwargs
+    ) -> list[Annotation]:
+        parseds = []
+
+        pred_batch, conf_batch = results
+        for preds, confs in zip(pred_batch, conf_batch):
+            mask = preds > 0
+            preds, confs = preds[mask], confs[mask]
+
+            text = "".join([self.category_names[pred] for pred in preds])
+
+            parsed = []
+            parsed.append(
+                Annotation.text_recognition(
+                    score=list(map(float, confs)),
+                    caption=text,
+                )
+            )
+            parseds.append(parsed)
+
+        return parseds
+
+
 def get_parser(task: str):
     if task == "classification":
         return ClassificationResultParser
     elif task == "object_detection":
         return ObjectDetectionResultParser
     elif task == "instance_segmentation":
         return InstanceSegmentationResultParser
+    elif task == "text_recognition":
+        return TextRecognitionResultParser
 
 
 class ModelWrapper(torch.nn.Module):
     def __init__(
         self,
         model: torch.nn.Module,
         preprocess: PreprocessFunction,
```

### Comparing `waffle_hub-0.2.2/waffle_hub/run.py` & `waffle_hub-0.2.3/waffle_hub/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import List
 
 import typer
 from rich import print
 
 from waffle_hub.dataset.dataset import Dataset
 from waffle_hub.hub.adapter.autocare_dlt import AutocareDLTHub
-from waffle_hub.hub.adapter.hugging_face import HuggingFaceHub
+from waffle_hub.hub.adapter.transformers import TransformersHub
 from waffle_hub.hub.adapter.ultralytics import UltralyticsHub
 
 dataset = typer.Typer(name="dataset")
 hub = typer.Typer(name="hub")
 app = typer.Typer()
 app.add_typer(dataset)
 app.add_typer(hub)
 
 BACKEND_MAP = {
     "ultralytics": UltralyticsHub,
-    "huggingface": HuggingFaceHub,
+    "transformers": TransformersHub,
     "autocare_dlt": AutocareDLTHub,
 }
 
 EXPORT_MAP = {
     "ultralytics": "YOLO",
-    "huggingface": "HUGGINGFACE",
+    "transformers": "TRANSFORMERS",
     "autocare_dlt": "AutocareDLT",
 }
 
 
 @hub.command(name="new")
 def _new_hub(
     backend: str = typer.Option(..., help="Backend to use"),
@@ -267,22 +267,22 @@
         name=name,
         root_dir=root_dir,
         yaml_path=yaml_path,
         task=task,
     )
 
 
-@dataset.command(name="from_huggingface")
-def _from_huggingface_dataset(
+@dataset.command(name="from_transformers")
+def _from_transformers_dataset(
     name: str = typer.Option(..., help="Name of the dataset"),
     root_dir: str = typer.Option(..., help="Root directory"),
     task: str = typer.Option(..., help="Task"),
     dataset_dir: str = typer.Option(..., help="Dataset directory"),
 ):
-    Dataset.from_huggingface(
+    Dataset.from_transformers(
         name=name,
         root_dir=root_dir,
         task=task,
         dataset_dir=dataset_dir,
     )
```

### Comparing `waffle_hub-0.2.2/waffle_hub/schema/base_schema.py` & `waffle_hub-0.2.3/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/schema/configs.py` & `waffle_hub-0.2.3/waffle_hub/schema/configs.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/schema/data.py` & `waffle_hub-0.2.3/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.3/waffle_hub/schema/fields/annotation.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.3/waffle_hub/schema/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.3/waffle_hub/schema/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.3/waffle_hub/schema/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/utils/callback.py` & `waffle_hub-0.2.3/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/utils/conversion.py` & `waffle_hub-0.2.3/waffle_hub/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/utils/data.py` & `waffle_hub-0.2.3/waffle_hub/utils/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.2/waffle_hub/utils/draw.py` & `waffle_hub-0.2.3/waffle_hub/utils/draw.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+import logging
+from pathlib import Path
 from typing import Union
 
 import cv2
 import numpy as np
+from PIL import Image, ImageDraw, ImageFont
+from waffle_utils.file.network import get_file_from_url
 
 from waffle_hub import TaskType
 from waffle_hub.schema.fields import Annotation
 
 FONT_FACE = cv2.FONT_HERSHEY_DUPLEX
 FONT_SCALE = 1.0
 FONT_WEIGHT = 2
-
 THICKNESS = 2
+FONT_URL = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/fonts/gulim.ttc"
+FONT_NAME = "gulim.ttc"
+
 
 # random colors with 1000 categories
 colors = np.random.randint(0, 255, (1000, 3), dtype="uint8").tolist()
 
 
 def draw_classification(
     image: np.ndarray,
@@ -92,40 +98,70 @@
         )
     mask = alpha > 0
     image[mask] = cv2.addWeighted(alpha, 0.3, image, 0.7, 0)[mask]
 
     return image
 
 
+def draw_text_recognition(
+    image: np.ndarray,
+    annotation: Annotation,
+    loc_x: int = 0,
+    loc_y: int = 10,
+):
+    # download font
+    try:
+        global FONT_NAME
+        if not Path(FONT_NAME).exists():
+            get_file_from_url(FONT_URL, FONT_NAME, True)
+        font = ImageFont.truetype(FONT_NAME, int(FONT_SCALE) * 25)
+    except:
+        font = ImageFont.load_default()
+        logging.warning("Don't load font file, Using default font.")
+
+    img_pil = Image.fromarray(image)
+    draw = ImageDraw.Draw(img_pil)
+    draw.text(
+        (loc_x, loc_y),
+        annotation.caption,
+        font=font,
+        fill=tuple(colors[0]),
+        stroke_width=FONT_WEIGHT,
+    )
+
+    image = np.array(img_pil)
+
+    return image
+
+
 def draw_results(
     image: Union[np.ndarray, str],
     results: list[Annotation],
     names: list[str],
 ):
 
     if isinstance(image, str):
         image = cv2.imread(image)
 
-    classification_results = [result for result in results if result.task == TaskType.CLASSIFICATION]
-    object_detection_results = [
-        result for result in results if result.task == TaskType.OBJECT_DETECTION
-    ]
-    instance_segmentation_results = [
-        result for result in results if result.task == TaskType.INSTANCE_SEGMENTATION
-    ]
+    task_results = {task: [] for task in TaskType}
+    for result in results:
+        task_results[result.task.upper()].append(result)
 
-    for i, result in enumerate(classification_results, start=1):
+    for i, result in enumerate(task_results[TaskType.CLASSIFICATION], start=1):
         image = draw_classification(
             image,
             result,
             names=names,
             loc_x=10,
             loc_y=30 * i,
         )
 
-    for i, result in enumerate(object_detection_results, start=1):
+    for i, result in enumerate(task_results[TaskType.OBJECT_DETECTION], start=1):
         image = draw_object_detection(image, result, names=names)
 
-    for i, result in enumerate(instance_segmentation_results, start=1):
+    for i, result in enumerate(task_results[TaskType.INSTANCE_SEGMENTATION], start=1):
         image = draw_instance_segmentation(image, result, names=names)
 
+    for i, result in enumerate(task_results[TaskType.TEXT_RECOGNITION], start=1):
+        image = draw_text_recognition(image, result, loc_x=10, loc_y=10)
+
     return image
```

### Comparing `waffle_hub-0.2.2/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.3/waffle_hub/utils/evaluate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+from functools import reduce
+from operator import eq
 from typing import Union
 
 import torch
 from torchmetrics.classification import Accuracy
 from torchmetrics.detection import mean_ap
+from torchmetrics.text import CharErrorRate
 
 from waffle_hub import TaskType
 from waffle_hub.schema.evaluate import (
     ClassificationMetric,
     InstanceSegmentationMetric,
     ObjectDetectionMetric,
+    TextRecognitionMetric,
 )
 from waffle_hub.schema.fields import Annotation
 
 
 def convert_to_torchmetric_format(total: list[Annotation], task: TaskType, prediction: bool = False):
 
     datas = []
@@ -49,21 +53,26 @@
                 data["boxes"].append(annotation.bbox)
                 data["labels"].append(annotation.category_id - 1)
                 if prediction:
                     data["scores"].append(annotation.score)
 
             datas.append(data)
 
+        elif task == TaskType.TEXT_RECOGNITION:
+            datas.append(annotations[0].caption)
+
         else:
             raise NotImplementedError
 
     if isinstance(datas[0], dict):
         datas = [{k: torch.tensor(v) for k, v in data.items()} for data in datas]
     elif isinstance(datas[0], int):
         datas = torch.tensor(datas)
+    elif isinstance(datas[0], str):
+        pass
     else:
         raise NotImplementedError
 
     return datas
 
 
 def evaluate_classification(
@@ -99,26 +108,40 @@
         class_metrics=True,
         num_classes=num_classes,
     )(preds, labels)
 
     return InstanceSegmentationMetric(float(map_dict["map"]))
 
 
+def evalute_text_recognition(
+    preds: list[Annotation], labels: list[Annotation], num_classes: int
+) -> ObjectDetectionMetric:
+
+    correct = reduce(lambda n, pair: n + eq(*pair), zip(preds, labels), 0)
+    acc = correct / len(preds)
+
+    return TextRecognitionMetric(float(acc))
+
+
 def evaluate_function(
     preds: list[Annotation],
     labels: list[Annotation],
     task: str,
     num_classes: int = None,
     *args,
     **kwargs
-) -> Union[ClassificationMetric, ObjectDetectionMetric, InstanceSegmentationMetric]:
+) -> Union[
+    ClassificationMetric, ObjectDetectionMetric, InstanceSegmentationMetric, TextRecognitionMetric
+]:
     preds = convert_to_torchmetric_format(preds, task, prediction=True)
     labels = convert_to_torchmetric_format(labels, task)
 
     if task == TaskType.CLASSIFICATION:
         return evaluate_classification(preds, labels, num_classes, *args, **kwargs)
     elif task == TaskType.OBJECT_DETECTION:
         return evaluate_object_detection(preds, labels, num_classes, *args, **kwargs)
     elif task == TaskType.INSTANCE_SEGMENTATION:
         return evaluate_segmentation(preds, labels, num_classes, *args, **kwargs)
+    elif task == TaskType.TEXT_RECOGNITION:
+        return evalute_text_recognition(preds, labels, num_classes, *args, **kwargs)
     else:
         raise NotImplementedError
```

### Comparing `waffle_hub-0.2.2/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.2.3/waffle_hub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.2.2
+Version: 0.2.3
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.2 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.3 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.2/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.3/waffle_hub.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 tests/test_cli.py
 tests/test_dataset.py
+tests/test_ddp.py
 tests/test_hub.py
 waffle_hub/__init__.py
 waffle_hub/run.py
 waffle_hub.egg-info/PKG-INFO
 waffle_hub.egg-info/SOURCES.txt
 waffle_hub.egg-info/dependency_links.txt
 waffle_hub.egg-info/entry_points.txt
 waffle_hub.egg-info/requires.txt
 waffle_hub.egg-info/top_level.txt
 waffle_hub/dataset/__init__.py
 waffle_hub/dataset/dataset.py
 waffle_hub/dataset/adapter/__init__.py
+waffle_hub/dataset/adapter/autocare_dlt.py
 waffle_hub/dataset/adapter/coco.py
-waffle_hub/dataset/adapter/huggingface.py
+waffle_hub/dataset/adapter/transformers.py
 waffle_hub/dataset/adapter/yolo.py
 waffle_hub/experimental/__init__.py
 waffle_hub/experimental/serve.py
 waffle_hub/experimental/auto_label/__init__.py
 waffle_hub/experimental/auto_label/grounding_dino.py
 waffle_hub/hub/__init__.py
 waffle_hub/hub/base_hub.py
 waffle_hub/hub/adapter/__init__.py
 waffle_hub/hub/adapter/autocare_dlt/__init__.py
 waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
 waffle_hub/hub/adapter/autocare_dlt/config.py
 waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
 waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
 waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
-waffle_hub/hub/adapter/hugging_face/__init__.py
-waffle_hub/hub/adapter/hugging_face/config.py
-waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
-waffle_hub/hub/adapter/hugging_face/train_input_helper.py
+waffle_hub/hub/adapter/transformers/__init__.py
+waffle_hub/hub/adapter/transformers/config.py
+waffle_hub/hub/adapter/transformers/train_input_helper.py
+waffle_hub/hub/adapter/transformers/transformers_hub.py
 waffle_hub/hub/adapter/ultralytics/__init__.py
 waffle_hub/hub/adapter/ultralytics/config.py
 waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
 waffle_hub/hub/model/__init__.py
 waffle_hub/hub/model/wrapper.py
 waffle_hub/schema/__init__.py
 waffle_hub/schema/base_schema.py
@@ -54,8 +56,9 @@
 waffle_hub/schema/fields/category.py
 waffle_hub/schema/fields/image.py
 waffle_hub/utils/__init__.py
 waffle_hub/utils/callback.py
 waffle_hub/utils/conversion.py
 waffle_hub/utils/data.py
 waffle_hub/utils/draw.py
-waffle_hub/utils/evaluate.py
+waffle_hub/utils/evaluate.py
+waffle_hub/utils/process.py
```

