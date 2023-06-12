# Comparing `tmp/neural-amp-modeler-0.5.2.tar.gz` & `tmp/neural-amp-modeler-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-amp-modeler-0.5.2.tar", last modified: Thu Apr 27 02:14:55 2023, max compression
+gzip compressed data, was "neural-amp-modeler-0.6.0.tar", last modified: Mon Jun 12 04:38:05 2023, max compression
```

## Comparing `neural-amp-modeler-0.5.2.tar` & `neural-amp-modeler-0.6.0.tar`

### file list

```diff
@@ -1,50 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.419704 neural-amp-modeler-0.5.2/
--rw-rw-rw-   0        0        0     1093 2022-04-21 06:27:49.000000 neural-amp-modeler-0.5.2/LICENSE
--rw-rw-rw-   0        0        0       50 2023-03-25 00:10:46.000000 neural-amp-modeler-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0      219 2023-04-27 02:14:55.419704 neural-amp-modeler-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4677 2023-04-27 02:02:18.000000 neural-amp-modeler-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.371704 neural-amp-modeler-0.5.2/nam/
--rw-rw-rw-   0        0        0      754 2023-03-19 00:42:20.000000 neural-amp-modeler-0.5.2/nam/__init__.py
--rw-rw-rw-   0        0        0      377 2023-03-25 00:10:46.000000 neural-amp-modeler-0.5.2/nam/_core.py
--rw-rw-rw-   0        0        0       23 2023-04-27 02:08:12.000000 neural-amp-modeler-0.5.2/nam/_version.py
--rw-rw-rw-   0        0        0    22751 2023-04-18 01:51:50.000000 neural-amp-modeler-0.5.2/nam/data.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.385703 neural-amp-modeler-0.5.2/nam/models/
--rw-rw-rw-   0        0        0      383 2023-02-16 06:08:00.000000 neural-amp-modeler-0.5.2/nam/models/__init__.py
--rw-rw-rw-   0        0        0      218 2023-04-09 17:49:31.000000 neural-amp-modeler-0.5.2/nam/models/_activations.py
--rw-rw-rw-   0        0        0     5510 2023-04-23 01:03:30.000000 neural-amp-modeler-0.5.2/nam/models/_base.py
--rw-rw-rw-   0        0        0     4675 2023-04-27 02:05:48.000000 neural-amp-modeler-0.5.2/nam/models/_exportable.py
--rw-rw-rw-   0        0        0      250 2022-09-03 21:37:15.000000 neural-amp-modeler-0.5.2/nam/models/_names.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.389702 neural-amp-modeler-0.5.2/nam/models/_resources/
--rw-rw-rw-   0        0        0   144044 2023-03-25 00:10:46.000000 neural-amp-modeler-0.5.2/nam/models/_resources/loudness_input.wav
--rw-rw-rw-   0        0        0    11326 2023-04-09 17:50:14.000000 neural-amp-modeler-0.5.2/nam/models/base.py
--rw-rw-rw-   0        0        0     9342 2022-09-04 21:58:20.000000 neural-amp-modeler-0.5.2/nam/models/conv_net.py
--rw-rw-rw-   0        0        0     2022 2022-09-03 21:37:15.000000 neural-amp-modeler-0.5.2/nam/models/linear.py
--rw-rw-rw-   0        0        0     2230 2023-04-23 01:03:30.000000 neural-amp-modeler-0.5.2/nam/models/losses.py
--rw-rw-rw-   0        0        0     1240 2023-04-27 02:03:11.000000 neural-amp-modeler-0.5.2/nam/models/metadata.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.394704 neural-amp-modeler-0.5.2/nam/models/parametric/
--rw-rw-rw-   0        0        0      108 2023-04-09 17:49:31.000000 neural-amp-modeler-0.5.2/nam/models/parametric/__init__.py
--rw-rw-rw-   0        0        0     6787 2023-04-09 17:49:31.000000 neural-amp-modeler-0.5.2/nam/models/parametric/catnets.py
--rw-rw-rw-   0        0        0    18792 2023-02-16 06:08:00.000000 neural-amp-modeler-0.5.2/nam/models/parametric/hyper_net.py
--rw-rw-rw-   0        0        0     1592 2022-09-03 21:37:15.000000 neural-amp-modeler-0.5.2/nam/models/parametric/params.py
--rw-rw-rw-   0        0        0    16701 2023-04-22 22:14:48.000000 neural-amp-modeler-0.5.2/nam/models/recurrent.py
--rw-rw-rw-   0        0        0     1177 2022-12-15 07:10:30.000000 neural-amp-modeler-0.5.2/nam/models/undersampling.py
--rw-rw-rw-   0        0        0    12766 2023-02-17 03:42:58.000000 neural-amp-modeler-0.5.2/nam/models/wavenet.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.406703 neural-amp-modeler-0.5.2/nam/train/
--rw-rw-rw-   0        0        0      111 2023-01-29 07:48:38.000000 neural-amp-modeler-0.5.2/nam/train/__init__.py
--rw-rw-rw-   0        0        0      690 2023-04-09 17:49:31.000000 neural-amp-modeler-0.5.2/nam/train/_version.py
--rw-rw-rw-   0        0        0     3351 2023-04-23 01:10:20.000000 neural-amp-modeler-0.5.2/nam/train/colab.py
--rw-rw-rw-   0        0        0    14470 2023-04-27 02:02:18.000000 neural-amp-modeler-0.5.2/nam/train/core.py
--rw-rw-rw-   0        0        0    19942 2023-04-27 02:03:19.000000 neural-amp-modeler-0.5.2/nam/train/gui.py
--rw-rw-rw-   0        0        0     1578 2023-02-14 06:14:54.000000 neural-amp-modeler-0.5.2/nam/train/ir.py
--rw-rw-rw-   0        0        0      321 2023-02-16 06:08:00.000000 neural-amp-modeler-0.5.2/nam/util.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.417703 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/
--rw-rw-rw-   0        0        0      219 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      970 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-27 02:14:55.000000 neural-amp-modeler-0.5.2/neural_amp_modeler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 02:14:55.419704 neural-amp-modeler-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-04-27 02:02:18.000000 neural-amp-modeler-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:14:55.418704 neural-amp-modeler-0.5.2/tests/
--rw-rw-rw-   0        0        0      250 2022-04-21 06:27:49.000000 neural-amp-modeler-0.5.2/tests/test_install.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.025730 neural-amp-modeler-0.6.0/
+-rw-r--r--   0 steve      (501) staff       (20)     1072 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural-amp-modeler-0.6.0/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)      211 2023-06-12 04:38:05.025209 neural-amp-modeler-0.6.0/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     4536 2023-06-12 04:35:43.000000 neural-amp-modeler-0.6.0/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.970623 neural-amp-modeler-0.6.0/nam/
+-rw-r--r--   0 steve      (501) staff       (20)      729 2023-03-18 16:36:25.000000 neural-amp-modeler-0.6.0/nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural-amp-modeler-0.6.0/nam/_core.py
+-rw-r--r--   0 steve      (501) staff       (20)       22 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)    25028 2023-06-12 04:30:52.000000 neural-amp-modeler-0.6.0/nam/data.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.984008 neural-amp-modeler-0.6.0/nam/models/
+-rw-r--r--   0 steve      (501) staff       (20)      372 2023-05-20 03:46:31.000000 neural-amp-modeler-0.6.0/nam/models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/nam/models/_activations.py
+-rw-r--r--   0 steve      (501) staff       (20)     5326 2023-05-17 02:24:00.000000 neural-amp-modeler-0.6.0/nam/models/_base.py
+-rw-r--r--   0 steve      (501) staff       (20)     4816 2023-05-07 19:58:11.000000 neural-amp-modeler-0.6.0/nam/models/_exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/models/_names.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.985183 neural-amp-modeler-0.6.0/nam/models/_resources/
+-rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural-amp-modeler-0.6.0/nam/models/_resources/loudness_input.wav
+-rw-r--r--   0 steve      (501) staff       (20)    13555 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     9052 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/models/conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     1952 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/models/linear.py
+-rw-r--r--   0 steve      (501) staff       (20)     2440 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/models/losses.py
+-rw-r--r--   0 steve      (501) staff       (20)     1187 2023-05-17 02:24:00.000000 neural-amp-modeler-0.6.0/nam/models/metadata.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.992068 neural-amp-modeler-0.6.0/nam/models/parametric/
+-rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/nam/models/parametric/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6572 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/nam/models/parametric/catnets.py
+-rw-r--r--   0 steve      (501) staff       (20)    18233 2023-05-20 03:46:31.000000 neural-amp-modeler-0.6.0/nam/models/parametric/hyper_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     1521 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/models/parametric/params.py
+-rw-r--r--   0 steve      (501) staff       (20)    16232 2023-04-25 01:51:12.000000 neural-amp-modeler-0.6.0/nam/models/recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)    13909 2023-05-07 19:58:11.000000 neural-amp-modeler-0.6.0/nam/models/wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.997691 neural-amp-modeler-0.6.0/nam/train/
+-rw-r--r--   0 steve      (501) staff       (20)      108 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      852 2023-05-17 02:24:00.000000 neural-amp-modeler-0.6.0/nam/train/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)     3911 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/train/colab.py
+-rw-r--r--   0 steve      (501) staff       (20)    30769 2023-06-12 04:30:52.000000 neural-amp-modeler-0.6.0/nam/train/core.py
+-rw-r--r--   0 steve      (501) staff       (20)    21047 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/train/gui.py
+-rw-r--r--   0 steve      (501) staff       (20)      307 2023-04-29 18:46:19.000000 neural-amp-modeler-0.6.0/nam/util.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.003270 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      211 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     1793 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       42 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      114 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       10 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-06-12 04:38:05.025895 neural-amp-modeler-0.6.0/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)      977 2023-06-12 04:30:52.000000 neural-amp-modeler-0.6.0/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.004405 neural-amp-modeler-0.6.0/tests/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-05-28 20:20:41.000000 neural-amp-modeler-0.6.0/tests/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.005306 neural-amp-modeler-0.6.0/tests/resources/
+-rw-r--r--   0 steve      (501) staff       (20)      676 2023-05-28 20:20:41.000000 neural-amp-modeler-0.6.0/tests/resources/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.006443 neural-amp-modeler-0.6.0/tests/test_bin/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.6.0/tests/test_bin/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.007316 neural-amp-modeler-0.6.0/tests/test_bin/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.6.0/tests/test_bin/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6583 2023-05-28 20:20:41.000000 neural-amp-modeler-0.6.0/tests/test_bin/test_train/test_main.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_install.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.010116 neural-amp-modeler-0.6.0/tests/test_nam/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)    10062 2023-06-12 04:30:52.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_data.py
+-rw-r--r--   0 steve      (501) staff       (20)      231 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_importable.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.017716 neural-amp-modeler-0.6.0/tests/test_nam/test_models/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      988 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     2754 2023-04-25 01:51:12.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_base.py
+-rw-r--r--   0 steve      (501) staff       (20)     1061 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     4588 2023-04-25 01:51:12.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)     1727 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_losses.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.020831 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/
+-rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     1218 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/test_catnets.py
+-rw-r--r--   0 steve      (501) staff       (20)     2474 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/test_hyper_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     1951 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)      817 2023-05-07 19:58:11.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.023909 neural-amp-modeler-0.6.0/tests/test_nam/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-29 20:17:32.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     4535 2023-05-28 20:20:41.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_train/test_core.py
+-rw-r--r--   0 steve      (501) staff       (20)      773 2023-04-29 20:17:32.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_train/test_version.py
```

### Comparing `neural-amp-modeler-0.5.2/LICENSE` & `neural-amp-modeler-0.6.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Steven Atkinson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Steven Atkinson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `neural-amp-modeler-0.5.2/README.md` & `neural-amp-modeler-0.6.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-# NAM: neural amp modeler
-
-This repository handles training, reamping, and exporting the weights of a model.
-For playing trained models in real time in a standalone application or plugin, see the partner repo,
-[NeuralAmpModelerPlugin](https://github.com/sdatkinson/NeuralAmpModelerPlugin).
-
-## How to use (Google Colab)
-
-If you don't have a good computer for training ML models, you use Google Colab to train
-in the cloud using the pre-made notebooks under `bin\train`.
-
-For the very easiest experience, open 
-[`easy_colab.ipynb` on Google Colab](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/b1aa204/bin/train/easy_colab.ipynb) 
-and follow the steps!
-
-For a little more visibility under the hood, you can use [colab.ipynb](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/main/bin/train/colab.ipynb) instead.
-
-**Pros:**
-
-- No local installation required!
-- Decent GPUs are available if you don't have one on your computer.
-
-**Cons:**
-
-- Uploading your data can take a long time.
-- The session will time out after a few hours (for free accounts), so extended
-  training runs aren't really feasible. Also, there's a usage limit so you can't hang
-  out all day. I've tried to set you up with a good model that should train reasonably
-  quickly!
-
-## How to use (Local)
-
-Alternatively, you can clone this repo to your computer and use it locally.
-
-### Installation
-
-Installation uses [Anaconda](https://www.anaconda.com/) for package management.
-
-For computers with a CUDA-capable GPU (recommended):
-
-```bash
-conda env create -f environment_gpu.yml
-```
-
-Otherwise, for a CPU-only install (will train much more slowly):
-
-```bash
-conda env create -f environment_cpu.yml
-```
-
-Then activate the environment you've created with
-
-```bash
-conda activate nam
-```
-
-### Train models (GUI)
-After installing, you can open a GUI trainer by running
-
-```bash
-nam
-```
-
-from the terminal.
-
-### Train models (Python script)
-For users looking to get more fine-grained control over the modeling process, 
-NAM includes a training script that can be run from the terminal. In order to run it
-#### Download audio files
-Download the [v1_1_1.wav](https://drive.google.com/file/d/1v2xFXeQ9W2Ks05XrqsMCs2viQcKPAwBk/view?usp=share_link) and [overdrive.wav](https://drive.google.com/file/d/14w2utgL16NozmESzAJO_I0_VCt-5Wgpv/view?usp=share_link) to a folder of your choice 
-
-#### Update data configuration 
-Edit `bin/train/data/single_pair.json` to point to relevant audio files 
-```json
-    "common": {
-        "x_path": "C:\\path\\to\\v1_1_1.wav",
-        "y_path": "C:\\path\\to\\overdrive.wav",
-        "delay": 0
-    }
-```
-
-#### Run training script
-Open up a terminal. Activate your nam environment and call the training with
-```bash
-python bin/train/main.py \
-bin/train/inputs/data/single_pair.json \
-bin/train/inputs/models/demonet.json \
-bin/train/inputs/learning/demo.json \
-bin/train/outputs/MyAmp
-```
-
-`data/single_pair.json` contains the information about the data you're training
-on   
-`models/demonet.json` contains information about the model architecture that
-is being trained. The example used here uses a `feather` configured `wavenet`.  
-`learning/demo.json` contains information about the training run itself (e.g. number of epochs).
-
-The configuration above runs a short (demo) training. For a real training you may prefer to run something like,
-
-```bash
-python bin/train/main.py \
-bin/train/inputs/data/single_pair.json \
-bin/train/inputs/models/wavenet.json \
-bin/train/inputs/learning/default.json \
-bin/train/outputs/MyAmp
-```
-
-As a side note, NAM uses [PyTorch Lightning](https://lightning.ai/pages/open-source/) 
-under the hood as a modeling framework, and you can control many of the Pytorch Lightning configuration options from `bin/train/inputs/learning/default.json`
-
-#### Export a model (to use with [the plugin](https://github.com/sdatkinson/NeuralAmpModelerPlugin))
-Exporting the trained model to a `.nam` file for use with the plugin can be done
-with:
-
-```bash
-python bin/export.py \
-path/to/config_model.json \
-path/to/checkpoints/epoch=123_val_loss=0.000010.ckpt \
-path/to/exported_models/MyAmp
-```
-
-Then, point the plugin at the exported `model.nam` file and you're good to go!
-
-### Other utilities
-
-#### Run a model on an input signal ("reamping")
-
-Handy if you want to just check it out without needing to use the plugin:
-
-```bash
-python bin/run.py \
-path/to/source.wav \
-path/to/config_model.json \
-path/to/checkpoints/epoch=123_val_loss=0.000010.ckpt \
-path/to/output.wav
-```
+# NAM: neural amp modeler
+
+This repository handles training, reamping, and exporting the weights of a model.
+For playing trained models in real time in a standalone application or plugin, see the partner repo,
+[NeuralAmpModelerPlugin](https://github.com/sdatkinson/NeuralAmpModelerPlugin).
+
+## How to use (Google Colab)
+
+If you don't have a good computer for training ML models, you use Google Colab to train
+in the cloud using the pre-made notebooks under `bin\train`.
+
+For the very easiest experience, open 
+[`easy_colab.ipynb` on Google Colab](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/f67f17b/bin/train/easy_colab.ipynb) 
+and follow the steps!
+
+For a little more visibility under the hood, you can use [colab.ipynb](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/main/bin/train/colab.ipynb) instead.
+
+**Pros:**
+
+- No local installation required!
+- Decent GPUs are available if you don't have one on your computer.
+
+**Cons:**
+
+- Uploading your data can take a long time.
+- The session will time out after a few hours (for free accounts), so extended
+  training runs aren't really feasible. Also, there's a usage limit so you can't hang
+  out all day. I've tried to set you up with a good model that should train reasonably
+  quickly!
+
+## How to use (Local)
+
+Alternatively, you can clone this repo to your computer and use it locally.
+
+### Installation
+
+Installation uses [Anaconda](https://www.anaconda.com/) for package management.
+
+For computers with a CUDA-capable GPU (recommended):
+
+```bash
+conda env create -f environment_gpu.yml
+```
+
+Otherwise, for a CPU-only install (will train much more slowly):
+
+```bash
+conda env create -f environment_cpu.yml
+```
+
+Then activate the environment you've created with
+
+```bash
+conda activate nam
+```
+
+### Train models (GUI)
+After installing, you can open a GUI trainer by running
+
+```bash
+nam
+```
+
+from the terminal.
+
+### Train models (Python script)
+For users looking to get more fine-grained control over the modeling process, 
+NAM includes a training script that can be run from the terminal. In order to run it
+#### Download audio files
+Download the [v1_1_1.wav](https://drive.google.com/file/d/1v2xFXeQ9W2Ks05XrqsMCs2viQcKPAwBk/view?usp=share_link) and [output.wav](https://drive.google.com/file/d/14w2utgL16NozmESzAJO_I0_VCt-5Wgpv/view?usp=share_link) to a folder of your choice 
+
+#### Update data configuration 
+Edit `bin/train/data/single_pair.json` to point to relevant audio files: 
+```json
+    "common": {
+        "x_path": "C:\\path\\to\\v1_1_1.wav",
+        "y_path": "C:\\path\\to\\output.wav",
+        "delay": 0
+    }
+```
+
+#### Run training script
+Open up a terminal. Activate your nam environment and call the training with
+```bash
+python bin/train/main.py \
+bin/train/inputs/data/single_pair.json \
+bin/train/inputs/models/demonet.json \
+bin/train/inputs/learning/demo.json \
+bin/train/outputs/MyAmp
+```
+
+`data/single_pair.json` contains the information about the data you're training
+on   
+`models/demonet.json` contains information about the model architecture that
+is being trained. The example used here uses a `feather` configured `wavenet`.  
+`learning/demo.json` contains information about the training run itself (e.g. number of epochs).
+
+The configuration above runs a short (demo) training. For a real training you may prefer to run something like,
+
+```bash
+python bin/train/main.py \
+bin/train/inputs/data/single_pair.json \
+bin/train/inputs/models/wavenet.json \
+bin/train/inputs/learning/default.json \
+bin/train/outputs/MyAmp
+```
+
+As a side note, NAM uses [PyTorch Lightning](https://lightning.ai/pages/open-source/) 
+under the hood as a modeling framework, and you can control many of the Pytorch Lightning configuration options from `bin/train/inputs/learning/default.json`
+
+#### Export a model (to use with [the plugin](https://github.com/sdatkinson/NeuralAmpModelerPlugin))
+Exporting the trained model to a `.nam` file for use with the plugin can be done
+with:
+
+```bash
+python bin/export.py \
+path/to/config_model.json \
+path/to/checkpoints/epoch=123_val_loss=0.000010.ckpt \
+path/to/exported_models/MyAmp
+```
+
+Then, point the plugin at the exported `model.nam` file and you're good to go!
+
+### Other utilities
+
+#### Run a model on an input signal ("reamping")
+
+Handy if you want to just check it out without needing to use the plugin:
+
+```bash
+python bin/run.py \
+path/to/source.wav \
+path/to/config_model.json \
+path/to/checkpoints/epoch=123_val_loss=0.000010.ckpt \
+path/to/output.wav
+```
```

