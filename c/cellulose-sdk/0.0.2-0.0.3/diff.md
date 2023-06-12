# Comparing `tmp/cellulose-sdk-0.0.2.tar.gz` & `tmp/cellulose-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellulose-sdk-0.0.2.tar", last modified: Thu Jun  8 00:06:06 2023, max compression
+gzip compressed data, was "cellulose-sdk-0.0.3.tar", last modified: Mon Jun 12 04:12:45 2023, max compression
```

## Comparing `cellulose-sdk-0.0.2.tar` & `cellulose-sdk-0.0.3.tar`

### file list

```diff
@@ -1,70 +1,78 @@
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.444011 cellulose-sdk-0.0.2/
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1066 2023-06-07 06:11:27.000000 cellulose-sdk-0.0.2/LICENSE
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1517 2023-06-08 00:06:06.443906 cellulose-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 tzhenghao   (501) staff       (20)      377 2023-06-07 06:13:41.000000 cellulose-sdk-0.0.2/README.md
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.437448 cellulose-sdk-0.0.2/cellulose/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/__init__.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.437749 cellulose-sdk-0.0.2/cellulose/api/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/api/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     3174 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/api/cellulose_context.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.438215 cellulose-sdk-0.0.2/cellulose/artifact/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/artifact/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      423 2023-06-08 00:02:40.000000 cellulose-sdk-0.0.2/cellulose/artifact/cellulose_artifact.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     6179 2023-06-08 00:03:53.000000 cellulose-sdk-0.0.2/cellulose/artifact/cellulose_artifact_manager.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.438909 cellulose-sdk-0.0.2/cellulose/base/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/base/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     2100 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/base/benchmark.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      102 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/base/checker.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      327 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/base/export.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      101 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/base/loader.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.439712 cellulose-sdk-0.0.2/cellulose/configs/
--rw-r--r--   0 tzhenghao   (501) staff       (20)      984 2023-06-07 05:08:49.000000 cellulose-sdk-0.0.2/cellulose/configs/.cellulose_config.toml
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/configs/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1996 2023-06-07 06:17:16.000000 cellulose-sdk-0.0.2/cellulose/configs/config.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     6885 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/configs/loader.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.439925 cellulose-sdk-0.0.2/cellulose/decorators/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/decorators/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     8400 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/decorators/cellulose.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.440058 cellulose-sdk-0.0.2/cellulose/infra/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/infra/__init__.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.440389 cellulose-sdk-0.0.2/cellulose/metrics/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/metrics/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      430 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/metrics/latency.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)       90 2023-06-07 04:03:32.000000 cellulose-sdk-0.0.2/cellulose/metrics/metrics.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.441308 cellulose-sdk-0.0.2/cellulose/onnx/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/onnx/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1608 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/onnx/benchmark.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      311 2023-06-07 06:23:27.000000 cellulose-sdk-0.0.2/cellulose/onnx/checker.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      499 2023-06-07 06:23:27.000000 cellulose-sdk-0.0.2/cellulose/onnx/loader.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      962 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/onnx/runtime.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.441557 cellulose-sdk-0.0.2/cellulose/output/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/output/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      403 2023-06-07 05:06:52.000000 cellulose-sdk-0.0.2/cellulose/output/output.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.441983 cellulose-sdk-0.0.2/cellulose/pytorch/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/pytorch/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1014 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/pytorch/benchmark.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     4819 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/pytorch/export.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.442113 cellulose-sdk-0.0.2/cellulose/scripts/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/scripts/__init__.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.442201 cellulose-sdk-0.0.2/cellulose/tensorflow/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/tensorflow/__init__.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.442955 cellulose-sdk-0.0.2/cellulose/utils/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/utils/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      895 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/utils/benchmark_results.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      967 2023-06-07 06:17:16.000000 cellulose-sdk-0.0.2/cellulose/utils/csv_utils.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      180 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/utils/devices.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      260 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/utils/engines.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      266 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/utils/numpy.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.443200 cellulose-sdk-0.0.2/cellulose/validation/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/validation/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      667 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/validation/validation.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)       32 2023-06-07 23:47:02.000000 cellulose-sdk-0.0.2/cellulose/version.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.443769 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1517 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/PKG-INFO
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1472 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 tzhenghao   (501) staff       (20)        1 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 tzhenghao   (501) staff       (20)      191 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/requires.txt
--rw-r--r--   0 tzhenghao   (501) staff       (20)       10 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/top_level.txt
--rw-r--r--   0 tzhenghao   (501) staff       (20)      505 2023-06-07 06:23:01.000000 cellulose-sdk-0.0.2/pyproject.toml
--rw-r--r--   0 tzhenghao   (501) staff       (20)       38 2023-06-08 00:06:06.444040 cellulose-sdk-0.0.2/setup.cfg
--rw-r--r--   0 tzhenghao   (501) staff       (20)     8573 2023-06-08 00:03:51.000000 cellulose-sdk-0.0.2/setup.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.799878 cellulose-sdk-0.0.3/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1066 2023-06-07 06:11:27.000000 cellulose-sdk-0.0.3/LICENSE
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1517 2023-06-12 04:12:45.799764 cellulose-sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      377 2023-06-07 06:13:41.000000 cellulose-sdk-0.0.3/README.md
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.791436 cellulose-sdk-0.0.3/cellulose/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.791622 cellulose-sdk-0.0.3/cellulose/api/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/api/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     4046 2023-06-11 00:08:12.000000 cellulose-sdk-0.0.3/cellulose/api/cellulose_context.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.792159 cellulose-sdk-0.0.3/cellulose/artifact/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/artifact/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      423 2023-06-08 00:02:40.000000 cellulose-sdk-0.0.3/cellulose/artifact/cellulose_artifact.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     6166 2023-06-10 23:43:16.000000 cellulose-sdk-0.0.3/cellulose/artifact/cellulose_artifact_manager.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.793140 cellulose-sdk-0.0.3/cellulose/base/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/base/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     2100 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.3/cellulose/base/benchmark.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      102 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/base/checker.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      327 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.3/cellulose/base/export.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      101 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/base/loader.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.793895 cellulose-sdk-0.0.3/cellulose/configs/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      984 2023-06-07 05:08:49.000000 cellulose-sdk-0.0.3/cellulose/configs/.cellulose_config.toml
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/configs/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1996 2023-06-07 06:17:16.000000 cellulose-sdk-0.0.3/cellulose/configs/config.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     6885 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.3/cellulose/configs/loader.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.794239 cellulose-sdk-0.0.3/cellulose/dashboard/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:59:37.000000 cellulose-sdk-0.0.3/cellulose/dashboard/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.794322 cellulose-sdk-0.0.3/cellulose/dashboard/api_resources/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-06-08 01:06:23.000000 cellulose-sdk-0.0.3/cellulose/dashboard/api_resources/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.794508 cellulose-sdk-0.0.3/cellulose/dashboard/api_resources/models/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-06-08 01:07:21.000000 cellulose-sdk-0.0.3/cellulose/dashboard/api_resources/models/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1142 2023-06-12 04:10:49.000000 cellulose-sdk-0.0.3/cellulose/dashboard/api_resources/models/onnx.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-06-08 01:05:40.000000 cellulose-sdk-0.0.3/cellulose/dashboard/credentials.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.794806 cellulose-sdk-0.0.3/cellulose/decorators/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/decorators/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     8400 2023-06-08 01:37:54.000000 cellulose-sdk-0.0.3/cellulose/decorators/cellulose.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.795064 cellulose-sdk-0.0.3/cellulose/infra/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/infra/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.795436 cellulose-sdk-0.0.3/cellulose/metrics/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/metrics/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      430 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.3/cellulose/metrics/latency.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)       90 2023-06-07 04:03:32.000000 cellulose-sdk-0.0.3/cellulose/metrics/metrics.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.796402 cellulose-sdk-0.0.3/cellulose/onnx/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/onnx/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1608 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.3/cellulose/onnx/benchmark.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      311 2023-06-11 00:02:42.000000 cellulose-sdk-0.0.3/cellulose/onnx/checker.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      499 2023-06-11 00:02:42.000000 cellulose-sdk-0.0.3/cellulose/onnx/loader.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      962 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/onnx/runtime.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.796754 cellulose-sdk-0.0.3/cellulose/output/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/output/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      403 2023-06-07 05:06:52.000000 cellulose-sdk-0.0.3/cellulose/output/output.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.797317 cellulose-sdk-0.0.3/cellulose/pytorch/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/pytorch/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1014 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.3/cellulose/pytorch/benchmark.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     4820 2023-06-08 01:36:03.000000 cellulose-sdk-0.0.3/cellulose/pytorch/export.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.797554 cellulose-sdk-0.0.3/cellulose/scripts/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/scripts/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.797638 cellulose-sdk-0.0.3/cellulose/tensorflow/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/tensorflow/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.798714 cellulose-sdk-0.0.3/cellulose/utils/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/utils/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      895 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.3/cellulose/utils/benchmark_results.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      967 2023-06-07 06:17:16.000000 cellulose-sdk-0.0.3/cellulose/utils/csv_utils.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      180 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/utils/devices.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      260 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/utils/engines.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      266 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/utils/numpy.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.798977 cellulose-sdk-0.0.3/cellulose/validation/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/validation/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      667 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.3/cellulose/validation/validation.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)       32 2023-06-12 04:12:06.000000 cellulose-sdk-0.0.3/cellulose/version.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-12 04:12:45.799572 cellulose-sdk-0.0.3/cellulose_sdk.egg-info/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1517 2023-06-12 04:12:45.000000 cellulose-sdk-0.0.3/cellulose_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1687 2023-06-12 04:12:45.000000 cellulose-sdk-0.0.3/cellulose_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        1 2023-06-12 04:12:45.000000 cellulose-sdk-0.0.3/cellulose_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      191 2023-06-12 04:12:45.000000 cellulose-sdk-0.0.3/cellulose_sdk.egg-info/requires.txt
+-rw-r--r--   0 tzhenghao   (501) staff       (20)       10 2023-06-12 04:12:45.000000 cellulose-sdk-0.0.3/cellulose_sdk.egg-info/top_level.txt
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      505 2023-06-07 06:23:01.000000 cellulose-sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 tzhenghao   (501) staff       (20)       38 2023-06-12 04:12:45.799910 cellulose-sdk-0.0.3/setup.cfg
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     8573 2023-06-08 00:03:51.000000 cellulose-sdk-0.0.3/setup.py
```

### Comparing `cellulose-sdk-0.0.2/LICENSE` & `cellulose-sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/PKG-INFO` & `cellulose-sdk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellulose-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cellulose Python SDK
 Home-page: https://www.cellulose.ai
 Author: Cellulose engineering team
 Author-email: zheng@cellulose.ai
 Project-URL: Homepage, https://www.cellulose.ai
 Project-URL: Documentation, http://docs.cellulose.ai
 Keywords: artificial intelligence,benchmarking,debugging,development,onnx,profiler,profiling,pytorch,tensorflow
