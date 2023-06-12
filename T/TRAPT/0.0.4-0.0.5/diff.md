# Comparing `tmp/TRAPT-0.0.4.tar.gz` & `tmp/TRAPT-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TRAPT-0.0.4.tar", last modified: Wed May 31 16:31:30 2023, max compression
+gzip compressed data, was "TRAPT-0.0.5.tar", last modified: Sun Jun 11 13:25:19 2023, max compression
```

## Comparing `TRAPT-0.0.4.tar` & `TRAPT-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:31:30.384137 TRAPT-0.0.4/
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     1071 2023-05-31 09:43:38.000000 TRAPT-0.0.4/LICENSE
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     2090 2023-05-31 16:31:30.384137 TRAPT-0.0.4/PKG-INFO
--rwxrwxrwx   0 tostring  (1000) tostring  (1000)     1454 2023-05-31 16:29:23.000000 TRAPT-0.0.4/README.md
--rw-rw-r--   0 tostring  (1000) tostring  (1000)      757 2023-05-31 16:27:36.000000 TRAPT-0.0.4/pyproject.toml
--rw-rw-r--   0 tostring  (1000) tostring  (1000)       38 2023-05-31 16:31:30.384137 TRAPT-0.0.4/setup.cfg
-drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:31:30.384137 TRAPT-0.0.4/src/
-drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:31:30.384137 TRAPT-0.0.4/src/TRAPT/
--rwxrwxrwx   0 tostring  (1000) tostring  (1000)     3631 2023-05-31 09:18:18.000000 TRAPT-0.0.4/src/TRAPT/CalcSampleRPMatrix.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     1852 2023-05-17 05:42:05.000000 TRAPT-0.0.4/src/TRAPT/CalcTRAUC.py
--rwxrwxrwx   0 tostring  (1000) tostring  (1000)     3918 2023-05-31 09:18:08.000000 TRAPT-0.0.4/src/TRAPT/CalcTRRPMatrix.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     1457 2023-05-31 09:18:02.000000 TRAPT-0.0.4/src/TRAPT/CalcTRSampleRPMatrix.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     6715 2023-05-31 09:17:55.000000 TRAPT-0.0.4/src/TRAPT/DLFS.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)    13559 2023-05-31 09:49:41.000000 TRAPT-0.0.4/src/TRAPT/DLVGAE.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     5141 2023-05-31 10:19:31.000000 TRAPT-0.0.4/src/TRAPT/TRAPT.py
--rw-rw-r--   0 tostring  (1000) tostring  (1000)        0 2023-05-31 09:11:06.000000 TRAPT-0.0.4/src/TRAPT/__init__.py
-drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-05-31 16:31:30.384137 TRAPT-0.0.4/src/TRAPT.egg-info/
--rw-rw-r--   0 tostring  (1000) tostring  (1000)     2090 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/PKG-INFO
--rw-rw-r--   0 tostring  (1000) tostring  (1000)      392 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/SOURCES.txt
--rw-rw-r--   0 tostring  (1000) tostring  (1000)        1 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/dependency_links.txt
--rw-rw-r--   0 tostring  (1000) tostring  (1000)       74 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/requires.txt
--rw-rw-r--   0 tostring  (1000) tostring  (1000)        6 2023-05-31 16:31:30.000000 TRAPT-0.0.4/src/TRAPT.egg-info/top_level.txt
+drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-06-11 13:25:19.785226 TRAPT-0.0.5/
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     1071 2023-06-01 16:41:01.000000 TRAPT-0.0.5/LICENSE
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     2090 2023-06-11 13:25:19.785226 TRAPT-0.0.5/PKG-INFO
+-rwxrwxrwx   0 tostring  (1000) tostring  (1000)     1454 2023-05-31 16:29:23.000000 TRAPT-0.0.5/README.md
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)      757 2023-06-11 13:23:04.000000 TRAPT-0.0.5/pyproject.toml
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)       38 2023-06-11 13:25:19.785226 TRAPT-0.0.5/setup.cfg
+drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-06-11 13:25:19.785226 TRAPT-0.0.5/src/
+drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-06-11 13:25:19.785226 TRAPT-0.0.5/src/TRAPT/
+-rwxrwxrwx   0 tostring  (1000) tostring  (1000)     3631 2023-05-31 09:18:18.000000 TRAPT-0.0.5/src/TRAPT/CalcSampleRPMatrix.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     1852 2023-05-17 05:42:05.000000 TRAPT-0.0.5/src/TRAPT/CalcTRAUC.py
+-rwxrwxrwx   0 tostring  (1000) tostring  (1000)     3918 2023-05-31 09:18:08.000000 TRAPT-0.0.5/src/TRAPT/CalcTRRPMatrix.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     1457 2023-05-31 09:18:02.000000 TRAPT-0.0.5/src/TRAPT/CalcTRSampleRPMatrix.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     6725 2023-06-11 13:17:57.000000 TRAPT-0.0.5/src/TRAPT/DLFS.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)    13559 2023-06-11 13:15:33.000000 TRAPT-0.0.5/src/TRAPT/DLVGAE.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     2842 2023-06-11 13:25:09.000000 TRAPT-0.0.5/src/TRAPT/TRAPT.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     2392 2023-06-11 13:14:24.000000 TRAPT-0.0.5/src/TRAPT/Tools.py
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)        0 2023-05-31 09:11:06.000000 TRAPT-0.0.5/src/TRAPT/__init__.py
+drwxrwxr-x   0 tostring  (1000) tostring  (1000)        0 2023-06-11 13:25:19.785226 TRAPT-0.0.5/src/TRAPT.egg-info/
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)     2090 2023-06-11 13:25:19.000000 TRAPT-0.0.5/src/TRAPT.egg-info/PKG-INFO
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)      411 2023-06-11 13:25:19.000000 TRAPT-0.0.5/src/TRAPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)        1 2023-06-11 13:25:19.000000 TRAPT-0.0.5/src/TRAPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)       74 2023-06-11 13:25:19.000000 TRAPT-0.0.5/src/TRAPT.egg-info/requires.txt
+-rw-rw-r--   0 tostring  (1000) tostring  (1000)        6 2023-06-11 13:25:19.000000 TRAPT-0.0.5/src/TRAPT.egg-info/top_level.txt
```

### Comparing `TRAPT-0.0.4/LICENSE` & `TRAPT-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.4/PKG-INFO` & `TRAPT-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TRAPT
-Version: 0.0.4
+Version: 0.0.5
 Summary: A novel deep learning framework for transcription regulators prediction via integraing large-scale epigenomic data.
 Author-email: zhangguorui <mp798378522@gmail.com>
 Project-URL: Homepage, https://github.com/LicLab-bio/TRAPT
 Project-URL: Bug Tracker, https://github.com/LicLab-bio/TRAPT/issues
 Project-URL: Blog, http://www.licpathway.net/TRAPT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `TRAPT-0.0.4/README.md` & `TRAPT-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.4/pyproject.toml` & `TRAPT-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "TRAPT"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="zhangguorui", email="mp798378522@gmail.com" },
 ]
 description = "A novel deep learning framework for transcription regulators prediction via integraing large-scale epigenomic data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `TRAPT-0.0.4/src/TRAPT/CalcSampleRPMatrix.py` & `TRAPT-0.0.5/src/TRAPT/CalcSampleRPMatrix.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.4/src/TRAPT/CalcTRAUC.py` & `TRAPT-0.0.5/src/TRAPT/CalcTRAUC.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.4/src/TRAPT/CalcTRRPMatrix.py` & `TRAPT-0.0.5/src/TRAPT/CalcTRRPMatrix.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.4/src/TRAPT/CalcTRSampleRPMatrix.py` & `TRAPT-0.0.5/src/TRAPT/CalcTRSampleRPMatrix.py`

 * *Files identical despite different names*