### Comparing `neural-amp-modeler-0.5.2/nam/__init__.py` & `neural-amp-modeler-0.6.0/nam/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# File: __init__.py
-# File Created: Tuesday, 2nd February 2021 9:42:50 pm
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-# Hack to recover graceful shutdowns in Windows.
-# This has to happen ASAP
-# See:
-# https://github.com/sdatkinson/neural-amp-modeler/issues/105
-# https://stackoverflow.com/a/44822794
-def _ensure_graceful_shutdowns():
-    import os
-
-    if os.name == "nt":  # OS is Windows
-        os.environ["FOR_DISABLE_CONSOLE_CTRL_HANDLER"] = "1"
-
-
-_ensure_graceful_shutdowns()
-
-from ._version import __version__  # Must be before models or else circular
-
-from . import _core  # noqa F401
-from . import data  # noqa F401
-from . import models  # noqa F401
-from . import util  # noqa F401
-from . import train  # noqa F401
+# File: __init__.py
+# File Created: Tuesday, 2nd February 2021 9:42:50 pm
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+# Hack to recover graceful shutdowns in Windows.
+# This has to happen ASAP
+# See:
+# https://github.com/sdatkinson/neural-amp-modeler/issues/105
+# https://stackoverflow.com/a/44822794
+def _ensure_graceful_shutdowns():
+    import os
+
+    if os.name == "nt":  # OS is Windows
+        os.environ["FOR_DISABLE_CONSOLE_CTRL_HANDLER"] = "1"
+
+
+_ensure_graceful_shutdowns()
+
+from ._version import __version__  # Must be before models or else circular
+
+from . import _core  # noqa F401
+from . import data  # noqa F401
+from . import models  # noqa F401
+from . import util  # noqa F401
+from . import train  # noqa F401
```

### Comparing `neural-amp-modeler-0.5.2/nam/data.py` & `neural-amp-modeler-0.6.0/nam/data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,667 +1,741 @@
-# File: data.py
-# Created Date: Saturday February 5th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-import abc
-from collections import namedtuple
-from copy import deepcopy
-from dataclasses import dataclass
-from enum import Enum
-from pathlib import Path
-from typing import Dict, Optional, Sequence, Tuple, Union
-
-import numpy as np
-import torch
-import wavio
-from scipy.interpolate import interp1d
-from torch.utils.data import Dataset as _Dataset
-from tqdm import tqdm
-
-from ._core import InitializableFromConfig
-
-_REQUIRED_SAMPWIDTH = 3
-REQUIRED_RATE = 48_000
-_REQUIRED_CHANNELS = 1  # Mono
-
-
-class Split(Enum):
-    TRAIN = "train"
-    VALIDATION = "validation"
-
-
-@dataclass
-class WavInfo:
-    sampwidth: int
-    rate: int
-
-
-class AudioShapeMismatchError(ValueError):
-    """
-    Exception where the shape (number of samples, number of channels) of two audio files
-    don't match but were supposed to.
-    """
-
-    def __init__(self, shape_expected, shape_actual, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._shape_expected = shape_expected
-        self._shape_actual = shape_actual
-
-    @property
-    def shape_expected(self):
-        return self._shape_expected
-
-    @property
-    def shape_actual(self):
-        return self._shape_actual
-
-
-def wav_to_np(
-    filename: Union[str, Path],
-    rate: Optional[int] = REQUIRED_RATE,
-    require_match: Optional[Union[str, Path]] = None,
-    required_shape: Optional[Tuple[int]] = None,
-    required_wavinfo: Optional[WavInfo] = None,
-    preroll: Optional[int] = None,
-    info: bool = False,
-) -> Union[np.ndarray, Tuple[np.ndarray, WavInfo]]:
-    """
-    :param preroll: Drop this many samples off the front
-    """
-    x_wav = wavio.read(str(filename))
-    assert x_wav.data.shape[1] == _REQUIRED_CHANNELS, "Mono"
-    assert x_wav.sampwidth == _REQUIRED_SAMPWIDTH, "24-bit"
-    if rate is not None and x_wav.rate != rate:
-        raise RuntimeError(
-            f"Explicitly expected sample rate of {rate}, but found {x_wav.rate} in "
-            f"file {filename}!"
-        )
-
-    if require_match is not None:
-        assert required_shape is None
-        assert required_wavinfo is None
-        y_wav = wavio.read(str(require_match))
-        required_shape = y_wav.data.shape
-        required_wavinfo = WavInfo(y_wav.sampwidth, y_wav.rate)
-    if required_wavinfo is not None:
-        if x_wav.rate != required_wavinfo.rate:
-            raise ValueError(
-                f"Mismatched rates {x_wav.rate} versus {required_wavinfo.rate}"
-            )
-    arr_premono = x_wav.data[preroll:] / (2.0 ** (8 * x_wav.sampwidth - 1))
-    if required_shape is not None:
-        if arr_premono.shape != required_shape:
-            raise AudioShapeMismatchError(
-                arr_premono.shape,
-                required_shape,
-                f"Mismatched shapes. Expected {required_shape}, but this is "
-                f"{arr_premono.shape}!",
-            )
-        # sampwidth fine--we're just casting to 32-bit float anyways
-    arr = arr_premono[:, 0]
-    return arr if not info else (arr, WavInfo(x_wav.sampwidth, x_wav.rate))
-
-
-def wav_to_tensor(
-    *args, info: bool = False, **kwargs
-) -> Union[torch.Tensor, Tuple[torch.Tensor, WavInfo]]:
-    out = wav_to_np(*args, info=info, **kwargs)
-    if info:
-        arr, info = out
-        return torch.Tensor(arr), info
-    else:
-        arr = out
-        return torch.Tensor(arr)
-
-
-def tensor_to_wav(x: torch.Tensor, *args, **kwargs):
-    np_to_wav(x.detach().cpu().numpy(), *args, **kwargs)
-
-
-def np_to_wav(
-    x: np.ndarray,
-    filename: Union[str, Path],
-    rate: int = 48_000,
-    sampwidth: int = 3,
-    scale="none",
-):
-    wavio.write(
-        str(filename),
-        (np.clip(x, -1.0, 1.0) * (2 ** (8 * sampwidth - 1))).astype(np.int32),
-        rate,
-        scale=scale,
-        sampwidth=sampwidth,
-    )
-
-
-class AbstractDataset(_Dataset, abc.ABC):
-    @abc.abstractmethod
-    def __getitem__(
-        self, idx: int
-    ) -> Union[
-        Tuple[torch.Tensor, torch.Tensor],
-        Tuple[torch.Tensor, torch.Tensor, torch.Tensor],
-    ]:
-        """
-        :return:
-            Case 1: Input (N1,), Output (N2,)
-            Case 2: Parameters (D,), Input (N1,), Output (N2,)
-        """
-        pass
-
-
-class _DelayInterpolationMethod(Enum):
-    """
-    :param LINEAR: Linear interpolation
-    :param CUBIC: Cubic spline interpolation
-    """
-
-    # Note: these match scipy.interpolate.interp1d kwarg "kind"
-    LINEAR = "linear"
-    CUBIC = "cubic"
-
-
-def _interpolate_delay(
-    x: torch.Tensor, delay: float, method: _DelayInterpolationMethod
-) -> np.ndarray:
-    """
-    NOTE: This breaks the gradient tape!
-    """
-    if delay == 0.0:
-        return x
-    t_in = np.arange(len(x))
-    n_out = len(x) - int(np.ceil(np.abs(delay)))
-    if delay > 0:
-        t_out = np.arange(n_out) + delay
-    elif delay < 0:
-        t_out = np.arange(len(x) - n_out, len(x)) - np.abs(delay)
-
-    return torch.Tensor(
-        interp1d(t_in, x.detach().cpu().numpy(), kind=method.value)(t_out)
-    )
-
-
-class XYError(ValueError):
-    """
-    Exceptions related to invalid x and y provided for data sets
-    """
-
-    pass
-
-
-class StartStopError(ValueError):
-    """
-    Exceptions related to invalid start and stop arguments
-    """
-
-    pass
-
-
-class StartError(StartStopError):
-    pass
-
-
-class StopError(StartStopError):
-    pass
-
-
-class Dataset(AbstractDataset, InitializableFromConfig):
-    """
-    Take a pair of matched audio files and serve input + output pairs.
-
-    No conditioning parameters associated w/ the data.
-    """
-
-    def __init__(
-        self,
-        x: torch.Tensor,
-        y: torch.Tensor,
-        nx: int,
-        ny: Optional[int],
-        start: Optional[int] = None,
-        stop: Optional[int] = None,
-        delay: Optional[Union[int, float]] = None,
-        delay_interpolation_method: Union[
-            str, _DelayInterpolationMethod
-        ] = _DelayInterpolationMethod.CUBIC,
-        y_scale: float = 1.0,
-        x_path: Optional[Union[str, Path]] = None,
-        y_path: Optional[Union[str, Path]] = None,
-        input_gain: float = 0.0,
-    ):
-        """
-        :param x: The input signal. A 1D array.
-        :param y: The associated output from the model. A 1D array.
-        :param nx: The number of samples required as input for the model. For example,
-            for a ConvNet, this would be the receptive field.
-        :param ny: How many samples to provide as the output array for a single "datum".
-            It's usually more computationally-efficient to provide a larger `ny` than 1
-            so that the forward pass can process more audio all at once. However, this
-            shouldn't be too large or else you won't be able to provide a large batch
-            size (where each input-output pair could be something substantially
-            different and improve batch diversity).
-        :param start: In samples; clip x and y up to this point.
-        :param stop: In samples; clip x and y past this point.
-        :param delay: In samples. Positive means we get rid of the start of x, end of y
-            (i.e. we are correcting for an alignment error in which y is delayed behind
-            x). If a non-integer delay is provided, then y is interpolated, with
-            the extra sample removed.
-        :param y_scale: Multiplies the output signal by a factor (e.g. if the data are
-            too quiet).
-        :param input_gain: In dB. If the input signal wasn't fed to the amp at unity
-            gain, you can indicate the gain here. The data set will multipy the raw
-            audio file by the specified gain so that the true input signal amplitude
-            experienced by the signal chain will be provided as input to the model. If
-            you are using a reamping setup, you can estimate this by reamping a
-            completely dry signal (i.e. connecting the interface output directly back
-            into the input with which the guitar was originally recorded.)
-        """
-        self._validate_x_y(x, y)
-        self._validate_start_stop(x, y, start, stop)
-        if not isinstance(delay_interpolation_method, _DelayInterpolationMethod):
-            delay_interpolation_method = _DelayInterpolationMethod(
-                delay_interpolation_method
-            )
-        x, y = [z[start:stop] for z in (x, y)]
-        if delay is not None and delay != 0:
-            x, y = self._apply_delay(x, y, delay, delay_interpolation_method)
-        x_scale = 10.0 ** (input_gain / 20.0)
-        x = x * x_scale
-        y = y * y_scale
-        self._x_path = x_path
-        self._y_path = y_path
-        self._validate_inputs_after_processing(x, y, nx, ny)
-        self._x = x
-        self._y = y
-        self._nx = nx
-        self._ny = ny if ny is not None else len(x) - nx + 1
-
-    def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor]:
-        """
-        :return:
-            Input (NX+NY-1,)
-            Output (NY,)
-        """
-        if idx >= len(self):
-            raise IndexError(f"Attempted to access datum {idx}, but len is {len(self)}")
-        i = idx * self._ny
-        j = i + self.y_offset
-        return self.x[i : i + self._nx + self._ny - 1], self.y[j : j + self._ny]
-
-    def __len__(self) -> int:
-        n = len(self.x)
-        # If ny were 1
-        single_pairs = n - self._nx + 1
-        return single_pairs // self._ny
-
-    @property
-    def ny(self) -> int:
-        return self._ny
-
-    @property
-    def x(self):
-        return self._x
-
-    @property
-    def y(self):
-        return self._y
-
-    @property
-    def y_offset(self) -> int:
-        return self._nx - 1
-
-    @classmethod
-    def parse_config(cls, config):
-        x, x_wavinfo = wav_to_tensor(config["x_path"], info=True)
-        rate = x_wavinfo.rate
-        try:
-            y = wav_to_tensor(
-                config["y_path"],
-                rate=rate,
-                preroll=config.get("y_preroll"),
-                required_shape=(len(x), 1),
-                required_wavinfo=x_wavinfo,
-            )
-        except AudioShapeMismatchError as e:
-            # Really verbose message since users see this.
-            x_samples, x_channels = e.shape_expected
-            y_samples, y_channels = e.shape_actual
-            msg = "Your audio files aren't the same shape as each other!"
-            if x_channels != y_channels:
-                ctosm = {1: "mono", 2: "stereo"}
-                msg += f"\n * The input is {ctosm[x_channels]}, but the output is {ctosm[y_channels]}!"
-            if x_samples != y_samples:
-
-                def sample_to_time(s, rate):
-                    seconds = s // rate
-                    remainder = s % rate
-                    hours, minutes = 0, 0
-                    seconds_per_hour = 3600
-                    while seconds >= seconds_per_hour:
-                        hours += 1
-                        seconds -= seconds_per_hour
-                    seconds_per_minute = 60
-                    while seconds >= seconds_per_minute:
-                        minutes += 1
-                        seconds -= seconds_per_minute
-                    return (
-                        f"{hours}:{minutes:02d}:{seconds:02d} and {remainder} samples"
-                    )
-
-                msg += f"\n * The input is {sample_to_time(x_samples, rate)} long"
-                msg += f"\n * The output is {sample_to_time(y_samples, rate)} long"
-            raise ValueError(msg)
-        return {
-            "x": x,
-            "y": y,
-            "nx": config["nx"],
-            "ny": config["ny"],
-            "start": config.get("start"),
-            "stop": config.get("stop"),
-            "delay": config.get("delay"),
-            "delay_interpolation_method": config.get(
-                "delay_interpolation_method", _DelayInterpolationMethod.CUBIC.value
-            ),
-            "y_scale": config.get("y_scale", 1.0),
-            "x_path": config["x_path"],
-            "y_path": config["y_path"],
-        }
-
-    @classmethod
-    def _apply_delay(
-        cls,
-        x: torch.Tensor,
-        y: torch.Tensor,
-        delay: Union[int, float],
-        method: _DelayInterpolationMethod,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        # Check for floats that could be treated like ints (simpler algorithm)
-        if isinstance(delay, float) and int(delay) == delay:
-            delay = int(delay)
-        if isinstance(delay, int):
-            return cls._apply_delay_int(x, y, delay)
-        elif isinstance(delay, float):
-            return cls._apply_delay_float(x, y, delay, method)
-
-    @classmethod
-    def _apply_delay_int(
-        cls, x: torch.Tensor, y: torch.Tensor, delay: int
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        if delay > 0:
-            x = x[:-delay]
-            y = y[delay:]
-        elif delay < 0:
-            x = x[-delay:]
-            y = y[:delay]
-        return x, y
-
-    @classmethod
-    def _apply_delay_float(
-        cls,
-        x: torch.Tensor,
-        y: torch.Tensor,
-        delay: float,
-        method: _DelayInterpolationMethod,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        n_out = len(y) - int(np.ceil(np.abs(delay)))
-        if delay > 0:
-            x = x[:n_out]
-        elif delay < 0:
-            x = x[-n_out:]
-        y = _interpolate_delay(y, delay, method)
-        return x, y
-
-    @classmethod
-    def _validate_start_stop(
-        self,
-        x: torch.Tensor,
-        y: torch.Tensor,
-        start: Optional[int] = None,
-        stop: Optional[int] = None,
-    ):
-        """
-        Check for potential input errors.
-
-        These may be valid indices in Python, but probably point to invalid usage, so
-        we will raise an exception if something fishy is going on (e.g. starting after
-        the end of the file, etc)
-        """
-        # We could do this whole thing with `if len(x[start: stop]==0`, but being more
-        # explicit makes the error messages better for users.
-        if start is None and stop is None:
-            return
-        if len(x) != len(y):
-            raise ValueError(
-                f"Input and output are different length. Input has {len(x)} samples, "
-                f"and output has {len(y)}"
-            )
-        n = len(x)
-        if start is not None:
-            # Start after the files' end?
-            if start >= n:
-                raise StartError(
-                    f"Arrays are only {n} samples long, but start was provided as {start}, "
-                    "which is beyond the end of the array!"
-                )
-            # Start before the files' beginning?
-            if start < -n:
-                raise StartError(
-                    f"Arrays are only {n} samples long, but start was provided as {start}, "
-                    "which is before the beginning of the array!"
-                )
-        if stop is not None:
-            # Stop after the files' end?
-            if stop > n:
-                raise StopError(
-                    f"Arrays are only {n} samples long, but stop was provided as {stop}, "
-                    "which is beyond the end of the array!"
-                )
-            # Start before the files' beginning?
-            if stop <= -n:
-                raise StopError(
-                    f"Arrays are only {n} samples long, but stop was provided as {stop}, "
-                    "which is before the beginning of the array!"
-                )
-        # Just in case...
-        if len(x[start:stop]) == 0:
-            raise StartStopError(
-                f"Array length {n} with start={start} and stop={stop} would get "
-                "rid of all of the data!"
-            )
-
-    @classmethod
-    def _validate_x_y(self, x, y):
-        if len(x) != len(y):
-            raise XYError(
-                f"Input and output aren't the same lengths! ({len(x)} vs {len(y)})"
-            )
-        # TODO channels
-        n = len(x)
-        if n == 0:
-            raise XYError("Input and output are empty!")
-
-    def _validate_inputs_after_processing(self, x, y, nx, ny):
-        assert x.ndim == 1
-        assert y.ndim == 1
-        assert len(x) == len(y)
-        if nx > len(x):
-            raise RuntimeError(  # TODO XYError?
-                f"Input of length {len(x)}, but receptive field is {nx}."
-            )
-        if ny is not None:
-            assert ny <= len(y) - nx + 1
-        if torch.abs(y).max() >= 1.0:
-            msg = "Output clipped."
-            if self._y_path is not None:
-                msg += f"Source is {self._y_path}"
-            raise ValueError(msg)
-
-
-class ParametricDataset(Dataset):
-    """
-    Additionally tracks some conditioning parameters
-    """
-
-    def __init__(self, params: Dict[str, Union[bool, float, int]], *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._keys = sorted(tuple(k for k in params.keys()))
-        self._vals = torch.Tensor([float(params[k]) for k in self._keys])
-
-    @classmethod
-    def init_from_config(cls, config):
-        if "slices" not in config:
-            return super().init_from_config(config)
-        else:
-            return cls.init_from_config_with_slices(config)
-
-    @classmethod
-    def init_from_config_with_slices(cls, config):
-        config, x, y, slices = cls.parse_config_with_slices(config)
-        datasets = []
-        for s in tqdm(slices, desc="Slices..."):
-            c = deepcopy(config)
-            start, stop, params = [s[k] for k in ("start", "stop", "params")]
-            c.update(x=x[start:stop], y=y[start:stop], params=params)
-            if "delay" in s:
-                c["delay"] = s["delay"]
-            datasets.append(ParametricDataset(**c))
-        return ConcatDataset(datasets)
-
-    @classmethod
-    def parse_config(cls, config):
-        assert "slices" not in config
-        params = config["params"]
-        return {
-            "params": params,
-            "id": config.get("id"),
-            "common_params": config.get("common_params"),
-            "param_map": config.get("param_map"),
-            **super().parse_config(config),
-        }
-
-    @classmethod
-    def parse_config_with_slices(cls, config):
-        slices = config["slices"]
-        config = super().parse_config(config)
-        x, y = [config.pop(k) for k in "xy"]
-        return config, x, y, slices
-
-    def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        """
-        :return:
-            Parameter values (D,)
-            Input (NX+NY-1,)
-            Output (NY,)
-        """
-        # FIXME don't override signature
-        x, y = super().__getitem__(idx)
-        return self.vals, x, y
-
-    @property
-    def keys(self) -> Tuple[str]:
-        return self._keys
-
-    @property
-    def vals(self):
-        return self._vals
-
-
-class ConcatDataset(AbstractDataset, InitializableFromConfig):
-    def __init__(self, datasets: Sequence[Dataset], flatten=True):
-        if flatten:
-            datasets = self._flatten_datasets(datasets)
-        self._validate_datasets(datasets)
-        self._datasets = datasets
-        self._lookup = self._make_lookup()
-
-    def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor]:
-        i, j = self._lookup[idx]
-        return self.datasets[i][j]
-
-    def __len__(self) -> int:
-        return sum(len(d) for d in self._datasets)
-
-    @property
-    def datasets(self):
-        return self._datasets
-
-    @classmethod
-    def parse_config(cls, config):
-        init = (
-            ParametricDataset.init_from_config
-            if config["parametric"]
-            else Dataset.init_from_config
-        )
-        return {
-            "datasets": tuple(
-                init(c) for c in tqdm(config["dataset_configs"], desc="Loading data")
-            )
-        }
-
-    def _flatten_datasets(self, datasets):
-        """
-        If any dataset is a ConcatDataset, pull it out
-        """
-        flattened = []
-        for d in datasets:
-            if isinstance(d, ConcatDataset):
-                flattened.extend(d.datasets)
-            else:
-                flattened.append(d)
-        return flattened
-
-    def _make_lookup(self):
-        """
-        For faster __getitem__
-        """
-        lookup = {}
-        offset = 0
-        j = 0  # Dataset index
-        for i in range(len(self)):
-            if offset == len(self.datasets[j]):
-                offset -= len(self.datasets[j])
-                j += 1
-            lookup[i] = (j, offset)
-            offset += 1
-        assert j == len(self.datasets) - 1
-        assert offset == len(self.datasets[-1])
-        return lookup
-
-    @classmethod
-    def _validate_datasets(cls, datasets: Sequence[Dataset]):
-        Reference = namedtuple("Reference", ("index", "val"))
-        ref_keys, ref_ny = None, None
-        for i, d in enumerate(datasets):
-            ref_ny = Reference(i, d.ny) if ref_ny is None else ref_ny
-            if d.ny != ref_ny.val:
-                raise ValueError(
-                    f"Mismatch between ny of datasets {ref_ny.index} ({ref_ny.val}) and {i} ({d.ny})"
-                )
-            if isinstance(d, ParametricDataset):
-                val = d.keys
-                if ref_keys is None:
-                    ref_keys = Reference(i, val)
-                if val != ref_keys.val:
-                    raise ValueError(
-                        f"Mismatch between keys of datasets {ref_keys.index} "
-                        f"({ref_keys.val}) and {i} ({val})"
-                    )
-
-
-def init_dataset(config, split: Split) -> AbstractDataset:
-    parametric = config.get("parametric", False)
-    base_config = config[split.value]
-    common = config.get("common", {})
-    if isinstance(base_config, dict):
-        init = (
-            ParametricDataset.init_from_config
-            if parametric
-            else Dataset.init_from_config
-        )
-        return init({**common, **base_config})
-    elif isinstance(base_config, list):
-        return ConcatDataset.init_from_config(
-            {
-                "parametric": parametric,
-                "dataset_configs": [{**common, **c} for c in base_config],
-            }
-        )
+# File: data.py
+# Created Date: Saturday February 5th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+import abc
+from collections import namedtuple
+from copy import deepcopy
+from dataclasses import dataclass
+from enum import Enum
+from pathlib import Path
+from typing import Dict, Optional, Sequence, Tuple, Union
+
+import numpy as np
+import torch
+import wavio
+from scipy.interpolate import interp1d
+from torch.utils.data import Dataset as _Dataset
+from tqdm import tqdm
+
+from ._core import InitializableFromConfig
+
+_REQUIRED_SAMPWIDTH = 3
+REQUIRED_RATE = 48_000
+_REQUIRED_CHANNELS = 1  # Mono
+
+
+class Split(Enum):
+    TRAIN = "train"
+    VALIDATION = "validation"
+
+
+@dataclass
+class WavInfo:
+    sampwidth: int
+    rate: int
+
+
+class AudioShapeMismatchError(ValueError):
+    """
+    Exception where the shape (number of samples, number of channels) of two audio files
+    don't match but were supposed to.
+    """
+
+    def __init__(self, shape_expected, shape_actual, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._shape_expected = shape_expected
+        self._shape_actual = shape_actual
+
+    @property
+    def shape_expected(self):
+        return self._shape_expected
+
+    @property
+    def shape_actual(self):
+        return self._shape_actual
+
+
+def wav_to_np(
+    filename: Union[str, Path],
+    rate: Optional[int] = REQUIRED_RATE,
+    require_match: Optional[Union[str, Path]] = None,
+    required_shape: Optional[Tuple[int]] = None,
+    required_wavinfo: Optional[WavInfo] = None,
+    preroll: Optional[int] = None,
+    info: bool = False,
+) -> Union[np.ndarray, Tuple[np.ndarray, WavInfo]]:
+    """
+    :param preroll: Drop this many samples off the front
+    """
+    x_wav = wavio.read(str(filename))
+    assert x_wav.data.shape[1] == _REQUIRED_CHANNELS, "Mono"
+    assert x_wav.sampwidth == _REQUIRED_SAMPWIDTH, "24-bit"
+    if rate is not None and x_wav.rate != rate:
+        raise RuntimeError(
+            f"Explicitly expected sample rate of {rate}, but found {x_wav.rate} in "
+            f"file {filename}!"
+        )
+
+    if require_match is not None:
+        assert required_shape is None
+        assert required_wavinfo is None
+        y_wav = wavio.read(str(require_match))
+        required_shape = y_wav.data.shape
+        required_wavinfo = WavInfo(y_wav.sampwidth, y_wav.rate)
+    if required_wavinfo is not None:
+        if x_wav.rate != required_wavinfo.rate:
+            raise ValueError(
+                f"Mismatched rates {x_wav.rate} versus {required_wavinfo.rate}"
+            )
+    arr_premono = x_wav.data[preroll:] / (2.0 ** (8 * x_wav.sampwidth - 1))
+    if required_shape is not None:
+        if arr_premono.shape != required_shape:
+            raise AudioShapeMismatchError(
+                required_shape,  # Expected
+                arr_premono.shape,  # Actual
+                f"Mismatched shapes. Expected {required_shape}, but this is "
+                f"{arr_premono.shape}!"
+            )
+        # sampwidth fine--we're just casting to 32-bit float anyways
+    arr = arr_premono[:, 0]
+    return arr if not info else (arr, WavInfo(x_wav.sampwidth, x_wav.rate))
+
+
+def wav_to_tensor(
+    *args, info: bool = False, **kwargs
+) -> Union[torch.Tensor, Tuple[torch.Tensor, WavInfo]]:
+    out = wav_to_np(*args, info=info, **kwargs)
+    if info:
+        arr, info = out
+        return torch.Tensor(arr), info
+    else:
+        arr = out
+        return torch.Tensor(arr)
+
+
+def tensor_to_wav(x: torch.Tensor, *args, **kwargs):
+    np_to_wav(x.detach().cpu().numpy(), *args, **kwargs)
+
+
+def np_to_wav(
+    x: np.ndarray,
+    filename: Union[str, Path],
+    rate: int = 48_000,
+    sampwidth: int = 3,
+    scale = None,
+    **kwargs
+):
+    if wavio.__version__ <= "0.0.4" and scale is None:
+        scale = "none"
+    wavio.write(
+        str(filename),
+        (np.clip(x, -1.0, 1.0) * (2 ** (8 * sampwidth - 1))).astype(np.int32),
+        rate,
+        scale=scale,
+        sampwidth=sampwidth,
+        **kwargs
+    )
+
+
+class AbstractDataset(_Dataset, abc.ABC):
+    @abc.abstractmethod
+    def __getitem__(
+        self, idx: int
+    ) -> Union[
+        Tuple[torch.Tensor, torch.Tensor],
+        Tuple[torch.Tensor, torch.Tensor, torch.Tensor],
+    ]:
+        """
+        :return:
+            Case 1: Input (N1,), Output (N2,)
+            Case 2: Parameters (D,), Input (N1,), Output (N2,)
+        """
+        pass
+
+
+class _DelayInterpolationMethod(Enum):
+    """
+    :param LINEAR: Linear interpolation
+    :param CUBIC: Cubic spline interpolation
+    """
+
+    # Note: these match scipy.interpolate.interp1d kwarg "kind"
+    LINEAR = "linear"
+    CUBIC = "cubic"
+
+
+def _interpolate_delay(
+    x: torch.Tensor, delay: float, method: _DelayInterpolationMethod
+) -> np.ndarray:
+    """
+    NOTE: This breaks the gradient tape!
+    """
+    if delay == 0.0:
+        return x
+    t_in = np.arange(len(x))
+    n_out = len(x) - int(np.ceil(np.abs(delay)))
+    if delay > 0:
+        t_out = np.arange(n_out) + delay
+    elif delay < 0:
+        t_out = np.arange(len(x) - n_out, len(x)) - np.abs(delay)
+
+    return torch.Tensor(
+        interp1d(t_in, x.detach().cpu().numpy(), kind=method.value)(t_out)
+    )
+
+
+class XYError(ValueError):
+    """
+    Exceptions related to invalid x and y provided for data sets
+    """
+
+    pass
+
+
+class StartStopError(ValueError):
+    """
+    Exceptions related to invalid start and stop arguments
+    """
+
+    pass
+
+
+class StartError(StartStopError):
+    pass
+
+
+class StopError(StartStopError):
+    pass
+
+
+# In seconds. Can't be 0.5 or else v1.wav is invalid! Oops!
+_DEFAULT_REQUIRE_INPUT_PRE_SILENCE = 0.4
+
+
+class Dataset(AbstractDataset, InitializableFromConfig):
+    """
+    Take a pair of matched audio files and serve input + output pairs.
+
+    No conditioning parameters associated w/ the data.
+    """
+
+    def __init__(
+        self,
+        x: torch.Tensor,
+        y: torch.Tensor,
+        nx: int,
+        ny: Optional[int],
+        start: Optional[int] = None,
+        stop: Optional[int] = None,
+        delay: Optional[Union[int, float]] = None,
+        delay_interpolation_method: Union[
+            str, _DelayInterpolationMethod
+        ] = _DelayInterpolationMethod.CUBIC,
+        y_scale: float = 1.0,
+        x_path: Optional[Union[str, Path]] = None,
+        y_path: Optional[Union[str, Path]] = None,
+        input_gain: float = 0.0,
+        rate: int = REQUIRED_RATE,
+        require_input_pre_silence: Optional[float] = _DEFAULT_REQUIRE_INPUT_PRE_SILENCE,
+    ):
+        """
+        :param x: The input signal. A 1D array.
+        :param y: The associated output from the model. A 1D array.
+        :param nx: The number of samples required as input for the model. For example,
+            for a ConvNet, this would be the receptive field.
+        :param ny: How many samples to provide as the output array for a single "datum".
+            It's usually more computationally-efficient to provide a larger `ny` than 1
+            so that the forward pass can process more audio all at once. However, this
+            shouldn't be too large or else you won't be able to provide a large batch
+            size (where each input-output pair could be something substantially
+            different and improve batch diversity).
+        :param start: In samples; clip x and y up to this point.
+        :param stop: In samples; clip x and y past this point.
+        :param delay: In samples. Positive means we get rid of the start of x, end of y
+            (i.e. we are correcting for an alignment error in which y is delayed behind
+            x). If a non-integer delay is provided, then y is interpolated, with
+            the extra sample removed.
+        :param y_scale: Multiplies the output signal by a factor (e.g. if the data are
+            too quiet).
+        :param input_gain: In dB. If the input signal wasn't fed to the amp at unity
+            gain, you can indicate the gain here. The data set will multipy the raw
+            audio file by the specified gain so that the true input signal amplitude
+            experienced by the signal chain will be provided as input to the model. If
+            you are using a reamping setup, you can estimate this by reamping a
+            completely dry signal (i.e. connecting the interface output directly back
+            into the input with which the guitar was originally recorded.)
+        :param rate: Sample rate for the data
+        :param require_input_pre_silence: If provided, require that this much time (in
+            seconds) preceding the start of the data set (`start`) have a silent input.
+            If it's not, then raise an exception because the output due to it will leak
+            into the data set that we're trying to use. If `None`, don't assert.
+        """
+        self._validate_x_y(x, y)
+        self._validate_start_stop(x, y, start, stop)
+        if not isinstance(delay_interpolation_method, _DelayInterpolationMethod):
+            delay_interpolation_method = _DelayInterpolationMethod(
+                delay_interpolation_method
+            )
+        if require_input_pre_silence is not None:
+            self._validate_preceding_silence(
+                x, start, int(require_input_pre_silence * rate)
+            )
+        x, y = [z[start:stop] for z in (x, y)]
+        if delay is not None and delay != 0:
+            x, y = self._apply_delay(x, y, delay, delay_interpolation_method)
+        x_scale = 10.0 ** (input_gain / 20.0)
+        x = x * x_scale
+        y = y * y_scale
+        self._x_path = x_path
+        self._y_path = y_path
+        self._validate_inputs_after_processing(x, y, nx, ny)
+        self._x = x
+        self._y = y
+        self._nx = nx
+        self._ny = ny if ny is not None else len(x) - nx + 1
+        self._rate = rate
+
+    def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        :return:
+            Input (NX+NY-1,)
+            Output (NY,)
+        """
+        if idx >= len(self):
+            raise IndexError(f"Attempted to access datum {idx}, but len is {len(self)}")
+        i = idx * self._ny
+        j = i + self.y_offset
+        return self.x[i : i + self._nx + self._ny - 1], self.y[j : j + self._ny]
+
+    def __len__(self) -> int:
+        n = len(self.x)
+        # If ny were 1
+        single_pairs = n - self._nx + 1
+        return single_pairs // self._ny
+
+    @property
+    def ny(self) -> int:
+        return self._ny
+
+    @property
+    def x(self) -> torch.Tensor:
+        """
+        The input audio data
+
+        :return: (N,)
+        """
+        return self._x
+
+    @property
+    def y(self) -> torch.Tensor:
+        """
+        The output audio data
+
+        :return: (N,)
+        """
+        return self._y
+
+    @property
+    def y_offset(self) -> int:
+        return self._nx - 1
+
+    @classmethod
+    def parse_config(cls, config):
+        x, x_wavinfo = wav_to_tensor(config["x_path"], info=True)
+        rate = x_wavinfo.rate
+        try:
+            y = wav_to_tensor(
+                config["y_path"],
+                rate=rate,
+                preroll=config.get("y_preroll"),
+                required_shape=(len(x), 1),
+                required_wavinfo=x_wavinfo,
+            )
+        except AudioShapeMismatchError as e:
+            # Really verbose message since users see this.
+            x_samples, x_channels = e.shape_expected
+            y_samples, y_channels = e.shape_actual
+            msg = "Your audio files aren't the same shape as each other!"
+            if x_channels != y_channels:
+                ctosm = {1: "mono", 2: "stereo"}
+                msg += f"\n * The input is {ctosm[x_channels]}, but the output is {ctosm[y_channels]}!"
+            if x_samples != y_samples:
+
+                def sample_to_time(s, rate):
+                    seconds = s // rate
+                    remainder = s % rate
+                    hours, minutes = 0, 0
+                    seconds_per_hour = 3600
+                    while seconds >= seconds_per_hour:
+                        hours += 1
+                        seconds -= seconds_per_hour
+                    seconds_per_minute = 60
+                    while seconds >= seconds_per_minute:
+                        minutes += 1
+                        seconds -= seconds_per_minute
+                    return (
+                        f"{hours}:{minutes:02d}:{seconds:02d} and {remainder} samples"
+                    )
+
+                msg += f"\n * The input is {sample_to_time(x_samples, rate)} long"
+                msg += f"\n * The output is {sample_to_time(y_samples, rate)} long"
+            raise ValueError(msg)
+        return {
+            "x": x,
+            "y": y,
+            "nx": config["nx"],
+            "ny": config["ny"],
+            "start": config.get("start"),
+            "stop": config.get("stop"),
+            "delay": config.get("delay"),
+            "delay_interpolation_method": config.get(
+                "delay_interpolation_method", _DelayInterpolationMethod.CUBIC.value
+            ),
+            "y_scale": config.get("y_scale", 1.0),
+            "x_path": config["x_path"],
+            "y_path": config["y_path"],
+            "rate": config.get("rate", REQUIRED_RATE),
+            "require_input_pre_silence": config.get(
+                "require_input_pre_silence", _DEFAULT_REQUIRE_INPUT_PRE_SILENCE
+            ),
+        }
+
+    @classmethod
+    def _apply_delay(
+        cls,
+        x: torch.Tensor,
+        y: torch.Tensor,
+        delay: Union[int, float],
+        method: _DelayInterpolationMethod,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        # Check for floats that could be treated like ints (simpler algorithm)
+        if isinstance(delay, float) and int(delay) == delay:
+            delay = int(delay)
+        if isinstance(delay, int):
+            return cls._apply_delay_int(x, y, delay)
+        elif isinstance(delay, float):
+            return cls._apply_delay_float(x, y, delay, method)
+
+    @classmethod
+    def _apply_delay_int(
+        cls, x: torch.Tensor, y: torch.Tensor, delay: int
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        if delay > 0:
+            x = x[:-delay]
+            y = y[delay:]
+        elif delay < 0:
+            x = x[-delay:]
+            y = y[:delay]
+        return x, y
+
+    @classmethod
+    def _apply_delay_float(
+        cls,
+        x: torch.Tensor,
+        y: torch.Tensor,
+        delay: float,
+        method: _DelayInterpolationMethod,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        n_out = len(y) - int(np.ceil(np.abs(delay)))
+        if delay > 0:
+            x = x[:n_out]
+        elif delay < 0:
+            x = x[-n_out:]
+        y = _interpolate_delay(y, delay, method)
+        return x, y
+
+    @classmethod
+    def _validate_start_stop(
+        self,
+        x: torch.Tensor,
+        y: torch.Tensor,
+        start: Optional[int] = None,
+        stop: Optional[int] = None,
+    ):
+        """
+        Check for potential input errors.
+
+        These may be valid indices in Python, but probably point to invalid usage, so
+        we will raise an exception if something fishy is going on (e.g. starting after
+        the end of the file, etc)
+        """
+        # We could do this whole thing with `if len(x[start: stop]==0`, but being more
+        # explicit makes the error messages better for users.
+        if start is None and stop is None:
+            return
+        if len(x) != len(y):
+            raise ValueError(
+                f"Input and output are different length. Input has {len(x)} samples, "
+                f"and output has {len(y)}"
+            )
+        n = len(x)
+        if start is not None:
+            # Start after the files' end?
+            if start >= n:
+                raise StartError(
+                    f"Arrays are only {n} samples long, but start was provided as {start}, "
+                    "which is beyond the end of the array!"
+                )
+            # Start before the files' beginning?
+            if start < -n:
+                raise StartError(
+                    f"Arrays are only {n} samples long, but start was provided as {start}, "
+                    "which is before the beginning of the array!"
+                )
+        if stop is not None:
+            # Stop after the files' end?
+            if stop > n:
+                raise StopError(
+                    f"Arrays are only {n} samples long, but stop was provided as {stop}, "
+                    "which is beyond the end of the array!"
+                )
+            # Start before the files' beginning?
+            if stop <= -n:
+                raise StopError(
+                    f"Arrays are only {n} samples long, but stop was provided as {stop}, "
+                    "which is before the beginning of the array!"
+                )
+        # Just in case...
+        if len(x[start:stop]) == 0:
+            raise StartStopError(
+                f"Array length {n} with start={start} and stop={stop} would get "
+                "rid of all of the data!"
+            )
+
+    @classmethod
+    def _validate_x_y(self, x, y):
+        if len(x) != len(y):
+            raise XYError(
+                f"Input and output aren't the same lengths! ({len(x)} vs {len(y)})"
+            )
+        # TODO channels
+        n = len(x)
+        if n == 0:
+            raise XYError("Input and output are empty!")
+
+    def _validate_inputs_after_processing(self, x, y, nx, ny):
+        assert x.ndim == 1
+        assert y.ndim == 1
+        assert len(x) == len(y)
+        if nx > len(x):
+            raise RuntimeError(  # TODO XYError?
+                f"Input of length {len(x)}, but receptive field is {nx}."
+            )
+        if ny is not None:
+            assert ny <= len(y) - nx + 1
+        if torch.abs(y).max() >= 1.0:
+            msg = "Output clipped."
+            if self._y_path is not None:
+                msg += f"Source is {self._y_path}"
+            raise ValueError(msg)
+
+    @classmethod
+    def _validate_preceding_silence(
+        cls, x: torch.Tensor, start: Optional[int], silent_samples: int
+    ):
+        """
+        Make sure that the input is silent before the starting index.
+        If it's not, then the output from that non-silent input will leak into the data
+        set and couldn't be predicted!
+
+        See: Issue #252
+
+        :param x: Input
+        :param start: Where the data starts
+        :param silent_samples: How many are expected to be silent
+        """
+        if start is None:
+            return
+        raw_check_start = start - silent_samples
+        check_start = max(raw_check_start, 0) if start >= 0 else min(raw_check_start, 0)
+        check_end = start
+        if not torch.all(x[check_start:check_end] == 0.0):
+            raise XYError(
+                f"Input provided isn't silent for at least {silent_samples} samples "
+                "before the starting index. Responses to this non-silent input may "
+                "leak into the dataset!"
+            )
+
+
+class ParametricDataset(Dataset):
+    """
+    Additionally tracks some conditioning parameters
+    """
+
+    def __init__(self, params: Dict[str, Union[bool, float, int]], *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._keys = sorted(tuple(k for k in params.keys()))
+        self._vals = torch.Tensor([float(params[k]) for k in self._keys])
+
+    @classmethod
+    def init_from_config(cls, config):
+        if "slices" not in config:
+            return super().init_from_config(config)
+        else:
+            return cls.init_from_config_with_slices(config)
+
+    @classmethod
+    def init_from_config_with_slices(cls, config):
+        config, x, y, slices = cls.parse_config_with_slices(config)
+        datasets = []
+        for s in tqdm(slices, desc="Slices..."):
+            c = deepcopy(config)
+            start, stop, params = [s[k] for k in ("start", "stop", "params")]
+            c.update(x=x[start:stop], y=y[start:stop], params=params)
+            if "delay" in s:
+                c["delay"] = s["delay"]
+            datasets.append(ParametricDataset(**c))
+        return ConcatDataset(datasets)
+
+    @classmethod
+    def parse_config(cls, config):
+        assert "slices" not in config
+        params = config["params"]
+        return {
+            "params": params,
+            "id": config.get("id"),
+            "common_params": config.get("common_params"),
+            "param_map": config.get("param_map"),
+            **super().parse_config(config),
+        }
+
+    @classmethod
+    def parse_config_with_slices(cls, config):
+        slices = config["slices"]
+        config = super().parse_config(config)
+        x, y = [config.pop(k) for k in "xy"]
+        return config, x, y, slices
+
+    def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        """
+        :return:
+            Parameter values (D,)
+            Input (NX+NY-1,)
+            Output (NY,)
+        """
+        # FIXME don't override signature
+        x, y = super().__getitem__(idx)
+        return self.vals, x, y
+
+    @property
+    def keys(self) -> Tuple[str]:
+        return self._keys
+
+    @property
+    def vals(self):
+        return self._vals
+
+
+class ConcatDataset(AbstractDataset, InitializableFromConfig):
+    def __init__(self, datasets: Sequence[Dataset], flatten=True):
+        if flatten:
+            datasets = self._flatten_datasets(datasets)
+        self._validate_datasets(datasets)
+        self._datasets = datasets
+        self._lookup = self._make_lookup()
+
+    def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor]:
+        i, j = self._lookup[idx]
+        return self.datasets[i][j]
+
+    def __len__(self) -> int:
+        """
+        How many data sets are in this data set
+        """
+        return sum(len(d) for d in self._datasets)
+
+    @property
+    def datasets(self):
+        return self._datasets
+
+    @classmethod
+    def parse_config(cls, config):
+        init = (
+            ParametricDataset.init_from_config
+            if config["parametric"]
+            else Dataset.init_from_config
+        )
+        return {
+            "datasets": tuple(
+                init(c) for c in tqdm(config["dataset_configs"], desc="Loading data")
+            )
+        }
+
+    def _flatten_datasets(self, datasets):
+        """
+        If any dataset is a ConcatDataset, pull it out
+        """
+        flattened = []
+        for d in datasets:
+            if isinstance(d, ConcatDataset):
+                flattened.extend(d.datasets)
+            else:
+                flattened.append(d)
+        return flattened
+
+    def _make_lookup(self):
+        """
+        For faster __getitem__
+        """
+        lookup = {}
+        offset = 0
+        j = 0  # Dataset index
+        for i in range(len(self)):
+            if offset == len(self.datasets[j]):
+                offset -= len(self.datasets[j])
+                j += 1
+            lookup[i] = (j, offset)
+            offset += 1
+        # Assert that we got to the last data set
+        if j != len(self.datasets) - 1:
+            raise RuntimeError(
+                f"During lookup population, didn't get to the last dataset (index "
+                f"{len(self.datasets)-1}). Instead index ended at {j}."
+            )
+        if offset != len(self.datasets[-1]):
+            raise RuntimeError(
+                "During lookup population, didn't end at the index of the last datum "
+                f"in the last dataset. Expected index {len(self.datasets[-1])}, got "
+                f"{offset} instead."
+            )
+        return lookup
+
+    @classmethod
+    def _validate_datasets(cls, datasets: Sequence[Dataset]):
+        Reference = namedtuple("Reference", ("index", "val"))
+        ref_keys, ref_ny = None, None
+        for i, d in enumerate(datasets):
+            ref_ny = Reference(i, d.ny) if ref_ny is None else ref_ny
+            if d.ny != ref_ny.val:
+                raise ValueError(
+                    f"Mismatch between ny of datasets {ref_ny.index} ({ref_ny.val}) and {i} ({d.ny})"
+                )
+            if isinstance(d, ParametricDataset):
+                val = d.keys
+                if ref_keys is None:
+                    ref_keys = Reference(i, val)
+                if val != ref_keys.val:
+                    raise ValueError(
+                        f"Mismatch between keys of datasets {ref_keys.index} "
+                        f"({ref_keys.val}) and {i} ({val})"
+                    )
+
+
+def init_dataset(config, split: Split) -> AbstractDataset:
+    parametric = config.get("parametric", False)
+    base_config = config[split.value]
+    common = config.get("common", {})
+    if isinstance(base_config, dict):
+        init = (
+            ParametricDataset.init_from_config
+            if parametric
+            else Dataset.init_from_config
+        )
+        return init({**common, **base_config})
+    elif isinstance(base_config, list):
+        return ConcatDataset.init_from_config(
+            {
+                "parametric": parametric,
+                "dataset_configs": [{**common, **c} for c in base_config],
+            }
+        )
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/_base.py` & `neural-amp-modeler-0.6.0/nam/models/_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-# File: _base.py
-# Created Date: Tuesday February 8th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-The foundation of the model without the PyTorch Lightning attributes (losses, training 
-steps)
-"""
-
-import abc
-import math
-import pkg_resources
-from typing import Any, Dict, Optional, Tuple, Union
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-from .._core import InitializableFromConfig
-from ..data import REQUIRED_RATE, wav_to_tensor
-from ._exportable import Exportable
-
-
-class _Base(nn.Module, InitializableFromConfig, Exportable):
-    @abc.abstractproperty
-    def pad_start_default(self) -> bool:
-        pass
-
-    @abc.abstractproperty
-    def receptive_field(self) -> int:
-        """
-        Receptive field of the model
-        """
-        pass
-
-    @abc.abstractmethod
-    def forward(self, *args, **kwargs) -> torch.Tensor:
-        pass
-
-    def _metadata_loudness(self, gain: float = 1.0, db: bool = True) -> float:
-        """
-        How loud is this model when given a standardized input?
-        In dB
-
-        :param gain: Multiplies input signal
-        """
-        x = wav_to_tensor(
-            pkg_resources.resource_filename(
-                "nam", "models/_resources/loudness_input.wav"
-            )
-        )
-        y = self._at_nominal_settings(gain * x)
-        loudness = torch.sqrt(torch.mean(torch.square(y)))
-        if db:
-            loudness = 20.0 * torch.log10(loudness)
-        return loudness.item()
-
-    def _metadata_gain(self) -> float:
-        """
-        Between 0 and 1, how much gain / compression does the model seem to have?
-        """
-        x = np.linspace(0.0, 1.0, 11)
-        y = np.array([self._metadata_loudness(gain=gain, db=False) for gain in x])
-        #
-        # O ^ o o o o o o
-        # u | o       x   +-------------------------------------+
-        # t | o     x     | x: Minimum gain (no compression)    |
-        # p | o   x       | o: Max gain     (100% compression)  |
-        # u | o x         +-------------------------------------+
-        # t | o
-        #   +------------->
-        #       Input
-        #
-        max_gain = y[-1] * len(x)  # "Square"
-        min_gain = 0.5 * max_gain  # "Triangle"
-        gain_range = max_gain - min_gain
-        this_gain = y.sum()
-        normalized_gain = (this_gain - min_gain) / gain_range
-        return np.clip(normalized_gain, 0.0, 1.0)
-
-    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
-        # parametric?...
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def _forward(self, *args) -> torch.Tensor:
-        """
-        The true forward method.
-
-        :param x: (N,L1)
-        :return: (N,L1-RF+1)
-        """
-        pass
-
-    def _export_input_output_args(self) -> Tuple[Any]:
-        """
-        Create any other args necessesary (e.g. params to eval at)
-        """
-        return ()
-
-    def _export_input_output(self) -> Tuple[np.ndarray, np.ndarray]:
-        args = self._export_input_output_args()
-        rate = REQUIRED_RATE
-        x = torch.cat(
-            [
-                torch.zeros((rate,)),
-                0.5
-                * torch.sin(
-                    2.0 * math.pi * 220.0 * torch.linspace(0.0, 1.0, rate + 1)[:-1]
-                ),
-                torch.zeros((rate,)),
-            ]
-        )
-        # Use pad start to ensure same length as requested by ._export_input_output()
-        return (
-            x.detach().cpu().numpy(),
-            self(*args, x, pad_start=True).detach().cpu().numpy(),
-        )
-
-
-class BaseNet(_Base):
-    def forward(self, x: torch.Tensor, pad_start: Optional[bool] = None):
-        pad_start = self.pad_start_default if pad_start is None else pad_start
-        scalar = x.ndim == 1
-        if scalar:
-            x = x[None]
-        if pad_start:
-            x = torch.cat((torch.zeros((len(x), self.receptive_field - 1)), x), dim=1)
-        y = self._forward(x)
-        if scalar:
-            y = y[0]
-        return y
-
-    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
-        return self(x)
-
-    @abc.abstractmethod
-    def _forward(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        The true forward method.
-
-        :param x: (N,L1)
-        :return: (N,L1-RF+1)
-        """
-        pass
-
-    def _get_non_user_metadata(self) -> Dict[str, Union[str, int, float]]:
-        d = super()._get_non_user_metadata()
-        d["loudness"] = self._metadata_loudness()
-        d["gain"] = self._metadata_gain()
-        return d
-
-
-class ParametricBaseNet(_Base):
-    """
-    Parametric inputs
-    """
-
-    def forward(
-        self, params: torch.Tensor, x: torch.Tensor, pad_start: Optional[bool] = None
-    ):
-        pad_start = self.pad_start_default if pad_start is None else pad_start
-        scalar = x.ndim == 1
-        if scalar:
-            x = x[None]
-            params = params[None]
-        if pad_start:
-            x = torch.cat((torch.zeros((len(x), self.receptive_field - 1)), x), dim=1)
-        y = self._forward(params, x)
-        if scalar:
-            y = y[0]
-        return y
-
-    @abc.abstractmethod
-    def _forward(self, params: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
-        """
-        The true forward method.
-
-        :param params: (N,D)
-        :param x: (N,L1)
-        :return: (N,L1-RF+1)
-        """
-        pass
+# File: _base.py
+# Created Date: Tuesday February 8th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+The foundation of the model without the PyTorch Lightning attributes (losses, training
+steps)
+"""
+
+import abc
+import math
+import pkg_resources
+from typing import Any, Dict, Optional, Tuple, Union
+
+import numpy as np
+import torch
+import torch.nn as nn
+
+from .._core import InitializableFromConfig
+from ..data import REQUIRED_RATE, wav_to_tensor
+from ._exportable import Exportable
+
+
+class _Base(nn.Module, InitializableFromConfig, Exportable):
+    @abc.abstractproperty
+    def pad_start_default(self) -> bool:
+        pass
+
+    @abc.abstractproperty
+    def receptive_field(self) -> int:
+        """
+        Receptive field of the model
+        """
+        pass
+
+    @abc.abstractmethod
+    def forward(self, *args, **kwargs) -> torch.Tensor:
+        pass
+
+    def _metadata_loudness(self, gain: float = 1.0, db: bool = True) -> float:
+        """
+        How loud is this model when given a standardized input?
+        In dB
+
+        :param gain: Multiplies input signal
+        """
+        x = wav_to_tensor(
+            pkg_resources.resource_filename(
+                "nam", "models/_resources/loudness_input.wav"
+            )
+        )
+        y = self._at_nominal_settings(gain * x)
+        loudness = torch.sqrt(torch.mean(torch.square(y)))
+        if db:
+            loudness = 20.0 * torch.log10(loudness)
+        return loudness.item()
+
+    def _metadata_gain(self) -> float:
+        """
+        Between 0 and 1, how much gain / compression does the model seem to have?
+        """
+        x = np.linspace(0.0, 1.0, 11)
+        y = np.array([self._metadata_loudness(gain=gain, db=False) for gain in x])
+        #
+        # O ^ o o o o o o
+        # u | o       x   +-------------------------------------+
+        # t | o     x     | x: Minimum gain (no compression)    |
+        # p | o   x       | o: Max gain     (100% compression)  |
+        # u | o x         +-------------------------------------+
+        # t | o
+        #   +------------->
+        #       Input
+        #
+        max_gain = y[-1] * len(x)  # "Square"
+        min_gain = 0.5 * max_gain  # "Triangle"
+        gain_range = max_gain - min_gain
+        this_gain = y.sum()
+        normalized_gain = (this_gain - min_gain) / gain_range
+        return np.clip(normalized_gain, 0.0, 1.0)
+
+    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
+        # parametric?...
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def _forward(self, *args) -> torch.Tensor:
+        """
+        The true forward method.
+
+        :param x: (N,L1)
+        :return: (N,L1-RF+1)
+        """
+        pass
+
+    def _export_input_output_args(self) -> Tuple[Any]:
+        """
+        Create any other args necessesary (e.g. params to eval at)
+        """
+        return ()
+
+    def _export_input_output(self) -> Tuple[np.ndarray, np.ndarray]:
+        args = self._export_input_output_args()
+        rate = REQUIRED_RATE
+        x = torch.cat(
+            [
+                torch.zeros((rate,)),
+                0.5
+                * torch.sin(
+                    2.0 * math.pi * 220.0 * torch.linspace(0.0, 1.0, rate + 1)[:-1]
+                ),
+                torch.zeros((rate,)),
+            ]
+        )
+        # Use pad start to ensure same length as requested by ._export_input_output()
+        return (
+            x.detach().cpu().numpy(),
+            self(*args, x, pad_start=True).detach().cpu().numpy(),
+        )
+
+
+class BaseNet(_Base):
+    def forward(self, x: torch.Tensor, pad_start: Optional[bool] = None):
+        pad_start = self.pad_start_default if pad_start is None else pad_start
+        scalar = x.ndim == 1
+        if scalar:
+            x = x[None]
+        if pad_start:
+            x = torch.cat((torch.zeros((len(x), self.receptive_field - 1)), x), dim=1)
+        y = self._forward(x)
+        if scalar:
+            y = y[0]
+        return y
+
+    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
+        return self(x)
+
+    @abc.abstractmethod
+    def _forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        The true forward method.
+
+        :param x: (N,L1)
+        :return: (N,L1-RF+1)
+        """
+        pass
+
+    def _get_non_user_metadata(self) -> Dict[str, Union[str, int, float]]:
+        d = super()._get_non_user_metadata()
+        d["loudness"] = self._metadata_loudness()
+        d["gain"] = self._metadata_gain()
+        return d
+
+
+class ParametricBaseNet(_Base):
+    """
+    Parametric inputs
+    """
+
+    def forward(
+        self, params: torch.Tensor, x: torch.Tensor, pad_start: Optional[bool] = None
+    ):
+        pad_start = self.pad_start_default if pad_start is None else pad_start
+        scalar = x.ndim == 1
+        if scalar:
+            x = x[None]
+            params = params[None]
+        if pad_start:
+            x = torch.cat((torch.zeros((len(x), self.receptive_field - 1)), x), dim=1)
+        y = self._forward(params, x)
+        if scalar:
+            y = y[0]
+        return y
+
+    @abc.abstractmethod
+    def _forward(self, params: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
+        """
+        The true forward method.
+
+        :param params: (N,D)
+        :param x: (N,L1)
+        :return: (N,L1-RF+1)
+        """
+        pass
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/_resources/loudness_input.wav` & `neural-amp-modeler-0.6.0/nam/models/_resources/loudness_input.wav`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.5.2/nam/models/conv_net.py` & `neural-amp-modeler-0.6.0/nam/models/conv_net.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-# File: conv_net.py
-# Created Date: Saturday February 5th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-import json
-import math
-from enum import Enum
-from functools import partial
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Optional, Sequence, Tuple, Union
-
-import numpy as np
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-from .. import __version__
-from ..data import REQUIRED_RATE, wav_to_tensor
-from ._activations import get_activation
-from ._base import BaseNet
-from ._names import ACTIVATION_NAME, BATCHNORM_NAME, CONV_NAME
-
-
-class TrainStrategy(Enum):
-    STRIDE = "stride"
-    DILATE = "dilate"
-
-
-default_train_strategy = TrainStrategy.DILATE
-
-
-class _Functional(nn.Module):
-    """
-    Define a layer by a function w/ no params
-    """
-
-    def __init__(self, op):
-        super().__init__()
-        self._op = op
-
-    def forward(self, *args, **kwargs):
-        return self._op(*args, **kwargs)
-
-
-class _IR(nn.Module):
-    def __init__(self, filename: Union[str, Path]):
-        super().__init__()
-        self.register_buffer("_weight", reversed(wav_to_tensor(filename))[None, None])
-
-    @property
-    def length(self) -> int:
-        return self._weight.shape[-1]
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        :param x: (N,D)
-        :return: (N,D-length+1)
-        """
-        return F.conv1d(x[:, None], self._weight)[:, 0]
-
-
-def _conv_net(
-    channels: int = 32,
-    dilations: Sequence[int] = None,
-    batchnorm: bool = False,
-    activation: str = "Tanh",
-) -> nn.Sequential:
-    def block(cin, cout, dilation):
-        net = nn.Sequential()
-        net.add_module(
-            CONV_NAME, nn.Conv1d(cin, cout, 2, dilation=dilation, bias=not batchnorm)
-        )
-        if batchnorm:
-            net.add_module(BATCHNORM_NAME, nn.BatchNorm1d(cout))
-        net.add_module(ACTIVATION_NAME, get_activation(activation))
-        return net
-
-    def check_and_expand(n, x):
-        if x.shape[1] < n:
-            raise ValueError(
-                f"Input of length {x.shape[1]} is shorter than model receptive field ({n})"
-            )
-        return x[:, None, :]
-
-    dilations = [1, 2, 4, 8] if dilations is None else dilations
-    receptive_field = sum(dilations) + 1
-    net = nn.Sequential()
-    net.add_module("expand", _Functional(partial(check_and_expand, receptive_field)))
-    cin = 1
-    cout = channels
-    for i, dilation in enumerate(dilations):
-        net.add_module(f"block_{i}", block(cin, cout, dilation))
-        cin = cout
-    net.add_module("head", nn.Conv1d(channels, 1, 1))
-    net.add_module("flatten", nn.Flatten())
-    return net
-
-
-class ConvNet(BaseNet):
-    """
-    A straightforward convolutional neural network.
-
-    Works surprisingly well!
-    """
-
-    def __init__(
-        self,
-        *args,
-        train_strategy: TrainStrategy = default_train_strategy,
-        ir: Optional[_IR] = None,
-        **kwargs,
-    ):
-        super().__init__()
-        self._net = _conv_net(*args, **kwargs)
-        assert train_strategy == TrainStrategy.DILATE, "Stride no longer supported"
-        self._train_strategy = train_strategy
-        self._num_blocks = self._get_num_blocks(self._net)
-        self._pad_start_default = True
-        self._ir = ir
-
-    @classmethod
-    def parse_config(cls, config):
-        config = super().parse_config(config)
-        config["train_strategy"] = TrainStrategy(
-            config.get("train_strategy", default_train_strategy.value)
-        )
-        config["ir"] = (
-            None if "ir_filename" not in config else _IR(config.pop("ir_filename"))
-        )
-        return config
-
-    @property
-    def pad_start_default(self) -> bool:
-        return self._pad_start_default
-
-    @property
-    def receptive_field(self) -> int:
-        net_rf = 1 + sum(
-            self._net._modules[f"block_{i}"]._modules["conv"].dilation[0]
-            for i in range(self._num_blocks)
-        )
-        # Minus 1 because it composes w/ the net
-        ir_rf = 0 if self._ir is None else self._ir.length - 1
-        return net_rf + ir_rf
-
-    @property
-    def _activation(self):
-        return (
-            self._net._modules["block_0"]._modules[ACTIVATION_NAME].__class__.__name__
-        )
-
-    @property
-    def _channels(self) -> int:
-        return self._net._modules["block_0"]._modules[CONV_NAME].weight.shape[0]
-
-    @property
-    def _num_layers(self) -> int:
-        return self._num_blocks
-
-    @property
-    def _batchnorm(self) -> bool:
-        return BATCHNORM_NAME in self._net._modules["block_0"]._modules
-
-    def export_cpp_header(self, filename: Path):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir)
-            self.export(Path(tmpdir))
-            with open(Path(tmpdir, "config.json"), "r") as fp:
-                _c = json.load(fp)
-            version = _c["version"]
-            config = _c["config"]
-            with open(filename, "w") as f:
-                f.writelines(
-                    (
-                        "#pragma once\n",
-                        "// Automatically-generated model file\n",
-                        "#include <vector>\n",
-                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
-                        f"const int CHANNELS = {config['channels']};\n",
-                        f"const bool BATCHNORM = {'true' if config['batchnorm'] else 'false'};\n",
-                        "std::vector<int> DILATIONS{"
-                        + ",".join([str(d) for d in config["dilations"]])
-                        + "};\n",
-                        f"const std::string ACTIVATION = \"{config['activation']}\";\n",
-                        "std::vector<float> PARAMS{"
-                        + ",".join(
-                            [f"{w:.16f}" for w in np.load(Path(tmpdir, "weights.npy"))]
-                        )
-                        + "};\n",
-                    )
-                )
-
-    def _export_config(self):
-        return {
-            "channels": self._channels,
-            "dilations": self._get_dilations(),
-            "batchnorm": self._batchnorm,
-            "activation": self._activation,
-        }
-
-    def _export_input_output(self, x=None) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        :return: (L,), (L,)
-        """
-        with torch.no_grad():
-            training = self.training
-            self.eval()
-            x = self._export_input_signal() if x is None else x
-            y = self(x, pad_start=True)
-            self.train(training)
-            return tuple(z.detach().cpu().numpy() for z in (x, y))
-
-    def _export_input_signal(self):
-        """
-        :return: (L,)
-        """
-        rate = REQUIRED_RATE
-        return torch.cat(
-            [
-                torch.zeros((rate,)),
-                0.5
-                * torch.sin(
-                    2.0 * math.pi * 220.0 * torch.linspace(0.0, 1.0, rate + 1)[:-1]
-                ),
-                torch.zeros((rate,)),
-            ]
-        )
-
-    def _export_weights(self) -> np.ndarray:
-        """
-        weights are serialized to weights.npy in the following order:
-        * (expand: no params)
-        * loop blocks 0,...,L-1
-            * conv:
-                * weight (Cout, Cin, K)
-                * bias (if no batchnorm) (Cout)
-            * BN
-                * running mean
-                * running_var
-                * weight (Cout)
-                * bias (Cout)
-                * eps ()
-        * head
-            * weight (C, 1, 1)
-            * bias (1, 1)
-        * (flatten: no params)
-        """
-        params = []
-        for i in range(self._num_layers):
-            block_name = f"block_{i}"
-            block = self._net._modules[block_name]
-            conv = block._modules[CONV_NAME]
-            params.append(conv.weight.flatten())
-            if conv.bias is not None:
-                params.append(conv.bias.flatten())
-            if self._batchnorm:
-                bn = block._modules[BATCHNORM_NAME]
-                params.append(bn.running_mean.flatten())
-                params.append(bn.running_var.flatten())
-                params.append(bn.weight.flatten())
-                params.append(bn.bias.flatten())
-                params.append(torch.Tensor([bn.eps]).to(bn.weight.device))
-        head = self._net._modules["head"]
-        params.append(head.weight.flatten())
-        params.append(head.bias.flatten())
-        params = torch.cat(params).detach().cpu().numpy()
-        return params
-
-    def _forward(self, x):
-        y = self._net(x)
-        if self._ir is not None:
-            y = self._ir(y)
-        return y
-
-    def _get_dilations(self) -> Tuple[int]:
-        return tuple(
-            self._net._modules[f"block_{i}"]._modules[CONV_NAME].dilation[0]
-            for i in range(self._num_blocks)
-        )
-
-    def _get_num_blocks(self, net: nn.Sequential):
-        i = 0
-        while True:
-            if f"block_{i}" not in net._modules:
-                break
-            else:
-                i += 1
-        return i
+# File: conv_net.py
+# Created Date: Saturday February 5th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+import json
+import math
+from enum import Enum
+from functools import partial
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from typing import Optional, Sequence, Tuple, Union
+
+import numpy as np
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+from .. import __version__
+from ..data import REQUIRED_RATE, wav_to_tensor
+from ._activations import get_activation
+from ._base import BaseNet
+from ._names import ACTIVATION_NAME, BATCHNORM_NAME, CONV_NAME
+
+
+class TrainStrategy(Enum):
+    STRIDE = "stride"
+    DILATE = "dilate"
+
+
+default_train_strategy = TrainStrategy.DILATE
+
+
+class _Functional(nn.Module):
+    """
+    Define a layer by a function w/ no params
+    """
+
+    def __init__(self, op):
+        super().__init__()
+        self._op = op
+
+    def forward(self, *args, **kwargs):
+        return self._op(*args, **kwargs)
+
+
+class _IR(nn.Module):
+    def __init__(self, filename: Union[str, Path]):
+        super().__init__()
+        self.register_buffer("_weight", reversed(wav_to_tensor(filename))[None, None])
+
+    @property
+    def length(self) -> int:
+        return self._weight.shape[-1]
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        :param x: (N,D)
+        :return: (N,D-length+1)
+        """
+        return F.conv1d(x[:, None], self._weight)[:, 0]
+
+
+def _conv_net(
+    channels: int = 32,
+    dilations: Sequence[int] = None,
+    batchnorm: bool = False,
+    activation: str = "Tanh",
+) -> nn.Sequential:
+    def block(cin, cout, dilation):
+        net = nn.Sequential()
+        net.add_module(
+            CONV_NAME, nn.Conv1d(cin, cout, 2, dilation=dilation, bias=not batchnorm)
+        )
+        if batchnorm:
+            net.add_module(BATCHNORM_NAME, nn.BatchNorm1d(cout))
+        net.add_module(ACTIVATION_NAME, get_activation(activation))
+        return net
+
+    def check_and_expand(n, x):
+        if x.shape[1] < n:
+            raise ValueError(
+                f"Input of length {x.shape[1]} is shorter than model receptive field ({n})"
+            )
+        return x[:, None, :]
+
+    dilations = [1, 2, 4, 8] if dilations is None else dilations
+    receptive_field = sum(dilations) + 1
+    net = nn.Sequential()
+    net.add_module("expand", _Functional(partial(check_and_expand, receptive_field)))
+    cin = 1
+    cout = channels
+    for i, dilation in enumerate(dilations):
+        net.add_module(f"block_{i}", block(cin, cout, dilation))
+        cin = cout
+    net.add_module("head", nn.Conv1d(channels, 1, 1))
+    net.add_module("flatten", nn.Flatten())
+    return net
+
+
+class ConvNet(BaseNet):
+    """
+    A straightforward convolutional neural network.
+
+    Works surprisingly well!
+    """
+
+    def __init__(
+        self,
+        *args,
+        train_strategy: TrainStrategy = default_train_strategy,
+        ir: Optional[_IR] = None,
+        **kwargs,
+    ):
+        super().__init__()
+        self._net = _conv_net(*args, **kwargs)
+        assert train_strategy == TrainStrategy.DILATE, "Stride no longer supported"
+        self._train_strategy = train_strategy
+        self._num_blocks = self._get_num_blocks(self._net)
+        self._pad_start_default = True
+        self._ir = ir
+
+    @classmethod
+    def parse_config(cls, config):
+        config = super().parse_config(config)
+        config["train_strategy"] = TrainStrategy(
+            config.get("train_strategy", default_train_strategy.value)
+        )
+        config["ir"] = (
+            None if "ir_filename" not in config else _IR(config.pop("ir_filename"))
+        )
+        return config
+
+    @property
+    def pad_start_default(self) -> bool:
+        return self._pad_start_default
+
+    @property
+    def receptive_field(self) -> int:
+        net_rf = 1 + sum(
+            self._net._modules[f"block_{i}"]._modules["conv"].dilation[0]
+            for i in range(self._num_blocks)
+        )
+        # Minus 1 because it composes w/ the net
+        ir_rf = 0 if self._ir is None else self._ir.length - 1
+        return net_rf + ir_rf
+
+    @property
+    def _activation(self):
+        return (
+            self._net._modules["block_0"]._modules[ACTIVATION_NAME].__class__.__name__
+        )
+
+    @property
+    def _channels(self) -> int:
+        return self._net._modules["block_0"]._modules[CONV_NAME].weight.shape[0]
+
+    @property
+    def _num_layers(self) -> int:
+        return self._num_blocks
+
+    @property
+    def _batchnorm(self) -> bool:
+        return BATCHNORM_NAME in self._net._modules["block_0"]._modules
+
+    def export_cpp_header(self, filename: Path):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir)
+            self.export(Path(tmpdir))
+            with open(Path(tmpdir, "config.json"), "r") as fp:
+                _c = json.load(fp)
+            version = _c["version"]
+            config = _c["config"]
+            with open(filename, "w") as f:
+                f.writelines(
+                    (
+                        "#pragma once\n",
+                        "// Automatically-generated model file\n",
+                        "#include <vector>\n",
+                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
+                        f"const int CHANNELS = {config['channels']};\n",
+                        f"const bool BATCHNORM = {'true' if config['batchnorm'] else 'false'};\n",
+                        "std::vector<int> DILATIONS{"
+                        + ",".join([str(d) for d in config["dilations"]])
+                        + "};\n",
+                        f"const std::string ACTIVATION = \"{config['activation']}\";\n",
+                        "std::vector<float> PARAMS{"
+                        + ",".join(
+                            [f"{w:.16f}" for w in np.load(Path(tmpdir, "weights.npy"))]
+                        )
+                        + "};\n",
+                    )
+                )
+
+    def _export_config(self):
+        return {
+            "channels": self._channels,
+            "dilations": self._get_dilations(),
+            "batchnorm": self._batchnorm,
+            "activation": self._activation,
+        }
+
+    def _export_input_output(self, x=None) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        :return: (L,), (L,)
+        """
+        with torch.no_grad():
+            training = self.training
+            self.eval()
+            x = self._export_input_signal() if x is None else x
+            y = self(x, pad_start=True)
+            self.train(training)
+            return tuple(z.detach().cpu().numpy() for z in (x, y))
+
+    def _export_input_signal(self):
+        """
+        :return: (L,)
+        """
+        rate = REQUIRED_RATE
+        return torch.cat(
+            [
+                torch.zeros((rate,)),
+                0.5
+                * torch.sin(
+                    2.0 * math.pi * 220.0 * torch.linspace(0.0, 1.0, rate + 1)[:-1]
+                ),
+                torch.zeros((rate,)),
+            ]
+        )
+
+    def _export_weights(self) -> np.ndarray:
+        """
+        weights are serialized to weights.npy in the following order:
+        * (expand: no params)
+        * loop blocks 0,...,L-1
+            * conv:
+                * weight (Cout, Cin, K)
+                * bias (if no batchnorm) (Cout)
+            * BN
+                * running mean
+                * running_var
+                * weight (Cout)
+                * bias (Cout)
+                * eps ()
+        * head
+            * weight (C, 1, 1)
+            * bias (1, 1)
+        * (flatten: no params)
+        """
+        params = []
+        for i in range(self._num_layers):
+            block_name = f"block_{i}"
+            block = self._net._modules[block_name]
+            conv = block._modules[CONV_NAME]
+            params.append(conv.weight.flatten())
+            if conv.bias is not None:
+                params.append(conv.bias.flatten())
+            if self._batchnorm:
+                bn = block._modules[BATCHNORM_NAME]
+                params.append(bn.running_mean.flatten())
+                params.append(bn.running_var.flatten())
+                params.append(bn.weight.flatten())
+                params.append(bn.bias.flatten())
+                params.append(torch.Tensor([bn.eps]).to(bn.weight.device))
+        head = self._net._modules["head"]
+        params.append(head.weight.flatten())
+        params.append(head.bias.flatten())
+        params = torch.cat(params).detach().cpu().numpy()
+        return params
+
+    def _forward(self, x):
+        y = self._net(x)
+        if self._ir is not None:
+            y = self._ir(y)
+        return y
+
+    def _get_dilations(self) -> Tuple[int]:
+        return tuple(
+            self._net._modules[f"block_{i}"]._modules[CONV_NAME].dilation[0]
+            for i in range(self._num_blocks)
+        )
+
+    def _get_num_blocks(self, net: nn.Sequential):
+        i = 0
+        while True:
+            if f"block_{i}" not in net._modules:
+                break
+            else:
+                i += 1
+        return i
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/linear.py` & `neural-amp-modeler-0.6.0/nam/models/linear.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# File: linear.py
-# Created Date: Tuesday February 8th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Linear model
-"""
-
-import json
-from pathlib import Path
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-from .._version import __version__
-from ._base import BaseNet
-
-
-class Linear(BaseNet):
-    def __init__(self, receptive_field: int, bias: bool = False):
-        super().__init__()
-        self._net = nn.Conv1d(1, 1, receptive_field, bias=bias)
-
-    @property
-    def pad_start_default(self) -> bool:
-        return True
-
-    @property
-    def receptive_field(self) -> int:
-        return self._net.weight.shape[2]
-
-    def export(self, outdir: Path):
-        training = self.training
-        self.eval()
-        with open(Path(outdir, "config.json"), "w") as fp:
-            json.dump(
-                {
-                    "version": __version__,
-                    "architecture": self.__class__.__name__,
-                    "config": {
-                        "receptive_field": self.receptive_field,
-                        "bias": self._bias,
-                    },
-                },
-                fp,
-                indent=4,
-            )
-
-        params = [self._net.weight.flatten()]
-        if self._bias:
-            params.append(self._net.bias.flatten())
-        params = torch.cat(params).detach().cpu().numpy()
-        # Hope I don't regret using np.save...
-        np.save(Path(outdir, "weights.npy"), params)
-
-        # And an input/output to verify correct computation:
-        x, y = self._export_input_output()
-        np.save(Path(outdir, "input.npy"), x.detach().cpu().numpy())
-        np.save(Path(outdir, "output.npy"), y.detach().cpu().numpy())
-
-        # And resume training state
-        self.train(training)
-
-    @property
-    def _bias(self) -> bool:
-        return self._net.bias is not None
-
-    def _forward(self, x: torch.Tensor) -> torch.Tensor:
-        return self._net(x[:, None])[:, 0]
+# File: linear.py
+# Created Date: Tuesday February 8th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Linear model
+"""
+
+import json
+from pathlib import Path
+
+import numpy as np
+import torch
+import torch.nn as nn
+
+from .._version import __version__
+from ._base import BaseNet
+
+
+class Linear(BaseNet):
+    def __init__(self, receptive_field: int, bias: bool = False):
+        super().__init__()
+        self._net = nn.Conv1d(1, 1, receptive_field, bias=bias)
+
+    @property
+    def pad_start_default(self) -> bool:
+        return True
+
+    @property
+    def receptive_field(self) -> int:
+        return self._net.weight.shape[2]
+
+    def export(self, outdir: Path):
+        training = self.training
+        self.eval()
+        with open(Path(outdir, "config.json"), "w") as fp:
+            json.dump(
+                {
+                    "version": __version__,
+                    "architecture": self.__class__.__name__,
+                    "config": {
+                        "receptive_field": self.receptive_field,
+                        "bias": self._bias,
+                    },
+                },
+                fp,
+                indent=4,
+            )
+
+        params = [self._net.weight.flatten()]
+        if self._bias:
+            params.append(self._net.bias.flatten())
+        params = torch.cat(params).detach().cpu().numpy()
+        # Hope I don't regret using np.save...
+        np.save(Path(outdir, "weights.npy"), params)
+
+        # And an input/output to verify correct computation:
+        x, y = self._export_input_output()
+        np.save(Path(outdir, "input.npy"), x.detach().cpu().numpy())
+        np.save(Path(outdir, "output.npy"), y.detach().cpu().numpy())
+
+        # And resume training state
+        self.train(training)
+
+    @property
+    def _bias(self) -> bool:
+        return self._net.bias is not None
+
+    def _forward(self, x: torch.Tensor) -> torch.Tensor:
+        return self._net(x[:, None])[:, 0]
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/losses.py` & `neural-amp-modeler-0.6.0/nam/models/losses.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,88 @@
-# File: losses.py
-# Created Date: Sunday January 22nd 2023
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Loss functions
-"""
-
-from typing import Optional
-
-import torch
-from auraloss.freq import MultiResolutionSTFTLoss
-
-___all__ = ["esr", "multi_resolution_stft_loss"]
-
-
-def esr(preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
-    """
-    ESR of (a batch of) predictions & targets
-
-    :param preds: (N,) or (B,N)
-    :param targets: Same as preds
-    :return: ()
-    """
-    if preds.ndim == 1 and targets.ndim == 1:
-        preds, targets = preds[None], targets[None]
-    if preds.ndim != 2:
-        raise ValueError(
-            f"Expect 2D predictions (batch_size, num_samples). Got {preds.shape}"
-        )
-    if targets.ndim != 2:
-        raise ValueError(
-            f"Expect 2D targets (batch_size, num_samples). Got {targets.shape}"
-        )
-    return torch.mean(
-        torch.mean(torch.square(preds - targets), dim=1)
-        / torch.mean(torch.square(targets), dim=1)
-    )
-
-
-def multi_resolution_stft_loss(
-    preds: torch.Tensor,
-    targets: torch.Tensor,
-    loss_func: Optional[MultiResolutionSTFTLoss] = None,
-    device: Optional[torch.device] = None,
-) -> torch.Tensor:
-    """
-    Experimental Multi Resolution Short Time Fourier Transform Loss using auraloss implementation.
-    B: Batch size
-    L: Sequence length
-
-    :param preds: (B,L)
-    :param targets: (B,L)
-    :param loss_func: A pre-initialized instance of the loss function module. Providing
-        this saves time.
-    :param device: If provided, send the preds and targets to the provided device.
-    :return: ()
-    """
-    loss_func = MultiResolutionSTFTLoss() if loss_func is None else loss_func
-    if device is not None:
-        preds, targets = [z.to(device) for z in (preds, targets)]
-    return loss_func(preds, targets)
-
-
-def mse_fft(preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
-    """
-    Fourier loss
-
-    :param preds: (N,) or (B,N)
-    :param targets: Same as preds
-    :return: ()
-    """
-    fp = torch.fft.fft(preds)
-    ft = torch.fft.fft(targets)
-    e = fp - ft
-    return torch.mean(torch.square(e.abs()))
+# File: losses.py
+# Created Date: Sunday January 22nd 2023
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Loss functions
+"""
+
+from typing import Optional
+
+import torch
+from auraloss.freq import MultiResolutionSTFTLoss
+
+___all__ = ["apply_pre_emphasis_filter", "esr", "multi_resolution_stft_loss"]
+
+
+def apply_pre_emphasis_filter(x: torch.Tensor, coef: float) -> torch.Tensor:
+    """
+    Apply first-order pre-emphsis filter
+
+    :param x: (*, L)
+    :param coef: The coefficient
+
+    :return: (*, L-1)
+    """
+    return x[..., 1:] - coef * x[..., :-1]
+
+
+def esr(preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
+    """
+    ESR of (a batch of) predictions & targets
+
+    :param preds: (N,) or (B,N)
+    :param targets: Same as preds
+    :return: ()
+    """
+    if preds.ndim == 1 and targets.ndim == 1:
+        preds, targets = preds[None], targets[None]
+    if preds.ndim != 2:
+        raise ValueError(
+            f"Expect 2D predictions (batch_size, num_samples). Got {preds.shape}"
+        )
+    if targets.ndim != 2:
+        raise ValueError(
+            f"Expect 2D targets (batch_size, num_samples). Got {targets.shape}"
+        )
+    return torch.mean(
+        torch.mean(torch.square(preds - targets), dim=1)
+        / torch.mean(torch.square(targets), dim=1)
+    )
+
+
+def multi_resolution_stft_loss(
+    preds: torch.Tensor,
+    targets: torch.Tensor,
+    loss_func: Optional[MultiResolutionSTFTLoss] = None,
+    device: Optional[torch.device] = None,
+) -> torch.Tensor:
+    """
+    Experimental Multi Resolution Short Time Fourier Transform Loss using auraloss implementation.
+    B: Batch size
+    L: Sequence length
+
+    :param preds: (B,L)
+    :param targets: (B,L)
+    :param loss_func: A pre-initialized instance of the loss function module. Providing
+        this saves time.
+    :param device: If provided, send the preds and targets to the provided device.
+    :return: ()
+    """
+    loss_func = MultiResolutionSTFTLoss() if loss_func is None else loss_func
+    if device is not None:
+        preds, targets = [z.to(device) for z in (preds, targets)]
+    return loss_func(preds, targets)
+
+
+def mse_fft(preds: torch.Tensor, targets: torch.Tensor) -> torch.Tensor:
+    """
+    Fourier loss
+
+    :param preds: (N,) or (B,N)
+    :param targets: Same as preds
+    :return: ()
+    """
+    fp = torch.fft.fft(preds)
+    ft = torch.fft.fft(targets)
+    e = fp - ft
+    return torch.mean(torch.square(e.abs()))
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/metadata.py` & `neural-amp-modeler-0.6.0/nam/models/metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-# File: metadata.py
-# Created Date: Wednesday April 12th 2023
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Metadata about models
-"""
-
-from enum import Enum
-from typing import Optional
-
-from pydantic import BaseModel
-
-__all__ = ["GearType", "ToneType", "Date", "UserMetadata"]
-
-
-# Note: if you change this enum, you need to update the options in easy_colab.ipynb!
-class GearType(Enum):
-    AMP = "amp"
-    PEDAL = "pedal"
-    AMP_CAB = "amp_cab"
-    AMP_PEDAL_CAB = "amp_pedal_cab"
-    PREAMP = "preamp"
-    STUDIO = "studio"
-
-# Note: if you change this enum, you need to update the options in easy_colab.ipynb!
-class ToneType(Enum):
-    CLEAN = "clean"
-    OVERDRIVE = "overdrive"
-    CRUNCH = "crunch"
-    HI_GAIN = "hi_gain"
-    FUZZ = "fuzz"
-
-
-class Date(BaseModel):
-    year: int
-    month: int
-    day: int
-    hour: int
-    minute: int
-    second: int
-
-
-class UserMetadata(BaseModel):
-    """
-    Metadata that users provide for a NAM model
-    """
-
-    name: Optional[str] = None
-    modeled_by: Optional[str] = None
-    gear_type: Optional[GearType] = None
-    gear_make: Optional[str] = None
-    gear_model: Optional[str] = None
-    tone_type: Optional[ToneType] = None
+# File: metadata.py
+# Created Date: Wednesday April 12th 2023
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Metadata about models
+"""
+
+from enum import Enum
+from typing import Optional
+
+from pydantic import BaseModel
+
+__all__ = ["GearType", "ToneType", "Date", "UserMetadata"]
+
+
+# Note: if you change this enum, you need to update the options in easy_colab.ipynb!
+class GearType(Enum):
+    AMP = "amp"
+    PEDAL = "pedal"
+    AMP_CAB = "amp_cab"
+    AMP_PEDAL_CAB = "amp_pedal_cab"
+    PREAMP = "preamp"
+    STUDIO = "studio"
+
+
+# Note: if you change this enum, you need to update the options in easy_colab.ipynb!
+class ToneType(Enum):
+    CLEAN = "clean"
+    OVERDRIVE = "overdrive"
+    CRUNCH = "crunch"
+    HI_GAIN = "hi_gain"
+    FUZZ = "fuzz"
+
+
+class Date(BaseModel):
+    year: int
+    month: int
+    day: int
+    hour: int
+    minute: int
+    second: int
+
+
+class UserMetadata(BaseModel):
+    """
+    Metadata that users provide for a NAM model
+    """
+
+    name: Optional[str] = None
+    modeled_by: Optional[str] = None
+    gear_type: Optional[GearType] = None
+    gear_make: Optional[str] = None
+    gear_model: Optional[str] = None
+    tone_type: Optional[ToneType] = None
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/parametric/catnets.py` & `neural-amp-modeler-0.6.0/nam/models/parametric/catnets.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-# File: catnets.py
-# Created Date: Wednesday June 22nd 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-"Cat nets" -- parametric models where the parametric input is concatenated to the
-input samples
-"""
-
-import abc
-import logging
-from enum import Enum
-from contextlib import contextmanager
-from pathlib import Path
-from typing import Any, Dict, Tuple
-
-import numpy as np
-import torch
-
-from .._base import ParametricBaseNet
-from ..recurrent import LSTM
-from ..wavenet import WaveNet
-from .params import Param
-
-logger = logging.getLogger(__name__)
-
-
-class _ShapeType(Enum):
-    CONV = "conv"  # (B,C,L)
-    RNN = "rnn"  # (B,L,D)
-
-
-class _CatMixin(ParametricBaseNet):
-    """
-    Parameteric nets that concatenate the params with the input at each time point
-    Mix in with a non-parametric class like
-
-    ```
-    class CatLSTM(LSTM, _CatMixin):
-        pass
-    ```
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        # Hacky, see .export()
-        self._sidedoor_parametric_config = None
-
-    @abc.abstractproperty
-    def _shape_type(self) -> _ShapeType:
-        pass
-
-    @abc.abstractproperty
-    def _single_class(self):
-        """ "
-        The class for the non-parametric model that this is extending
-        """
-        # TODO verify that single class satisfies requirements
-        # ._export_weights()
-        # ._export_input_output()
-        pass  # HACK
-
-    def export(self, outdir: Path, parametric_config: Dict[str, Param], **kwargs):
-        """
-        Interface for exporting.
-        You should create at least a `config.json` containing the fields:
-        * "version" (str)
-        * "architecture" (str)
-        * "config": (dict w/ other necessary data like tensor shapes etc)
-
-        :param outdir: Assumed to exist. Can be edited inside at will.
-        """
-        with self._use_parametric_config(parametric_config):
-            return super().export(outdir, **kwargs)
-
-    def export_cpp_header(self, filename: Path, parametric_config: Dict[str, Param]):
-        with self._use_parametric_config(parametric_config):
-            return super().export_cpp_header(filename)
-
-    def _export_config(self):
-        """
-        Adds in the sidedoored parametric pieces
-
-        :paramtric_config: the dict of parameter info (name, type, etc)
-        """
-        config = super()._export_config()
-        if not isinstance(config, dict):
-            raise TypeError(
-                f"Parameteric models' base configs must be a dict; got {type(config)}"
-            )
-        parametric_key = "parametric"
-        if parametric_key in config:
-            raise ValueError(
-                f'Already found parametric key "{parametric_key}" in base config dict.'
-            )
-        # Yucky sidedoor
-        config[parametric_key] = {
-            k: v.to_json() for k, v in self._sidedoor_parametric_config.items()
-        }
-        return config
-
-    def _export_cpp_header_parametric(self, config):
-        if config is None:
-            return self._single_class._export_cpp_head_parametric(self, config)
-        s_parametric = [
-            'nlohmann::json PARAMETRIC = nlohmann::json::parse(R"(\n',
-            "  {\n",
-        ]
-        for i, (key, val) in enumerate(config.items(), 1):
-            s_parametric.append(f'    "{key}": ' "{\n")
-            for j, (k2, v2) in enumerate(val.items(), 1):
-                v_str = f'"{v2}"' if isinstance(v2, str) else str(v2)
-                s_parametric.append(
-                    f'      "{k2}": {v_str}' + (",\n" if j < len(val) else "\n")
-                )
-            s_parametric.append("    }" f"{',' if i < len(config) else ''}\n")
-        s_parametric.append("  }\n")
-        s_parametric.append(')");\n')
-        return tuple(s_parametric)
-
-    def _export_input_output_args(self) -> Tuple[torch.Tensor]:
-        return (self._sidedoor_params_to_tensor(),)
-
-    def _forward(self, params, x):
-        """
-        :param params: (N,D)
-        :param x: (N,L1)
-
-        :return: (N,L2)
-        """
-        sequence_length = x.shape[1]
-        x_augmented = (
-            torch.cat(
-                [
-                    x[..., None],
-                    torch.tile(params[:, None, :], (1, sequence_length, 1)),
-                ],
-                dim=2,
-            )
-            if self._shape_type == _ShapeType.RNN
-            else torch.cat(
-                [x[:, None, :], torch.tile(params[..., None], (1, 1, sequence_length))],
-                dim=1,
-            )
-        )
-        return self._single_class._forward(self, x_augmented)
-
-    def _sidedoor_params_to_tensor(self) -> torch.Tensor:
-        param_names = sorted([k for k in self._sidedoor_parametric_config.keys()])
-        params = torch.Tensor(
-            [self._sidedoor_parametric_config[k].default_value for k in param_names]
-        )
-        return params
-
-    @contextmanager
-    def _use_parametric_config(self, c):
-        """
-        Sneaks in the parametric config while exporting
-        """
-        try:
-            self._sidedoor_parametric_config = c
-            yield None
-        finally:
-            self._sidedoor_parametric_config = None
-
-
-class CatLSTM(_CatMixin, LSTM):
-    @property
-    def _shape_type(self) -> _ShapeType:
-        return _ShapeType.RNN
-
-    @property
-    def _single_class(self):
-        return LSTM
-
-    def _append_default_params(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        Requires sidedoor'd params
-
-        :param x: (B,L)
-        :return: (B,L,1+D)
-        """
-        assert x.ndim == 2
-        params = self._sidedoor_params_to_tensor()
-        sequence_length = x.shape[1]
-        return torch.cat(
-            [
-                x[:, :, None],
-                torch.tile(params[None, None, :], (1, sequence_length, 1)),
-            ],
-            dim=2,
-        )
-
-    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
-        if self._input_size != 1:
-            logger.warning(
-                "Nominal settings aren't defined for parametric models; outputting unity"
-            )
-            return x
-        params = torch.zeros(()).to(x.device)
-        return self(params, x)
-
-    def _get_initial_state(self) -> Tuple[torch.Tensor, torch.Tensor]:
-        inputs = self._append_default_params(torch.zeros((1, 48_000)))
-        return super()._get_initial_state(inputs=inputs)
-
-
-class CatWaveNet(_CatMixin, WaveNet):
-    @property
-    def _shape_type(self) -> _ShapeType:
-        return _ShapeType.CONV
-
-    @property
-    def _single_class(self):
-        return WaveNet
+# File: catnets.py
+# Created Date: Wednesday June 22nd 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+"Cat nets" -- parametric models where the parametric input is concatenated to the
+input samples
+"""
+
+import abc
+import logging
+from enum import Enum
+from contextlib import contextmanager
+from pathlib import Path
+from typing import Any, Dict, Tuple
+
+import numpy as np
+import torch
+
+from .._base import ParametricBaseNet
+from ..recurrent import LSTM
+from ..wavenet import WaveNet
+from .params import Param
+
+logger = logging.getLogger(__name__)
+
+
+class _ShapeType(Enum):
+    CONV = "conv"  # (B,C,L)
+    RNN = "rnn"  # (B,L,D)
+
+
+class _CatMixin(ParametricBaseNet):
+    """
+    Parameteric nets that concatenate the params with the input at each time point
+    Mix in with a non-parametric class like
+
+    ```
+    class CatLSTM(LSTM, _CatMixin):
+        pass
+    ```
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # Hacky, see .export()
+        self._sidedoor_parametric_config = None
+
+    @abc.abstractproperty
+    def _shape_type(self) -> _ShapeType:
+        pass
+
+    @abc.abstractproperty
+    def _single_class(self):
+        """ "
+        The class for the non-parametric model that this is extending
+        """
+        # TODO verify that single class satisfies requirements
+        # ._export_weights()
+        # ._export_input_output()
+        pass  # HACK
+
+    def export(self, outdir: Path, parametric_config: Dict[str, Param], **kwargs):
+        """
+        Interface for exporting.
+        You should create at least a `config.json` containing the fields:
+        * "version" (str)
+        * "architecture" (str)
+        * "config": (dict w/ other necessary data like tensor shapes etc)
+
+        :param outdir: Assumed to exist. Can be edited inside at will.
+        """
+        with self._use_parametric_config(parametric_config):
+            return super().export(outdir, **kwargs)
+
+    def export_cpp_header(self, filename: Path, parametric_config: Dict[str, Param]):
+        with self._use_parametric_config(parametric_config):
+            return super().export_cpp_header(filename)
+
+    def _export_config(self):
+        """
+        Adds in the sidedoored parametric pieces
+
+        :paramtric_config: the dict of parameter info (name, type, etc)
+        """
+        config = super()._export_config()
+        if not isinstance(config, dict):
+            raise TypeError(
+                f"Parameteric models' base configs must be a dict; got {type(config)}"
+            )
+        parametric_key = "parametric"
+        if parametric_key in config:
+            raise ValueError(
+                f'Already found parametric key "{parametric_key}" in base config dict.'
+            )
+        # Yucky sidedoor
+        config[parametric_key] = {
+            k: v.to_json() for k, v in self._sidedoor_parametric_config.items()
+        }
+        return config
+
+    def _export_cpp_header_parametric(self, config):
+        if config is None:
+            return self._single_class._export_cpp_head_parametric(self, config)
+        s_parametric = [
+            'nlohmann::json PARAMETRIC = nlohmann::json::parse(R"(\n',
+            "  {\n",
+        ]
+        for i, (key, val) in enumerate(config.items(), 1):
+            s_parametric.append(f'    "{key}": ' "{\n")
+            for j, (k2, v2) in enumerate(val.items(), 1):
+                v_str = f'"{v2}"' if isinstance(v2, str) else str(v2)
+                s_parametric.append(
+                    f'      "{k2}": {v_str}' + (",\n" if j < len(val) else "\n")
+                )
+            s_parametric.append("    }" f"{',' if i < len(config) else ''}\n")
+        s_parametric.append("  }\n")
+        s_parametric.append(')");\n')
+        return tuple(s_parametric)
+
+    def _export_input_output_args(self) -> Tuple[torch.Tensor]:
+        return (self._sidedoor_params_to_tensor(),)
+
+    def _forward(self, params, x):
+        """
+        :param params: (N,D)
+        :param x: (N,L1)
+
+        :return: (N,L2)
+        """
+        sequence_length = x.shape[1]
+        x_augmented = (
+            torch.cat(
+                [
+                    x[..., None],
+                    torch.tile(params[:, None, :], (1, sequence_length, 1)),
+                ],
+                dim=2,
+            )
+            if self._shape_type == _ShapeType.RNN
+            else torch.cat(
+                [x[:, None, :], torch.tile(params[..., None], (1, 1, sequence_length))],
+                dim=1,
+            )
+        )
+        return self._single_class._forward(self, x_augmented)
+
+    def _sidedoor_params_to_tensor(self) -> torch.Tensor:
+        param_names = sorted([k for k in self._sidedoor_parametric_config.keys()])
+        params = torch.Tensor(
+            [self._sidedoor_parametric_config[k].default_value for k in param_names]
+        )
+        return params
+
+    @contextmanager
+    def _use_parametric_config(self, c):
+        """
+        Sneaks in the parametric config while exporting
+        """
+        try:
+            self._sidedoor_parametric_config = c
+            yield None
+        finally:
+            self._sidedoor_parametric_config = None
+
+
+class CatLSTM(_CatMixin, LSTM):
+    @property
+    def _shape_type(self) -> _ShapeType:
+        return _ShapeType.RNN
+
+    @property
+    def _single_class(self):
+        return LSTM
+
+    def _append_default_params(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        Requires sidedoor'd params
+
+        :param x: (B,L)
+        :return: (B,L,1+D)
+        """
+        assert x.ndim == 2
+        params = self._sidedoor_params_to_tensor()
+        sequence_length = x.shape[1]
+        return torch.cat(
+            [
+                x[:, :, None],
+                torch.tile(params[None, None, :], (1, sequence_length, 1)),
+            ],
+            dim=2,
+        )
+
+    def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
+        if self._input_size != 1:
+            logger.warning(
+                "Nominal settings aren't defined for parametric models; outputting unity"
+            )
+            return x
+        params = torch.zeros(()).to(x.device)
+        return self(params, x)
+
+    def _get_initial_state(self) -> Tuple[torch.Tensor, torch.Tensor]:
+        inputs = self._append_default_params(torch.zeros((1, 48_000)))
+        return super()._get_initial_state(inputs=inputs)
+
+
+class CatWaveNet(_CatMixin, WaveNet):
+    @property
+    def _shape_type(self) -> _ShapeType:
+        return _ShapeType.CONV
+
+    @property
+    def _single_class(self):
+        return WaveNet
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/parametric/hyper_net.py` & `neural-amp-modeler-0.6.0/nam/models/parametric/hyper_net.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,559 +1,559 @@
-# File: hyper_net.py
-# Created Date: Sunday May 29th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-import abc
-import json
-import math
-from dataclasses import dataclass
-from enum import Enum
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Any, Callable, List, Optional, Tuple
-
-import numpy as np
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torch.nn.init import (
-    calculate_gain,
-    _calculate_correct_fan,
-    _calculate_fan_in_and_fan_out,
-)
-
-from ..._version import __version__
-from .._base import ParametricBaseNet
-
-
-class SpecialLayers(Enum):
-    CONV = "conv"
-    BATCHNORM = "batchnorm"
-
-
-@dataclass
-class LayerSpec:
-    """
-    Helps the hypernet
-    """
-
-    special_type: Optional[str]
-    shapes: Tuple[Tuple[int]]
-    norms: Tuple[float]
-    biases: Tuple[float]
-
-
-class _NetLayer(nn.Module, abc.ABC):
-    @abc.abstractproperty
-    def num_tensors(self) -> int:
-        pass
-
-    @abc.abstractmethod
-    def get_spec(self) -> LayerSpec:
-        pass
-
-
-class _Conv(nn.Conv1d, _NetLayer):
-    @property
-    def num_tensors(self):
-        return 2 if self.bias is not None else 1
-
-    def forward(self, params, inputs):
-        # Use depthwise convolution trick to process the convolutions together
-        cout, cin, kernel_size = self.weight.shape
-        n = len(params[0])
-        weight = params[0].reshape((n * cout, cin, kernel_size))  # (N, CinCout)
-        bias = params[1].flatten() if self.bias is not None else None
-        groups = n
-        return F.conv1d(
-            inputs.reshape((1, n * cin, -1)),
-            weight,
-            bias=bias,
-            stride=self.stride,
-            padding=self.padding,
-            dilation=self.dilation,
-            groups=groups,
-        ).reshape((n, cout, -1))
-
-    def get_spec(self):
-        shapes = (
-            (self.weight.shape,)
-            if self.bias is None
-            else (self.weight.shape, self.bias.shape)
-        )
-        norms = (
-            (self._weight_norm(),)
-            if self.bias is None
-            else (self._weight_norm(), self._bias_norm())
-        )
-        biases = (0,) if self.bias is None else (0, 0)
-        return LayerSpec(SpecialLayers("conv"), shapes, norms, biases)
-
-    def _bias_norm(self):
-        # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv1d
-        fan = _calculate_fan_in_and_fan_out(self.weight.data)[0]
-        bound = 1.0 / math.sqrt(fan)
-        std = math.sqrt(1.0 / 12.0) * (2 * bound)
-        # LayerNorm handles division by number of dimensions...
-        return std
-
-    def _weight_norm(self):
-        """
-        Std of the unfiorm distribution used in initialization
-        """
-        # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv1d
-        fan = _calculate_correct_fan(self.weight.data, "fan_in")
-        # Kaiming uniform w/ a=sqrt(5)
-        gain = calculate_gain("leaky_relu", 5.0)
-        std = gain / math.sqrt(fan)
-        # LayerNorm handles division by number of dimensions...
-        return std
-
-
-class _BatchNorm(nn.BatchNorm1d, _NetLayer):
-    def __init__(self, num_features, *args, affine=True, **kwargs):
-        # Handle affine params outside of parent class
-        super().__init__(num_features, *args, affine=False, **kwargs)
-        self._num_features = num_features
-        assert affine
-        self._affine = affine
-
-    @property
-    def num_tensors(self) -> int:
-        return 2
-
-    def get_spec(self) -> LayerSpec:
-        return LayerSpec(
-            SpecialLayers.BATCHNORM,
-            ((self._num_features,), (self._num_features,)),
-            (1.0e-5, 1.0e-5),
-            (1.0, 0.0),
-        )
-
-    def forward(self, params, inputs):
-        """
-        Only change is we need to provide *params into F.batch_norm instead of 
-        self.weight, self.bias
-        """
-        # Also use "inputs" instead of "input" to not collide w/ builtin (ew)
-        weight, bias = [z[:, :, None] for z in params]
-        pre_affine = super().forward(inputs)
-        return weight * pre_affine + bias
-
-
-class _Affine(nn.Module):
-    def __init__(self, scale: torch.Tensor, bias: torch.Tensor):
-        super().__init__()
-        self._weight = nn.Parameter(scale)
-        self._bias = nn.Parameter(bias)
-
-    @property
-    def bias(self) -> nn.Parameter:
-        return self._bias
-
-    @property
-    def weight(self) -> nn.Parameter:
-        return self._weight
-
-    def forward(self, inputs):
-        return self._weight * inputs + self._bias
-
-
-class HyperNet(nn.Module):
-    """
-    MLP followed by layer norms on split-up dims
-    """
-
-    def __init__(self, d_in, net, numels, norms, biases):
-        super().__init__()
-        self._net = net
-        # Figure out the scale factor empirically
-        norm0 = net(torch.randn((10_000, d_in))).std(dim=0).mean().item()
-        self._cum_numel = torch.cat(
-            [torch.LongTensor([0]), torch.cumsum(torch.LongTensor(numels), dim=0)]
-        )
-        affine_scale = torch.cat(
-            [torch.full((numel,), norm / norm0) for numel, norm in zip(numels, norms)]
-        )
-        affine_bias = torch.cat(
-            [
-                torch.full((numel,), bias, dtype=torch.float)
-                for numel, bias in zip(numels, biases)
-            ]
-        )
-        self._affine = _Affine(affine_scale, affine_bias)
-
-    @property
-    def batchnorm(self) -> bool:
-        """
-        Does the hypernet use batchnorm layers
-        """
-        return any(isinstance(m, nn.BatchNorm1d) for m in self.modules())
-
-    @property
-    def input_dim(self) -> int:
-        return self._net[0][0].weight.shape[1]
-
-    @property
-    def num_layers(self) -> int:
-        return len([layer for layer in self._net if isinstance(layer, _HyperNetBlock)])
-
-    @property
-    def num_units(self) -> int:
-        return self._net[0][0].weight.shape[0]
-
-    def forward(self, x) -> Tuple[torch.Tensor]:
-        """
-        Just return a flat array of param tensors for now
-        """
-        y = self._affine(self._net(x))
-        return tuple(
-            y[:, i:j] for i, j in zip(self._cum_numel[:-1], self._cum_numel[1:])
-        )
-
-    def get_export_params(self) -> np.ndarray:
-        params = []
-        for block in self._net[:-1]:
-            linear = block[0]
-            params.append(linear.weight.flatten())
-            params.append(linear.bias.flatten())
-            if self.batchnorm:
-                bn = block[1]
-                params.append(bn.running_mean.flatten())
-                params.append(bn.running_var.flatten())
-                params.append(bn.weight.flatten())
-                params.append(bn.bias.flatten())
-                params.append(torch.Tensor([bn.eps]).to(bn.weight.device))
-            assert len(block) <= 3, "Linear-(BN)-activation"
-            assert (
-                len([p for p in block[-1].parameters()]) == 0
-            ), "No params in activation"
-        head = self._net[-1]
-        params.append(head.weight.flatten())
-        params.append(head.bias.flatten())
-        affine = self._affine
-        params.append(affine.weight.flatten())
-        params.append(affine.bias.flatten())
-        return torch.cat(params).detach().cpu().numpy()
-
-
-class _Activation(abc.ABC):
-    """
-    Indicate that a module is an activation within the main net
-    """
-
-    @abc.abstractproperty
-    def name(self) -> str:
-        """
-        What to call the layer by when making a config w/ it
-        """
-        pass
-
-
-def _extend_activation(C, name: str) -> _Activation:
-    class Activation(C, _NetLayer, _Activation):
-        @property
-        def name(self):
-            return name
-
-        @property
-        def num_tensors(self) -> int:
-            return 0
-
-        def get_spec(self) -> LayerSpec:
-            return LayerSpec(None, (), (), ())
-
-        def forward(self, params, inputs):
-            return super().forward(inputs)
-
-    return Activation
-
-
-_Tanh = _extend_activation(nn.Tanh, "Tanh")
-_ReLU = _extend_activation(nn.ReLU, "ReLU")
-_Flatten = _extend_activation(nn.Flatten, "Flatten")  # Hah, works
-
-
-def _get_activation(name):
-    return {"Tanh": _Tanh, "ReLU": _ReLU}[name]()
-
-
-class _HyperNetBlock(nn.Sequential):
-    """
-    For IDing blocks of the hypernet
-    """
-
-    pass
-
-
-class HyperConvNet(ParametricBaseNet):
-    """
-    For parameteric data
-
-    Conditioning is input to a hypernetwork that outputs the parameters of the conv net.
-    """
-
-    def __init__(
-        self, hyper_net: HyperNet, net: Callable[[Any, torch.Tensor], torch.Tensor]
-    ):
-        super().__init__()
-        self._hyper_net = hyper_net
-        self._net = net
-
-    @classmethod
-    def parse_config(cls, config):
-        config = super().parse_config(config)
-        net, specs = cls._get_net(config["net"])
-        hyper_net = cls._get_hyper_net(config["hyper_net"], specs)
-        return {"hyper_net": hyper_net, "net": net}
-
-    @property
-    def pad_start_default(self) -> bool:
-        return True
-
-    @property
-    def receptive_field(self) -> int:
-        # Last conv is the collapser--compensate w/ a minus 1
-        return sum([m.dilation[0] for m in self._net if isinstance(m, _Conv)]) + 1 - 1
-
-    def export(self, outdir: Path, include_snapshot: bool=False):
-        """
-        Files created:
-        * config.json
-        * weights.npy
-        * test_signal_params.npy
-        * test_signal_input.npy
-        * test_signal_output.npy
-
-        weights are serialized to weights.npy in the following order:
-        * Hypernet
-            * Loop layers:
-                * Linear
-                    * weights (din*dout)
-                    * biases (dout)
-                * BN
-                    * running_mean (d)
-                    * running_var (d)
-                    * weight (d)
-                    * bias (d)
-                    * eps ()
-                * activation
-                    * (Assume no params bc Tanh)
-            * Linear out
-                * weights (units*dy)
-                * bias (dy)
-            * affine
-                * weights (dy)
-                * bias (dy)
-        * Main net
-            (Layers are conv-BN-act)
-            (All params are outputted by the hypernet except the BatchNorm buffers!)
-            * Loop layers
-                * BN
-                    * running_mean
-                    * running_var
-                    * eps ()
-        * (flatten: no params)
-
-        A test input & output are also provided, input.npy and output.npy
-        """
-        training = self.training
-        self.eval()
-        with open(Path(outdir, "config.json"), "w") as fp:
-            json.dump(self._export_config(), fp, indent=4)
-
-        # Hope I don't regret using np.save...
-        np.save(Path(outdir, "weights.npy"), self._export_weights())
-
-        # And an input/output to verify correct computation:
-        if include_snapshot:
-            params, x, y = self._export_input_output()
-            np.save(Path(outdir, "test_signal_params.npy"), params.detach().cpu().numpy())
-            np.save(Path(outdir, "test_signal_input.npy"), x.detach().cpu().numpy())
-            np.save(Path(outdir, "test_signal_output.npy"), y.detach().cpu().numpy())
-
-        # And resume training state
-        self.train(training)
-
-    def export_cpp_header(self, filename: Path):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir)
-            self.export(Path(tmpdir))
-            with open(Path(tmpdir, "config.json"), "r") as fp:
-                _c = json.load(fp)
-            version = _c["version"]
-            config = _c["config"]
-            params = np.load(Path(tmpdir, "weights.npy"))
-        with open(filename, "w") as f:
-            f.writelines(
-                (
-                    "#pragma once\n",
-                    "// Automatically-generated model file\n",
-                    "// HyperConvNet model\n" "#include <vector>\n",
-                    f'#define PYTHON_MODEL_VERSION "{version}"\n',
-                    f'const int HYPER_NET_INPUT_DIM = {config["hyper_net"]["input_dim"]};\n',
-                    f'const int HYPER_NET_NUM_LAYERS = {config["hyper_net"]["num_layers"]};\n',
-                    f'const int HYPER_NET_NUM_UNITS = {config["hyper_net"]["num_units"]};\n',
-                    f'const int HYPER_NET_BATCHNORM = {"true" if config["hyper_net"]["batchnorm"] else "false"};\n',
-                    f"const int CHANNELS = {config['net']['channels']};\n",
-                    f"const bool BATCHNORM = {'true' if config['net']['batchnorm'] else 'false'};\n",
-                    "std::vector<int> DILATIONS{"
-                    + ",".join([str(d) for d in config["net"]["dilations"]])
-                    + "};\n",
-                    f"const std::string ACTIVATION = \"{config['net']['activation']}\";\n",
-                    "std::vector<float> PARAMS{"
-                    + ",".join([f"{w:.16f}" for w in params])
-                    + "};\n",
-                )
-            )
-
-    @classmethod
-    def _get_net(cls, config):
-        channels = config["channels"]
-        dilations = config["dilations"]
-        batchnorm = config["batchnorm"]
-        activation = config["activation"]
-
-        layers = []
-        layer_specs = []
-        cin = 1
-        for dilation in dilations:
-            layer = _Conv(cin, channels, 2, dilation=dilation, bias=not batchnorm)
-            layers.append(layer)
-            layer_specs.append(layer.get_spec())
-            if batchnorm:
-                # Slow momentum on main net bc it's wild
-                layer = _BatchNorm(channels, momentum=0.01)
-                layers.append(layer)
-                layer_specs.append(layer.get_spec())
-            layer = _get_activation(activation)
-            layers.append(layer)
-            layer_specs.append(layer.get_spec())
-            cin = channels
-        layer = _Conv(cin, 1, 1)
-        layers.append(layer)
-        layer_specs.append(layer.get_spec())
-        layer = _Flatten()
-        layers.append(layer)
-        layer_specs.append(layer.get_spec())
-
-        return nn.ModuleList(layers), layer_specs
-
-    @classmethod
-    def _get_hyper_net(cls, config, specs) -> HyperNet:
-        def block(dx, dy, batchnorm) -> _HyperNetBlock:
-            layer_list = [nn.Linear(dx, dy)]
-            if batchnorm:
-                layer_list.append(nn.BatchNorm1d(dy))
-            layer_list.append(nn.ReLU())
-            return _HyperNetBlock(*layer_list)
-
-        num_inputs = config["num_inputs"]
-        num_layers = config["num_layers"]
-        num_units = config["num_units"]
-        batchnorm = config["batchnorm"]
-        # Flatten specs
-        numels = [np.prod(np.array(shape)) for spec in specs for shape in spec.shapes]
-        norms = [norm for spec in specs for norm in spec.norms]
-        biases = [bias for spec in specs for bias in spec.biases]
-        num_outputs = sum(numels)
-
-        din, layer_list = num_inputs, []
-        for _ in range(num_layers):
-            layer_list.append(block(din, num_units, batchnorm))
-            din = num_units
-        layer_list.append(nn.Linear(din, num_outputs))
-        net = nn.Sequential(*layer_list)
-
-        return HyperNet(num_inputs, net, numels, norms, biases)
-
-    @property
-    def _activation(self) -> str:
-        """
-        What activation does the main net use
-        """
-        for m in self._net.modules():
-            if isinstance(m, _Activation):
-                return m.name
-
-    @property
-    def _batchnorm(self) -> bool:
-        return any(isinstance(x, _BatchNorm) for x in self._net)
-
-    @property
-    def _channels(self) -> int:
-        return self._net[0].weight.shape[0]
-
-    @property
-    def _net_no_head(self):
-        return self._net[:-2]
-
-    def _forward(self, params: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
-        net_params = self._hyper_net(params)
-        i = 0
-        for m in self._net:
-            j = i + m.num_tensors
-            x = m(net_params[i:j], x)
-            i = j
-        assert j == len(net_params)
-        return x
-
-    def _get_dilations(self) -> List[int]:
-        dilations = []
-        for (
-            layer
-        ) in self._net_no_head:  # Last two layers are a 1D conv head and flatten
-            if isinstance(layer, _Conv):
-                dilations.append(layer.dilation[0])
-        return dilations
-
-    def _export_config(self):
-        return {
-            "version": __version__,
-            "architecture": "HyperConvNet",
-            "config": {
-                "hyper_net": {
-                    "input_dim": self._hyper_net.input_dim,
-                    "num_layers": self._hyper_net.num_layers,
-                    "num_units": self._hyper_net.num_units,
-                    "batchnorm": self._hyper_net.batchnorm,
-                },
-                "net": {
-                    "channels": self._channels,
-                    "dilations": self._get_dilations(),
-                    "batchnorm": self._batchnorm,
-                    "activation": self._activation,
-                },
-            },
-        }
-
-    def _export_weights(self) -> np.ndarray:
-        """
-        Flatten the parameters of the network to be exported.
-        See doctsring for .export() for ensured layout.
-        """
-        return np.concatenate(
-            [self._hyper_net.get_export_params(), self._export_net_weights()]
-        )
-
-    def _export_net_weights(self) -> np.ndarray:
-        """
-        Only the buffers--parameters are outputted by the hypernet!
-        """
-        params = []
-        for bn in self._net_no_head:
-            if isinstance(bn, _BatchNorm):
-                params.append(bn.running_mean.flatten())
-                params.append(bn.running_var.flatten())
-                params.append(torch.Tensor([bn.eps]).to(bn.running_mean.device))
-        return (
-            np.array([])
-            if len(params) == 0
-            else torch.cat(params).detach().cpu().numpy()
-        )
-
-    def _export_input_output(self) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        params = torch.randn((self._hyper_net.input_dim,))
-        x = torch.randn((2 * self.receptive_field,))
-        x = 0.5 * x / x.abs().max()
-        y = self(params, x)
-        return params, x, y
+# File: hyper_net.py
+# Created Date: Sunday May 29th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+import abc
+import json
+import math
+from dataclasses import dataclass
+from enum import Enum
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from typing import Any, Callable, List, Optional, Tuple
+
+import numpy as np
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from torch.nn.init import (
+    calculate_gain,
+    _calculate_correct_fan,
+    _calculate_fan_in_and_fan_out,
+)
+
+from ..._version import __version__
+from .._base import ParametricBaseNet
+
+
+class SpecialLayers(Enum):
+    CONV = "conv"
+    BATCHNORM = "batchnorm"
+
+
+@dataclass
+class LayerSpec:
+    """
+    Helps the hypernet
+    """
+
+    special_type: Optional[str]
+    shapes: Tuple[Tuple[int]]
+    norms: Tuple[float]
+    biases: Tuple[float]
+
+
+class _NetLayer(nn.Module, abc.ABC):
+    @abc.abstractproperty
+    def num_tensors(self) -> int:
+        pass
+
+    @abc.abstractmethod
+    def get_spec(self) -> LayerSpec:
+        pass
+
+
+class _Conv(nn.Conv1d, _NetLayer):
+    @property
+    def num_tensors(self):
+        return 2 if self.bias is not None else 1
+
+    def forward(self, params, inputs):
+        # Use depthwise convolution trick to process the convolutions together
+        cout, cin, kernel_size = self.weight.shape
+        n = len(params[0])
+        weight = params[0].reshape((n * cout, cin, kernel_size))  # (N, CinCout)
+        bias = params[1].flatten() if self.bias is not None else None
+        groups = n
+        return F.conv1d(
+            inputs.reshape((1, n * cin, -1)),
+            weight,
+            bias=bias,
+            stride=self.stride,
+            padding=self.padding,
+            dilation=self.dilation,
+            groups=groups,
+        ).reshape((n, cout, -1))
+
+    def get_spec(self):
+        shapes = (
+            (self.weight.shape,)
+            if self.bias is None
+            else (self.weight.shape, self.bias.shape)
+        )
+        norms = (
+            (self._weight_norm(),)
+            if self.bias is None
+            else (self._weight_norm(), self._bias_norm())
+        )
+        biases = (0,) if self.bias is None else (0, 0)
+        return LayerSpec(SpecialLayers("conv"), shapes, norms, biases)
+
+    def _bias_norm(self):
+        # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv1d
+        fan = _calculate_fan_in_and_fan_out(self.weight.data)[0]
+        bound = 1.0 / math.sqrt(fan)
+        std = math.sqrt(1.0 / 12.0) * (2 * bound)
+        # LayerNorm handles division by number of dimensions...
+        return std
+
+    def _weight_norm(self):
+        """
+        Std of the unfiorm distribution used in initialization
+        """
+        # https://pytorch.org/docs/stable/_modules/torch/nn/modules/conv.html#Conv1d
+        fan = _calculate_correct_fan(self.weight.data, "fan_in")
+        # Kaiming uniform w/ a=sqrt(5)
+        gain = calculate_gain("leaky_relu", 5.0)
+        std = gain / math.sqrt(fan)
+        # LayerNorm handles division by number of dimensions...
+        return std
+
+
+class _BatchNorm(nn.BatchNorm1d, _NetLayer):
+    def __init__(self, num_features, *args, affine=True, **kwargs):
+        # Handle affine params outside of parent class
+        super().__init__(num_features, *args, affine=False, **kwargs)
+        self._num_features = num_features
+        assert affine
+        self._affine = affine
+
+    @property
+    def num_tensors(self) -> int:
+        return 2
+
+    def get_spec(self) -> LayerSpec:
+        return LayerSpec(
+            SpecialLayers.BATCHNORM,
+            ((self._num_features,), (self._num_features,)),
+            (1.0e-5, 1.0e-5),
+            (1.0, 0.0),
+        )
+
+    def forward(self, params, inputs):
+        """
+        Only change is we need to provide *params into F.batch_norm instead of 
+        self.weight, self.bias
+        """
+        # Also use "inputs" instead of "input" to not collide w/ builtin (ew)
+        weight, bias = [z[:, :, None] for z in params]
+        pre_affine = super().forward(inputs)
+        return weight * pre_affine + bias
+
+
+class _Affine(nn.Module):
+    def __init__(self, scale: torch.Tensor, bias: torch.Tensor):
+        super().__init__()
+        self._weight = nn.Parameter(scale)
+        self._bias = nn.Parameter(bias)
+
+    @property
+    def bias(self) -> nn.Parameter:
+        return self._bias
+
+    @property
+    def weight(self) -> nn.Parameter:
+        return self._weight
+
+    def forward(self, inputs):
+        return self._weight * inputs + self._bias
+
+
+class HyperNet(nn.Module):
+    """
+    MLP followed by layer norms on split-up dims
+    """
+
+    def __init__(self, d_in, net, numels, norms, biases):
+        super().__init__()
+        self._net = net
+        # Figure out the scale factor empirically
+        norm0 = net(torch.randn((10_000, d_in))).std(dim=0).mean().item()
+        self._cum_numel = torch.cat(
+            [torch.LongTensor([0]), torch.cumsum(torch.LongTensor(numels), dim=0)]
+        )
+        affine_scale = torch.cat(
+            [torch.full((numel,), norm / norm0) for numel, norm in zip(numels, norms)]
+        )
+        affine_bias = torch.cat(
+            [
+                torch.full((numel,), bias, dtype=torch.float)
+                for numel, bias in zip(numels, biases)
+            ]
+        )
+        self._affine = _Affine(affine_scale, affine_bias)
+
+    @property
+    def batchnorm(self) -> bool:
+        """
+        Does the hypernet use batchnorm layers
+        """
+        return any(isinstance(m, nn.BatchNorm1d) for m in self.modules())
+
+    @property
+    def input_dim(self) -> int:
+        return self._net[0][0].weight.shape[1]
+
+    @property
+    def num_layers(self) -> int:
+        return len([layer for layer in self._net if isinstance(layer, _HyperNetBlock)])
+
+    @property
+    def num_units(self) -> int:
+        return self._net[0][0].weight.shape[0]
+
+    def forward(self, x) -> Tuple[torch.Tensor]:
+        """
+        Just return a flat array of param tensors for now
+        """
+        y = self._affine(self._net(x))
+        return tuple(
+            y[:, i:j] for i, j in zip(self._cum_numel[:-1], self._cum_numel[1:])
+        )
+
+    def get_export_params(self) -> np.ndarray:
+        params = []
+        for block in self._net[:-1]:
+            linear = block[0]
+            params.append(linear.weight.flatten())
+            params.append(linear.bias.flatten())
+            if self.batchnorm:
+                bn = block[1]
+                params.append(bn.running_mean.flatten())
+                params.append(bn.running_var.flatten())
+                params.append(bn.weight.flatten())
+                params.append(bn.bias.flatten())
+                params.append(torch.Tensor([bn.eps]).to(bn.weight.device))
+            assert len(block) <= 3, "Linear-(BN)-activation"
+            assert (
+                len([p for p in block[-1].parameters()]) == 0
+            ), "No params in activation"
+        head = self._net[-1]
+        params.append(head.weight.flatten())
+        params.append(head.bias.flatten())
+        affine = self._affine
+        params.append(affine.weight.flatten())
+        params.append(affine.bias.flatten())
+        return torch.cat(params).detach().cpu().numpy()
+
+
+class _Activation(abc.ABC):
+    """
+    Indicate that a module is an activation within the main net
+    """
+
+    @abc.abstractproperty
+    def name(self) -> str:
+        """
+        What to call the layer by when making a config w/ it
+        """
+        pass
+
+
+def _extend_activation(C, name: str) -> _Activation:
+    class Activation(C, _NetLayer, _Activation):
+        @property
+        def name(self):
+            return name
+
+        @property
+        def num_tensors(self) -> int:
+            return 0
+
+        def get_spec(self) -> LayerSpec:
+            return LayerSpec(None, (), (), ())
+
+        def forward(self, params, inputs):
+            return super().forward(inputs)
+
+    return Activation
+
+
+_Tanh = _extend_activation(nn.Tanh, "Tanh")
+_ReLU = _extend_activation(nn.ReLU, "ReLU")
+_Flatten = _extend_activation(nn.Flatten, "Flatten")  # Hah, works
+
+
+def _get_activation(name):
+    return {"Tanh": _Tanh, "ReLU": _ReLU}[name]()
+
+
+class _HyperNetBlock(nn.Sequential):
+    """
+    For IDing blocks of the hypernet
+    """
+
+    pass
+
+
+class HyperConvNet(ParametricBaseNet):
+    """
+    For parameteric data
+
+    Conditioning is input to a hypernetwork that outputs the parameters of the conv net.
+    """
+
+    def __init__(
+        self, hyper_net: HyperNet, net: Callable[[Any, torch.Tensor], torch.Tensor]
+    ):
+        super().__init__()
+        self._hyper_net = hyper_net
+        self._net = net
+
+    @classmethod
+    def parse_config(cls, config):
+        config = super().parse_config(config)
+        net, specs = cls._get_net(config["net"])
+        hyper_net = cls._get_hyper_net(config["hyper_net"], specs)
+        return {"hyper_net": hyper_net, "net": net}
+
+    @property
+    def pad_start_default(self) -> bool:
+        return True
+
+    @property
+    def receptive_field(self) -> int:
+        # Last conv is the collapser--compensate w/ a minus 1
+        return sum([m.dilation[0] for m in self._net if isinstance(m, _Conv)]) + 1 - 1
+
+    def export(self, outdir: Path, include_snapshot: bool=False):
+        """
+        Files created:
+        * config.json
+        * weights.npy
+        * test_signal_params.npy
+        * test_signal_input.npy
+        * test_signal_output.npy
+
+        weights are serialized to weights.npy in the following order:
+        * Hypernet
+            * Loop layers:
+                * Linear
+                    * weights (din*dout)
+                    * biases (dout)
+                * BN
+                    * running_mean (d)
+                    * running_var (d)
+                    * weight (d)
+                    * bias (d)
+                    * eps ()
+                * activation
+                    * (Assume no params bc Tanh)
+            * Linear out
+                * weights (units*dy)
+                * bias (dy)
+            * affine
+                * weights (dy)
+                * bias (dy)
+        * Main net
+            (Layers are conv-BN-act)
+            (All params are outputted by the hypernet except the BatchNorm buffers!)
+            * Loop layers
+                * BN
+                    * running_mean
+                    * running_var
+                    * eps ()
+        * (flatten: no params)
+
+        A test input & output are also provided, input.npy and output.npy
+        """
+        training = self.training
+        self.eval()
+        with open(Path(outdir, "config.json"), "w") as fp:
+            json.dump(self._export_config(), fp, indent=4)
+
+        # Hope I don't regret using np.save...
+        np.save(Path(outdir, "weights.npy"), self._export_weights())
+
+        # And an input/output to verify correct computation:
+        if include_snapshot:
+            params, x, y = self._export_input_output()
+            np.save(Path(outdir, "test_signal_params.npy"), params.detach().cpu().numpy())
+            np.save(Path(outdir, "test_signal_input.npy"), x.detach().cpu().numpy())
+            np.save(Path(outdir, "test_signal_output.npy"), y.detach().cpu().numpy())
+
+        # And resume training state
+        self.train(training)
+
+    def export_cpp_header(self, filename: Path):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir)
+            self.export(Path(tmpdir))
+            with open(Path(tmpdir, "config.json"), "r") as fp:
+                _c = json.load(fp)
+            version = _c["version"]
+            config = _c["config"]
+            params = np.load(Path(tmpdir, "weights.npy"))
+        with open(filename, "w") as f:
+            f.writelines(
+                (
+                    "#pragma once\n",
+                    "// Automatically-generated model file\n",
+                    "// HyperConvNet model\n" "#include <vector>\n",
+                    f'#define PYTHON_MODEL_VERSION "{version}"\n',
+                    f'const int HYPER_NET_INPUT_DIM = {config["hyper_net"]["input_dim"]};\n',
+                    f'const int HYPER_NET_NUM_LAYERS = {config["hyper_net"]["num_layers"]};\n',
+                    f'const int HYPER_NET_NUM_UNITS = {config["hyper_net"]["num_units"]};\n',
+                    f'const int HYPER_NET_BATCHNORM = {"true" if config["hyper_net"]["batchnorm"] else "false"};\n',
+                    f"const int CHANNELS = {config['net']['channels']};\n",
+                    f"const bool BATCHNORM = {'true' if config['net']['batchnorm'] else 'false'};\n",
+                    "std::vector<int> DILATIONS{"
+                    + ",".join([str(d) for d in config["net"]["dilations"]])
+                    + "};\n",
+                    f"const std::string ACTIVATION = \"{config['net']['activation']}\";\n",
+                    "std::vector<float> PARAMS{"
+                    + ",".join([f"{w:.16f}" for w in params])
+                    + "};\n",
+                )
+            )
+
+    @classmethod
+    def _get_net(cls, config):
+        channels = config["channels"]
+        dilations = config["dilations"]
+        batchnorm = config["batchnorm"]
+        activation = config["activation"]
+
+        layers = []
+        layer_specs = []
+        cin = 1
+        for dilation in dilations:
+            layer = _Conv(cin, channels, 2, dilation=dilation, bias=not batchnorm)
+            layers.append(layer)
+            layer_specs.append(layer.get_spec())
+            if batchnorm:
+                # Slow momentum on main net bc it's wild
+                layer = _BatchNorm(channels, momentum=0.01)
+                layers.append(layer)
+                layer_specs.append(layer.get_spec())
+            layer = _get_activation(activation)
+            layers.append(layer)
+            layer_specs.append(layer.get_spec())
+            cin = channels
+        layer = _Conv(cin, 1, 1)
+        layers.append(layer)
+        layer_specs.append(layer.get_spec())
+        layer = _Flatten()
+        layers.append(layer)
+        layer_specs.append(layer.get_spec())
+
+        return nn.ModuleList(layers), layer_specs
+
+    @classmethod
+    def _get_hyper_net(cls, config, specs) -> HyperNet:
+        def block(dx, dy, batchnorm) -> _HyperNetBlock:
+            layer_list = [nn.Linear(dx, dy)]
+            if batchnorm:
+                layer_list.append(nn.BatchNorm1d(dy))
+            layer_list.append(nn.ReLU())
+            return _HyperNetBlock(*layer_list)
+
+        num_inputs = config["num_inputs"]
+        num_layers = config["num_layers"]
+        num_units = config["num_units"]
+        batchnorm = config["batchnorm"]
+        # Flatten specs
+        numels = [np.prod(np.array(shape)) for spec in specs for shape in spec.shapes]
+        norms = [norm for spec in specs for norm in spec.norms]
+        biases = [bias for spec in specs for bias in spec.biases]
+        num_outputs = sum(numels)
+
+        din, layer_list = num_inputs, []
+        for _ in range(num_layers):
+            layer_list.append(block(din, num_units, batchnorm))
+            din = num_units
+        layer_list.append(nn.Linear(din, num_outputs))
+        net = nn.Sequential(*layer_list)
+
+        return HyperNet(num_inputs, net, numels, norms, biases)
+
+    @property
+    def _activation(self) -> str:
+        """
+        What activation does the main net use
+        """
+        for m in self._net.modules():
+            if isinstance(m, _Activation):
+                return m.name
+
+    @property
+    def _batchnorm(self) -> bool:
+        return any(isinstance(x, _BatchNorm) for x in self._net)
+
+    @property
+    def _channels(self) -> int:
+        return self._net[0].weight.shape[0]
+
+    @property
+    def _net_no_head(self):
+        return self._net[:-2]
+
+    def _forward(self, params: torch.Tensor, x: torch.Tensor) -> torch.Tensor:
+        net_params = self._hyper_net(params)
+        i = 0
+        for m in self._net:
+            j = i + m.num_tensors
+            x = m(net_params[i:j], x)
+            i = j
+        assert j == len(net_params)
+        return x
+
+    def _get_dilations(self) -> List[int]:
+        dilations = []
+        for (
+            layer
+        ) in self._net_no_head:  # Last two layers are a 1D conv head and flatten
+            if isinstance(layer, _Conv):
+                dilations.append(layer.dilation[0])
+        return dilations
+
+    def _export_config(self):
+        return {
+            "version": __version__,
+            "architecture": "HyperConvNet",
+            "config": {
+                "hyper_net": {
+                    "input_dim": self._hyper_net.input_dim,
+                    "num_layers": self._hyper_net.num_layers,
+                    "num_units": self._hyper_net.num_units,
+                    "batchnorm": self._hyper_net.batchnorm,
+                },
+                "net": {
+                    "channels": self._channels,
+                    "dilations": self._get_dilations(),
+                    "batchnorm": self._batchnorm,
+                    "activation": self._activation,
+                },
+            },
+        }
+
+    def _export_weights(self) -> np.ndarray:
+        """
+        Flatten the parameters of the network to be exported.
+        See doctsring for .export() for ensured layout.
+        """
+        return np.concatenate(
+            [self._hyper_net.get_export_params(), self._export_net_weights()]
+        )
+
+    def _export_net_weights(self) -> np.ndarray:
+        """
+        Only the buffers--parameters are outputted by the hypernet!
+        """
+        params = []
+        for bn in self._net_no_head:
+            if isinstance(bn, _BatchNorm):
+                params.append(bn.running_mean.flatten())
+                params.append(bn.running_var.flatten())
+                params.append(torch.Tensor([bn.eps]).to(bn.running_mean.device))
+        return (
+            np.array([])
+            if len(params) == 0
+            else torch.cat(params).detach().cpu().numpy()
+        )
+
+    def _export_input_output(self) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        params = torch.randn((self._hyper_net.input_dim,))
+        x = torch.randn((2 * self.receptive_field,))
+        x = 0.5 * x / x.abs().max()
+        y = self(params, x)
+        return params, x, y
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/parametric/params.py` & `neural-amp-modeler-0.6.0/nam/models/parametric/params.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# File: params.py
-# Created Date: Sunday July 17th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Handling parametric inputs
-"""
-
-import abc
-import inspect
-from dataclasses import dataclass, fields
-from enum import Enum
-from typing import Any
-
-from ..._core import InitializableFromConfig
-
-
-# class ParamType(Enum):
-#     CONTINUOUS = "continuous"
-#     BOOLEAN = "boolean"
-
-
-@dataclass
-class Param(InitializableFromConfig):
-    default_value: Any
-
-    @classmethod
-    def init_from_config(cls, config):
-        C, kwargs = cls.parse_config(config)
-        return C(**kwargs)
-
-    @classmethod
-    def parse_config(cls, config):
-        for C in [
-            _C
-            for _C in globals().values()
-            if inspect.isclass(_C) and _C is not Param and issubclass(_C, Param)
-        ]:
-            if C.typestr() == config["type"]:
-                config.pop("type")
-                break
-        else:
-            raise ValueError(f"Unrecognized aprameter type {config['type']}")
-        return C, config
-
-    @abc.abstractclassmethod
-    def typestr(cls) -> str:
-        pass
-
-    def to_json(self):
-        return {
-            "type": self.typestr(),
-            **{f.name: getattr(self, f.name) for f in fields(self)},
-        }
-
-
-@dataclass
-class BooleanParam(Param):
-    @classmethod
-    def typestr(cls) -> str:
-        return "boolean"
-
-
-@dataclass
-class ContinuousParam(Param):
-    minval: float
-    maxval: float
-
-    @classmethod
-    def typestr(self) -> str:
-        return "continuous"
+# File: params.py
+# Created Date: Sunday July 17th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Handling parametric inputs
+"""
+
+import abc
+import inspect
+from dataclasses import dataclass, fields
+from enum import Enum
+from typing import Any
+
+from ..._core import InitializableFromConfig
+
+
+# class ParamType(Enum):
+#     CONTINUOUS = "continuous"
+#     BOOLEAN = "boolean"
+
+
+@dataclass
+class Param(InitializableFromConfig):
+    default_value: Any
+
+    @classmethod
+    def init_from_config(cls, config):
+        C, kwargs = cls.parse_config(config)
+        return C(**kwargs)
+
+    @classmethod
+    def parse_config(cls, config):
+        for C in [
+            _C
+            for _C in globals().values()
+            if inspect.isclass(_C) and _C is not Param and issubclass(_C, Param)
+        ]:
+            if C.typestr() == config["type"]:
+                config.pop("type")
+                break
+        else:
+            raise ValueError(f"Unrecognized aprameter type {config['type']}")
+        return C, config
+
+    @abc.abstractclassmethod
+    def typestr(cls) -> str:
+        pass
+
+    def to_json(self):
+        return {
+            "type": self.typestr(),
+            **{f.name: getattr(self, f.name) for f in fields(self)},
+        }
+
+
+@dataclass
+class BooleanParam(Param):
+    @classmethod
+    def typestr(cls) -> str:
+        return "boolean"
+
+
+@dataclass
+class ContinuousParam(Param):
+    minval: float
+    maxval: float
+
+    @classmethod
+    def typestr(self) -> str:
+        return "continuous"
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/recurrent.py` & `neural-amp-modeler-0.6.0/nam/models/recurrent.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,469 +1,469 @@
-# File: recurrent.py
-# Created Date: Saturday July 2nd 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-Recurrent models (LSTM)
-
-TODO batch_first=False (I get it...)
-"""
-
-import json
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Optional, Tuple
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-from ._base import BaseNet
-
-
-# TODO merge LSTMCore into LSTM
-
-
-class _L(nn.LSTM):
-    """
-    Tweaks to PyTorch LSTM module
-    * Up the remembering
-    """
-
-    def reset_parameters(self) -> None:
-        super().reset_parameters()
-        # https://danijar.com/tips-for-training-recurrent-neural-networks/
-        # forget += 1
-        # ifgo
-        value = 2.0
-        idx_input = slice(0, self.hidden_size)
-        idx_forget = slice(self.hidden_size, 2 * self.hidden_size)
-        for layer in range(self.num_layers):
-            for input in ("i", "h"):
-                # Balance out the scale of the cell w/ a -=1
-                getattr(self, f"bias_{input}h_l{layer}").data[idx_input] -= value
-                getattr(self, f"bias_{input}h_l{layer}").data[idx_forget] += value
-
-
-# State:
-# L: Number of LSTM layers
-# DH: Hidden state dimension
-# [0]: hidden (L,DH)
-# [1]: cell (L,DH)
-_LSTMHiddenType = torch.Tensor
-_LSTMCellType = torch.Tensor
-_LSTMHiddenCellType = Tuple[_LSTMHiddenType, _LSTMCellType]
-
-
-class LSTMCore(_L):
-    def __init__(
-        self,
-        *args,
-        train_burn_in: Optional[int] = None,
-        train_truncate: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
-        if not self.batch_first:
-            raise NotImplementedError("Need batch first")
-        self._train_burn_in = train_burn_in
-        self._train_truncate = train_truncate
-        assert len(args) < 3, "Provide as kwargs"
-        self._initial_cell = nn.Parameter(
-            torch.zeros((self.num_layers, self.hidden_size))
-        )
-        self._initial_hidden = nn.Parameter(
-            torch.zeros((self.num_layers, self.hidden_size))
-        )
-
-    def forward(self, x, hidden_state=None):
-        """
-        Same as nn.LSTM.forward except:
-        * Learned inital state
-        * truncated BPTT when .training
-        """
-        if x.ndim != 3:
-            raise NotImplementedError("Need (B,L,D)")
-        last_hidden_state = (
-            self._initial_state(None if x.ndim == 2 else len(x))
-            if hidden_state is None
-            else hidden_state
-        )
-        if not self.training or self._train_truncate is None:
-            output_features = super().forward(x, last_hidden_state)[0]
-        else:
-            output_features_list = []
-            if self._train_burn_in is not None:
-                last_output_features, last_hidden_state = super().forward(
-                    x[:, : self._train_burn_in, :], last_hidden_state
-                )
-                output_features_list.append(last_output_features.detach())
-            burn_in_offset = 0 if self._train_burn_in is None else self._train_burn_in
-            for i in range(burn_in_offset, x.shape[1], self._train_truncate):
-                if i > burn_in_offset:
-                    # Don't detach the burn-in state so that we can learn it.
-                    last_hidden_state = tuple(z.detach() for z in last_hidden_state)
-                last_output_features, last_hidden_state = super().forward(
-                    x[:, i : i + self._train_truncate, :], last_hidden_state
-                )
-                output_features_list.append(last_output_features)
-            output_features = torch.cat(output_features_list, dim=1)
-        return output_features
-
-    def _initial_state(self, n: Optional[int]) -> _LSTMHiddenCellType:
-        return (
-            (self._initial_hidden, self._initial_cell)
-            if n is None
-            else (
-                torch.tile(self._initial_hidden[:, None], (1, n, 1)),
-                torch.tile(self._initial_cell[:, None], (1, n, 1)),
-            )
-        )
-
-
-class LSTM(BaseNet):
-    """
-    ABC for recurrent architectures
-    """
-
-    def __init__(
-        self,
-        hidden_size,
-        train_burn_in: Optional[int] = None,
-        train_truncate: Optional[int] = None,
-        input_size: int = 1,
-        **lstm_kwargs,
-    ):
-        """
-        :param hidden_size: for LSTM
-        :param train_burn_in: Detach calculations from first (this many) samples when
-            training to burn in the hidden state.
-        :param train_truncate: detach the hidden & cell states every this many steps
-            during training so that backpropagation through time is faster + to simulate
-            better starting states for h(t0)&c(t0) (instead of zeros)
-            TODO recognition head to start the hidden state in a good place?
-        :param input_size: Usually 1 (mono input). A catnet extending this might change
-            it and provide the parametric inputs as additional input dimensions.
-        """
-        super().__init__()
-        if "batch_first" in lstm_kwargs:
-            raise ValueError("batch_first cannot be set.")
-        self._input_size = input_size
-        self._core = _L(self._input_size, hidden_size, batch_first=True, **lstm_kwargs)
-        self._head = nn.Linear(hidden_size, 1)
-        self._train_burn_in = train_burn_in
-        self._train_truncate = train_truncate
-        self._initial_cell = nn.Parameter(
-            torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
-        )
-        self._initial_hidden = nn.Parameter(
-            torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
-        )
-
-    @property
-    def receptive_field(self) -> int:
-        return 1
-
-    @property
-    def pad_start_default(self) -> bool:
-        # I should simplify this...
-        return True
-
-    def export_cpp_header(self, filename: Path):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir)
-            LSTM.export(self, Path(tmpdir))  # Hacky...need to work w/ CatLSTM
-            with open(Path(tmpdir, "model.nam"), "r") as fp:
-                _c = json.load(fp)
-            version = _c["version"]
-            config = _c["config"]
-            s_parametric = self._export_cpp_header_parametric(config.get("parametric"))
-            with open(filename, "w") as f:
-                f.writelines(
-                    (
-                        "#pragma once\n",
-                        "// Automatically-generated model file\n",
-                        "#include <vector>\n",
-                        '#include "json.hpp"\n',
-                        '#include "lstm.h"\n',
-                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
-                        f'const int NUM_LAYERS = {config["num_layers"]};\n',
-                        f'const int INPUT_SIZE = {config["input_size"]};\n',
-                        f'const int HIDDEN_SIZE = {config["hidden_size"]};\n',
-                    )
-                    + s_parametric
-                    + (
-                        "std::vector<float> PARAMS{"
-                        + ", ".join([f"{w:.16f}f" for w in _c["weights"]])
-                        + "};\n",
-                    )
-                )
-
-    def export_onnx(self, filename: Path):
-        if self._input_size != 1:
-            raise NotImplementedError("Multi-dimensional inputs not supported yet")
-        o = _ONNXWrapped(self)
-        x = torch.randn((64,))  # (S,)
-        h, c = [z[:, 0, :] for z in self._initial_state(1)]  # (L,DH), (L,DH)
-        torch.onnx.export(
-            o,
-            (x, h, c),
-            filename,
-            input_names=["x", "hin", "cin"],
-            output_names=["y", "hout", "cout"],
-            dynamic_axes={"x": {0: "num_frames"}, "y": {0: "num_frames"}},
-        )
-
-    def forward_onnx(
-        self, x: torch.Tensor, h: _LSTMHiddenType, c: _LSTMCellType
-    ) -> Tuple[torch.Tensor, _LSTMHiddenType, _LSTMCellType]:
-        """
-        Forward pass used by ONNX export
-        Only supports scalar inputs right now.
-
-        N: Sequeence length
-        L: Number of layers
-        DH: Hidden state dimension
-
-        :param x: (N,)
-        :param state: (L, DH)
-        :param cell: (L, DH)
-
-        :return: (N,), (L, DH), (L, DH)
-        """
-        features, (h, c) = self._core(x[None, :, None], (h[:, None, :], c[:, None, :]))
-        y = self._apply_head(features)  # (1,S)
-        return y[0, :], h[:, 0, :], c[:, 0, :]
-
-    def _apply_head(self, features: torch.Tensor) -> torch.Tensor:
-        """
-        :param features: (B,S,DH)
-        :return: (B,S)
-        """
-        return self._head(features)[:, :, 0]
-
-    def _forward(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        :param x: (B,L) or (B,L,D)
-        :return: (B,L)
-        """
-        last_hidden_state = self._initial_state(len(x))
-        if x.ndim == 2:
-            x = x[:, :, None]
-        if not self.training or self._train_truncate is None:
-            output_features = self._core(x, last_hidden_state)[0]
-        else:
-            output_features_list = []
-            if self._train_burn_in is not None:
-                last_output_features, last_hidden_state = self._core(
-                    x[:, : self._train_burn_in, :], last_hidden_state
-                )
-                output_features_list.append(last_output_features.detach())
-            burn_in_offset = 0 if self._train_burn_in is None else self._train_burn_in
-            for i in range(burn_in_offset, x.shape[1], self._train_truncate):
-                if i > burn_in_offset:
-                    # Don't detach the burn-in state so that we can learn it.
-                    last_hidden_state = tuple(z.detach() for z in last_hidden_state)
-                last_output_features, last_hidden_state = self._core(
-                    x[:, i : i + self._train_truncate, :], last_hidden_state
-                )
-                output_features_list.append(last_output_features)
-            output_features = torch.cat(output_features_list, dim=1)
-        return self._apply_head(output_features)
-
-    def _export_cell_weights(
-        self, i: int, hidden_state: torch.Tensor, cell_state: torch.Tensor
-    ) -> np.ndarray:
-        """
-        * weight matrix (xh -> ifco)
-        * bias vector
-        * Initial hidden state
-        * Initial cell state
-        """
-
-        tensors = [
-            torch.cat(
-                [
-                    getattr(self._core, f"weight_ih_l{i}").data,
-                    getattr(self._core, f"weight_hh_l{i}").data,
-                ],
-                dim=1,
-            ),
-            getattr(self._core, f"bias_ih_l{i}").data
-            + getattr(self._core, f"bias_hh_l{i}").data,
-            hidden_state,
-            cell_state,
-        ]
-        return np.concatenate([z.detach().cpu().numpy().flatten() for z in tensors])
-
-    def _export_config(self):
-        return {
-            "input_size": self._core.input_size,
-            "hidden_size": self._core.hidden_size,
-            "num_layers": self._core.num_layers,
-        }
-
-    def _export_cpp_header_parametric(self, config):
-        # TODO refactor to merge w/ WaveNet implementation
-        if config is not None:
-            raise ValueError("Got non-None parametric config")
-        return ("nlohmann::json PARAMETRIC {};\n",)
-
-    def _export_weights(self):
-        """
-        * Loop over cells:
-            * weight matrix (xh -> ifco)
-            * bias vector
-            * Initial hidden state
-            * Initial cell state
-        * Head weights
-        * Head bias
-        """
-        return np.concatenate(
-            [
-                self._export_cell_weights(i, h, c)
-                for i, (h, c) in enumerate(zip(*self._get_initial_state()))
-            ]
-            + [
-                self._head.weight.data.detach().cpu().numpy().flatten(),
-                self._head.bias.data.detach().cpu().numpy().flatten(),
-            ]
-        )
-
-    def _get_initial_state(self, inputs=None) -> _LSTMHiddenCellType:
-        """
-        Convenience function to find a good hidden state to start the plugin at
-
-        DX=input size
-        L=num layers
-        S=sequence length
-        :param inputs: (1,S,DX)
-
-        :return: (L,DH), (L,DH)
-        """
-        inputs = torch.zeros((1, 48_000, 1)) if inputs is None else inputs
-        _, (h, c) = self._core(inputs)
-        return h, c
-
-    def _initial_state(self, n: Optional[int]) -> _LSTMHiddenCellType:
-        """
-        Literally what the forward pass starts with.
-        Default is zeroes; this should be better since it can be learned.
-        """
-        return (
-            (self._initial_hidden, self._initial_cell)
-            if n is None
-            else (
-                torch.tile(self._initial_hidden[:, None], (1, n, 1)),
-                torch.tile(self._initial_cell[:, None], (1, n, 1)),
-            )
-        )
-
-
-class _ONNXWrapped(nn.Module):
-    def __init__(self, net: LSTM):
-        super().__init__()
-        self._net = net
-
-    def forward(
-        self, x: torch.Tensor, hidden: _LSTMHiddenType, cell: _LSTMCellType
-    ) -> Tuple[torch.Tensor, _LSTMHiddenType, _LSTMCellType]:
-        """
-        N: Sequeence length
-        L: Number of layers
-        DH: Hidden state dimension
-
-        :param x: (N,)
-        :param state: (L, DH)
-        :param cell: (L, DH)
-
-        :return: (N,), (L, DH), (L, DH)
-        """
-        return self._net.forward_onnx(x, hidden, cell)
-
-
-# TODO refactor together
-
-
-class _SkippyLSTM(nn.Module):
-    def __init__(
-        self, input_size, hidden_size, skip_in: bool = False, num_layers=1, **kwargs
-    ):
-        super().__init__()
-        layers_per_lstm = 1
-        self._skip_in = skip_in
-        self._lstms = nn.ModuleList(
-            [
-                _L(
-                    self._layer_input_size(input_size, hidden_size, i),
-                    hidden_size,
-                    layers_per_lstm,
-                    batch_first=True,
-                )
-                for i in range(num_layers)
-            ]
-        )
-        self._initial_hidden = nn.Parameter(
-            torch.zeros((self.num_layers, layers_per_lstm, self.hidden_size))
-        )
-        self._initial_cell = nn.Parameter(
-            torch.zeros((self.num_layers, layers_per_lstm, self.hidden_size))
-        )
-
-    @property
-    def hidden_size(self):
-        return self._lstms[0].hidden_size
-
-    @property
-    def input_size(self):
-        return self._lstms[0].input_size
-
-    @property
-    def num_layers(self):
-        return len(self._lstms)
-
-    @property
-    def output_size(self):
-        return self.num_layers * self.hidden_size
-
-    def forward(self, input, state=None):
-        """
-        :param input: (N,L,DX)
-        :param state: ((L,Li,N,DH), (L,Li,N,DH))
-
-        :return: (N,L,L*DH), ((L,Li,N,DH), (L,Li,N,DH))
-        """
-        h0, c0 = self.initial_state(input) if state is None else state
-        hiddens, h_arr, c_arr, hidden = [], [], [], None
-        for layer, h0i, c0i in zip(self._lstms, h0, c0):
-            if self._skip_in:
-                # TODO dense-block
-                layer_input = (
-                    input if hidden is None else torch.cat([input, hidden], dim=2)
-                )
-            else:
-                layer_input = input if hidden is None else hidden
-            hidden, (hi, ci) = layer(layer_input, (h0i, c0i))
-            hiddens.append(hidden)
-            h_arr.append(hi)
-            c_arr.append(ci)
-        return (torch.cat(hiddens, dim=2), (torch.stack(h_arr), torch.stack(c_arr)))
-
-    def initial_state(self, input: torch.Tensor):
-        """
-        Initial states for all the layers
-
-        :return: (L,B,Li,DH)
-        """
-        assert input.ndim == 3, "Batch only for now"
-        batch_size = len(input)  # Assume batch_first
-        return (
-            torch.tile(self._initial_hidden[:, :, None], (1, 1, batch_size, 1)),
-            torch.tile(self._initial_cell[:, :, None], (1, 1, batch_size, 1)),
-        )
-
-    def _layer_input_size(self, input_size, hidden_size, i) -> int:
-        # TODO dense-block
-        if self._skip_in:
-            return input_size + (0 if i == 0 else hidden_size)
-        else:
-            return input_size if i == 0 else hidden_size
+# File: recurrent.py
+# Created Date: Saturday July 2nd 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+Recurrent models (LSTM)
+
+TODO batch_first=False (I get it...)
+"""
+
+import json
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from typing import Optional, Tuple
+
+import numpy as np
+import torch
+import torch.nn as nn
+
+from ._base import BaseNet
+
+
+# TODO merge LSTMCore into LSTM
+
+
+class _L(nn.LSTM):
+    """
+    Tweaks to PyTorch LSTM module
+    * Up the remembering
+    """
+
+    def reset_parameters(self) -> None:
+        super().reset_parameters()
+        # https://danijar.com/tips-for-training-recurrent-neural-networks/
+        # forget += 1
+        # ifgo
+        value = 2.0
+        idx_input = slice(0, self.hidden_size)
+        idx_forget = slice(self.hidden_size, 2 * self.hidden_size)
+        for layer in range(self.num_layers):
+            for input in ("i", "h"):
+                # Balance out the scale of the cell w/ a -=1
+                getattr(self, f"bias_{input}h_l{layer}").data[idx_input] -= value
+                getattr(self, f"bias_{input}h_l{layer}").data[idx_forget] += value
+
+
+# State:
+# L: Number of LSTM layers
+# DH: Hidden state dimension
+# [0]: hidden (L,DH)
+# [1]: cell (L,DH)
+_LSTMHiddenType = torch.Tensor
+_LSTMCellType = torch.Tensor
+_LSTMHiddenCellType = Tuple[_LSTMHiddenType, _LSTMCellType]
+
+
+class LSTMCore(_L):
+    def __init__(
+        self,
+        *args,
+        train_burn_in: Optional[int] = None,
+        train_truncate: Optional[int] = None,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        if not self.batch_first:
+            raise NotImplementedError("Need batch first")
+        self._train_burn_in = train_burn_in
+        self._train_truncate = train_truncate
+        assert len(args) < 3, "Provide as kwargs"
+        self._initial_cell = nn.Parameter(
+            torch.zeros((self.num_layers, self.hidden_size))
+        )
+        self._initial_hidden = nn.Parameter(
+            torch.zeros((self.num_layers, self.hidden_size))
+        )
+
+    def forward(self, x, hidden_state=None):
+        """
+        Same as nn.LSTM.forward except:
+        * Learned inital state
+        * truncated BPTT when .training
+        """
+        if x.ndim != 3:
+            raise NotImplementedError("Need (B,L,D)")
+        last_hidden_state = (
+            self._initial_state(None if x.ndim == 2 else len(x))
+            if hidden_state is None
+            else hidden_state
+        )
+        if not self.training or self._train_truncate is None:
+            output_features = super().forward(x, last_hidden_state)[0]
+        else:
+            output_features_list = []
+            if self._train_burn_in is not None:
+                last_output_features, last_hidden_state = super().forward(
+                    x[:, : self._train_burn_in, :], last_hidden_state
+                )
+                output_features_list.append(last_output_features.detach())
+            burn_in_offset = 0 if self._train_burn_in is None else self._train_burn_in
+            for i in range(burn_in_offset, x.shape[1], self._train_truncate):
+                if i > burn_in_offset:
+                    # Don't detach the burn-in state so that we can learn it.
+                    last_hidden_state = tuple(z.detach() for z in last_hidden_state)
+                last_output_features, last_hidden_state = super().forward(
+                    x[:, i : i + self._train_truncate, :], last_hidden_state
+                )
+                output_features_list.append(last_output_features)
+            output_features = torch.cat(output_features_list, dim=1)
+        return output_features
+
+    def _initial_state(self, n: Optional[int]) -> _LSTMHiddenCellType:
+        return (
+            (self._initial_hidden, self._initial_cell)
+            if n is None
+            else (
+                torch.tile(self._initial_hidden[:, None], (1, n, 1)),
+                torch.tile(self._initial_cell[:, None], (1, n, 1)),
+            )
+        )
+
+
+class LSTM(BaseNet):
+    """
+    ABC for recurrent architectures
+    """
+
+    def __init__(
+        self,
+        hidden_size,
+        train_burn_in: Optional[int] = None,
+        train_truncate: Optional[int] = None,
+        input_size: int = 1,
+        **lstm_kwargs,
+    ):
+        """
+        :param hidden_size: for LSTM
+        :param train_burn_in: Detach calculations from first (this many) samples when
+            training to burn in the hidden state.
+        :param train_truncate: detach the hidden & cell states every this many steps
+            during training so that backpropagation through time is faster + to simulate
+            better starting states for h(t0)&c(t0) (instead of zeros)
+            TODO recognition head to start the hidden state in a good place?
+        :param input_size: Usually 1 (mono input). A catnet extending this might change
+            it and provide the parametric inputs as additional input dimensions.
+        """
+        super().__init__()
+        if "batch_first" in lstm_kwargs:
+            raise ValueError("batch_first cannot be set.")
+        self._input_size = input_size
+        self._core = _L(self._input_size, hidden_size, batch_first=True, **lstm_kwargs)
+        self._head = nn.Linear(hidden_size, 1)
+        self._train_burn_in = train_burn_in
+        self._train_truncate = train_truncate
+        self._initial_cell = nn.Parameter(
+            torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
+        )
+        self._initial_hidden = nn.Parameter(
+            torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
+        )
+
+    @property
+    def receptive_field(self) -> int:
+        return 1
+
+    @property
+    def pad_start_default(self) -> bool:
+        # I should simplify this...
+        return True
+
+    def export_cpp_header(self, filename: Path):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir)
+            LSTM.export(self, Path(tmpdir))  # Hacky...need to work w/ CatLSTM
+            with open(Path(tmpdir, "model.nam"), "r") as fp:
+                _c = json.load(fp)
+            version = _c["version"]
+            config = _c["config"]
+            s_parametric = self._export_cpp_header_parametric(config.get("parametric"))
+            with open(filename, "w") as f:
+                f.writelines(
+                    (
+                        "#pragma once\n",
+                        "// Automatically-generated model file\n",
+                        "#include <vector>\n",
+                        '#include "json.hpp"\n',
+                        '#include "lstm.h"\n',
+                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
+                        f'const int NUM_LAYERS = {config["num_layers"]};\n',
+                        f'const int INPUT_SIZE = {config["input_size"]};\n',
+                        f'const int HIDDEN_SIZE = {config["hidden_size"]};\n',
+                    )
+                    + s_parametric
+                    + (
+                        "std::vector<float> PARAMS{"
+                        + ", ".join([f"{w:.16f}f" for w in _c["weights"]])
+                        + "};\n",
+                    )
+                )
+
+    def export_onnx(self, filename: Path):
+        if self._input_size != 1:
+            raise NotImplementedError("Multi-dimensional inputs not supported yet")
+        o = _ONNXWrapped(self)
+        x = torch.randn((64,))  # (S,)
+        h, c = [z[:, 0, :] for z in self._initial_state(1)]  # (L,DH), (L,DH)
+        torch.onnx.export(
+            o,
+            (x, h, c),
+            filename,
+            input_names=["x", "hin", "cin"],
+            output_names=["y", "hout", "cout"],
+            dynamic_axes={"x": {0: "num_frames"}, "y": {0: "num_frames"}},
+        )
+
+    def forward_onnx(
+        self, x: torch.Tensor, h: _LSTMHiddenType, c: _LSTMCellType
+    ) -> Tuple[torch.Tensor, _LSTMHiddenType, _LSTMCellType]:
+        """
+        Forward pass used by ONNX export
+        Only supports scalar inputs right now.
+
+        N: Sequeence length
+        L: Number of layers
+        DH: Hidden state dimension
+
+        :param x: (N,)
+        :param state: (L, DH)
+        :param cell: (L, DH)
+
+        :return: (N,), (L, DH), (L, DH)
+        """
+        features, (h, c) = self._core(x[None, :, None], (h[:, None, :], c[:, None, :]))
+        y = self._apply_head(features)  # (1,S)
+        return y[0, :], h[:, 0, :], c[:, 0, :]
+
+    def _apply_head(self, features: torch.Tensor) -> torch.Tensor:
+        """
+        :param features: (B,S,DH)
+        :return: (B,S)
+        """
+        return self._head(features)[:, :, 0]
+
+    def _forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        :param x: (B,L) or (B,L,D)
+        :return: (B,L)
+        """
+        last_hidden_state = self._initial_state(len(x))
+        if x.ndim == 2:
+            x = x[:, :, None]
+        if not self.training or self._train_truncate is None:
+            output_features = self._core(x, last_hidden_state)[0]
+        else:
+            output_features_list = []
+            if self._train_burn_in is not None:
+                last_output_features, last_hidden_state = self._core(
+                    x[:, : self._train_burn_in, :], last_hidden_state
+                )
+                output_features_list.append(last_output_features.detach())
+            burn_in_offset = 0 if self._train_burn_in is None else self._train_burn_in
+            for i in range(burn_in_offset, x.shape[1], self._train_truncate):
+                if i > burn_in_offset:
+                    # Don't detach the burn-in state so that we can learn it.
+                    last_hidden_state = tuple(z.detach() for z in last_hidden_state)
+                last_output_features, last_hidden_state = self._core(
+                    x[:, i : i + self._train_truncate, :], last_hidden_state
+                )
+                output_features_list.append(last_output_features)
+            output_features = torch.cat(output_features_list, dim=1)
+        return self._apply_head(output_features)
+
+    def _export_cell_weights(
+        self, i: int, hidden_state: torch.Tensor, cell_state: torch.Tensor
+    ) -> np.ndarray:
+        """
+        * weight matrix (xh -> ifco)
+        * bias vector
+        * Initial hidden state
+        * Initial cell state
+        """
+
+        tensors = [
+            torch.cat(
+                [
+                    getattr(self._core, f"weight_ih_l{i}").data,
+                    getattr(self._core, f"weight_hh_l{i}").data,
+                ],
+                dim=1,
+            ),
+            getattr(self._core, f"bias_ih_l{i}").data
+            + getattr(self._core, f"bias_hh_l{i}").data,
+            hidden_state,
+            cell_state,
+        ]
+        return np.concatenate([z.detach().cpu().numpy().flatten() for z in tensors])
+
+    def _export_config(self):
+        return {
+            "input_size": self._core.input_size,
+            "hidden_size": self._core.hidden_size,
+            "num_layers": self._core.num_layers,
+        }
+
+    def _export_cpp_header_parametric(self, config):
+        # TODO refactor to merge w/ WaveNet implementation
+        if config is not None:
+            raise ValueError("Got non-None parametric config")
+        return ("nlohmann::json PARAMETRIC {};\n",)
+
+    def _export_weights(self):
+        """
+        * Loop over cells:
+            * weight matrix (xh -> ifco)
+            * bias vector
+            * Initial hidden state
+            * Initial cell state
+        * Head weights
+        * Head bias
+        """
+        return np.concatenate(
+            [
+                self._export_cell_weights(i, h, c)
+                for i, (h, c) in enumerate(zip(*self._get_initial_state()))
+            ]
+            + [
+                self._head.weight.data.detach().cpu().numpy().flatten(),
+                self._head.bias.data.detach().cpu().numpy().flatten(),
+            ]
+        )
+
+    def _get_initial_state(self, inputs=None) -> _LSTMHiddenCellType:
+        """
+        Convenience function to find a good hidden state to start the plugin at
+
+        DX=input size
+        L=num layers
+        S=sequence length
+        :param inputs: (1,S,DX)
+
+        :return: (L,DH), (L,DH)
+        """
+        inputs = torch.zeros((1, 48_000, 1)) if inputs is None else inputs
+        _, (h, c) = self._core(inputs)
+        return h, c
+
+    def _initial_state(self, n: Optional[int]) -> _LSTMHiddenCellType:
+        """
+        Literally what the forward pass starts with.
+        Default is zeroes; this should be better since it can be learned.
+        """
+        return (
+            (self._initial_hidden, self._initial_cell)
+            if n is None
+            else (
+                torch.tile(self._initial_hidden[:, None], (1, n, 1)),
+                torch.tile(self._initial_cell[:, None], (1, n, 1)),
+            )
+        )
+
+
+class _ONNXWrapped(nn.Module):
+    def __init__(self, net: LSTM):
+        super().__init__()
+        self._net = net
+
+    def forward(
+        self, x: torch.Tensor, hidden: _LSTMHiddenType, cell: _LSTMCellType
+    ) -> Tuple[torch.Tensor, _LSTMHiddenType, _LSTMCellType]:
+        """
+        N: Sequeence length
+        L: Number of layers
+        DH: Hidden state dimension
+
+        :param x: (N,)
+        :param state: (L, DH)
+        :param cell: (L, DH)
+
+        :return: (N,), (L, DH), (L, DH)
+        """
+        return self._net.forward_onnx(x, hidden, cell)
+
+
+# TODO refactor together
+
+
+class _SkippyLSTM(nn.Module):
+    def __init__(
+        self, input_size, hidden_size, skip_in: bool = False, num_layers=1, **kwargs
+    ):
+        super().__init__()
+        layers_per_lstm = 1
+        self._skip_in = skip_in
+        self._lstms = nn.ModuleList(
+            [
+                _L(
+                    self._layer_input_size(input_size, hidden_size, i),
+                    hidden_size,
+                    layers_per_lstm,
+                    batch_first=True,
+                )
+                for i in range(num_layers)
+            ]
+        )
+        self._initial_hidden = nn.Parameter(
+            torch.zeros((self.num_layers, layers_per_lstm, self.hidden_size))
+        )
+        self._initial_cell = nn.Parameter(
+            torch.zeros((self.num_layers, layers_per_lstm, self.hidden_size))
+        )
+
+    @property
+    def hidden_size(self):
+        return self._lstms[0].hidden_size
+
+    @property
+    def input_size(self):
+        return self._lstms[0].input_size
+
+    @property
+    def num_layers(self):
+        return len(self._lstms)
+
+    @property
+    def output_size(self):
+        return self.num_layers * self.hidden_size
+
+    def forward(self, input, state=None):
+        """
+        :param input: (N,L,DX)
+        :param state: ((L,Li,N,DH), (L,Li,N,DH))
+
+        :return: (N,L,L*DH), ((L,Li,N,DH), (L,Li,N,DH))
+        """
+        h0, c0 = self.initial_state(input) if state is None else state
+        hiddens, h_arr, c_arr, hidden = [], [], [], None
+        for layer, h0i, c0i in zip(self._lstms, h0, c0):
+            if self._skip_in:
+                # TODO dense-block
+                layer_input = (
+                    input if hidden is None else torch.cat([input, hidden], dim=2)
+                )
+            else:
+                layer_input = input if hidden is None else hidden
+            hidden, (hi, ci) = layer(layer_input, (h0i, c0i))
+            hiddens.append(hidden)
+            h_arr.append(hi)
+            c_arr.append(ci)
+        return (torch.cat(hiddens, dim=2), (torch.stack(h_arr), torch.stack(c_arr)))
+
+    def initial_state(self, input: torch.Tensor):
+        """
+        Initial states for all the layers
+
+        :return: (L,B,Li,DH)
+        """
+        assert input.ndim == 3, "Batch only for now"
+        batch_size = len(input)  # Assume batch_first
+        return (
+            torch.tile(self._initial_hidden[:, :, None], (1, 1, batch_size, 1)),
+            torch.tile(self._initial_cell[:, :, None], (1, 1, batch_size, 1)),
+        )
+
+    def _layer_input_size(self, input_size, hidden_size, i) -> int:
+        # TODO dense-block
+        if self._skip_in:
+            return input_size + (0 if i == 0 else hidden_size)
+        else:
+            return input_size if i == 0 else hidden_size
```

### Comparing `neural-amp-modeler-0.5.2/nam/models/wavenet.py` & `neural-amp-modeler-0.6.0/nam/models/wavenet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,395 +1,436 @@
-# File: wavenet.py
-# Created Date: Friday July 29th 2022
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-WaveNet implementation
-https://arxiv.org/abs/1609.03499
-"""
-
-import json
-from copy import deepcopy
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Dict, Optional, Sequence, Tuple
-
-import numpy as np
-import torch
-import torch.nn as nn
-
-from ._activations import get_activation
-from ._base import BaseNet
-from ._names import ACTIVATION_NAME, CONV_NAME
-
-
-class Conv1d(nn.Conv1d):
-    def export_weights(self) -> torch.Tensor:
-        tensors = []
-        if self.weight is not None:
-            tensors.append(self.weight.data.flatten())
-        if self.bias is not None:
-            tensors.append(self.bias.data.flatten())
-        if len(tensors) == 0:
-            return torch.zeros((0,))
-        else:
-            return torch.cat(tensors)
-
-
-class _Layer(nn.Module):
-    def __init__(
-        self,
-        condition_size: int,
-        channels: int,
-        kernel_size: int,
-        dilation: int,
-        activation: str,
-        gated: bool,
-    ):
-        super().__init__()
-        # Input mixer takes care of the bias
-        mid_channels = 2 * channels if gated else channels
-        self._conv = Conv1d(channels, mid_channels, kernel_size, dilation=dilation)
-        # Custom init: favors direct input-output
-        # self._conv.weight.data.zero_()
-        self._input_mixer = Conv1d(condition_size, mid_channels, 1, bias=False)
-        self._activation = get_activation(activation)
-        self._activation_name = activation
-        self._1x1 = Conv1d(channels, channels, 1)
-        self._gated = gated
-
-    @property
-    def activation_name(self) -> str:
-        return self._activation_name
-
-    @property
-    def conv(self) -> Conv1d:
-        return self._conv
-
-    @property
-    def gated(self) -> bool:
-        return self._gated
-
-    @property
-    def kernel_size(self) -> int:
-        return self._conv.kernel_size[0]
-
-    def export_weights(self) -> torch.Tensor:
-        return torch.cat(
-            [
-                self.conv.export_weights(),
-                self._input_mixer.export_weights(),
-                self._1x1.export_weights(),
-            ]
-        )
-
-    def forward(
-        self, x: torch.Tensor, h: Optional[torch.Tensor], out_length: int
-    ) -> Tuple[Optional[torch.Tensor], torch.Tensor]:
-        """
-        :param x: (B,C,L1) From last layer
-        :param h: (B,DX,L2) Conditioning. If first, ignored.
-
-        :return:
-            If not final:
-                (B,C,L1-d) to next layer
-                (B,C,L1-d) to mixer
-            If final, next layer is None
-        """
-        zconv = self.conv(x)
-        z1 = zconv + self._input_mixer(h)[:, :, -zconv.shape[2] :]
-        post_activation = (
-            self._activation(z1)
-            if not self._gated
-            else (
-                self._activation(z1[:, : self._channels])
-                * torch.sigmoid(z1[:, self._channels :])
-            )
-        )
-        return (
-            x[:, :, -post_activation.shape[2] :] + self._1x1(post_activation),
-            post_activation[:, :, -out_length:],
-        )
-
-    @property
-    def _channels(self) -> int:
-        return self._1x1.in_channels
-
-
-class _Layers(nn.Module):
-    """
-    Takes in the input and condition (and maybe the head input so far); outputs the
-    layer output and head input.
-
-    The original WaveNet only uses one of these, but you can stack multiple of this
-    module to vary the channels throughout with minimal extra channel-changing conv
-    layers.
-    """
-
-    def __init__(
-        self,
-        input_size: int,
-        condition_size: int,
-        head_size,
-        channels: int,
-        kernel_size: int,
-        dilations: Sequence[int],
-        activation: str = "Tanh",
-        gated: bool = True,
-        head_bias: bool = True,
-    ):
-        super().__init__()
-        self._rechannel = Conv1d(input_size, channels, 1, bias=False)
-        self._layers = nn.ModuleList(
-            [
-                _Layer(
-                    condition_size, channels, kernel_size, dilation, activation, gated
-                )
-                for dilation in dilations
-            ]
-        )
-        # Convert the head input from channels to head_size
-        self._head_rechannel = Conv1d(channels, head_size, 1, bias=head_bias)
-
-        self._config = {
-            "input_size": input_size,
-            "condition_size": condition_size,
-            "head_size": head_size,
-            "channels": channels,
-            "kernel_size": kernel_size,
-            "dilations": dilations,
-            "activation": activation,
-            "gated": gated,
-            "head_bias": head_bias,
-        }
-
-    @property
-    def receptive_field(self) -> int:
-        return 1 + (self._kernel_size - 1) * sum(self._dilations)
-
-    def export_config(self):
-        return deepcopy(self._config)
-
-    def export_weights(self) -> torch.Tensor:
-        return torch.cat(
-            [self._rechannel.export_weights()]
-            + [layer.export_weights() for layer in self._layers]
-            + [self._head_rechannel.export_weights()]
-        )
-
-    def forward(
-        self,
-        x: torch.Tensor,
-        c: torch.Tensor,
-        head_input: Optional[torch.Tensor] = None,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        """
-        :param x: (B,Dx,L) layer input
-        :param c: (B,Dc,L) condition
-
-        :return:
-            (B,Dc,L-R+1) head input
-            (B,Dc,L-R+1) layer output
-        """
-        out_length = x.shape[2] - (self.receptive_field - 1)
-        x = self._rechannel(x)
-        for layer in self._layers:
-            x, head_term = layer(x, c, out_length)  # Ensures head_term sample length
-            head_input = (
-                head_term
-                if head_input is None
-                else head_input[:, :, -out_length:] + head_term
-            )
-        return self._head_rechannel(head_input), x
-
-    @property
-    def _dilations(self) -> Sequence[int]:
-        return self._config["dilations"]
-
-    @property
-    def _kernel_size(self) -> int:
-        return self._layers[0].kernel_size
-
-
-class _Head(nn.Module):
-    def __init__(
-        self,
-        in_channels: int,
-        channels: int,
-        activation: str,
-        num_layers: int,
-        out_channels: int,
-    ):
-        super().__init__()
-
-        def block(cx, cy):
-            net = nn.Sequential()
-            net.add_module(ACTIVATION_NAME, get_activation(activation))
-            net.add_module(CONV_NAME, Conv1d(cx, cy, 1))
-            return net
-
-        assert num_layers > 0
-
-        layers = nn.Sequential()
-        cin = in_channels
-        for i in range(num_layers):
-            layers.add_module(
-                f"layer_{i}",
-                block(cin, channels if i != num_layers - 1 else out_channels),
-            )
-            cin = channels
-        self._layers = layers
-
-        self._config = {
-            "channels": channels,
-            "activation": activation,
-            "num_layers": num_layers,
-            "out_channels": out_channels,
-        }
-
-    def export_config(self):
-        return deepcopy(self._config)
-
-    def export_weights(self) -> torch.Tensor:
-        return torch.cat([layer[1].export_weights() for layer in self._layers])
-
-    def forward(self, *args, **kwargs):
-        return self._layers(*args, **kwargs)
-
-
-class _WaveNet(nn.Module):
-    def __init__(
-        self,
-        layers_configs: Sequence[Dict],
-        head_config: Optional[Dict] = None,
-        head_scale: float = 1.0,
-    ):
-        super().__init__()
-
-        self._layers = nn.ModuleList([_Layers(**lc) for lc in layers_configs])
-        self._head = None if head_config is None else _Head(**head_config)
-        self._head_scale = head_scale
-
-    @property
-    def receptive_field(self) -> int:
-        return 1 + sum([(layer.receptive_field - 1) for layer in self._layers])
-
-    def export_config(self):
-        return {
-            "layers": [layers.export_config() for layers in self._layers],
-            "head": None if self._head is None else self._head.export_config(),
-            "head_scale": self._head_scale,
-        }
-
-    def export_weights(self) -> np.ndarray:
-        """
-        :return: 1D array
-        """
-        weights = torch.cat([layer.export_weights() for layer in self._layers])
-        if self._head is not None:
-            weights = torch.cat([weights, self._head.export_weights()])
-        weights = torch.cat([weights, torch.Tensor([self._head_scale])])
-        return weights.detach().cpu().numpy()
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        """
-        :param x: (B,Cx,L)
-        :return: (B,Cy,L-R)
-        """
-        y, head_input = x, None
-        for layer in self._layers:
-            head_input, y = layer(y, x, head_input=head_input)
-        head_input = self._head_scale * head_input
-        return head_input if self._head is None else self._head(head_input)
-
-
-class WaveNet(BaseNet):
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        self._net = _WaveNet(*args, **kwargs)
-
-    @property
-    def pad_start_default(self) -> bool:
-        return True
-
-    @property
-    def receptive_field(self) -> int:
-        return self._net.receptive_field
-
-    def export_cpp_header(self, filename: Path):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir)
-            WaveNet.export(self, Path(tmpdir))  # Hacky...need to work w/ CatWaveNet
-            with open(Path(tmpdir, "model.nam"), "r") as fp:
-                _c = json.load(fp)
-            version = _c["version"]
-            config = _c["config"]
-
-            if config["head"] is not None:
-                raise NotImplementedError("No heads yet")
-            # head_scale
-            # with_head
-            # parametric
-
-            # String for layer array params:
-            s_lap = (
-                "const std::vector<wavenet::LayerArrayParams> LAYER_ARRAY_PARAMS{\n",
-            )
-            for i, lc in enumerate(config["layers"], 1):
-                s_lap_line = (
-                    f'  wavenet::LayerArrayParams({lc["input_size"]}, '
-                    f'{lc["condition_size"]}, {lc["head_size"]}, {lc["channels"]}, '
-                    f'{lc["kernel_size"]}, std::vector<int> '
-                    "{"
-                    + ", ".join([str(d) for d in lc["dilations"]])
-                    + "}, "
-                    + (
-                        f'"{lc["activation"]}", {str(lc["gated"]).lower()}, '
-                        f'{str(lc["head_bias"]).lower()})'
-                    )
-                )
-                if i < len(config["layers"]):
-                    s_lap_line += ","
-                s_lap_line += "\n"
-                s_lap += (s_lap_line,)
-            s_lap += ("};\n",)
-            s_parametric = self._export_cpp_header_parametric(config.get("parametric"))
-            with open(filename, "w") as f:
-                f.writelines(
-                    (
-                        "#pragma once\n",
-                        "// Automatically-generated model file\n",
-                        "#include <vector>\n",
-                        '#include "json.hpp"\n',
-                        '#include "wavenet.h"\n',
-                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
-                    )
-                    + s_lap
-                    + (
-                        f'const float HEAD_SCALE = {config["head_scale"]};\n',
-                        "const bool WITH_HEAD = false;\n",
-                    )
-                    + s_parametric
-                    + (
-                        "std::vector<float> PARAMS{"
-                        + ", ".join([f"{w:.16f}f" for w in _c["weights"]])
-                        + "};\n",
-                    )
-                )
-
-    def _export_config(self):
-        return self._net.export_config()
-
-    def _export_cpp_header_parametric(self, config):
-        if config is not None:
-            raise ValueError("Got non-None parametric config")
-        return ("nlohmann::json PARAMETRIC {};\n",)
-
-    def _export_weights(self) -> np.ndarray:
-        return self._net.export_weights()
-
-    def _forward(self, x):
-        if x.ndim == 2:
-            x = x[:, None, :]
-        y = self._net(x)
-        assert y.shape[1] == 1
-        return y[:, 0, :]
+# File: wavenet.py
+# Created Date: Friday July 29th 2022
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+WaveNet implementation
+https://arxiv.org/abs/1609.03499
+"""
+
+import json
+from copy import deepcopy
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from typing import Dict, Optional, Sequence, Tuple
+
+import numpy as np
+import torch
+import torch.nn as nn
+
+from ._activations import get_activation
+from ._base import BaseNet
+from ._names import ACTIVATION_NAME, CONV_NAME
+
+
+class Conv1d(nn.Conv1d):
+    def export_weights(self) -> torch.Tensor:
+        tensors = []
+        if self.weight is not None:
+            tensors.append(self.weight.data.flatten())
+        if self.bias is not None:
+            tensors.append(self.bias.data.flatten())
+        if len(tensors) == 0:
+            return torch.zeros((0,))
+        else:
+            return torch.cat(tensors)
+
+    def import_weights(self, weights: torch.Tensor, i: int) -> int:
+        if self.weight is not None:
+            n = self.weight.numel()
+            self.weight.data = (
+                weights[i : i + n].reshape(self.weight.shape).to(self.weight.device)
+            )
+            i += n
+        if self.bias is not None:
+            n = self.bias.numel()
+            self.bias.data = (
+                weights[i : i + n].reshape(self.bias.shape).to(self.bias.device)
+            )
+            i += n
+        return i
+
+
+class _Layer(nn.Module):
+    def __init__(
+        self,
+        condition_size: int,
+        channels: int,
+        kernel_size: int,
+        dilation: int,
+        activation: str,
+        gated: bool,
+    ):
+        super().__init__()
+        # Input mixer takes care of the bias
+        mid_channels = 2 * channels if gated else channels
+        self._conv = Conv1d(channels, mid_channels, kernel_size, dilation=dilation)
+        # Custom init: favors direct input-output
+        # self._conv.weight.data.zero_()
+        self._input_mixer = Conv1d(condition_size, mid_channels, 1, bias=False)
+        self._activation = get_activation(activation)
+        self._activation_name = activation
+        self._1x1 = Conv1d(channels, channels, 1)
+        self._gated = gated
+
+    @property
+    def activation_name(self) -> str:
+        return self._activation_name
+
+    @property
+    def conv(self) -> Conv1d:
+        return self._conv
+
+    @property
+    def gated(self) -> bool:
+        return self._gated
+
+    @property
+    def kernel_size(self) -> int:
+        return self._conv.kernel_size[0]
+
+    def export_weights(self) -> torch.Tensor:
+        return torch.cat(
+            [
+                self.conv.export_weights(),
+                self._input_mixer.export_weights(),
+                self._1x1.export_weights(),
+            ]
+        )
+
+    def forward(
+        self, x: torch.Tensor, h: Optional[torch.Tensor], out_length: int
+    ) -> Tuple[Optional[torch.Tensor], torch.Tensor]:
+        """
+        :param x: (B,C,L1) From last layer
+        :param h: (B,DX,L2) Conditioning. If first, ignored.
+
+        :return:
+            If not final:
+                (B,C,L1-d) to next layer
+                (B,C,L1-d) to mixer
+            If final, next layer is None
+        """
+        zconv = self.conv(x)
+        z1 = zconv + self._input_mixer(h)[:, :, -zconv.shape[2] :]
+        post_activation = (
+            self._activation(z1)
+            if not self._gated
+            else (
+                self._activation(z1[:, : self._channels])
+                * torch.sigmoid(z1[:, self._channels :])
+            )
+        )
+        return (
+            x[:, :, -post_activation.shape[2] :] + self._1x1(post_activation),
+            post_activation[:, :, -out_length:],
+        )
+
+    def import_weights(self, weights: torch.Tensor, i: int) -> int:
+        i = self.conv.import_weights(weights, i)
+        i = self._input_mixer.import_weights(weights, i)
+        return self._1x1.import_weights(weights, i)
+
+    @property
+    def _channels(self) -> int:
+        return self._1x1.in_channels
+
+
+class _Layers(nn.Module):
+    """
+    Takes in the input and condition (and maybe the head input so far); outputs the
+    layer output and head input.
+
+    The original WaveNet only uses one of these, but you can stack multiple of this
+    module to vary the channels throughout with minimal extra channel-changing conv
+    layers.
+    """
+
+    def __init__(
+        self,
+        input_size: int,
+        condition_size: int,
+        head_size,
+        channels: int,
+        kernel_size: int,
+        dilations: Sequence[int],
+        activation: str = "Tanh",
+        gated: bool = True,
+        head_bias: bool = True,
+    ):
+        super().__init__()
+        self._rechannel = Conv1d(input_size, channels, 1, bias=False)
+        self._layers = nn.ModuleList(
+            [
+                _Layer(
+                    condition_size, channels, kernel_size, dilation, activation, gated
+                )
+                for dilation in dilations
+            ]
+        )
+        # Convert the head input from channels to head_size
+        self._head_rechannel = Conv1d(channels, head_size, 1, bias=head_bias)
+
+        self._config = {
+            "input_size": input_size,
+            "condition_size": condition_size,
+            "head_size": head_size,
+            "channels": channels,
+            "kernel_size": kernel_size,
+            "dilations": dilations,
+            "activation": activation,
+            "gated": gated,
+            "head_bias": head_bias,
+        }
+
+    @property
+    def receptive_field(self) -> int:
+        return 1 + (self._kernel_size - 1) * sum(self._dilations)
+
+    def export_config(self):
+        return deepcopy(self._config)
+
+    def export_weights(self) -> torch.Tensor:
+        return torch.cat(
+            [self._rechannel.export_weights()]
+            + [layer.export_weights() for layer in self._layers]
+            + [self._head_rechannel.export_weights()]
+        )
+
+    def import_weights(self, weights: torch.Tensor, i: int) -> int:
+        i = self._rechannel.import_weights(weights, i)
+        for layer in self._layers:
+            i = layer.import_weights(weights, i)
+        return self._head_rechannel.import_weights(weights, i)
+
+    def forward(
+        self,
+        x: torch.Tensor,
+        c: torch.Tensor,
+        head_input: Optional[torch.Tensor] = None,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        :param x: (B,Dx,L) layer input
+        :param c: (B,Dc,L) condition
+
+        :return:
+            (B,Dc,L-R+1) head input
+            (B,Dc,L-R+1) layer output
+        """
+        out_length = x.shape[2] - (self.receptive_field - 1)
+        x = self._rechannel(x)
+        for layer in self._layers:
+            x, head_term = layer(x, c, out_length)  # Ensures head_term sample length
+            head_input = (
+                head_term
+                if head_input is None
+                else head_input[:, :, -out_length:] + head_term
+            )
+        return self._head_rechannel(head_input), x
+
+    @property
+    def _dilations(self) -> Sequence[int]:
+        return self._config["dilations"]
+
+    @property
+    def _kernel_size(self) -> int:
+        return self._layers[0].kernel_size
+
+
+class _Head(nn.Module):
+    def __init__(
+        self,
+        in_channels: int,
+        channels: int,
+        activation: str,
+        num_layers: int,
+        out_channels: int,
+    ):
+        super().__init__()
+
+        def block(cx, cy):
+            net = nn.Sequential()
+            net.add_module(ACTIVATION_NAME, get_activation(activation))
+            net.add_module(CONV_NAME, Conv1d(cx, cy, 1))
+            return net
+
+        assert num_layers > 0
+
+        layers = nn.Sequential()
+        cin = in_channels
+        for i in range(num_layers):
+            layers.add_module(
+                f"layer_{i}",
+                block(cin, channels if i != num_layers - 1 else out_channels),
+            )
+            cin = channels
+        self._layers = layers
+
+        self._config = {
+            "channels": channels,
+            "activation": activation,
+            "num_layers": num_layers,
+            "out_channels": out_channels,
+        }
+
+    def export_config(self):
+        return deepcopy(self._config)
+
+    def export_weights(self) -> torch.Tensor:
+        return torch.cat([layer[1].export_weights() for layer in self._layers])
+
+    def forward(self, *args, **kwargs):
+        return self._layers(*args, **kwargs)
+
+    def import_weights(self, weights: torch.Tensor, i: int) -> int:
+        for layer in self._layers:
+            i = layer[1].import_weights(weights, i)
+        return i
+
+
+class _WaveNet(nn.Module):
+    def __init__(
+        self,
+        layers_configs: Sequence[Dict],
+        head_config: Optional[Dict] = None,
+        head_scale: float = 1.0,
+    ):
+        super().__init__()
+
+        self._layers = nn.ModuleList([_Layers(**lc) for lc in layers_configs])
+        self._head = None if head_config is None else _Head(**head_config)
+        self._head_scale = head_scale
+
+    @property
+    def receptive_field(self) -> int:
+        return 1 + sum([(layer.receptive_field - 1) for layer in self._layers])
+
+    def export_config(self):
+        return {
+            "layers": [layers.export_config() for layers in self._layers],
+            "head": None if self._head is None else self._head.export_config(),
+            "head_scale": self._head_scale,
+        }
+
+    def export_weights(self) -> np.ndarray:
+        """
+        :return: 1D array
+        """
+        weights = torch.cat([layer.export_weights() for layer in self._layers])
+        if self._head is not None:
+            weights = torch.cat([weights, self._head.export_weights()])
+        weights = torch.cat([weights, torch.Tensor([self._head_scale])])
+        return weights.detach().cpu().numpy()
+
+    def import_weights(self, weights: torch.Tensor):
+        i = 0
+        for layer in self._layers:
+            i = layer.import_weights(weights, i)
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        :param x: (B,Cx,L)
+        :return: (B,Cy,L-R)
+        """
+        y, head_input = x, None
+        for layer in self._layers:
+            head_input, y = layer(y, x, head_input=head_input)
+        head_input = self._head_scale * head_input
+        return head_input if self._head is None else self._head(head_input)
+
+
+class WaveNet(BaseNet):
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        self._net = _WaveNet(*args, **kwargs)
+
+    @property
+    def pad_start_default(self) -> bool:
+        return True
+
+    @property
+    def receptive_field(self) -> int:
+        return self._net.receptive_field
+
+    def export_cpp_header(self, filename: Path):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir)
+            WaveNet.export(self, Path(tmpdir))  # Hacky...need to work w/ CatWaveNet
+            with open(Path(tmpdir, "model.nam"), "r") as fp:
+                _c = json.load(fp)
+            version = _c["version"]
+            config = _c["config"]
+
+            if config["head"] is not None:
+                raise NotImplementedError("No heads yet")
+            # head_scale
+            # with_head
+            # parametric
+
+            # String for layer array params:
+            s_lap = (
+                "const std::vector<wavenet::LayerArrayParams> LAYER_ARRAY_PARAMS{\n",
+            )
+            for i, lc in enumerate(config["layers"], 1):
+                s_lap_line = (
+                    f'  wavenet::LayerArrayParams({lc["input_size"]}, '
+                    f'{lc["condition_size"]}, {lc["head_size"]}, {lc["channels"]}, '
+                    f'{lc["kernel_size"]}, std::vector<int> '
+                    "{"
+                    + ", ".join([str(d) for d in lc["dilations"]])
+                    + "}, "
+                    + (
+                        f'"{lc["activation"]}", {str(lc["gated"]).lower()}, '
+                        f'{str(lc["head_bias"]).lower()})'
+                    )
+                )
+                if i < len(config["layers"]):
+                    s_lap_line += ","
+                s_lap_line += "\n"
+                s_lap += (s_lap_line,)
+            s_lap += ("};\n",)
+            s_parametric = self._export_cpp_header_parametric(config.get("parametric"))
+            with open(filename, "w") as f:
+                f.writelines(
+                    (
+                        "#pragma once\n",
+                        "// Automatically-generated model file\n",
+                        "#include <vector>\n",
+                        '#include "json.hpp"\n',
+                        '#include "wavenet.h"\n',
+                        f'#define PYTHON_MODEL_VERSION "{version}"\n',
+                    )
+                    + s_lap
+                    + (
+                        f'const float HEAD_SCALE = {config["head_scale"]};\n',
+                        "const bool WITH_HEAD = false;\n",
+                    )
+                    + s_parametric
+                    + (
+                        "std::vector<float> PARAMS{"
+                        + ", ".join([f"{w:.16f}f" for w in _c["weights"]])
+                        + "};\n",
+                    )
+                )
+
+    def import_weights(self, weights: Sequence[float]):
+        if not isinstance(weights, torch.Tensor):
+            weights = torch.Tensor(weights)
+        self._net.import_weights(weights)
+
+    def _export_config(self):
+        return self._net.export_config()
+
+    def _export_cpp_header_parametric(self, config):
+        if config is not None:
+            raise ValueError("Got non-None parametric config")
+        return ("nlohmann::json PARAMETRIC {};\n",)
+
+    def _export_weights(self) -> np.ndarray:
+        return self._net.export_weights()
+
+    def _forward(self, x):
+        if x.ndim == 2:
+            x = x[:, None, :]
+        y = self._net(x)
+        assert y.shape[1] == 1
+        return y[:, 0, :]
```

### Comparing `neural-amp-modeler-0.5.2/nam/train/gui.py` & `neural-amp-modeler-0.6.0/nam/train/gui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,664 +1,721 @@
-# File: gui.py
-# Created Date: Saturday February 25th 2023
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-"""
-GUI for training
-
-Usage:
->>> from nam.train.gui import run
->>> run()
-"""
-
-
-# Hack to recover graceful shutdowns in Windows.
-# This has to happen ASAP
-# See:
-# https://github.com/sdatkinson/neural-amp-modeler/issues/105
-# https://stackoverflow.com/a/44822794
-def _ensure_graceful_shutdowns():
-    import os
-
-    if os.name == "nt":  # OS is Windows
-        os.environ["FOR_DISABLE_CONSOLE_CTRL_HANDLER"] = "1"
-
-
-_ensure_graceful_shutdowns()
-
-import re
-import tkinter as tk
-from dataclasses import dataclass
-from enum import Enum
-from functools import partial
-from pathlib import Path
-from tkinter import filedialog
-from typing import Callable, Optional, Sequence
-
-try:
-    from nam import __version__
-    from nam.train import core
-    from nam.models.metadata import GearType, UserMetadata, ToneType
-
-    _install_is_valid = True
-except ImportError:
-    _install_is_valid = False
-_BUTTON_WIDTH = 20
-_BUTTON_HEIGHT = 2
-_TEXT_WIDTH = 70
-
-_DEFAULT_NUM_EPOCHS = 100
-_DEFAULT_DELAY = None
-
-_ADVANCED_OPTIONS_LEFT_WIDTH = 12
-_ADVANCED_OPTIONS_RIGHT_WIDTH = 12
-_METADATA_RIGHT_WIDTH = 60
-
-
-@dataclass
-class _AdvancedOptions(object):
-    architecture: core.Architecture
-    num_epochs: int
-    delay: Optional[int]
-
-
-class _PathType(Enum):
-    FILE = "file"
-    DIRECTORY = "directory"
-    MULTIFILE = "multifile"
-
-
-class _PathButton(object):
-    """
-    Button and the path
-    """
-
-    def __init__(
-        self,
-        frame: tk.Frame,
-        button_text: str,
-        info_str: str,
-        path_type: _PathType,
-        hooks: Optional[Sequence[Callable[[], None]]] = None,
-    ):
-        self._button_text = button_text
-        self._info_str = info_str
-        self._path: Optional[Path] = None
-        self._path_type = path_type
-        self._button = tk.Button(
-            frame,
-            text=button_text,
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._set_val,
-        )
-        self._button.pack(side=tk.LEFT)
-        self._label = tk.Label(
-            frame,
-            width=_TEXT_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            bg=None,
-            anchor="w",
-        )
-        self._label.pack(side=tk.RIGHT)
-        self._hooks = hooks
-        self._set_text()
-
-    @property
-    def val(self) -> Optional[Path]:
-        return self._path
-
-    def _set_text(self):
-        if self._path is None:
-            self._label["fg"] = "red"
-            self._label["text"] = self._info_str
-        else:
-            val = self.val
-            val = val[0] if isinstance(val, tuple) and len(val) == 1 else val
-            self._label["fg"] = "black"
-            self._label["text"] = f"{self._button_text.capitalize()} set to {val}"
-
-    def _set_val(self):
-        res = {
-            _PathType.FILE: filedialog.askopenfilename,
-            _PathType.DIRECTORY: filedialog.askdirectory,
-            _PathType.MULTIFILE: filedialog.askopenfilenames,
-        }[self._path_type]()
-        if res != "":
-            self._path = res
-        self._set_text()
-
-        if self._hooks is not None:
-            for h in self._hooks:
-                h()
-
-
-class _GUI(object):
-    def __init__(self):
-        self._root = tk.Tk()
-        self._root.title(f"NAM Trainer - v{__version__}")
-
-        # Buttons for paths:
-        self._frame_input_path = tk.Frame(self._root)
-        self._frame_input_path.pack()
-        self._path_button_input = _PathButton(
-            self._frame_input_path,
-            "Input Audio",
-            "Select input DI file (eg: v1_1_1.wav)",
-            _PathType.FILE,
-            hooks=[self._check_button_states],
-        )
-
-        self._frame_output_path = tk.Frame(self._root)
-        self._frame_output_path.pack()
-        self._path_button_output = _PathButton(
-            self._frame_output_path,
-            "Output Audio",
-            "Select output (reamped) audio - choose multiple files to enable batch training",
-            _PathType.MULTIFILE,
-            hooks=[self._check_button_states],
-        )
-
-        self._frame_train_destination = tk.Frame(self._root)
-        self._frame_train_destination.pack()
-        self._path_button_train_destination = _PathButton(
-            self._frame_train_destination,
-            "Train Destination",
-            "Select training output directory",
-            _PathType.DIRECTORY,
-            hooks=[self._check_button_states],
-        )
-
-        # Metadata
-        self.user_metadata = UserMetadata()
-        self._frame_metadata = tk.Frame(self._root)
-        self._frame_metadata.pack()
-        self._button_metadata = tk.Button(
-            self._frame_metadata,
-            text="Metadata...",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._open_metadata,
-        )
-        self._button_metadata.pack()
-        self.user_metadata_flag = False
-
-        # This should probably be to the right somewhere
-        self._get_additional_options_frame()
-
-        # Advanced options for training
-        default_architecture = core.Architecture.STANDARD
-        self.advanced_options = _AdvancedOptions(
-            default_architecture, _DEFAULT_NUM_EPOCHS, _DEFAULT_DELAY
-        )
-        # Window to edit them:
-        self._frame_advanced_options = tk.Frame(self._root)
-        self._frame_advanced_options.pack()
-        self._button_advanced_options = tk.Button(
-            self._frame_advanced_options,
-            text="Advanced options...",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._open_advanced_options,
-        )
-        self._button_advanced_options.pack()
-
-        # Train button
-        self._frame_train = tk.Frame(self._root)
-        self._frame_train.pack()
-        self._button_train = tk.Button(
-            self._frame_train,
-            text="Train",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._train,
-        )
-        self._button_train.pack()
-
-        self._check_button_states()
-
-    def _get_additional_options_frame(self):
-        # Checkboxes
-        self._frame_silent = tk.Frame(self._root)
-        self._frame_silent.pack(side=tk.LEFT)
-
-        # Silent run (bypass popups)
-        self._silent = tk.BooleanVar()
-        self._chkbox_silent = tk.Checkbutton(
-            self._frame_silent,
-            text="Silent run (suggested for batch training)",
-            variable=self._silent,
-        )
-        self._chkbox_silent.grid(row=1, column=1, sticky="W")
-
-        # Auto save the end plot
-        self._save_plot = tk.BooleanVar()
-        self._save_plot.set(True)  # default this to true
-        self._chkbox_save_plot = tk.Checkbutton(
-            self._frame_silent,
-            text="Save ESR plot automatically",
-            variable=self._save_plot,
-        )
-        self._chkbox_save_plot.grid(row=2, column=1, sticky="W")
-
-    def mainloop(self):
-        self._root.mainloop()
-
-    def _open_advanced_options(self):
-        """
-        Open advanced options
-        """
-        ao = _AdvancedOptionsGUI(self)
-        # I should probably disable the main GUI...
-        ao.mainloop()
-        # ...and then re-enable it once it gets closed.
-
-    def _open_metadata(self):
-        """
-        Open dialog for metadata
-        """
-        mdata = _UserMetadataGUI(self)
-        # I should probably disable the main GUI...
-        mdata.mainloop()
-
-    def _train(self):
-        # Advanced options:
-        num_epochs = self.advanced_options.num_epochs
-        architecture = self.advanced_options.architecture
-        delay = self.advanced_options.delay
-        file_list = self._path_button_output.val
-
-        # Advanced-er options
-        # If you're poking around looking for these, then maybe it's time to learn to
-        # use the command-line scripts ;)
-        lr = 0.004
-        lr_decay = 0.007
-        seed = 0
-
-        # Run it
-        for file in file_list:
-            print("Now training {}".format(file))
-            basename = re.sub(r"\.wav$", "", file.split("/")[-1])
-
-            trained_model = core.train(
-                self._path_button_input.val,
-                file,
-                self._path_button_train_destination.val,
-                epochs=num_epochs,
-                delay=delay,
-                architecture=architecture,
-                lr=lr,
-                lr_decay=lr_decay,
-                seed=seed,
-                silent=self._silent.get(),
-                save_plot=self._save_plot.get(),
-                modelname=basename,
-            )
-            print("Model training complete!")
-            print("Exporting...")
-            outdir = self._path_button_train_destination.val
-            print(f"Exporting trained model to {outdir}...")
-            trained_model.net.export(
-                outdir,
-                basename=basename,
-                user_metadata=self.user_metadata
-                if self.user_metadata_flag
-                else UserMetadata(),
-            )
-            # Metadata was only valid for 1 run, so make sure it's not used again unless
-            # the user re-visits the window and clicks "ok"
-            self.user_metadata_flag = False
-            print("Done!")
-
-    def _check_button_states(self):
-        """
-        Determine if any buttons should be disabled
-        """
-        # Train button is diabled unless all paths are set
-        if any(
-            pb.val is None
-            for pb in (
-                self._path_button_input,
-                self._path_button_output,
-                self._path_button_train_destination,
-            )
-        ):
-            self._button_train["state"] = tk.DISABLED
-            return
-        self._button_train["state"] = tk.NORMAL
-
-
-# some typing functions
-def _non_negative_int(val):
-    val = int(val)
-    if val < 0:
-        val = 0
-    return val
-
-
-def _int_or_null(val):
-    val = val.rstrip()
-    if val == "null":
-        return val
-    return int(val)
-
-
-def _int_or_null_inv(val):
-    return "null" if val is None else str(val)
-
-
-def _rstripped_str(val):
-    return str(val).rstrip()
-
-
-class _LabeledOptionMenu(object):
-    """
-    Label (left) and radio buttons (right)
-    """
-
-    def __init__(
-        self, frame: tk.Frame, label: str, choices: Enum, default: Optional[Enum] = None
-    ):
-        """
-        :param command: Called to propagate option selection. Is provided with the
-            value corresponding to the radio button selected.
-        """
-        self._frame = frame
-        self._choices = choices
-        height = _BUTTON_HEIGHT
-        bg = None
-        fg = "black"
-        self._label = tk.Label(
-            frame,
-            width=_ADVANCED_OPTIONS_LEFT_WIDTH,
-            height=height,
-            fg=fg,
-            bg=bg,
-            anchor="w",
-            text=label,
-        )
-        self._label.pack(side=tk.LEFT)
-
-        frame_menu = tk.Frame(frame)
-        frame_menu.pack(side=tk.RIGHT)
-
-        self._selected_value = None
-        default = (list(choices)[0] if default is None else default).value
-        self._menu = tk.OptionMenu(
-            frame_menu,
-            tk.StringVar(master=frame, value=default, name=label),
-            # default,
-            *[choice.value for choice in choices],  #  if choice.value!=default],
-            command=self._set,
-        )
-        self._menu.config(width=_ADVANCED_OPTIONS_RIGHT_WIDTH)
-        self._menu.pack(side=tk.RIGHT)
-        # Initialize
-        self._set(default)
-
-    def get(self) -> Enum:
-        return self._selected_value
-
-    def _set(self, val: str):
-        """
-        Set the value selected
-        """
-        self._selected_value = self._choices(val)
-
-
-class _LabeledText(object):
-    """
-    Label (left) and text input (right)
-    """
-
-    def __init__(
-        self,
-        frame: tk.Frame,
-        label: str,
-        default=None,
-        type=None,
-        left_width=_ADVANCED_OPTIONS_LEFT_WIDTH,
-        right_width=_ADVANCED_OPTIONS_RIGHT_WIDTH,
-    ):
-        """
-        :param command: Called to propagate option selection. Is provided with the
-            value corresponding to the radio button selected.
-        :param type: If provided, casts value to given type
-        """
-        self._frame = frame
-        label_height = 2
-        text_height = 1
-        self._label = tk.Label(
-            frame,
-            width=left_width,
-            height=label_height,
-            fg="black",
-            bg=None,
-            anchor="w",
-            text=label,
-        )
-        self._label.pack(side=tk.LEFT)
-
-        self._text = tk.Text(
-            frame,
-            width=right_width,
-            height=text_height,
-            fg="black",
-            bg=None,
-        )
-        self._text.pack(side=tk.RIGHT)
-
-        self._type = type
-
-        if default is not None:
-            self._text.insert("1.0", str(default))
-
-    def get(self):
-        try:
-            val = self._text.get("1.0", tk.END)  # Line 1, character zero (wat)
-            if self._type is not None:
-                val = self._type(val)
-            return val
-        except tk.TclError:
-            return None
-
-
-class _AdvancedOptionsGUI(object):
-    """
-    A window to hold advanced options (Architecture and number of epochs)
-    """
-
-    def __init__(self, parent: _GUI):
-        self._parent = parent
-        self._root = tk.Tk()
-        self._root.title("Advanced Options")
-
-        # Architecture: radio buttons
-        self._frame_architecture = tk.Frame(self._root)
-        self._frame_architecture.pack()
-        self._architecture = _LabeledOptionMenu(
-            self._frame_architecture,
-            "Architecture",
-            core.Architecture,
-            default=self._parent.advanced_options.architecture,
-        )
-
-        # Number of epochs: text box
-        self._frame_epochs = tk.Frame(self._root)
-        self._frame_epochs.pack()
-
-        self._epochs = _LabeledText(
-            self._frame_epochs,
-            "Epochs",
-            default=str(self._parent.advanced_options.num_epochs),
-            type=_non_negative_int,
-        )
-
-        # Delay: text box
-        self._frame_delay = tk.Frame(self._root)
-        self._frame_delay.pack()
-
-        self._delay = _LabeledText(
-            self._frame_delay,
-            "Delay",
-            default=_int_or_null_inv(self._parent.advanced_options.delay),
-            type=_int_or_null,
-        )
-
-        # "Ok": apply and destory
-        self._frame_ok = tk.Frame(self._root)
-        self._frame_ok.pack()
-        self._button_ok = tk.Button(
-            self._frame_ok,
-            text="Ok",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._apply_and_destroy,
-        )
-        self._button_ok.pack()
-
-    def mainloop(self):
-        self._root.mainloop()
-
-    def _apply_and_destroy(self):
-        """
-        Set values to parent and destroy this object
-        """
-        self._parent.advanced_options.architecture = self._architecture.get()
-        epochs = self._epochs.get()
-        if epochs is not None:
-            self._parent.advanced_options.num_epochs = epochs
-        delay = self._delay.get()
-        # Value None is returned as "null" to disambiguate from non-set.
-        if delay is not None:
-            self._parent.advanced_options.delay = None if delay == "null" else delay
-        self._root.destroy()
-
-
-class _UserMetadataGUI(object):
-    # Things that are auto-filled:
-    # Model date
-    # gain
-    def __init__(self, parent: _GUI):
-        self._parent = parent
-        self._root = tk.Tk()
-        self._root.title("Metadata")
-
-        LabeledText = partial(_LabeledText, right_width=_METADATA_RIGHT_WIDTH)
-
-        # Name
-        self._frame_name = tk.Frame(self._root)
-        self._frame_name.pack()
-        self._name = LabeledText(
-            self._frame_name,
-            "NAM name",
-            default=parent.user_metadata.name,
-            type=_rstripped_str,
-        )
-        # Modeled by
-        self._frame_modeled_by = tk.Frame(self._root)
-        self._frame_modeled_by.pack()
-        self._modeled_by = LabeledText(
-            self._frame_modeled_by,
-            "Modeled by",
-            default=parent.user_metadata.modeled_by,
-            type=_rstripped_str,
-        )
-        # Gear make
-        self._frame_gear_make = tk.Frame(self._root)
-        self._frame_gear_make.pack()
-        self._gear_make = LabeledText(
-            self._frame_gear_make,
-            "Gear make",
-            default=parent.user_metadata.gear_make,
-            type=_rstripped_str,
-        )
-        # Gear model
-        self._frame_gear_model = tk.Frame(self._root)
-        self._frame_gear_model.pack()
-        self._gear_model = LabeledText(
-            self._frame_gear_model,
-            "Gear model",
-            default=parent.user_metadata.gear_model,
-            type=_rstripped_str,
-        )
-        # Gear type
-        self._frame_gear_type = tk.Frame(self._root)
-        self._frame_gear_type.pack()
-        self._gear_type = _LabeledOptionMenu(
-            self._frame_gear_type,
-            "Gear type",
-            GearType,
-            default=parent.user_metadata.gear_type,
-        )
-        # Tone type
-        self._frame_tone_type = tk.Frame(self._root)
-        self._frame_tone_type.pack()
-        self._tone_type = _LabeledOptionMenu(
-            self._frame_tone_type,
-            "Tone type",
-            ToneType,
-            default=parent.user_metadata.tone_type,
-        )
-
-        # "Ok": apply and destory
-        self._frame_ok = tk.Frame(self._root)
-        self._frame_ok.pack()
-        self._button_ok = tk.Button(
-            self._frame_ok,
-            text="Ok",
-            width=_BUTTON_WIDTH,
-            height=_BUTTON_HEIGHT,
-            fg="black",
-            command=self._apply_and_destroy,
-        )
-        self._button_ok.pack()
-
-    def mainloop(self):
-        self._root.mainloop()
-
-    def _apply_and_destroy(self):
-        """
-        Set values to parent and destroy this object
-        """
-        self._parent.user_metadata.name = self._name.get()
-        self._parent.user_metadata.modeled_by = self._modeled_by.get()
-        self._parent.user_metadata.gear_make = self._gear_make.get()
-        self._parent.user_metadata.gear_model = self._gear_model.get()
-        self._parent.user_metadata.gear_type = self._gear_type.get()
-        self._parent.user_metadata.tone_type = self._tone_type.get()
-        self._parent.user_metadata_flag = True
-
-        self._root.destroy()
-
-
-def _install_error():
-    window = tk.Tk()
-    window.title("ERROR")
-    label = tk.Label(
-        window,
-        width=45,
-        height=2,
-        text="The NAM training software has not been installed correctly.",
-    )
-    label.pack()
-    button = tk.Button(window, width=10, height=2, text="Quit", command=window.destroy)
-    button.pack()
-    window.mainloop()
-
-
-def run():
-    if _install_is_valid:
-        _gui = _GUI()
-        _gui.mainloop()
-    else:
-        _install_error()
-
-
-if __name__ == "__main__":
-    run()
+# File: gui.py
+# Created Date: Saturday February 25th 2023
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+"""
+GUI for training
+
+Usage:
+>>> from nam.train.gui import run
+>>> run()
+"""
+
+
+# Hack to recover graceful shutdowns in Windows.
+# This has to happen ASAP
+# See:
+# https://github.com/sdatkinson/neural-amp-modeler/issues/105
+# https://stackoverflow.com/a/44822794
+def _ensure_graceful_shutdowns():
+    import os
+
+    if os.name == "nt":  # OS is Windows
+        os.environ["FOR_DISABLE_CONSOLE_CTRL_HANDLER"] = "1"
+
+
+_ensure_graceful_shutdowns()
+
+import re
+import tkinter as tk
+from dataclasses import dataclass
+from enum import Enum
+from functools import partial
+from pathlib import Path
+from tkinter import filedialog
+from typing import Callable, Dict, Optional, Sequence
+
+try:
+    import torch
+
+    from nam import __version__
+    from nam.train import core
+    from nam.models.metadata import GearType, UserMetadata, ToneType
+
+    _install_is_valid = True
+    _HAVE_ACCELERATOR = torch.cuda.is_available() or torch.backends.mps.is_available()
+except ImportError:
+    _install_is_valid = False
+    _HAVE_ACCELERATOR = False
+
+if _HAVE_ACCELERATOR:
+    _DEFAULT_NUM_EPOCHS = 100
+    _DEFAULT_BATCH_SIZE = 16
+    _DEFAULT_LR_DECAY = 0.007
+else:
+    _DEFAULT_NUM_EPOCHS = 20
+    _DEFAULT_BATCH_SIZE = 1
+    _DEFAULT_LR_DECAY = 0.05
+_BUTTON_WIDTH = 20
+_BUTTON_HEIGHT = 2
+_TEXT_WIDTH = 70
+
+_DEFAULT_DELAY = None
+_DEFAULT_IGNORE_CHECKS = False
+
+_ADVANCED_OPTIONS_LEFT_WIDTH = 12
+_ADVANCED_OPTIONS_RIGHT_WIDTH = 12
+_METADATA_RIGHT_WIDTH = 60
+
+
+@dataclass
+class _AdvancedOptions(object):
+    architecture: core.Architecture
+    num_epochs: int
+    delay: Optional[int]
+    ignore_checks: bool
+
+
+class _PathType(Enum):
+    FILE = "file"
+    DIRECTORY = "directory"
+    MULTIFILE = "multifile"
+
+
+class _PathButton(object):
+    """
+    Button and the path
+    """
+
+    def __init__(
+        self,
+        frame: tk.Frame,
+        button_text: str,
+        info_str: str,
+        path_type: _PathType,
+        hooks: Optional[Sequence[Callable[[], None]]] = None,
+    ):
+        self._button_text = button_text
+        self._info_str = info_str
+        self._path: Optional[Path] = None
+        self._path_type = path_type
+        self._button = tk.Button(
+            frame,
+            text=button_text,
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._set_val,
+        )
+        self._button.pack(side=tk.LEFT)
+        self._label = tk.Label(
+            frame,
+            width=_TEXT_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            bg=None,
+            anchor="w",
+        )
+        self._label.pack(side=tk.RIGHT)
+        self._hooks = hooks
+        self._set_text()
+
+    @property
+    def val(self) -> Optional[Path]:
+        return self._path
+
+    def _set_text(self):
+        if self._path is None:
+            self._label["fg"] = "red"
+            self._label["text"] = self._info_str
+        else:
+            val = self.val
+            val = val[0] if isinstance(val, tuple) and len(val) == 1 else val
+            self._label["fg"] = "black"
+            self._label["text"] = f"{self._button_text.capitalize()} set to {val}"
+
+    def _set_val(self):
+        res = {
+            _PathType.FILE: filedialog.askopenfilename,
+            _PathType.DIRECTORY: filedialog.askdirectory,
+            _PathType.MULTIFILE: filedialog.askopenfilenames,
+        }[self._path_type]()
+        if res != "":
+            self._path = res
+        self._set_text()
+
+        if self._hooks is not None:
+            for h in self._hooks:
+                h()
+
+
+class _CheckboxKeys(Enum):
+    """
+    Keys for checkboxes
+    """
+
+    FIT_CAB = "fit_cab"
+    SILENT_TRAINING = "silent_training"
+    SAVE_PLOT = "save_plot"
+    IGNORE_DATA_CHECKS = "ignore_data_checks"
+
+
+class _GUI(object):
+    def __init__(self):
+        self._root = tk.Tk()
+        self._root.title(f"NAM Trainer - v{__version__}")
+
+        # Buttons for paths:
+        self._frame_input_path = tk.Frame(self._root)
+        self._frame_input_path.pack()
+        self._path_button_input = _PathButton(
+            self._frame_input_path,
+            "Input Audio",
+            "Select input DI file (eg: v1_1_1.wav)",
+            _PathType.FILE,
+            hooks=[self._check_button_states],
+        )
+
+        self._frame_output_path = tk.Frame(self._root)
+        self._frame_output_path.pack()
+        self._path_button_output = _PathButton(
+            self._frame_output_path,
+            "Output Audio",
+            "Select output (reamped) audio - choose multiple files to enable batch training",
+            _PathType.MULTIFILE,
+            hooks=[self._check_button_states],
+        )
+
+        self._frame_train_destination = tk.Frame(self._root)
+        self._frame_train_destination.pack()
+        self._path_button_train_destination = _PathButton(
+            self._frame_train_destination,
+            "Train Destination",
+            "Select training output directory",
+            _PathType.DIRECTORY,
+            hooks=[self._check_button_states],
+        )
+
+        # Metadata
+        self.user_metadata = UserMetadata()
+        self._frame_metadata = tk.Frame(self._root)
+        self._frame_metadata.pack()
+        self._button_metadata = tk.Button(
+            self._frame_metadata,
+            text="Metadata...",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._open_metadata,
+        )
+        self._button_metadata.pack()
+        self.user_metadata_flag = False
+
+        # This should probably be to the right somewhere
+        self._get_additional_options_frame()
+
+        # Advanced options for training
+        default_architecture = core.Architecture.STANDARD
+        self.advanced_options = _AdvancedOptions(
+            default_architecture,
+            _DEFAULT_NUM_EPOCHS,
+            _DEFAULT_DELAY,
+            _DEFAULT_IGNORE_CHECKS,
+        )
+        # Window to edit them:
+        self._frame_advanced_options = tk.Frame(self._root)
+        self._frame_advanced_options.pack()
+        self._button_advanced_options = tk.Button(
+            self._frame_advanced_options,
+            text="Advanced options...",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._open_advanced_options,
+        )
+        self._button_advanced_options.pack()
+
+        # Train button
+        self._frame_train = tk.Frame(self._root)
+        self._frame_train.pack()
+        self._button_train = tk.Button(
+            self._frame_train,
+            text="Train",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._train,
+        )
+        self._button_train.pack()
+
+        self._check_button_states()
+
+    def _check_button_states(self):
+        """
+        Determine if any buttons should be disabled
+        """
+        # Train button is disabled unless all paths are set
+        if any(
+            pb.val is None
+            for pb in (
+                self._path_button_input,
+                self._path_button_output,
+                self._path_button_train_destination,
+            )
+        ):
+            self._button_train["state"] = tk.DISABLED
+            return
+        self._button_train["state"] = tk.NORMAL
+
+    def _get_additional_options_frame(self):
+        # Checkboxes
+        # TODO get these definitions into __init__()
+        self._frame_checkboxes = tk.Frame(self._root)
+        self._frame_checkboxes.pack(side=tk.LEFT)
+        row = 1
+
+        @dataclass
+        class Checkbox(object):
+            variable: tk.BooleanVar
+            check_button: tk.Checkbutton
+
+        def make_checkbox(
+            key: _CheckboxKeys, text: str, default_value: bool
+        ) -> Checkbox:
+            variable = tk.BooleanVar()
+            variable.set(default_value)
+            check_button = tk.Checkbutton(
+                self._frame_checkboxes, text=text, variable=variable
+            )
+            self._checkboxes[key] = Checkbox(variable, check_button)
+
+        self._checkboxes: Dict[_CheckboxKeys, Checkbox] = dict()
+        make_checkbox(_CheckboxKeys.FIT_CAB, "Cab modeling", False)
+        make_checkbox(
+            _CheckboxKeys.SILENT_TRAINING,
+            "Silent run (suggested for batch training)",
+            False,
+        )
+        make_checkbox(_CheckboxKeys.SAVE_PLOT, "Save ESR plot automatically", True)
+        make_checkbox(
+            _CheckboxKeys.IGNORE_DATA_CHECKS,
+            "Ignore data quality checks (DO AT YOUR OWN RISK!)",
+            False,
+        )
+
+        # Grid them:
+        row = 1
+        for v in self._checkboxes.values():
+            v.check_button.grid(row=row, column=1, sticky="W")
+            row += 1
+
+    def mainloop(self):
+        self._root.mainloop()
+
+    def _open_advanced_options(self):
+        """
+        Open advanced options
+        """
+        ao = _AdvancedOptionsGUI(self)
+        # I should probably disable the main GUI...
+        ao.mainloop()
+        # ...and then re-enable it once it gets closed.
+
+    def _open_metadata(self):
+        """
+        Open dialog for metadata
+        """
+        mdata = _UserMetadataGUI(self)
+        # I should probably disable the main GUI...
+        mdata.mainloop()
+
+    def _train(self):
+        # Advanced options:
+        num_epochs = self.advanced_options.num_epochs
+        architecture = self.advanced_options.architecture
+        delay = self.advanced_options.delay
+        file_list = self._path_button_output.val
+
+        # Advanced-er options
+        # If you're poking around looking for these, then maybe it's time to learn to
+        # use the command-line scripts ;)
+        lr = 0.004
+        lr_decay = _DEFAULT_LR_DECAY
+        batch_size = _DEFAULT_BATCH_SIZE
+        seed = 0
+
+        # Run it
+        for file in file_list:
+            print("Now training {}".format(file))
+            basename = re.sub(r"\.wav$", "", file.split("/")[-1])
+
+            trained_model = core.train(
+                self._path_button_input.val,
+                file,
+                self._path_button_train_destination.val,
+                epochs=num_epochs,
+                delay=delay,
+                architecture=architecture,
+                batch_size=batch_size,
+                lr=lr,
+                lr_decay=lr_decay,
+                seed=seed,
+                silent=self._checkboxes[_CheckboxKeys.SILENT_TRAINING].variable.get(),
+                save_plot=self._checkboxes[_CheckboxKeys.SAVE_PLOT].variable.get(),
+                modelname=basename,
+                ignore_checks=self._checkboxes[
+                    _CheckboxKeys.IGNORE_DATA_CHECKS
+                ].variable.get(),
+                local=True,
+                fit_cab=self._checkboxes[_CheckboxKeys.FIT_CAB].variable.get(),
+            )
+            if trained_model is None:
+                print("Model training failed! Skip exporting...")
+                continue
+            print("Model training complete!")
+            print("Exporting...")
+            outdir = self._path_button_train_destination.val
+            print(f"Exporting trained model to {outdir}...")
+            trained_model.net.export(
+                outdir,
+                basename=basename,
+                user_metadata=self.user_metadata
+                if self.user_metadata_flag
+                else UserMetadata(),
+            )
+            print("Done!")
+
+        # Metadata was only valid for 1 run, so make sure it's not used again unless
+        # the user re-visits the window and clicks "ok"
+        self.user_metadata_flag = False
+
+
+# some typing functions
+def _non_negative_int(val):
+    val = int(val)
+    if val < 0:
+        val = 0
+    return val
+
+
+def _int_or_null(val):
+    val = val.rstrip()
+    if val == "null":
+        return val
+    return int(val)
+
+
+def _int_or_null_inv(val):
+    return "null" if val is None else str(val)
+
+
+def _rstripped_str(val):
+    return str(val).rstrip()
+
+
+class _LabeledOptionMenu(object):
+    """
+    Label (left) and radio buttons (right)
+    """
+
+    def __init__(
+        self, frame: tk.Frame, label: str, choices: Enum, default: Optional[Enum] = None
+    ):
+        """
+        :param command: Called to propagate option selection. Is provided with the
+            value corresponding to the radio button selected.
+        """
+        self._frame = frame
+        self._choices = choices
+        height = _BUTTON_HEIGHT
+        bg = None
+        fg = "black"
+        self._label = tk.Label(
+            frame,
+            width=_ADVANCED_OPTIONS_LEFT_WIDTH,
+            height=height,
+            fg=fg,
+            bg=bg,
+            anchor="w",
+            text=label,
+        )
+        self._label.pack(side=tk.LEFT)
+
+        frame_menu = tk.Frame(frame)
+        frame_menu.pack(side=tk.RIGHT)
+
+        self._selected_value = None
+        default = (list(choices)[0] if default is None else default).value
+        self._menu = tk.OptionMenu(
+            frame_menu,
+            tk.StringVar(master=frame, value=default, name=label),
+            # default,
+            *[choice.value for choice in choices],  #  if choice.value!=default],
+            command=self._set,
+        )
+        self._menu.config(width=_ADVANCED_OPTIONS_RIGHT_WIDTH)
+        self._menu.pack(side=tk.RIGHT)
+        # Initialize
+        self._set(default)
+
+    def get(self) -> Enum:
+        return self._selected_value
+
+    def _set(self, val: str):
+        """
+        Set the value selected
+        """
+        self._selected_value = self._choices(val)
+
+
+class _LabeledText(object):
+    """
+    Label (left) and text input (right)
+    """
+
+    def __init__(
+        self,
+        frame: tk.Frame,
+        label: str,
+        default=None,
+        type=None,
+        left_width=_ADVANCED_OPTIONS_LEFT_WIDTH,
+        right_width=_ADVANCED_OPTIONS_RIGHT_WIDTH,
+    ):
+        """
+        :param command: Called to propagate option selection. Is provided with the
+            value corresponding to the radio button selected.
+        :param type: If provided, casts value to given type
+        """
+        self._frame = frame
+        label_height = 2
+        text_height = 1
+        self._label = tk.Label(
+            frame,
+            width=left_width,
+            height=label_height,
+            fg="black",
+            bg=None,
+            anchor="w",
+            text=label,
+        )
+        self._label.pack(side=tk.LEFT)
+
+        self._text = tk.Text(
+            frame,
+            width=right_width,
+            height=text_height,
+            fg="black",
+            bg=None,
+        )
+        self._text.pack(side=tk.RIGHT)
+
+        self._type = type
+
+        if default is not None:
+            self._text.insert("1.0", str(default))
+
+    def get(self):
+        try:
+            val = self._text.get("1.0", tk.END)  # Line 1, character zero (wat)
+            if self._type is not None:
+                val = self._type(val)
+            return val
+        except tk.TclError:
+            return None
+
+
+class _AdvancedOptionsGUI(object):
+    """
+    A window to hold advanced options (Architecture and number of epochs)
+    """
+
+    def __init__(self, parent: _GUI):
+        self._parent = parent
+        self._root = tk.Tk()
+        self._root.title("Advanced Options")
+
+        # Architecture: radio buttons
+        self._frame_architecture = tk.Frame(self._root)
+        self._frame_architecture.pack()
+        self._architecture = _LabeledOptionMenu(
+            self._frame_architecture,
+            "Architecture",
+            core.Architecture,
+            default=self._parent.advanced_options.architecture,
+        )
+
+        # Number of epochs: text box
+        self._frame_epochs = tk.Frame(self._root)
+        self._frame_epochs.pack()
+
+        self._epochs = _LabeledText(
+            self._frame_epochs,
+            "Epochs",
+            default=str(self._parent.advanced_options.num_epochs),
+            type=_non_negative_int,
+        )
+
+        # Delay: text box
+        self._frame_delay = tk.Frame(self._root)
+        self._frame_delay.pack()
+
+        self._delay = _LabeledText(
+            self._frame_delay,
+            "Delay",
+            default=_int_or_null_inv(self._parent.advanced_options.delay),
+            type=_int_or_null,
+        )
+
+        # "Ok": apply and destory
+        self._frame_ok = tk.Frame(self._root)
+        self._frame_ok.pack()
+        self._button_ok = tk.Button(
+            self._frame_ok,
+            text="Ok",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._apply_and_destroy,
+        )
+        self._button_ok.pack()
+
+    def mainloop(self):
+        self._root.mainloop()
+
+    def _apply_and_destroy(self):
+        """
+        Set values to parent and destroy this object
+        """
+        self._parent.advanced_options.architecture = self._architecture.get()
+        epochs = self._epochs.get()
+        if epochs is not None:
+            self._parent.advanced_options.num_epochs = epochs
+        delay = self._delay.get()
+        # Value None is returned as "null" to disambiguate from non-set.
+        if delay is not None:
+            self._parent.advanced_options.delay = None if delay == "null" else delay
+        self._root.destroy()
+
+
+class _UserMetadataGUI(object):
+    # Things that are auto-filled:
+    # Model date
+    # gain
+    def __init__(self, parent: _GUI):
+        self._parent = parent
+        self._root = tk.Tk()
+        self._root.title("Metadata")
+
+        LabeledText = partial(_LabeledText, right_width=_METADATA_RIGHT_WIDTH)
+
+        # Name
+        self._frame_name = tk.Frame(self._root)
+        self._frame_name.pack()
+        self._name = LabeledText(
+            self._frame_name,
+            "NAM name",
+            default=parent.user_metadata.name,
+            type=_rstripped_str,
+        )
+        # Modeled by
+        self._frame_modeled_by = tk.Frame(self._root)
+        self._frame_modeled_by.pack()
+        self._modeled_by = LabeledText(
+            self._frame_modeled_by,
+            "Modeled by",
+            default=parent.user_metadata.modeled_by,
+            type=_rstripped_str,
+        )
+        # Gear make
+        self._frame_gear_make = tk.Frame(self._root)
+        self._frame_gear_make.pack()
+        self._gear_make = LabeledText(
+            self._frame_gear_make,
+            "Gear make",
+            default=parent.user_metadata.gear_make,
+            type=_rstripped_str,
+        )
+        # Gear model
+        self._frame_gear_model = tk.Frame(self._root)
+        self._frame_gear_model.pack()
+        self._gear_model = LabeledText(
+            self._frame_gear_model,
+            "Gear model",
+            default=parent.user_metadata.gear_model,
+            type=_rstripped_str,
+        )
+        # Gear type
+        self._frame_gear_type = tk.Frame(self._root)
+        self._frame_gear_type.pack()
+        self._gear_type = _LabeledOptionMenu(
+            self._frame_gear_type,
+            "Gear type",
+            GearType,
+            default=parent.user_metadata.gear_type,
+        )
+        # Tone type
+        self._frame_tone_type = tk.Frame(self._root)
+        self._frame_tone_type.pack()
+        self._tone_type = _LabeledOptionMenu(
+            self._frame_tone_type,
+            "Tone type",
+            ToneType,
+            default=parent.user_metadata.tone_type,
+        )
+
+        # "Ok": apply and destory
+        self._frame_ok = tk.Frame(self._root)
+        self._frame_ok.pack()
+        self._button_ok = tk.Button(
+            self._frame_ok,
+            text="Ok",
+            width=_BUTTON_WIDTH,
+            height=_BUTTON_HEIGHT,
+            fg="black",
+            command=self._apply_and_destroy,
+        )
+        self._button_ok.pack()
+
+    def mainloop(self):
+        self._root.mainloop()
+
+    def _apply_and_destroy(self):
+        """
+        Set values to parent and destroy this object
+        """
+        self._parent.user_metadata.name = self._name.get()
+        self._parent.user_metadata.modeled_by = self._modeled_by.get()
+        self._parent.user_metadata.gear_make = self._gear_make.get()
+        self._parent.user_metadata.gear_model = self._gear_model.get()
+        self._parent.user_metadata.gear_type = self._gear_type.get()
+        self._parent.user_metadata.tone_type = self._tone_type.get()
+        self._parent.user_metadata_flag = True
+
+        self._root.destroy()
+
+
+def _install_error():
+    window = tk.Tk()
+    window.title("ERROR")
+    label = tk.Label(
+        window,
+        width=45,
+        height=2,
+        text="The NAM training software has not been installed correctly.",
+    )
+    label.pack()
+    button = tk.Button(window, width=10, height=2, text="Quit", command=window.destroy)
+    button.pack()
+    window.mainloop()
+
+
+def run():
+    if _install_is_valid:
+        _gui = _GUI()
+        _gui.mainloop()
+    else:
+        _install_error()
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `neural-amp-modeler-0.5.2/setup.py` & `neural-amp-modeler-0.6.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# File: setup.py
-# Created Date: 2020-04-08
-# Author: Steven Atkinson (steven@atkinson.mn)
-
-from distutils.util import convert_path
-from setuptools import setup, find_packages
-
-main_ns = {}
-ver_path = convert_path("nam/_version.py")
-with open(ver_path) as ver_file:
-    exec(ver_file.read(), main_ns)
-
-requirements = [
-    "auraloss==0.3.0",
-    "matplotlib",
-    "numpy",
-    "pydantic",
-    "pytorch_lightning",
-    "scipy",
-    "sounddevice",
-    "tensorboard",
-    "torch",
-    "tqdm",
-    "wavio<=0.0.4",  # Breaking change in 0.0.5
-]
-
-setup(
-    name="neural-amp-modeler",
-    version=main_ns["__version__"],
-    description="Neural amp modeler",
-    author="Steven Atkinson",
-    author_email="steven@atkinson.mn",
-    url="https://github.com/sdatkinson/",
-    install_requires=requirements,
-    packages=find_packages(),
-    include_package_data=True,
-    entry_points={
-        "console_scripts": [
-            "nam = nam.train.gui:run",
-        ]
-    },
-)
+# File: setup.py
+# Created Date: 2020-04-08
+# Author: Steven Atkinson (steven@atkinson.mn)
+
+from distutils.util import convert_path
+from setuptools import setup, find_packages
+
+main_ns = {}
+ver_path = convert_path("nam/_version.py")
+with open(ver_path) as ver_file:
+    exec(ver_file.read(), main_ns)
+
+requirements = [
+    "auraloss==0.3.0",
+    "matplotlib",
+    "numpy",
+    "pydantic",
+    "pytorch_lightning",
+    "scipy",
+    "sounddevice",
+    "tensorboard",
+    "torch",
+    "tqdm",
+    "wavio>=0.0.5",  # Breaking change with older versions
+]
+
+setup(
+    name="neural-amp-modeler",
+    version=main_ns["__version__"],
+    description="Neural amp modeler",
+    author="Steven Atkinson",
+    author_email="steven@atkinson.mn",
+    url="https://github.com/sdatkinson/",
+    install_requires=requirements,
+    packages=find_packages(),
+    include_package_data=True,
+    entry_points={
+        "console_scripts": [
+            "nam = nam.train.gui:run",
+        ]
+    },
+)
```

