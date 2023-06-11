# Comparing `tmp/libauc-1.3.0rc6.tar.gz` & `tmp/libauc-1.3.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libauc-1.3.0rc6.tar", last modified: Sun Jun 11 21:38:29 2023, max compression
+gzip compressed data, was "libauc-1.3.0rc7.tar", last modified: Sun Jun 11 22:39:18 2023, max compression
```

## Comparing `libauc-1.3.0rc6.tar` & `libauc-1.3.0rc7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.937466 libauc-1.3.0rc6/
--rwx------   0 zhuoning   (501) staff       (20)    11357 2023-03-02 14:10:38.000000 libauc-1.3.0rc6/LICENSE
--rw-r--r--   0 zhuoning   (501) staff       (20)     4143 2023-06-11 21:38:29.937344 libauc-1.3.0rc6/PKG-INFO
--rw-r--r--   0 zhuoning   (501) staff       (20)     3657 2023-06-11 20:04:36.000000 libauc-1.3.0rc6/README.md
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.931314 libauc-1.3.0rc6/libauc/
--rwx------   0 zhuoning   (501) staff       (20)      112 2023-06-11 21:38:17.000000 libauc-1.3.0rc6/libauc/__init__.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.933121 libauc-1.3.0rc6/libauc/datasets/
--rwx------   0 zhuoning   (501) staff       (20)      245 2023-06-09 06:42:38.000000 libauc-1.3.0rc6/libauc/datasets/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     2621 2023-06-10 17:15:47.000000 libauc-1.3.0rc6/libauc/datasets/breastcancer.py
--rwx------   0 zhuoning   (501) staff       (20)     2176 2023-06-10 17:15:53.000000 libauc-1.3.0rc6/libauc/datasets/cat_vs_dog.py
--rwx------   0 zhuoning   (501) staff       (20)     9859 2023-05-18 04:21:28.000000 libauc-1.3.0rc6/libauc/datasets/chexpert.py
--rwx------   0 zhuoning   (501) staff       (20)     6292 2023-05-24 19:24:50.000000 libauc-1.3.0rc6/libauc/datasets/cifar.py
--rwx------   0 zhuoning   (501) staff       (20)     1561 2023-06-09 06:42:09.000000 libauc-1.3.0rc6/libauc/datasets/dataset.py
--rwx------   0 zhuoning   (501) staff       (20)    12399 2023-03-09 21:50:47.000000 libauc-1.3.0rc6/libauc/datasets/folder.py
--rwx------   0 zhuoning   (501) staff       (20)     4854 2023-06-07 00:13:14.000000 libauc-1.3.0rc6/libauc/datasets/melanoma.py
--rwx------   0 zhuoning   (501) staff       (20)    13133 2023-06-11 19:11:48.000000 libauc-1.3.0rc6/libauc/datasets/movielens.py
--rwx------   0 zhuoning   (501) staff       (20)     1497 2023-06-09 07:05:10.000000 libauc-1.3.0rc6/libauc/datasets/musk2.py
--rwx------   0 zhuoning   (501) staff       (20)     2960 2023-03-02 14:10:38.000000 libauc-1.3.0rc6/libauc/datasets/stl10.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.934018 libauc-1.3.0rc6/libauc/losses/
--rwx------   0 zhuoning   (501) staff       (20)      117 2023-06-07 19:59:42.000000 libauc-1.3.0rc6/libauc/losses/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    49557 2023-06-10 17:45:01.000000 libauc-1.3.0rc6/libauc/losses/auc.py
--rwx------   0 zhuoning   (501) staff       (20)    23658 2023-06-11 21:19:11.000000 libauc-1.3.0rc6/libauc/losses/contrastive.py
--rwx------   0 zhuoning   (501) staff       (20)     2893 2023-06-08 21:37:05.000000 libauc-1.3.0rc6/libauc/losses/losses.py
--rwx------   0 zhuoning   (501) staff       (20)    15077 2023-06-10 06:44:38.000000 libauc-1.3.0rc6/libauc/losses/mil.py
--rwx------   0 zhuoning   (501) staff       (20)     3038 2023-06-11 04:06:56.000000 libauc-1.3.0rc6/libauc/losses/perf_at_top.py
--rwx------   0 zhuoning   (501) staff       (20)    12996 2023-06-11 04:07:47.000000 libauc-1.3.0rc6/libauc/losses/ranking.py
--rwx------   0 zhuoning   (501) staff       (20)     2618 2023-06-03 03:28:07.000000 libauc-1.3.0rc6/libauc/losses/surrogate.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.934220 libauc-1.3.0rc6/libauc/metrics/
--rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:29.000000 libauc-1.3.0rc6/libauc/metrics/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     8416 2023-06-11 21:32:30.000000 libauc-1.3.0rc6/libauc/metrics/metrics.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.934894 libauc-1.3.0rc6/libauc/models/
--rwx------   0 zhuoning   (501) staff       (20)      153 2023-05-26 02:45:25.000000 libauc-1.3.0rc6/libauc/models/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    13913 2023-05-18 03:12:04.000000 libauc-1.3.0rc6/libauc/models/densenet.py
--rwx------   0 zhuoning   (501) staff       (20)     8626 2023-05-26 04:26:36.000000 libauc-1.3.0rc6/libauc/models/mil_models.py
--rwx------   0 zhuoning   (501) staff       (20)     3479 2023-06-07 00:10:14.000000 libauc-1.3.0rc6/libauc/models/neumf.py
--rwx------   0 zhuoning   (501) staff       (20)     1284 2023-06-07 00:11:49.000000 libauc-1.3.0rc6/libauc/models/perceptron.py
--rwx------   0 zhuoning   (501) staff       (20)    16352 2023-05-18 03:13:49.000000 libauc-1.3.0rc6/libauc/models/resnet.py
--rwx------   0 zhuoning   (501) staff       (20)     6836 2023-05-26 02:54:35.000000 libauc-1.3.0rc6/libauc/models/resnet_cifar.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.936585 libauc-1.3.0rc6/libauc/optimizers/
--rwx------   0 zhuoning   (501) staff       (20)      350 2023-06-01 06:26:46.000000 libauc-1.3.0rc6/libauc/optimizers/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)     9062 2023-06-11 20:55:33.000000 libauc-1.3.0rc6/libauc/optimizers/adam.py
--rwx------   0 zhuoning   (501) staff       (20)     8911 2023-06-11 20:49:33.000000 libauc-1.3.0rc6/libauc/optimizers/adamw.py
--rwx------   0 zhuoning   (501) staff       (20)    12775 2023-06-11 21:05:07.000000 libauc-1.3.0rc6/libauc/optimizers/isogclr.py
--rw-r--r--   0 zhuoning   (501) staff       (20)     1760 2023-06-02 02:43:22.000000 libauc-1.3.0rc6/libauc/optimizers/lars.py
--rwx------   0 zhuoning   (501) staff       (20)     8217 2023-06-08 21:20:22.000000 libauc-1.3.0rc6/libauc/optimizers/midam.py
--rwx------   0 zhuoning   (501) staff       (20)    11591 2023-06-11 20:56:14.000000 libauc-1.3.0rc6/libauc/optimizers/pdsca.py
--rwx------   0 zhuoning   (501) staff       (20)    14772 2023-06-11 20:57:02.000000 libauc-1.3.0rc6/libauc/optimizers/pesg.py
--rwx------   0 zhuoning   (501) staff       (20)     8297 2023-06-11 20:57:22.000000 libauc-1.3.0rc6/libauc/optimizers/sgd.py
--rwx------   0 zhuoning   (501) staff       (20)    13546 2023-06-11 21:01:55.000000 libauc-1.3.0rc6/libauc/optimizers/soap.py
--rwx------   0 zhuoning   (501) staff       (20)    11774 2023-06-11 21:05:08.000000 libauc-1.3.0rc6/libauc/optimizers/sogclr.py
--rwx------   0 zhuoning   (501) staff       (20)    12722 2023-06-11 20:51:48.000000 libauc-1.3.0rc6/libauc/optimizers/song.py
--rwx------   0 zhuoning   (501) staff       (20)    13216 2023-06-11 20:53:19.000000 libauc-1.3.0rc6/libauc/optimizers/sopa.py
--rwx------   0 zhuoning   (501) staff       (20)    13344 2023-06-11 20:52:35.000000 libauc-1.3.0rc6/libauc/optimizers/sopa_s.py
--rwx------   0 zhuoning   (501) staff       (20)    12918 2023-06-11 20:54:05.000000 libauc-1.3.0rc6/libauc/optimizers/sota_s.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.936807 libauc-1.3.0rc6/libauc/sampler/
--rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:26.000000 libauc-1.3.0rc6/libauc/sampler/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    20482 2023-06-11 19:54:36.000000 libauc-1.3.0rc6/libauc/sampler/sampler.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.937187 libauc-1.3.0rc6/libauc/utils/
--rwx------   0 zhuoning   (501) staff       (20)       50 2023-06-01 06:26:50.000000 libauc-1.3.0rc6/libauc/utils/__init__.py
--rwx------   0 zhuoning   (501) staff       (20)    20264 2023-06-11 21:37:02.000000 libauc-1.3.0rc6/libauc/utils/paper_utils.py
--rwx------   0 zhuoning   (501) staff       (20)     4706 2023-06-11 05:08:04.000000 libauc-1.3.0rc6/libauc/utils/utils.py
-drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 21:38:29.931879 libauc-1.3.0rc6/libauc.egg-info/
--rw-r--r--   0 zhuoning   (501) staff       (20)     4143 2023-06-11 21:38:29.000000 libauc-1.3.0rc6/libauc.egg-info/PKG-INFO
--rw-r--r--   0 zhuoning   (501) staff       (20)     1470 2023-06-11 21:38:29.000000 libauc-1.3.0rc6/libauc.egg-info/SOURCES.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)        1 2023-06-11 21:38:29.000000 libauc-1.3.0rc6/libauc.egg-info/dependency_links.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)       76 2023-06-11 21:38:29.000000 libauc-1.3.0rc6/libauc.egg-info/requires.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)        7 2023-06-11 21:38:29.000000 libauc-1.3.0rc6/libauc.egg-info/top_level.txt
--rw-r--r--   0 zhuoning   (501) staff       (20)       38 2023-06-11 21:38:29.937506 libauc-1.3.0rc6/setup.cfg
--rw-r--r--   0 zhuoning   (501) staff       (20)      982 2023-06-11 21:38:16.000000 libauc-1.3.0rc6/setup.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.663941 libauc-1.3.0rc7/
+-rwx------   0 zhuoning   (501) staff       (20)    11357 2023-03-02 14:10:38.000000 libauc-1.3.0rc7/LICENSE
+-rw-r--r--   0 zhuoning   (501) staff       (20)     4143 2023-06-11 22:39:18.663842 libauc-1.3.0rc7/PKG-INFO
+-rw-r--r--   0 zhuoning   (501) staff       (20)     3657 2023-06-11 20:04:36.000000 libauc-1.3.0rc7/README.md
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.657560 libauc-1.3.0rc7/libauc/
+-rwx------   0 zhuoning   (501) staff       (20)      112 2023-06-11 22:39:04.000000 libauc-1.3.0rc7/libauc/__init__.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.659453 libauc-1.3.0rc7/libauc/datasets/
+-rwx------   0 zhuoning   (501) staff       (20)      245 2023-06-09 06:42:38.000000 libauc-1.3.0rc7/libauc/datasets/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     2621 2023-06-10 17:15:47.000000 libauc-1.3.0rc7/libauc/datasets/breastcancer.py
+-rwx------   0 zhuoning   (501) staff       (20)     2176 2023-06-10 17:15:53.000000 libauc-1.3.0rc7/libauc/datasets/cat_vs_dog.py
+-rwx------   0 zhuoning   (501) staff       (20)     9859 2023-05-18 04:21:28.000000 libauc-1.3.0rc7/libauc/datasets/chexpert.py
+-rwx------   0 zhuoning   (501) staff       (20)     6292 2023-05-24 19:24:50.000000 libauc-1.3.0rc7/libauc/datasets/cifar.py
+-rwx------   0 zhuoning   (501) staff       (20)     1561 2023-06-09 06:42:09.000000 libauc-1.3.0rc7/libauc/datasets/dataset.py
+-rwx------   0 zhuoning   (501) staff       (20)    12399 2023-03-09 21:50:47.000000 libauc-1.3.0rc7/libauc/datasets/folder.py
+-rwx------   0 zhuoning   (501) staff       (20)     4854 2023-06-07 00:13:14.000000 libauc-1.3.0rc7/libauc/datasets/melanoma.py
+-rwx------   0 zhuoning   (501) staff       (20)    13133 2023-06-11 19:11:48.000000 libauc-1.3.0rc7/libauc/datasets/movielens.py
+-rwx------   0 zhuoning   (501) staff       (20)     1497 2023-06-09 07:05:10.000000 libauc-1.3.0rc7/libauc/datasets/musk2.py
+-rwx------   0 zhuoning   (501) staff       (20)     2960 2023-03-02 14:10:38.000000 libauc-1.3.0rc7/libauc/datasets/stl10.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.660457 libauc-1.3.0rc7/libauc/losses/
+-rwx------   0 zhuoning   (501) staff       (20)      117 2023-06-07 19:59:42.000000 libauc-1.3.0rc7/libauc/losses/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    49557 2023-06-10 17:45:01.000000 libauc-1.3.0rc7/libauc/losses/auc.py
+-rwx------   0 zhuoning   (501) staff       (20)    23658 2023-06-11 21:19:11.000000 libauc-1.3.0rc7/libauc/losses/contrastive.py
+-rwx------   0 zhuoning   (501) staff       (20)     2893 2023-06-08 21:37:05.000000 libauc-1.3.0rc7/libauc/losses/losses.py
+-rwx------   0 zhuoning   (501) staff       (20)    15077 2023-06-10 06:44:38.000000 libauc-1.3.0rc7/libauc/losses/mil.py
+-rwx------   0 zhuoning   (501) staff       (20)     3038 2023-06-11 04:06:56.000000 libauc-1.3.0rc7/libauc/losses/perf_at_top.py
+-rwx------   0 zhuoning   (501) staff       (20)    12996 2023-06-11 04:07:47.000000 libauc-1.3.0rc7/libauc/losses/ranking.py
+-rwx------   0 zhuoning   (501) staff       (20)     2618 2023-06-03 03:28:07.000000 libauc-1.3.0rc7/libauc/losses/surrogate.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.660682 libauc-1.3.0rc7/libauc/metrics/
+-rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:29.000000 libauc-1.3.0rc7/libauc/metrics/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     8416 2023-06-11 21:32:30.000000 libauc-1.3.0rc7/libauc/metrics/metrics.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.661504 libauc-1.3.0rc7/libauc/models/
+-rwx------   0 zhuoning   (501) staff       (20)      153 2023-05-26 02:45:25.000000 libauc-1.3.0rc7/libauc/models/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    13913 2023-05-18 03:12:04.000000 libauc-1.3.0rc7/libauc/models/densenet.py
+-rwx------   0 zhuoning   (501) staff       (20)     8626 2023-05-26 04:26:36.000000 libauc-1.3.0rc7/libauc/models/mil_models.py
+-rwx------   0 zhuoning   (501) staff       (20)     3479 2023-06-07 00:10:14.000000 libauc-1.3.0rc7/libauc/models/neumf.py
+-rwx------   0 zhuoning   (501) staff       (20)     1284 2023-06-07 00:11:49.000000 libauc-1.3.0rc7/libauc/models/perceptron.py
+-rwx------   0 zhuoning   (501) staff       (20)    16352 2023-05-18 03:13:49.000000 libauc-1.3.0rc7/libauc/models/resnet.py
+-rwx------   0 zhuoning   (501) staff       (20)     6836 2023-05-26 02:54:35.000000 libauc-1.3.0rc7/libauc/models/resnet_cifar.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.663119 libauc-1.3.0rc7/libauc/optimizers/
+-rwx------   0 zhuoning   (501) staff       (20)      350 2023-06-01 06:26:46.000000 libauc-1.3.0rc7/libauc/optimizers/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)     9062 2023-06-11 20:55:33.000000 libauc-1.3.0rc7/libauc/optimizers/adam.py
+-rwx------   0 zhuoning   (501) staff       (20)     8911 2023-06-11 20:49:33.000000 libauc-1.3.0rc7/libauc/optimizers/adamw.py
+-rwx------   0 zhuoning   (501) staff       (20)    12775 2023-06-11 21:05:07.000000 libauc-1.3.0rc7/libauc/optimizers/isogclr.py
+-rw-r--r--   0 zhuoning   (501) staff       (20)     1760 2023-06-02 02:43:22.000000 libauc-1.3.0rc7/libauc/optimizers/lars.py
+-rwx------   0 zhuoning   (501) staff       (20)     8217 2023-06-08 21:20:22.000000 libauc-1.3.0rc7/libauc/optimizers/midam.py
+-rwx------   0 zhuoning   (501) staff       (20)    11591 2023-06-11 20:56:14.000000 libauc-1.3.0rc7/libauc/optimizers/pdsca.py
+-rwx------   0 zhuoning   (501) staff       (20)    14772 2023-06-11 20:57:02.000000 libauc-1.3.0rc7/libauc/optimizers/pesg.py
+-rwx------   0 zhuoning   (501) staff       (20)     8297 2023-06-11 20:57:22.000000 libauc-1.3.0rc7/libauc/optimizers/sgd.py
+-rwx------   0 zhuoning   (501) staff       (20)    13546 2023-06-11 21:01:55.000000 libauc-1.3.0rc7/libauc/optimizers/soap.py
+-rwx------   0 zhuoning   (501) staff       (20)    11774 2023-06-11 21:05:08.000000 libauc-1.3.0rc7/libauc/optimizers/sogclr.py
+-rwx------   0 zhuoning   (501) staff       (20)    12722 2023-06-11 20:51:48.000000 libauc-1.3.0rc7/libauc/optimizers/song.py
+-rwx------   0 zhuoning   (501) staff       (20)    13216 2023-06-11 20:53:19.000000 libauc-1.3.0rc7/libauc/optimizers/sopa.py
+-rwx------   0 zhuoning   (501) staff       (20)    13344 2023-06-11 20:52:35.000000 libauc-1.3.0rc7/libauc/optimizers/sopa_s.py
+-rwx------   0 zhuoning   (501) staff       (20)    13081 2023-06-11 21:54:28.000000 libauc-1.3.0rc7/libauc/optimizers/sota_s.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.663323 libauc-1.3.0rc7/libauc/sampler/
+-rwx------   0 zhuoning   (501) staff       (20)       23 2023-05-25 23:27:26.000000 libauc-1.3.0rc7/libauc/sampler/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    20482 2023-06-11 19:54:36.000000 libauc-1.3.0rc7/libauc/sampler/sampler.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.663698 libauc-1.3.0rc7/libauc/utils/
+-rwx------   0 zhuoning   (501) staff       (20)       50 2023-06-01 06:26:50.000000 libauc-1.3.0rc7/libauc/utils/__init__.py
+-rwx------   0 zhuoning   (501) staff       (20)    19617 2023-06-11 22:38:49.000000 libauc-1.3.0rc7/libauc/utils/paper_utils.py
+-rwx------   0 zhuoning   (501) staff       (20)     4706 2023-06-11 05:08:04.000000 libauc-1.3.0rc7/libauc/utils/utils.py
+drwxr-xr-x   0 zhuoning   (501) staff       (20)        0 2023-06-11 22:39:18.658137 libauc-1.3.0rc7/libauc.egg-info/
+-rw-r--r--   0 zhuoning   (501) staff       (20)     4143 2023-06-11 22:39:18.000000 libauc-1.3.0rc7/libauc.egg-info/PKG-INFO
+-rw-r--r--   0 zhuoning   (501) staff       (20)     1470 2023-06-11 22:39:18.000000 libauc-1.3.0rc7/libauc.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)        1 2023-06-11 22:39:18.000000 libauc-1.3.0rc7/libauc.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)       76 2023-06-11 22:39:18.000000 libauc-1.3.0rc7/libauc.egg-info/requires.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)        7 2023-06-11 22:39:18.000000 libauc-1.3.0rc7/libauc.egg-info/top_level.txt
+-rw-r--r--   0 zhuoning   (501) staff       (20)       38 2023-06-11 22:39:18.663978 libauc-1.3.0rc7/setup.cfg
+-rw-r--r--   0 zhuoning   (501) staff       (20)      982 2023-06-11 22:39:08.000000 libauc-1.3.0rc7/setup.py
```

### Comparing `libauc-1.3.0rc6/LICENSE` & `libauc-1.3.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/PKG-INFO` & `libauc-1.3.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.0rc6
+Version: 1.3.0rc7
 Summary: LibAUC: A Deep Learning Library for X-Risk Optimization
 Home-page: https://github.com/Optimization-AI/LibAUC
 Author: Zhuoning Yuan
 Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc6 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc7 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE LibAUC: A Deep Learning for X-Risk Optimization
 ---