```

### Comparing `cellulose-sdk-0.0.2/cellulose/api/cellulose_context.py` & `cellulose-sdk-0.0.3/cellulose/api/cellulose_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # Standard imports
 import logging
 from pathlib import Path
 
 # Third party imports
+import click
 from pydantic.dataclasses import dataclass
 
 # Cellulose imports
 from cellulose.artifact.cellulose_artifact_manager import (
     CelluloseArtifactManager,
 )
 from cellulose.configs.loader import ConfigLoader
+from cellulose.dashboard.api_resources.models.onnx import upload_onnx_model
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_TARGET_DIRECTORY = Path.cwd()
 
 
 @dataclass
 class CelluloseContext:
     config_loader = ConfigLoader()
     artifact_manager = CelluloseArtifactManager()
 
-    def __init__(self):
+    def __init__(self, api_key: str):
         logger.info("Initializing Cellulose context...")
         logger.info("Loading Cellulose configs...")
         self.load_config()
         logger.info("Initializing Cellulose artifact manager...")
         self.artifact_manager.init()
+        self.api_key = api_key
 
     def load_config(self):
         """
         Internal!
         Loads the Cellulose configs
         """
         # Initialize and parse workspace level configs.
@@ -45,22 +48,42 @@
         ------
         torch_model (nn.Module): The PyTorch model.
         input: Input tensors to the PyTorch model.
         export_args: Other (both required and optional) arguments specific to
         the underlying export workflow. Please read our documentation for full
         details.
         """
-        torch_model.cellulose.export_model(
+        export_output = torch_model.cellulose.export_model(
             config_loader=self.config_loader,
             artifact_manager=self.artifact_manager,
             torch_model=torch_model,
             input=input,
             **export_args,
         )
 
+        click.secho(
+            "Uploading ONNX model to Cellulose dashboard...", fg="yellow"
+        )
+        response = upload_onnx_model(
+            api_key=self.api_key, onnx_file=export_output.onnx.onnx_file
+        )
+
+        if response.status_code == 200 or response.status_code == 201:
+            click.secho("Done!", fg="green")
+        else:
+            click.secho(
+                "Failed to upload ONNX model to Cellulose dashboard",
+                fg="red",
+            )
+            click.secho("Please check your API key and try again.", fg="red")
+            click.secho(
+                "If the problem persists, please contact us at support@cellulose.ai",
+                fg="red",
+            )
+
     def benchmark(self, torch_model, input, **benchmark_args):
         """
         This method benchmarks the given PyTorch model and input. Please refer
         to our documentation for full set of options.
 
         Params
         ------
