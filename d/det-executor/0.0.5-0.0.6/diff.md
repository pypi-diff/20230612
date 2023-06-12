# Comparing `tmp/det_executor-0.0.5.tar.gz` & `tmp/det_executor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "det_executor-0.0.5.tar", last modified: Thu Apr  6 14:00:55 2023, max compression
+gzip compressed data, was "det_executor-0.0.6.tar", last modified: Mon Jun 12 18:34:29 2023, max compression
```

## Comparing `det_executor-0.0.5.tar` & `det_executor-0.0.6.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-06 14:00:55.005237 det_executor-0.0.5/
--rw-rw-r--   0 user      (1000) user      (1000)    35149 2023-02-06 08:34:12.000000 det_executor-0.0.5/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     1565 2023-04-06 14:00:55.005237 det_executor-0.0.5/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1063 2023-04-06 13:57:47.000000 det_executor-0.0.5/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-06 14:00:55.005237 det_executor-0.0.5/det_executor/
--rw-rw-r--   0 user      (1000) user      (1000)       86 2023-02-02 09:08:14.000000 det_executor-0.0.5/det_executor/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     8168 2023-04-06 13:59:28.000000 det_executor-0.0.5/det_executor/api.py
--rw-rw-r--   0 user      (1000) user      (1000)     2695 2023-02-01 13:22:18.000000 det_executor-0.0.5/det_executor/image.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-06 14:00:55.005237 det_executor-0.0.5/det_executor/models/
--rw-rw-r--   0 user      (1000) user      (1000)        6 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    81799 2023-02-02 09:07:33.000000 det_executor-0.0.5/det_executor/models/common.py
--rw-rw-r--   0 user      (1000) user      (1000)    10288 2023-02-02 09:07:33.000000 det_executor-0.0.5/det_executor/models/experimental.py
--rw-rw-r--   0 user      (1000) user      (1000)    40024 2023-02-02 09:07:33.000000 det_executor-0.0.5/det_executor/models/yolo.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-06 14:00:55.005237 det_executor-0.0.5/det_executor/utils/
--rw-rw-r--   0 user      (1000) user      (1000)      161 2023-02-01 13:36:59.000000 det_executor-0.0.5/det_executor/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2248 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/activations.py
--rw-rw-r--   0 user      (1000) user      (1000)     5616 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/add_nms.py
--rw-rw-r--   0 user      (1000) user      (1000)     6417 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/autoanchor.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-06 14:00:55.005237 det_executor-0.0.5/det_executor/utils/aws/
--rw-rw-r--   0 user      (1000) user      (1000)        5 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/aws/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1112 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/aws/resume.py
--rw-rw-r--   0 user      (1000) user      (1000)    56222 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/datasets.py
--rw-rw-r--   0 user      (1000) user      (1000)    36750 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/general.py
--rw-rw-r--   0 user      (1000) user      (1000)     3294 2023-02-01 10:41:23.000000 det_executor-0.0.5/det_executor/utils/google_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)      259 2023-02-01 13:35:09.000000 det_executor-0.0.5/det_executor/utils/load_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)    74934 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/loss.py
--rw-rw-r--   0 user      (1000) user      (1000)     5947 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/metrics.py
--rw-rw-r--   0 user      (1000) user      (1000)    15467 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/torch_utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-06 14:00:55.005237 det_executor-0.0.5/det_executor/utils/wandb_logging/
--rw-rw-r--   0 user      (1000) user      (1000)        6 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/wandb_logging/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      815 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/wandb_logging/log_dataset.py
--rw-rw-r--   0 user      (1000) user      (1000)    16265 2022-11-30 11:55:21.000000 det_executor-0.0.5/det_executor/utils/wandb_logging/wandb_utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-06 14:00:55.005237 det_executor-0.0.5/det_executor.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1565 2023-04-06 14:00:55.000000 det_executor-0.0.5/det_executor.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      972 2023-04-06 14:00:55.000000 det_executor-0.0.5/det_executor.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-06 14:00:55.000000 det_executor-0.0.5/det_executor.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       94 2023-04-06 14:00:55.000000 det_executor-0.0.5/det_executor.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       13 2023-04-06 14:00:55.000000 det_executor-0.0.5/det_executor.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-06 14:00:55.005237 det_executor-0.0.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      923 2023-04-06 14:00:35.000000 det_executor-0.0.5/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-06 14:00:55.005237 det_executor-0.0.5/test/
--rw-rw-r--   0 user      (1000) user      (1000)      216 2023-02-06 08:07:46.000000 det_executor-0.0.5/test/test_val.py
+drwxr-xr-x   0 maxwolf    (501) staff       (20)        0 2023-06-12 18:34:29.632429 det_executor-0.0.6/
+-rw-r--r--   0 maxwolf    (501) staff       (20)    35149 2023-06-12 09:54:59.000000 det_executor-0.0.6/LICENSE
+-rw-r--r--   0 maxwolf    (501) staff       (20)     6474 2023-06-12 18:34:29.632182 det_executor-0.0.6/PKG-INFO
+-rw-r--r--   0 maxwolf    (501) staff       (20)     5972 2023-06-12 18:31:15.000000 det_executor-0.0.6/README.md
+drwxr-xr-x   0 maxwolf    (501) staff       (20)        0 2023-06-12 18:34:29.624775 det_executor-0.0.6/det_executor/
+-rw-r--r--   0 maxwolf    (501) staff       (20)       86 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/__init__.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     2857 2023-06-12 18:09:45.000000 det_executor-0.0.6/det_executor/api.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     3153 2023-06-12 17:55:26.000000 det_executor-0.0.6/det_executor/arches.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     1197 2023-06-12 18:05:58.000000 det_executor-0.0.6/det_executor/base.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     2695 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/image.py
+drwxr-xr-x   0 maxwolf    (501) staff       (20)        0 2023-06-12 18:34:29.626413 det_executor-0.0.6/det_executor/models/
+-rw-r--r--   0 maxwolf    (501) staff       (20)        6 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/models/__init__.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)    81799 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/models/common.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)    10288 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/models/experimental.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)    40024 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/models/yolo.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     2458 2023-06-12 18:18:45.000000 det_executor-0.0.6/det_executor/transformer.py
+drwxr-xr-x   0 maxwolf    (501) staff       (20)        0 2023-06-12 18:34:29.630690 det_executor-0.0.6/det_executor/utils/
+-rw-r--r--   0 maxwolf    (501) staff       (20)      161 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/__init__.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     2248 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/activations.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     5616 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/add_nms.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     6417 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/autoanchor.py
+drwxr-xr-x   0 maxwolf    (501) staff       (20)        0 2023-06-12 18:34:29.631103 det_executor-0.0.6/det_executor/utils/aws/
+-rw-r--r--   0 maxwolf    (501) staff       (20)        5 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/aws/__init__.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     1112 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/aws/resume.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)    56222 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/datasets.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)    36750 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/general.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     3294 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/google_utils.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)      259 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/load_utils.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)    74934 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/loss.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     5947 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/metrics.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)    15467 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/torch_utils.py
+drwxr-xr-x   0 maxwolf    (501) staff       (20)        0 2023-06-12 18:34:29.631710 det_executor-0.0.6/det_executor/utils/wandb_logging/
+-rw-r--r--   0 maxwolf    (501) staff       (20)        6 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/wandb_logging/__init__.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)      815 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/wandb_logging/log_dataset.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)    16265 2023-06-12 09:54:59.000000 det_executor-0.0.6/det_executor/utils/wandb_logging/wandb_utils.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     3447 2023-06-12 17:27:24.000000 det_executor-0.0.6/det_executor/v7.py
+-rw-r--r--   0 maxwolf    (501) staff       (20)     1211 2023-06-12 17:21:07.000000 det_executor-0.0.6/det_executor/v8.py
+drwxr-xr-x   0 maxwolf    (501) staff       (20)        0 2023-06-12 18:34:29.625712 det_executor-0.0.6/det_executor.egg-info/
+-rw-r--r--   0 maxwolf    (501) staff       (20)     6474 2023-06-12 18:34:29.000000 det_executor-0.0.6/det_executor.egg-info/PKG-INFO
+-rw-r--r--   0 maxwolf    (501) staff       (20)     1083 2023-06-12 18:34:29.000000 det_executor-0.0.6/det_executor.egg-info/SOURCES.txt
+-rw-r--r--   0 maxwolf    (501) staff       (20)        1 2023-06-12 18:34:29.000000 det_executor-0.0.6/det_executor.egg-info/dependency_links.txt
+-rw-r--r--   0 maxwolf    (501) staff       (20)      110 2023-06-12 18:34:29.000000 det_executor-0.0.6/det_executor.egg-info/requires.txt
+-rw-r--r--   0 maxwolf    (501) staff       (20)       13 2023-06-12 18:34:29.000000 det_executor-0.0.6/det_executor.egg-info/top_level.txt
+-rw-r--r--   0 maxwolf    (501) staff       (20)       38 2023-06-12 18:34:29.632497 det_executor-0.0.6/setup.cfg
+-rw-r--r--   0 maxwolf    (501) staff       (20)      977 2023-06-12 18:32:04.000000 det_executor-0.0.6/setup.py
+drwxr-xr-x   0 maxwolf    (501) staff       (20)        0 2023-06-12 18:34:29.631941 det_executor-0.0.6/tests/
+-rw-r--r--   0 maxwolf    (501) staff       (20)      647 2023-06-12 12:39:49.000000 det_executor-0.0.6/tests/test_val.py
```

### Comparing `det_executor-0.0.5/LICENSE` & `det_executor-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/image.py` & `det_executor-0.0.6/det_executor/image.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/models/common.py` & `det_executor-0.0.6/det_executor/models/common.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/models/experimental.py` & `det_executor-0.0.6/det_executor/models/experimental.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/models/yolo.py` & `det_executor-0.0.6/det_executor/models/yolo.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/activations.py` & `det_executor-0.0.6/det_executor/utils/activations.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/add_nms.py` & `det_executor-0.0.6/det_executor/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/autoanchor.py` & `det_executor-0.0.6/det_executor/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/aws/resume.py` & `det_executor-0.0.6/det_executor/utils/aws/resume.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/datasets.py` & `det_executor-0.0.6/det_executor/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/general.py` & `det_executor-0.0.6/det_executor/utils/general.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/google_utils.py` & `det_executor-0.0.6/det_executor/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/loss.py` & `det_executor-0.0.6/det_executor/utils/loss.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/metrics.py` & `det_executor-0.0.6/det_executor/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/torch_utils.py` & `det_executor-0.0.6/det_executor/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/wandb_logging/log_dataset.py` & `det_executor-0.0.6/det_executor/utils/wandb_logging/log_dataset.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor/utils/wandb_logging/wandb_utils.py` & `det_executor-0.0.6/det_executor/utils/wandb_logging/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `det_executor-0.0.5/det_executor.egg-info/SOURCES.txt` & `det_executor-0.0.6/det_executor.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 LICENSE
 README.md
 setup.py
 det_executor/__init__.py
 det_executor/api.py
+det_executor/arches.py
+det_executor/base.py
 det_executor/image.py
+det_executor/transformer.py
+det_executor/v7.py
+det_executor/v8.py
 det_executor.egg-info/PKG-INFO
 det_executor.egg-info/SOURCES.txt
 det_executor.egg-info/dependency_links.txt
 det_executor.egg-info/requires.txt
 det_executor.egg-info/top_level.txt
 det_executor/models/__init__.py
 det_executor/models/common.py
@@ -25,8 +30,8 @@
 det_executor/utils/metrics.py
 det_executor/utils/torch_utils.py
 det_executor/utils/aws/__init__.py
 det_executor/utils/aws/resume.py
 det_executor/utils/wandb_logging/__init__.py
 det_executor/utils/wandb_logging/log_dataset.py
 det_executor/utils/wandb_logging/wandb_utils.py
-test/test_val.py
+tests/test_val.py
```

### Comparing `det_executor-0.0.5/setup.py` & `det_executor-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import os
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-requirements = ['pyyaml', 'opencv-python', 'torch', 'torchvision',
-                'requests', 'wget', 'tqdm', 'ultralytics', 'black', 'colorama', 'pthflops']
+requirements = [
+    "pyyaml",
+    "opencv-python",
+    "torch",
+    "torchvision",
+    "requests",
+    "wget",
+    "tqdm",
+    "ultralytics",
+    "black",
+    "colorama",
+    "transformers",
+    "imageio[av]",
+]
 
 setuptools.setup(
     name="det_executor",
-    version="0.0.5",
+    version="0.0.6",
     author="Maxim Volkovskiy",
     author_email="maxwolf8852@gmail.com",
     description="Python package with latest versions of YOLO architecture for training and inference",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maxwolf8852/DetExecutor.git",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
 )
```