```

### Comparing `libauc-1.3.0rc6/README.md` & `libauc-1.3.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/breastcancer.py` & `libauc-1.3.0rc7/libauc/datasets/breastcancer.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/cat_vs_dog.py` & `libauc-1.3.0rc7/libauc/datasets/cat_vs_dog.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/chexpert.py` & `libauc-1.3.0rc7/libauc/datasets/chexpert.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/cifar.py` & `libauc-1.3.0rc7/libauc/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/dataset.py` & `libauc-1.3.0rc7/libauc/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/folder.py` & `libauc-1.3.0rc7/libauc/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/melanoma.py` & `libauc-1.3.0rc7/libauc/datasets/melanoma.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/movielens.py` & `libauc-1.3.0rc7/libauc/datasets/movielens.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/musk2.py` & `libauc-1.3.0rc7/libauc/datasets/musk2.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/datasets/stl10.py` & `libauc-1.3.0rc7/libauc/datasets/stl10.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/losses/auc.py` & `libauc-1.3.0rc7/libauc/losses/auc.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/losses/contrastive.py` & `libauc-1.3.0rc7/libauc/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/losses/losses.py` & `libauc-1.3.0rc7/libauc/losses/losses.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/losses/mil.py` & `libauc-1.3.0rc7/libauc/losses/mil.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/losses/perf_at_top.py` & `libauc-1.3.0rc7/libauc/losses/perf_at_top.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/losses/ranking.py` & `libauc-1.3.0rc7/libauc/losses/ranking.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/losses/surrogate.py` & `libauc-1.3.0rc7/libauc/losses/surrogate.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/metrics/metrics.py` & `libauc-1.3.0rc7/libauc/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/models/densenet.py` & `libauc-1.3.0rc7/libauc/models/densenet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/models/mil_models.py` & `libauc-1.3.0rc7/libauc/models/mil_models.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/models/neumf.py` & `libauc-1.3.0rc7/libauc/models/neumf.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/models/perceptron.py` & `libauc-1.3.0rc7/libauc/models/perceptron.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/models/resnet.py` & `libauc-1.3.0rc7/libauc/models/resnet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/models/resnet_cifar.py` & `libauc-1.3.0rc7/libauc/models/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/adam.py` & `libauc-1.3.0rc7/libauc/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/adamw.py` & `libauc-1.3.0rc7/libauc/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/isogclr.py` & `libauc-1.3.0rc7/libauc/optimizers/isogclr.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/lars.py` & `libauc-1.3.0rc7/libauc/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/midam.py` & `libauc-1.3.0rc7/libauc/optimizers/midam.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/pdsca.py` & `libauc-1.3.0rc7/libauc/optimizers/pdsca.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/pesg.py` & `libauc-1.3.0rc7/libauc/optimizers/pesg.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/sgd.py` & `libauc-1.3.0rc7/libauc/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/soap.py` & `libauc-1.3.0rc7/libauc/optimizers/soap.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/sogclr.py` & `libauc-1.3.0rc7/libauc/optimizers/sogclr.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/song.py` & `libauc-1.3.0rc7/libauc/optimizers/song.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/sopa.py` & `libauc-1.3.0rc7/libauc/optimizers/sopa.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/sopa_s.py` & `libauc-1.3.0rc7/libauc/optimizers/sopa_s.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/optimizers/sota_s.py` & `libauc-1.3.0rc7/libauc/optimizers/sota_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,18 @@
                      model_acc[i].data = model_acc[i].data + p.data
                        
             elif self.mode == 'sgd':
               for i, p in enumerate(group['params']):
                   if p.grad is None:
                       continue
                   #d_p = p.grad