### Comparing `TRAPT-0.0.4/src/TRAPT/DLFS.py` & `TRAPT-0.0.5/src/TRAPT/DLFS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import random
+import sys
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
 from keras import Input, Model
 from keras import backend as K
 from keras.callbacks import EarlyStopping
 from keras.layers import Dense, Dropout
 from keras.models import Model
 from keras.optimizers import Adam
 from keras.regularizers import Regularizer
 
-
 def seed_tensorflow(seed=2023):
     random.seed(seed)
     np.random.seed(seed)
     tf.random.set_seed(seed)
 
 
 def custom_sigmoid(x, t=1):
```

### Comparing `TRAPT-0.0.4/src/TRAPT/DLVGAE.py` & `TRAPT-0.0.5/src/TRAPT/DLVGAE.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from torch import Tensor, nn
 from torch.nn.functional import binary_cross_entropy, kl_div, mse_loss
 from torch.utils.data import DataLoader
 from torch_geometric.data import Data
 from torch_geometric.nn import VGAE, GCNConv, InnerProductDecoder
 from tqdm import tqdm
 
-from TRAPT.TRAPT import RPMatrix
+from TRAPT.Tools import RPMatrix
 
 
 def seed_torch(seed=2023):
     random.seed(seed)
     os.environ['PYTHONHASHSEED'] = str(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
```

### Comparing `TRAPT-0.0.4/src/TRAPT.egg-info/PKG-INFO` & `TRAPT-0.0.5/src/TRAPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TRAPT
-Version: 0.0.4
+Version: 0.0.5
 Summary: A novel deep learning framework for transcription regulators prediction via integraing large-scale epigenomic data.
 Author-email: zhangguorui <mp798378522@gmail.com>
 Project-URL: Homepage, https://github.com/LicLab-bio/TRAPT
 Project-URL: Bug Tracker, https://github.com/LicLab-bio/TRAPT/issues
 Project-URL: Blog, http://www.licpathway.net/TRAPT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

