# Comparing `tmp/basetrainer-0.7.1.tar.gz` & `tmp/basetrainer-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/basetrainer-0.7.1.tar", last modified: Fri Mar 17 10:21:30 2023, max compression
+gzip compressed data, was "dist/basetrainer-0.7.3.tar", last modified: Mon Jun 12 07:32:41 2023, max compression
```

## Comparing `basetrainer-0.7.1.tar` & `basetrainer-0.7.3.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:30.000000 basetrainer-0.7.1/
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer/
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer/callbacks/
--rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/callbacks/__init__.py
--rw-rw----   0 dm        (1000) dm        (1000)     1166 2022-01-26 04:35:31.000000 basetrainer-0.7.1/basetrainer/callbacks/callbacks.py
--rw-rw----   0 dm        (1000) dm        (1000)     3103 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/callbacks/log_history.py
--rw-rw----   0 dm        (1000) dm        (1000)     1497 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/callbacks/losses_recorder.py
--rw-rw----   0 dm        (1000) dm        (1000)     7158 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/callbacks/model_checkpoint.py
--rw-rw----   0 dm        (1000) dm        (1000)     3208 2022-02-08 08:35:30.000000 basetrainer-0.7.1/basetrainer/callbacks/multi_losses_recorder.py
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer/criterion/
--rwxrwx---   0 dm        (1000) dm        (1000)        1 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/criterion/__init__.py
--rwxrwx---   0 dm        (1000) dm        (1000)     4592 2023-03-17 10:16:56.000000 basetrainer-0.7.1/basetrainer/criterion/criterion.py
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer/engine/
--rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/engine/__init__.py
--rw-rw----   0 dm        (1000) dm        (1000)     1510 2022-01-26 04:35:31.000000 basetrainer-0.7.1/basetrainer/engine/base.py
--rw-rw----   0 dm        (1000) dm        (1000)     7863 2022-01-17 09:22:27.000000 basetrainer-0.7.1/basetrainer/engine/comm.py
--rw-rw----   0 dm        (1000) dm        (1000)     5377 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/engine/engine.py
--rw-rw----   0 dm        (1000) dm        (1000)     3920 2022-01-17 09:22:27.000000 basetrainer-0.7.1/basetrainer/engine/launch.py
--rwxrwx---   0 dm        (1000) dm        (1000)     3229 2023-02-09 01:05:46.000000 basetrainer-0.7.1/basetrainer/engine/onnx_engine.py
--rw-rw----   0 dm        (1000) dm        (1000)     4977 2023-03-17 10:19:56.000000 basetrainer-0.7.1/basetrainer/engine/trainer.py
--rw-rw----   0 dm        (1000) dm        (1000)    11939 2023-03-17 10:16:56.000000 basetrainer-0.7.1/basetrainer/engine/trt_engine.py
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer/metric/
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/
--rwxrwx---   0 dm        (1000) dm        (1000)      168 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/__init__.py
--rwxrwx---   0 dm        (1000) dm        (1000)     3122 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/acc.py
--rwxrwx---   0 dm        (1000) dm        (1000)     5450 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/classification_report.py
--rwxrwx---   0 dm        (1000) dm        (1000)     6586 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/eval_utils.py
--rwxrwx---   0 dm        (1000) dm        (1000)     1634 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/evaluate.py
--rwxrwx---   0 dm        (1000) dm        (1000)     2071 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/iou.py
--rwxrwx---   0 dm        (1000) dm        (1000)     4905 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/metrics.py
--rwxrwx---   0 dm        (1000) dm        (1000)     1424 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/pandas_tools.py
--rwxrwx---   0 dm        (1000) dm        (1000)     9529 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/pr.py
--rwxrwx---   0 dm        (1000) dm        (1000)     2469 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/psnr.py
--rwxrwx---   0 dm        (1000) dm        (1000)     7712 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/roc.py
--rwxrwx---   0 dm        (1000) dm        (1000)     7781 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/eval_tools/verification.py
--rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/__init__.py
--rw-rw----   0 dm        (1000) dm        (1000)     3807 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/metric/accuracy_recorder.py
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer/models/
--rw-rw----   0 dm        (1000) dm        (1000)      119 2022-01-17 09:46:24.000000 basetrainer-0.7.1/basetrainer/models/__init__.py
--rw-rw----   0 dm        (1000) dm        (1000)     3339 2022-01-17 09:50:52.000000 basetrainer-0.7.1/basetrainer/models/build_models.py
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer/optimizer/
--rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/optimizer/__init__.py
--rw-rw----   0 dm        (1000) dm        (1000)     2588 2023-03-17 10:16:56.000000 basetrainer-0.7.1/basetrainer/optimizer/build_optimizer.py
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer/pruning/
--rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/pruning/__init__.py
--rw-rw----   0 dm        (1000) dm        (1000)    12177 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/pruning/nni_pruning.py
--rw-rw----   0 dm        (1000) dm        (1000)     2693 2022-01-17 09:22:27.000000 basetrainer-0.7.1/basetrainer/pruning/slim_pruning.py
--rw-rw----   0 dm        (1000) dm        (1000)     6843 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/pruning/torch_pruning.py
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:30.000000 basetrainer-0.7.1/basetrainer/scheduler/
--rw-rw----   0 dm        (1000) dm        (1000)     2982 2022-12-16 02:49:37.000000 basetrainer-0.7.1/basetrainer/scheduler/CosineAnnealingLR.py
--rw-rw----   0 dm        (1000) dm        (1000)     2140 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/scheduler/ExponentialLR.py
--rw-rw----   0 dm        (1000) dm        (1000)     2633 2022-12-16 02:49:37.000000 basetrainer-0.7.1/basetrainer/scheduler/LambdaLR.py
--rw-rw----   0 dm        (1000) dm        (1000)     3018 2021-12-28 07:55:23.000000 basetrainer-0.7.1/basetrainer/scheduler/MultiStepLR.py
--rw-rw----   0 dm        (1000) dm        (1000)     4378 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/scheduler/MultiStepValue.py
--rw-rw----   0 dm        (1000) dm        (1000)     1657 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/scheduler/WarmUpLR.py
--rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/scheduler/__init__.py
--rw-rw----   0 dm        (1000) dm        (1000)     2150 2022-12-16 02:49:37.000000 basetrainer-0.7.1/basetrainer/scheduler/build_scheduler.py
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:30.000000 basetrainer-0.7.1/basetrainer/utils/
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:30.000000 basetrainer-0.7.1/basetrainer/utils/converter/
--rw-rw----   0 dm        (1000) dm        (1000)      130 2023-01-05 11:21:37.000000 basetrainer-0.7.1/basetrainer/utils/converter/__init__.py
--rw-rw----   0 dm        (1000) dm        (1000)     2764 2023-01-05 11:21:37.000000 basetrainer-0.7.1/basetrainer/utils/converter/onnx2trt.py
--rw-rw----   0 dm        (1000) dm        (1000)     3097 2023-02-09 01:05:46.000000 basetrainer-0.7.1/basetrainer/utils/converter/pytorch2onnx.py
--rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/utils/__init__.py
--rwxrwx---   0 dm        (1000) dm        (1000)    26662 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/utils/file_utils.py
--rwxrwx---   0 dm        (1000) dm        (1000)    83732 2022-01-26 04:35:31.000000 basetrainer-0.7.1/basetrainer/utils/image_utils.py
--rwxrwx---   0 dm        (1000) dm        (1000)     6849 2023-01-05 11:21:37.000000 basetrainer-0.7.1/basetrainer/utils/log.py
--rwxrwx---   0 dm        (1000) dm        (1000)     3781 2022-01-26 04:35:31.000000 basetrainer-0.7.1/basetrainer/utils/plot_utils.py
--rw-rw----   0 dm        (1000) dm        (1000)     5027 2022-01-26 04:35:31.000000 basetrainer-0.7.1/basetrainer/utils/setup_config.py
--rw-rw----   0 dm        (1000) dm        (1000)     1399 2021-12-28 07:55:24.000000 basetrainer-0.7.1/basetrainer/utils/summary.py
--rw-rw----   0 dm        (1000) dm        (1000)     4171 2023-01-05 11:21:37.000000 basetrainer-0.7.1/basetrainer/utils/torch_data.py
--rwxrwx---   0 dm        (1000) dm        (1000)    16389 2023-01-05 11:21:37.000000 basetrainer-0.7.1/basetrainer/utils/torch_tools.py
--rw-rw----   0 dm        (1000) dm        (1000)      141 2023-03-17 10:21:24.000000 basetrainer-0.7.1/basetrainer/__init__.py
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer.egg-info/
--rw-rw----   0 dm        (1000) dm        (1000)    20185 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer.egg-info/PKG-INFO
--rw-rw----   0 dm        (1000) dm        (1000)     2362 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer.egg-info/SOURCES.txt
--rw-rw----   0 dm        (1000) dm        (1000)        1 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer.egg-info/dependency_links.txt
--rw-rw----   0 dm        (1000) dm        (1000)        1 2022-01-17 09:23:42.000000 basetrainer-0.7.1/basetrainer.egg-info/not-zip-safe
--rw-rw----   0 dm        (1000) dm        (1000)       12 2023-03-17 10:21:29.000000 basetrainer-0.7.1/basetrainer.egg-info/top_level.txt
-drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-03-17 10:21:30.000000 basetrainer-0.7.1/test/
--rw-rw----   0 dm        (1000) dm        (1000)     3108 2022-12-16 02:49:37.000000 basetrainer-0.7.1/test/test_scheduler.py
--rwxrwx---   0 dm        (1000) dm        (1000)     1073 2021-12-28 07:55:19.000000 basetrainer-0.7.1/LICENCE
--rw-rw----   0 dm        (1000) dm        (1000)    14418 2023-03-17 10:16:56.000000 basetrainer-0.7.1/README.md
--rw-rw----   0 dm        (1000) dm        (1000)    19938 2023-03-17 10:21:22.000000 basetrainer-0.7.1/README.rst
--rwxrwx---   0 dm        (1000) dm        (1000)     2060 2022-11-15 01:48:02.000000 basetrainer-0.7.1/setup.py
--rw-rw----   0 dm        (1000) dm        (1000)    20185 2023-03-17 10:21:30.000000 basetrainer-0.7.1/PKG-INFO
--rw-rw----   0 dm        (1000) dm        (1000)       38 2023-03-17 10:21:30.000000 basetrainer-0.7.1/setup.cfg
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:39.000000 basetrainer-0.7.3/
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer/
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer/callbacks/
+-rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/callbacks/__init__.py
+-rw-rw----   0 dm        (1000) dm        (1000)     1166 2022-01-26 04:35:31.000000 basetrainer-0.7.3/basetrainer/callbacks/callbacks.py
+-rw-rw----   0 dm        (1000) dm        (1000)     3103 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/callbacks/log_history.py
+-rw-rw----   0 dm        (1000) dm        (1000)     1497 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/callbacks/losses_recorder.py
+-rw-rw----   0 dm        (1000) dm        (1000)     7158 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/callbacks/model_checkpoint.py
+-rw-rw----   0 dm        (1000) dm        (1000)     3208 2022-02-08 08:35:30.000000 basetrainer-0.7.3/basetrainer/callbacks/multi_losses_recorder.py
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer/criterion/
+-rwxrwx---   0 dm        (1000) dm        (1000)        1 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/criterion/__init__.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     4592 2023-03-17 10:16:56.000000 basetrainer-0.7.3/basetrainer/criterion/criterion.py
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer/engine/
+-rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/engine/__init__.py
+-rw-rw----   0 dm        (1000) dm        (1000)     1510 2022-01-26 04:35:31.000000 basetrainer-0.7.3/basetrainer/engine/base.py
+-rw-rw----   0 dm        (1000) dm        (1000)     7863 2022-01-17 09:22:27.000000 basetrainer-0.7.3/basetrainer/engine/comm.py
+-rw-rw----   0 dm        (1000) dm        (1000)     5377 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/engine/engine.py
+-rw-rw----   0 dm        (1000) dm        (1000)     3920 2022-01-17 09:22:27.000000 basetrainer-0.7.3/basetrainer/engine/launch.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     3229 2023-02-09 01:05:46.000000 basetrainer-0.7.3/basetrainer/engine/onnx_engine.py
+-rw-rw----   0 dm        (1000) dm        (1000)     4977 2023-03-17 10:31:40.000000 basetrainer-0.7.3/basetrainer/engine/trainer.py
+-rw-rw----   0 dm        (1000) dm        (1000)    11939 2023-02-14 05:39:26.000000 basetrainer-0.7.3/basetrainer/engine/trt_engine.py
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer/metric/
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/
+-rwxrwx---   0 dm        (1000) dm        (1000)      168 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/__init__.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     3122 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/acc.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     5457 2023-06-12 07:17:34.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/classification_report.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     6586 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/eval_utils.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     1634 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/evaluate.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     2071 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/iou.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     4905 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/metrics.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     1424 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/pandas_tools.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     9529 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/pr.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     2469 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/psnr.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     7712 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/roc.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     7781 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/eval_tools/verification.py
+-rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/metric/__init__.py
+-rw-rw----   0 dm        (1000) dm        (1000)     4304 2023-03-21 00:46:53.000000 basetrainer-0.7.3/basetrainer/metric/accuracy_recorder.py
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer/models/
+-rw-rw----   0 dm        (1000) dm        (1000)      119 2022-01-17 09:46:24.000000 basetrainer-0.7.3/basetrainer/models/__init__.py
+-rw-rw----   0 dm        (1000) dm        (1000)     3339 2022-01-17 09:50:52.000000 basetrainer-0.7.3/basetrainer/models/build_models.py
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer/optimizer/
+-rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/optimizer/__init__.py
+-rw-rw----   0 dm        (1000) dm        (1000)     2588 2023-03-17 10:16:56.000000 basetrainer-0.7.3/basetrainer/optimizer/build_optimizer.py
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer/pruning/
+-rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/pruning/__init__.py
+-rw-rw----   0 dm        (1000) dm        (1000)    12177 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/pruning/nni_pruning.py
+-rw-rw----   0 dm        (1000) dm        (1000)     2693 2022-01-17 09:22:27.000000 basetrainer-0.7.3/basetrainer/pruning/slim_pruning.py
+-rw-rw----   0 dm        (1000) dm        (1000)     6843 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/pruning/torch_pruning.py
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:39.000000 basetrainer-0.7.3/basetrainer/scheduler/
+-rw-rw----   0 dm        (1000) dm        (1000)     2982 2022-12-16 02:49:37.000000 basetrainer-0.7.3/basetrainer/scheduler/CosineAnnealingLR.py
+-rw-rw----   0 dm        (1000) dm        (1000)     2140 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/scheduler/ExponentialLR.py
+-rw-rw----   0 dm        (1000) dm        (1000)     2633 2022-12-16 02:49:37.000000 basetrainer-0.7.3/basetrainer/scheduler/LambdaLR.py
+-rw-rw----   0 dm        (1000) dm        (1000)     3018 2021-12-28 07:55:23.000000 basetrainer-0.7.3/basetrainer/scheduler/MultiStepLR.py
+-rw-rw----   0 dm        (1000) dm        (1000)     4378 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/scheduler/MultiStepValue.py
+-rw-rw----   0 dm        (1000) dm        (1000)     1657 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/scheduler/WarmUpLR.py
+-rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/scheduler/__init__.py
+-rw-rw----   0 dm        (1000) dm        (1000)     2150 2022-12-16 02:49:37.000000 basetrainer-0.7.3/basetrainer/scheduler/build_scheduler.py
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:39.000000 basetrainer-0.7.3/basetrainer/utils/
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:39.000000 basetrainer-0.7.3/basetrainer/utils/converter/
+-rw-rw----   0 dm        (1000) dm        (1000)      130 2023-01-05 11:21:37.000000 basetrainer-0.7.3/basetrainer/utils/converter/__init__.py
+-rw-rw----   0 dm        (1000) dm        (1000)     2764 2023-01-05 11:21:37.000000 basetrainer-0.7.3/basetrainer/utils/converter/onnx2trt.py
+-rw-rw----   0 dm        (1000) dm        (1000)     3097 2023-02-09 01:05:46.000000 basetrainer-0.7.3/basetrainer/utils/converter/pytorch2onnx.py
+-rw-rw----   0 dm        (1000) dm        (1000)      119 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/utils/__init__.py
+-rwxrwx---   0 dm        (1000) dm        (1000)    26662 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/utils/file_utils.py
+-rw-rw----   0 dm        (1000) dm        (1000)     5722 2023-03-30 05:42:18.000000 basetrainer-0.7.3/basetrainer/utils/heatmap_utils.py
+-rwxrwx---   0 dm        (1000) dm        (1000)    83732 2022-01-26 04:35:31.000000 basetrainer-0.7.3/basetrainer/utils/image_utils.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     6849 2023-01-05 11:21:37.000000 basetrainer-0.7.3/basetrainer/utils/log.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     3781 2022-01-26 04:35:31.000000 basetrainer-0.7.3/basetrainer/utils/plot_utils.py
+-rw-rw----   0 dm        (1000) dm        (1000)     5027 2022-01-26 04:35:31.000000 basetrainer-0.7.3/basetrainer/utils/setup_config.py
+-rw-rw----   0 dm        (1000) dm        (1000)     1399 2021-12-28 07:55:24.000000 basetrainer-0.7.3/basetrainer/utils/summary.py
+-rw-rw----   0 dm        (1000) dm        (1000)     4171 2023-01-05 11:21:37.000000 basetrainer-0.7.3/basetrainer/utils/torch_data.py
+-rwxrwx---   0 dm        (1000) dm        (1000)    17049 2023-03-22 06:56:49.000000 basetrainer-0.7.3/basetrainer/utils/torch_tools.py
+-rw-rw----   0 dm        (1000) dm        (1000)     6261 2023-03-30 05:42:01.000000 basetrainer-0.7.3/basetrainer/utils/torchcam_utils.py
+-rw-rw----   0 dm        (1000) dm        (1000)      141 2023-06-12 07:18:48.000000 basetrainer-0.7.3/basetrainer/__init__.py
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer.egg-info/
+-rw-rw----   0 dm        (1000) dm        (1000)    20185 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer.egg-info/PKG-INFO
+-rw-rw----   0 dm        (1000) dm        (1000)     2422 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer.egg-info/SOURCES.txt
+-rw-rw----   0 dm        (1000) dm        (1000)        1 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer.egg-info/dependency_links.txt
+-rw-rw----   0 dm        (1000) dm        (1000)        1 2022-01-17 09:23:42.000000 basetrainer-0.7.3/basetrainer.egg-info/not-zip-safe
+-rw-rw----   0 dm        (1000) dm        (1000)       12 2023-06-12 07:32:38.000000 basetrainer-0.7.3/basetrainer.egg-info/top_level.txt
+drwxrwx---   0 dm        (1000) dm        (1000)        0 2023-06-12 07:32:39.000000 basetrainer-0.7.3/test/
+-rw-rw----   0 dm        (1000) dm        (1000)     3108 2022-12-16 02:49:37.000000 basetrainer-0.7.3/test/test_scheduler.py
+-rwxrwx---   0 dm        (1000) dm        (1000)     1073 2021-12-28 07:55:19.000000 basetrainer-0.7.3/LICENCE
+-rw-rw----   0 dm        (1000) dm        (1000)    14418 2023-03-17 10:16:56.000000 basetrainer-0.7.3/README.md
+-rwxrwx---   0 dm        (1000) dm        (1000)     2060 2023-06-12 07:31:06.000000 basetrainer-0.7.3/setup.py
+-rw-rw----   0 dm        (1000) dm        (1000)    20185 2023-06-12 07:32:39.000000 basetrainer-0.7.3/PKG-INFO
+-rw-rw----   0 dm        (1000) dm        (1000)       38 2023-06-12 07:32:39.000000 basetrainer-0.7.3/setup.cfg
```

### Comparing `basetrainer-0.7.1/basetrainer/callbacks/callbacks.py` & `basetrainer-0.7.3/basetrainer/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/callbacks/log_history.py` & `basetrainer-0.7.3/basetrainer/callbacks/log_history.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/callbacks/losses_recorder.py` & `basetrainer-0.7.3/basetrainer/callbacks/losses_recorder.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/callbacks/model_checkpoint.py` & `basetrainer-0.7.3/basetrainer/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/callbacks/multi_losses_recorder.py` & `basetrainer-0.7.3/basetrainer/callbacks/multi_losses_recorder.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/criterion/criterion.py` & `basetrainer-0.7.3/basetrainer/criterion/criterion.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/engine/base.py` & `basetrainer-0.7.3/basetrainer/engine/base.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/engine/comm.py` & `basetrainer-0.7.3/basetrainer/engine/comm.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/engine/engine.py` & `basetrainer-0.7.3/basetrainer/engine/engine.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/engine/launch.py` & `basetrainer-0.7.3/basetrainer/engine/launch.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/engine/onnx_engine.py` & `basetrainer-0.7.3/basetrainer/engine/onnx_engine.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/engine/trainer.py` & `basetrainer-0.7.3/basetrainer/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/engine/trt_engine.py` & `basetrainer-0.7.3/basetrainer/engine/trt_engine.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/acc.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/acc.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/classification_report.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/classification_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     '''
     if target_names is None:
         target_names = list(set(pred_labels) | set(true_labels))
         target_names.sort()
     else:
         true_labels = [target_names[int(i)] for i in true_labels]
         pred_labels = [target_names[int(i)] for i in pred_labels]
-    conf_matrix = metrics.confusion_matrix(true_labels, pred_labels, target_names)
+    conf_matrix = metrics.confusion_matrix(true_labels, pred_labels, labels=target_names)
     if normalization:
         conf_matrix = conf_matrix.astype('float') / conf_matrix.sum(axis=1)[:, np.newaxis]  # 归一化
     pdf = pd.DataFrame(conf_matrix, columns=target_names, index=target_names)
     # print("Confusion Matrix:\n",pdf)
     if filename is not None:
         create_file_path(filename)
         pandas_tools.save_csv(filename, pdf, save_index=True)
```

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/eval_utils.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/eval_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/evaluate.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/evaluate.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/iou.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/iou.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/metrics.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/metrics.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/pandas_tools.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/pandas_tools.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/pr.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/pr.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/psnr.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/psnr.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/roc.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/roc.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/eval_tools/verification.py` & `basetrainer-0.7.3/basetrainer/metric/eval_tools/verification.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/metric/accuracy_recorder.py` & `basetrainer-0.7.3/basetrainer/metric/accuracy_recorder.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         self.confusion_matrix = confusion_matrix
         self.train_top1 = AverageMeter()
         self.test_top1 = AverageMeter()
         self.true_labels = np.ones(0)
         self.pred_labels = np.ones(0)
         self.logger = log.get_logger()
         self.epoch = 0
+        self.test_max_acc = 0
 
     def on_epoch_begin(self, epoch, logs: dict = {}):
         self.train_top1.reset()
         self.epoch = epoch
 
     def on_test_begin(self, logs: dict = {}):
         self.test_top1.reset()
@@ -45,24 +46,32 @@
 
     def on_test_end(self, logs: dict = {}):
         acc = accuracy_score(self.true_labels, self.pred_labels) * 100.0
         report = classification_report.get_classification_report(self.true_labels,
                                                                  self.pred_labels,
                                                                  target_names=self.target_names)
         self.logger.info("\nAcc:{:.4f}\n{}".format(acc, report))
-        if self.confusion_matrix:
-            confuse_file = os.path.join(self.confusion_matrix, "confusion_matrix_{:0=3d}.csv".format(self.epoch))
+        if self.confusion_matrix and acc >= self.test_max_acc:
+            self.test_max_acc = acc
+            file_utils.remove_prefix_files(self.confusion_matrix, "confusion_matrix_*")
+            confuse_file = os.path.join(self.confusion_matrix,
+                                        "confusion_matrix_{:0=3d}_{:.4f}.csv".format(self.epoch, acc))
             conf_matrix = classification_report.get_confusion_matrix(self.true_labels,
                                                                      self.pred_labels,
                                                                      self.target_names,
                                                                      filename=confuse_file)
+            self.logger.info("save confuse file in:{} ".format(confuse_file))
 
     @staticmethod
     def summary(phase, average_meter: AverageMeter, indicator, inputs, outputs, logs: dict = {}):
-        targets, labels = inputs[0], inputs[1].cpu()
+        if isinstance(inputs, dict):
+            targets, labels = inputs['image'], inputs["label"].cpu()
+        else:
+            targets, labels = inputs[0], inputs[1].cpu()
+        if isinstance(outputs, tuple): outputs = outputs[0]
         outputs = torch.nn.functional.softmax(outputs, dim=1).cpu()
         pred_score, pred_index = torch.max(outputs, dim=1)
         acc, = accuracy(outputs.data, labels, topk=(1,))
         # fix a bug: n = labels.size(0)
         average_meter.update(acc.data.item(), labels.size(0))
         logs[phase] = logs[phase] if phase in logs else {}
         logs[phase][indicator] = average_meter.avg
```

### Comparing `basetrainer-0.7.1/basetrainer/models/build_models.py` & `basetrainer-0.7.3/basetrainer/models/build_models.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/optimizer/build_optimizer.py` & `basetrainer-0.7.3/basetrainer/optimizer/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/pruning/nni_pruning.py` & `basetrainer-0.7.3/basetrainer/pruning/nni_pruning.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/pruning/slim_pruning.py` & `basetrainer-0.7.3/basetrainer/pruning/slim_pruning.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/pruning/torch_pruning.py` & `basetrainer-0.7.3/basetrainer/pruning/torch_pruning.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/scheduler/CosineAnnealingLR.py` & `basetrainer-0.7.3/basetrainer/scheduler/CosineAnnealingLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/scheduler/ExponentialLR.py` & `basetrainer-0.7.3/basetrainer/scheduler/ExponentialLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/scheduler/LambdaLR.py` & `basetrainer-0.7.3/basetrainer/scheduler/LambdaLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/scheduler/MultiStepLR.py` & `basetrainer-0.7.3/basetrainer/scheduler/MultiStepLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/scheduler/MultiStepValue.py` & `basetrainer-0.7.3/basetrainer/scheduler/MultiStepValue.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/scheduler/WarmUpLR.py` & `basetrainer-0.7.3/basetrainer/scheduler/WarmUpLR.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/scheduler/build_scheduler.py` & `basetrainer-0.7.3/basetrainer/scheduler/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/converter/onnx2trt.py` & `basetrainer-0.7.3/basetrainer/utils/converter/onnx2trt.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/converter/pytorch2onnx.py` & `basetrainer-0.7.3/basetrainer/utils/converter/pytorch2onnx.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/file_utils.py` & `basetrainer-0.7.3/basetrainer/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/image_utils.py` & `basetrainer-0.7.3/basetrainer/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/log.py` & `basetrainer-0.7.3/basetrainer/utils/log.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/plot_utils.py` & `basetrainer-0.7.3/basetrainer/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/setup_config.py` & `basetrainer-0.7.3/basetrainer/utils/setup_config.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/summary.py` & `basetrainer-0.7.3/basetrainer/utils/summary.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/torch_data.py` & `basetrainer-0.7.3/basetrainer/utils/torch_data.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/basetrainer/utils/torch_tools.py` & `basetrainer-0.7.3/basetrainer/utils/torch_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -338,30 +338,38 @@
     FLOPs 的全称是 floating points of operations，即浮点运算次数，用来衡量模型的计算复杂度。
     计算 FLOPs 实际上是计算模型中乘法和加法的运算次数。
     卷积层的浮点运算次数不仅取决于卷积核的大小和输入输出通道数，还取决于特征图的大小；
     而全连接层的浮点运算次数和参数量是相同的。
     ====================================================
     :param model:
     :param batch_size:
-    :param input_size:
+    :param input_size: (W,H) or (B, C, H, W)
     :param plot: plot model
     :param device:
     :return:
     """
     from torchsummary import summary
     from torchstat import stat
-    inputs = torch.randn(size=(batch_size, 3, input_size[1], input_size[0]))
+    if len(input_size) == 2:
+        shape = (batch_size, 3, input_size[1], input_size[0])
+    elif len(input_size) == 4:
+        shape = tuple(input_size)
+    else:
+        raise Exception("input_size error:{}".format(input_size))
+    B, C, H, W = shape
+    # inputs = torch.randn(size=(B, 3, input_size[1], input_size[0]))
+    inputs = torch.randn(size=shape)
     inputs = inputs.to(device)
     model = model.to(device)
     model.eval()
     output = model(inputs)
     # 统计模型参数
-    summary(model, input_size=(3, input_size[1], input_size[0]), batch_size=batch_size, device=device)
+    summary(model, input_size=(C, H, W), batch_size=B, device=device)
     # 统计模型参数和计算FLOPs
-    stat(model, (3, input_size[1], input_size[0]))
+    stat(model, (C, H, W))
     # summary可能报错，可使用该方法
     # summary_v2(model, inputs, item_length=26, verbose=True)
     # from thop import profile
     # macs, params = profile(model, inputs=(inputs,))
     # print("Total Flops :{}".format(macs))
     # print("Total params:{}".format(params))
     print("===" * 10)
@@ -379,21 +387,28 @@
     这有助于在模型压缩过程中检查模型的复杂度。
     注意，对于结构化的剪枝，仅根据掩码来标识保留的滤波器，不会考虑剪枝的输入通道，
     因此，计算出的 FLOPs 会比实际数值要大（即，模型加速后的计算值）。
     我们支持两种模式来收集模块信息。 第一种是 default 模式，它只采集卷积操作和线性操作的信息。
     第二种是 full 模式，它还会收集其他操作的信息。 用户可以轻松地使用我们收集的 results 进行进一步的分析。
     :param model:
     :param batch_size:
-    :param input_size:
+    :param input_size: (W,H) or (B, C, H, W)
     :param plot:
     :param device:
     :return:
     """
     from nni.compression.pytorch.utils.counter import count_flops_params
-    inputs = torch.randn(size=(batch_size, 3, input_size[1], input_size[0]))
+    if len(input_size) == 2:
+        shape = (batch_size, 3, input_size[1], input_size[0])
+    elif len(input_size) == 4:
+        shape = tuple(input_size)
+    else:
+        raise Exception("input_size error:{}".format(input_size))
+    B, C, H, W = shape
+    inputs = torch.randn(size=shape)
     inputs = inputs.to(device)
     model = model.to(device)
     model.eval()
     output = model(inputs)
     flops, params, _ = count_flops_params(model, inputs, verbose=True)
     info = f"Model FLOPs {flops / 1e6:.2f}M, Params {params / 1e6:.2f}M"
     print(info)
@@ -419,30 +434,37 @@
     FLOPs 的全称是 floating points of operations，即浮点运算次数，用来衡量模型的计算复杂度。
     计算 FLOPs 实际上是计算模型中乘法和加法的运算次数。
     卷积层的浮点运算次数不仅取决于卷积核的大小和输入输出通道数，还取决于特征图的大小；
     而全连接层的浮点运算次数和参数量是相同的。
     ====================================================
     :param model:
     :param batch_size:
-    :param input_size:
+    :param input_size: (W,H) or (B, C, H, W)
     :param plot: plot model
     :param device:
     :return:
     """
     from torchinfo import summary
     from torchstat import stat
-    inputs = torch.randn(size=(batch_size, 3, input_size[1], input_size[0]))
+    if len(input_size) == 2:
+        shape = (batch_size, 3, input_size[1], input_size[0])
+    elif len(input_size) == 4:
+        shape = tuple(input_size)
+    else:
+        raise Exception("input_size error:{}".format(input_size))
+    B, C, H, W = shape
+    inputs = torch.randn(size=shape)
     inputs = inputs.to(device)
     model = model.to(device)
     model.eval()
     output = model(inputs)
     # 统计模型参数
-    summary(model, input_size=(batch_size, 3, input_size[1], input_size[0]), device=device)
+    summary(model, input_size=shape, device=device)
     # 统计模型参数和计算FLOPs
-    stat(model, (3, input_size[1], input_size[0]))
+    stat(model, (C, H, W))
     # summary可能报错，可使用该方法
     # summary_v2(model, inputs, item_length=26, verbose=True)
     # from thop import profile
     # macs, params = profile(model, inputs=(inputs,))
     # print("Total Flops :{}".format(macs))
     # print("Total params:{}".format(params))
     print("===" * 10)
```

### Comparing `basetrainer-0.7.1/basetrainer.egg-info/PKG-INFO` & `basetrainer-0.7.3/basetrainer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basetrainer
-Version: 0.7.1
+Version: 0.7.3
 Summary: basetrainer
 Home-page: https://github.com/PanJinquan/Pytorch-Base-Trainer
 Author: PanJinquan
 Author-email: pan_jinquan@163.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
```

### Comparing `basetrainer-0.7.1/basetrainer.egg-info/SOURCES.txt` & `basetrainer-0.7.3/basetrainer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENCE
 README.md
-README.rst
 setup.py
 basetrainer/__init__.py
 basetrainer.egg-info/PKG-INFO
 basetrainer.egg-info/SOURCES.txt
 basetrainer.egg-info/dependency_links.txt
 basetrainer.egg-info/not-zip-safe
 basetrainer.egg-info/top_level.txt
@@ -52,18 +51,20 @@
 basetrainer/scheduler/MultiStepLR.py
 basetrainer/scheduler/MultiStepValue.py
 basetrainer/scheduler/WarmUpLR.py
 basetrainer/scheduler/__init__.py
 basetrainer/scheduler/build_scheduler.py
 basetrainer/utils/__init__.py
 basetrainer/utils/file_utils.py
+basetrainer/utils/heatmap_utils.py
 basetrainer/utils/image_utils.py
 basetrainer/utils/log.py
 basetrainer/utils/plot_utils.py
 basetrainer/utils/setup_config.py
 basetrainer/utils/summary.py
 basetrainer/utils/torch_data.py
 basetrainer/utils/torch_tools.py
+basetrainer/utils/torchcam_utils.py
 basetrainer/utils/converter/__init__.py
 basetrainer/utils/converter/onnx2trt.py
 basetrainer/utils/converter/pytorch2onnx.py
 test/test_scheduler.py
```

### Comparing `basetrainer-0.7.1/test/test_scheduler.py` & `basetrainer-0.7.3/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/LICENCE` & `basetrainer-0.7.3/LICENCE`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/README.md` & `basetrainer-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `basetrainer-0.7.1/README.rst` & `basetrainer-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: basetrainer
+Version: 0.7.3
+Summary: basetrainer
+Home-page: https://github.com/PanJinquan/Pytorch-Base-Trainer
+Author: PanJinquan
+Author-email: pan_jinquan@163.com
+License: MIT
+Platform: UNKNOWN
+License-File: LICENCE
+
 Pytorch-Base-Trainer(PBT)
 =========================
 
 -  开源不易,麻烦给个【Star】
 -  Github: https://github.com/PanJinquan/Pytorch-Base-Trainer
 -  pip安装包： https://pypi.org/project/basetrainer/
 -  博客地址：https://panjinquan.blog.csdn.net/article/details/122662902
@@ -339,7 +350,9 @@
 ------
 
 +------------+------------------------+
 | 作者       | PKing                  |
 +============+========================+
 | 联系方式   | pan\_jinquan@163.com   |
 +------------+------------------------+
+
+
```

### Comparing `basetrainer-0.7.1/setup.py` & `basetrainer-0.7.3/setup.py`

 * *Files identical despite different names*