-                  d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  if epoch_decay > 0:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + epoch_decay*(p.data - model_ref[i].data) + weight_decay*p.data
+                  else:
+                    d_p = torch.clamp(p.grad.data , -clip_value, clip_value) + weight_decay*p.data
                   if momentum != 0:
                       param_state = self.state[p]
                       if 'momentum_buffer' not in param_state:
                           buf = param_state['momentum_buffer'] = torch.clone(d_p).detach()
                       else:
                           buf = param_state['momentum_buffer']
                           buf.mul_(momentum).add_(d_p, alpha=1 - dampening)
```

### Comparing `libauc-1.3.0rc6/libauc/sampler/sampler.py` & `libauc-1.3.0rc7/libauc/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc/utils/paper_utils.py` & `libauc-1.3.0rc7/libauc/utils/paper_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 import time
 import shutil
 import math
 import numpy as np
 import logging
+from typing import Dict, Any
 from collections import Counter
 from tqdm import tqdm, trange
 from sklearn.metrics import roc_auc_score
 from ..metrics import ndcg_at_k, map_at_k
 
 _logger = logging.getLogger(__name__)
 
@@ -196,50 +197,38 @@
     for milestone in eval(lr_schedule):
         lr *= 0.25 if epoch >= milestone else 1
     for param_group in optimizer.param_groups:
         param_group['lr'] = lr
 
 def evaluate_method(predictions, ratings, topk, metrics):
     """
-        args:
-            predictions: (-1, n_candidates) shape, the first column is the score for ground-truth item
-            ratings: (# of users, # of pos items)
-            topk: top-K value list
-            metrics: metric string list
-        return: 
-            a result dict, the keys are metric@topk
+    :param predictions: (-1, n_candidates) shape, the first column is the score for ground-truth item
+    :param ratings: (# of users, # of pos items)
+    :param topk: top-K value list
+    :param metrics: metric string list
+    :return: a result dict, the keys are metric@topk
     """
     evaluations = dict()