```

### Comparing `cellulose-sdk-0.0.2/cellulose/artifact/cellulose_artifact_manager.py` & `cellulose-sdk-0.0.3/cellulose/artifact/cellulose_artifact_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,46 +84,46 @@
         This method loads a current CelluloseArtifact.
         NOTE: It will also reinitialize the Cellulose file context. This means
         you may lose context on unsaved / unexported Cellulose files.
         """
         logger.info("Reinitialize the Cellulose context...")
         self.init()
 
-        # TODO(LEX-33): Implement proper loading of Cellulose artifact from a
+        # TODO: Implement proper loading of Cellulose artifact from a
         #               file path.
         logger.info(
             "Loading Cellulose artifact: {cellulose_artifact_path}...".format(
                 cellulose_artifact_path=cellulose_artifact_path
             )
         )
         # self.cellulose_artifact = cellulose_artifact
 
     def append(self, file: Path):
         """
         This method appends a file to the list of file paths in Cellulose
         artifact.
 
         Params
-        ------
+        -----
         file: Path - The file path to be embedded within Cellulose artifact.
         """
-        # TODO(LEX-39): Verify if .load() file path to Cellulose artifact is
+        # TODO: Verify if .load() file path to Cellulose artifact is
         # valid
         self.cellulose_artifact.file_paths.append(file)
         # Add metadata associated with it too.
 
     def export(self, name: str, target_directory: str):
         """
         This method takes in a name for the Cellulose output artifact and
         target directory for where to place it.
 
         Params
         ------
         name: str - The name of the Cellulose artifact.
