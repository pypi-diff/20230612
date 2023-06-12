# Comparing `tmp/libmultilabel-0.3.0.tar.gz` & `tmp/libmultilabel-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmultilabel-0.3.0.tar", last modified: Fri Jun  9 23:22:52 2023, max compression
+gzip compressed data, was "libmultilabel-0.3.1.tar", last modified: Mon Jun 12 14:02:48 2023, max compression
```

## Comparing `libmultilabel-0.3.0.tar` & `libmultilabel-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.048615 libmultilabel-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-09 23:22:52.048615 libmultilabel-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.044615 libmultilabel-0.3.0/libmultilabel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.044615 libmultilabel-0.3.0/libmultilabel/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22536 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/linear/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.044615 libmultilabel-0.3.0/libmultilabel/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.048615 libmultilabel-0.3.0/libmultilabel/nn/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/bert_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/caml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/kim_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/labelwise_attention_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/networks/xml_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/libmultilabel/nn/nn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:22:52.044615 libmultilabel-0.3.0/libmultilabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 23:22:52.000000 libmultilabel-0.3.0/libmultilabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 23:22:37.000000 libmultilabel-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-09 23:22:52.048615 libmultilabel-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22536 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/linear/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17132 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel/nn/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/bert_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/caml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/kim_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/labelwise_attention_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/networks/xml_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/libmultilabel/nn/nn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:48.529157 libmultilabel-0.3.1/libmultilabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 14:02:48.000000 libmultilabel-0.3.1/libmultilabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-12 14:02:37.000000 libmultilabel-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-12 14:02:48.533157 libmultilabel-0.3.1/setup.cfg
```

### Comparing `libmultilabel-0.3.0/LICENSE` & `libmultilabel-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/PKG-INFO` & `libmultilabel-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
```

### Comparing `libmultilabel-0.3.0/README.md` & `libmultilabel-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/common_utils.py` & `libmultilabel-0.3.1/libmultilabel/common_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/linear/data_utils.py` & `libmultilabel-0.3.1/libmultilabel/linear/data_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/linear/linear.py` & `libmultilabel-0.3.1/libmultilabel/linear/linear.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/linear/metrics.py` & `libmultilabel-0.3.1/libmultilabel/linear/metrics.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/linear/preprocessor.py` & `libmultilabel-0.3.1/libmultilabel/linear/preprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,14 +94,19 @@
             try:
                 if "train" in dataset:
                     dataset_tf["train"]["x"] = self.vectorizer.transform(dataset["train"]["x"])
                 if "test" in dataset:
                     dataset_tf["test"]["x"] = self.vectorizer.transform(dataset["test"]["x"])
             except AttributeError:
                 raise AttributeError("Tfidf vectorizer has not been fitted.")
+        else:
+            if "train" in dataset:
+                dataset_tf["train"]["x"] = dataset["train"]["x"]
+            if "test" in dataset:
+                dataset_tf["test"]["x"] = dataset["test"]["x"]
 
         # transform a collection of raw labels to a binary matrix
         if "train" in dataset:
             dataset_tf["train"]["y"] = self.binarizer.transform(dataset["train"]["y"]).astype("d")
         if "test" in dataset:
             dataset_tf["test"]["y"] = self.binarizer.transform(dataset["test"]["y"]).astype("d")
```

### Comparing `libmultilabel-0.3.0/libmultilabel/linear/tree.py` & `libmultilabel-0.3.1/libmultilabel/linear/tree.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/linear/utils.py` & `libmultilabel-0.3.1/libmultilabel/linear/utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/logging.py` & `libmultilabel-0.3.1/libmultilabel/logging.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/data_utils.py` & `libmultilabel-0.3.1/libmultilabel/nn/data_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/metrics.py` & `libmultilabel-0.3.1/libmultilabel/nn/metrics.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/model.py` & `libmultilabel-0.3.1/libmultilabel/nn/model.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/networks/__init__.py` & `libmultilabel-0.3.1/libmultilabel/nn/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/networks/bert.py` & `libmultilabel-0.3.1/libmultilabel/nn/networks/bert.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/networks/bert_attention.py` & `libmultilabel-0.3.1/libmultilabel/nn/networks/bert_attention.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/networks/caml.py` & `libmultilabel-0.3.1/libmultilabel/nn/networks/caml.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/networks/kim_cnn.py` & `libmultilabel-0.3.1/libmultilabel/nn/networks/kim_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/networks/labelwise_attention_networks.py` & `libmultilabel-0.3.1/libmultilabel/nn/networks/labelwise_attention_networks.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/networks/modules.py` & `libmultilabel-0.3.1/libmultilabel/nn/networks/modules.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/networks/xml_cnn.py` & `libmultilabel-0.3.1/libmultilabel/nn/networks/xml_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel/nn/nn_utils.py` & `libmultilabel-0.3.1/libmultilabel/nn/nn_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/libmultilabel.egg-info/PKG-INFO` & `libmultilabel-0.3.1/libmultilabel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
```

### Comparing `libmultilabel-0.3.0/libmultilabel.egg-info/SOURCES.txt` & `libmultilabel-0.3.1/libmultilabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.3.0/setup.cfg` & `libmultilabel-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libmultilabel
-version = 0.3.0
+version = 0.3.1
 author = LibMultiLabel Team
 license = MIT License
 license_file = LICENSE
 description = A library for multi-label text classification
 long_description = See documentation here: https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 url = https://github.com/ASUS-AICS/LibMultiLabel
 project_urls =
```