-
-    num_of_users, num_pos_items = ratings.shape
-    sorted_ratings = -np.sort(-ratings)            # descending order !!
-    discounters = np.tile([np.log2(i+1) for i in range(1, 1+num_pos_items)], (num_of_users, 1))
-    normalizer_mat = (np.exp2(sorted_ratings) - 1) / discounters
-
-    sort_idx = (-predictions).argsort(axis=1)    # index of sorted predictions (max->min)
-    gt_rank = np.array([np.argwhere(sort_idx == i)[:, 1]+1 for i in range(num_pos_items)]).T  # rank of the ground-truth (start from 1)
     for k in topk:
-        hit = (gt_rank <= k)
         for metric in metrics:
             key = '{}@{}'.format(metric, k)
             if metric == 'NDCG':
-                evaluations[key] = ndcg_at_k(ratings, normalizer_mat, hit, gt_rank, k)
-            elif metric == 'MAP':
-                evaluations[key] = map_at_k(hit, gt_rank)
+                evaluations[key] = ndcg_at_k(ratings, predictions, k)
             else:
                 raise ValueError('Undefined evaluation metric: {}.'.format(metric))
     return evaluations
 
-def evaluate(model, data_set, topks, metrics, eval_batch_size=250, num_pos=10):
+
+def evaluate(model, data_set, topks, metrics):
     """
-        The output of this function is a 2D-array, each row corresponds to all the candidates,
-        and the ground-truth item poses the first.
+    The returned prediction is a 2D-array, each row corresponds to all the candidates,
+    and the ground-truth item poses the first.
+    Example: ground-truth items: [1, 2], 2 negative items for each instance: [[3,4], [5,6]]
+             predictions like: [[1,3,4], [2,5,6]]
     """
