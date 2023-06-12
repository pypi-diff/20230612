# Comparing `tmp/easy_local_features-0.1.tar.gz` & `tmp/easy_local_features-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_local_features-0.1.tar", last modified: Fri Jun  9 09:41:55 2023, max compression
+gzip compressed data, was "easy_local_features-0.2.tar", last modified: Mon Jun 12 15:30:11 2023, max compression
```

## Comparing `easy_local_features-0.1.tar` & `easy_local_features-0.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-09 09:41:55.553380 easy_local_features-0.1/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      110 2023-06-09 09:41:55.553380 easy_local_features-0.1/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      595 2023-06-09 08:29:10.000000 easy_local_features-0.1/README.md
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-09 09:41:55.553380 easy_local_features-0.1/easy_local_features/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-09 08:29:10.000000 easy_local_features-0.1/easy_local_features/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2508 2023-06-09 09:27:24.000000 easy_local_features-0.1/easy_local_features/baseline_deal.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6102 2023-06-09 08:29:10.000000 easy_local_features-0.1/easy_local_features/baseline_disk.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4458 2023-06-09 08:29:10.000000 easy_local_features-0.1/easy_local_features/baseline_r2d2.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3979 2023-06-09 08:29:10.000000 easy_local_features-0.1/easy_local_features/baseline_superglue.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2063 2023-06-09 08:29:10.000000 easy_local_features-0.1/easy_local_features/baseline_superpoint.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-09 09:41:55.553380 easy_local_features-0.1/easy_local_features.egg-info/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      110 2023-06-09 09:41:55.000000 easy_local_features-0.1/easy_local_features.egg-info/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      418 2023-06-09 09:41:55.000000 easy_local_features-0.1/easy_local_features.egg-info/SOURCES.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-06-09 09:41:55.000000 easy_local_features-0.1/easy_local_features.egg-info/dependency_links.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       20 2023-06-09 09:41:55.000000 easy_local_features-0.1/easy_local_features.egg-info/top_level.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       38 2023-06-09 09:41:55.553380 easy_local_features-0.1/setup.cfg
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      287 2023-06-09 08:57:40.000000 easy_local_features-0.1/setup.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 15:30:11.961047 easy_local_features-0.2/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      110 2023-06-12 15:30:11.961047 easy_local_features-0.2/PKG-INFO
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      595 2023-06-09 08:29:10.000000 easy_local_features-0.2/README.md
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 15:30:11.961047 easy_local_features-0.2/easy_local_features/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    34252 2023-06-12 15:25:31.000000 easy_local_features-0.2/easy_local_features/baseline_dalf.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2496 2023-06-12 15:18:17.000000 easy_local_features-0.2/easy_local_features/baseline_deal.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6102 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/baseline_disk.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4458 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/baseline_r2d2.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3979 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/baseline_superglue.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2063 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/baseline_superpoint.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 15:30:11.961047 easy_local_features-0.2/easy_local_features/datasets/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 07:43:29.000000 easy_local_features-0.2/easy_local_features/datasets/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3034 2023-06-12 07:45:31.000000 easy_local_features-0.2/easy_local_features/datasets/download.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 15:30:11.961047 easy_local_features-0.2/easy_local_features.egg-info/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      110 2023-06-12 15:30:11.000000 easy_local_features-0.2/easy_local_features.egg-info/PKG-INFO
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      537 2023-06-12 15:30:11.000000 easy_local_features-0.2/easy_local_features.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-06-12 15:30:11.000000 easy_local_features-0.2/easy_local_features.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       20 2023-06-12 15:30:11.000000 easy_local_features-0.2/easy_local_features.egg-info/top_level.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       38 2023-06-12 15:30:11.961047 easy_local_features-0.2/setup.cfg
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      287 2023-06-12 15:28:28.000000 easy_local_features-0.2/setup.py
```

### Comparing `easy_local_features-0.1/README.md` & `easy_local_features-0.2/README.md`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.1/easy_local_features/baseline_deal.py` & `easy_local_features-0.2/easy_local_features/baseline_deal.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             device = torch.device("cpu")
 
         # /home/USER/.cache/torch/hub/checkpoints/
         if model_path is None:
             cache_path = os.path.join(os.path.expanduser('~'), '.cache', 'torch', 'hub', 'checkpoints', 'DEAL')
         else:
             cache_path = model_path
-            
+
         if not os.path.exists(cache_path):
             os.makedirs(cache_path, exist_ok=True)
 
         self.deal = torch.hub.load('verlab/DEAL_NeurIPS_2021', 'DEAL', True, cache_path)
         self.deal.device = device
         self.deal.net.eval()
         self.sift = cv2.SIFT_create(max_kps)
```

### Comparing `easy_local_features-0.1/easy_local_features/baseline_disk.py` & `easy_local_features-0.2/easy_local_features/baseline_disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.1/easy_local_features/baseline_r2d2.py` & `easy_local_features-0.2/easy_local_features/baseline_r2d2.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.1/easy_local_features/baseline_superglue.py` & `easy_local_features-0.2/easy_local_features/baseline_superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.1/easy_local_features/baseline_superpoint.py` & `easy_local_features-0.2/easy_local_features/baseline_superpoint.py`

 * *Files identical despite different names*