-        For example, "my_benchmarks" to export a "my_benchmarks.cellulose"
+        For example, "my_benchmarks" to export a "my_benchmarks.cellulose.zip"
         target_directory: str - The target directory for where to place this
         generated ".cellulose" artifact.
         """
         cellulose_artifact_filename = (
             self.generate_cellulose_artifact_filename(name=name)
         )
         output_cellulose_artifact_path = Path(target_directory).joinpath(
```

### Comparing `cellulose-sdk-0.0.2/cellulose/base/benchmark.py` & `cellulose-sdk-0.0.3/cellulose/base/benchmark.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/configs/.cellulose_config.toml` & `cellulose-sdk-0.0.3/cellulose/configs/.cellulose_config.toml`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/configs/config.py` & `cellulose-sdk-0.0.3/cellulose/configs/config.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/configs/loader.py` & `cellulose-sdk-0.0.3/cellulose/configs/loader.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/decorators/cellulose.py` & `cellulose-sdk-0.0.3/cellulose/decorators/cellulose.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/onnx/benchmark.py` & `cellulose-sdk-0.0.3/cellulose/onnx/benchmark.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/onnx/runtime.py` & `cellulose-sdk-0.0.3/cellulose/onnx/runtime.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/pytorch/benchmark.py` & `cellulose-sdk-0.0.3/cellulose/pytorch/benchmark.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/pytorch/export.py` & `cellulose-sdk-0.0.3/cellulose/pytorch/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         if self.model_config.export_config.enable_onnx_export:
             msg = "Exporting ONNX..."
             logger.info(msg)
             export_output.onnx = self.export_onnx(
                 torch_model=torch_model,
                 input=input,
             )
+
         return export_output
 
     def export_torchscript(
         self,
         torch_model,
     ) -> TorchScriptOutput:
         """
```

### Comparing `cellulose-sdk-0.0.2/cellulose/utils/benchmark_results.py` & `cellulose-sdk-0.0.3/cellulose/utils/benchmark_results.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/utils/csv_utils.py` & `cellulose-sdk-0.0.3/cellulose/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose/validation/validation.py` & `cellulose-sdk-0.0.3/cellulose/validation/validation.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.2/cellulose_sdk.egg-info/PKG-INFO` & `cellulose-sdk-0.0.3/cellulose_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellulose-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cellulose Python SDK
 Home-page: https://www.cellulose.ai
 Author: Cellulose engineering team
 Author-email: zheng@cellulose.ai
 Project-URL: Homepage, https://www.cellulose.ai
 Project-URL: Documentation, http://docs.cellulose.ai
 Keywords: artificial intelligence,benchmarking,debugging,development,onnx,profiler,profiling,pytorch,tensorflow
```

### Comparing `cellulose-sdk-0.0.2/cellulose_sdk.egg-info/SOURCES.txt` & `cellulose-sdk-0.0.3/cellulose_sdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 cellulose/base/checker.py
 cellulose/base/export.py
 cellulose/base/loader.py
 cellulose/configs/.cellulose_config.toml
 cellulose/configs/__init__.py
 cellulose/configs/config.py
 cellulose/configs/loader.py
+cellulose/dashboard/__init__.py
+cellulose/dashboard/credentials.py
+cellulose/dashboard/api_resources/__init__.py
+cellulose/dashboard/api_resources/models/__init__.py
+cellulose/dashboard/api_resources/models/onnx.py
 cellulose/decorators/__init__.py
 cellulose/decorators/cellulose.py
 cellulose/infra/__init__.py
 cellulose/metrics/__init__.py
 cellulose/metrics/latency.py
 cellulose/metrics/metrics.py
 cellulose/onnx/__init__.py
```

### Comparing `cellulose-sdk-0.0.2/setup.py` & `cellulose-sdk-0.0.3/setup.py`

 * *Files identical despite different names*