-    EVAL_BATCH_SIZE = eval_batch_size
-    NUM_POS = num_pos
     DEVICE = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
     model.eval()
     predictions = list()
     ratings = list()
     for idx in trange(0, len(data_set), EVAL_BATCH_SIZE):
         batch = data_set.get_batch(idx, EVAL_BATCH_SIZE)
         prediction = model(batch_to_gpu(batch, DEVICE))['prediction']
@@ -267,18 +256,14 @@
     return ','.join(format_str)
 
 
 '''
 Helper functions for iSogCLR
 '''
 
-
-
-from typing import Dict, Any
-
 class Scheduler:
     """ 
     Parameter Scheduler Base Class.
     
     A scheduler base class that can be used to schedule any optimizer parameter groups.
 
     Unlike the builtin PyTorch schedulers, this is intended to be consistently called
```

### Comparing `libauc-1.3.0rc6/libauc/utils/utils.py` & `libauc-1.3.0rc7/libauc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/libauc.egg-info/PKG-INFO` & `libauc-1.3.0rc7/libauc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.0rc6
+Version: 1.3.0rc7
 Summary: LibAUC: A Deep Learning Library for X-Risk Optimization
 Home-page: https://github.com/Optimization-AI/LibAUC
 Author: Zhuoning Yuan
 Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc6 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.0rc7 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE LibAUC: A Deep Learning for X-Risk Optimization
 ---
```

### Comparing `libauc-1.3.0rc6/libauc.egg-info/SOURCES.txt` & `libauc-1.3.0rc7/libauc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libauc-1.3.0rc6/setup.py` & `libauc-1.3.0rc7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
   
 setuptools.setup(
   name="libauc",
-  version="1.3.0rc6",
+  version="1.3.0rc7",
   author="Zhuoning Yuan",
   author_email="yzhuoning@gmail.com",
   description="LibAUC: A Deep Learning Library for X-Risk Optimization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Optimization-AI/LibAUC",
   packages=setuptools.find_packages(),
```

