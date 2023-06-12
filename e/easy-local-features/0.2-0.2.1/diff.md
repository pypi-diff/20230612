# Comparing `tmp/easy_local_features-0.2.tar.gz` & `tmp/easy_local_features-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_local_features-0.2.tar", last modified: Mon Jun 12 15:30:11 2023, max compression
+gzip compressed data, was "easy_local_features-0.2.1.tar", last modified: Mon Jun 12 16:09:28 2023, max compression
```

## Comparing `easy_local_features-0.2.tar` & `easy_local_features-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 15:30:11.961047 easy_local_features-0.2/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      110 2023-06-12 15:30:11.961047 easy_local_features-0.2/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      595 2023-06-09 08:29:10.000000 easy_local_features-0.2/README.md
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 15:30:11.961047 easy_local_features-0.2/easy_local_features/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    34252 2023-06-12 15:25:31.000000 easy_local_features-0.2/easy_local_features/baseline_dalf.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2496 2023-06-12 15:18:17.000000 easy_local_features-0.2/easy_local_features/baseline_deal.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6102 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/baseline_disk.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4458 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/baseline_r2d2.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3979 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/baseline_superglue.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2063 2023-06-09 08:29:10.000000 easy_local_features-0.2/easy_local_features/baseline_superpoint.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 15:30:11.961047 easy_local_features-0.2/easy_local_features/datasets/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 07:43:29.000000 easy_local_features-0.2/easy_local_features/datasets/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3034 2023-06-12 07:45:31.000000 easy_local_features-0.2/easy_local_features/datasets/download.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 15:30:11.961047 easy_local_features-0.2/easy_local_features.egg-info/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      110 2023-06-12 15:30:11.000000 easy_local_features-0.2/easy_local_features.egg-info/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      537 2023-06-12 15:30:11.000000 easy_local_features-0.2/easy_local_features.egg-info/SOURCES.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-06-12 15:30:11.000000 easy_local_features-0.2/easy_local_features.egg-info/dependency_links.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       20 2023-06-12 15:30:11.000000 easy_local_features-0.2/easy_local_features.egg-info/top_level.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       38 2023-06-12 15:30:11.961047 easy_local_features-0.2/setup.cfg
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      287 2023-06-12 15:28:28.000000 easy_local_features-0.2/setup.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      927 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/PKG-INFO
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      773 2023-06-12 16:04:27.000000 easy_local_features-0.2.1/README.md
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.757359 easy_local_features-0.2.1/easy_local_features/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      327 2023-06-12 16:00:57.000000 easy_local_features-0.2.1/easy_local_features/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    34250 2023-06-12 15:41:05.000000 easy_local_features-0.2.1/easy_local_features/baseline_dalf.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2496 2023-06-12 15:18:17.000000 easy_local_features-0.2.1/easy_local_features/baseline_deal.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6102 2023-06-09 08:29:10.000000 easy_local_features-0.2.1/easy_local_features/baseline_disk.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4458 2023-06-09 08:29:10.000000 easy_local_features-0.2.1/easy_local_features/baseline_r2d2.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3979 2023-06-09 08:29:10.000000 easy_local_features-0.2.1/easy_local_features/baseline_superglue.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2063 2023-06-09 08:29:10.000000 easy_local_features-0.2.1/easy_local_features/baseline_superpoint.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/easy_local_features/datasets/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 07:43:29.000000 easy_local_features-0.2.1/easy_local_features/datasets/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3034 2023-06-12 07:45:31.000000 easy_local_features-0.2.1/easy_local_features/datasets/download.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.757359 easy_local_features-0.2.1/easy_local_features.egg-info/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      927 2023-06-12 16:09:28.000000 easy_local_features-0.2.1/easy_local_features.egg-info/PKG-INFO
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      575 2023-06-12 16:09:28.000000 easy_local_features-0.2.1/easy_local_features.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-06-12 16:09:28.000000 easy_local_features-0.2.1/easy_local_features.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       20 2023-06-12 16:09:28.000000 easy_local_features-0.2.1/easy_local_features.egg-info/top_level.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       38 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/setup.cfg
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      548 2023-06-12 16:09:23.000000 easy_local_features-0.2.1/setup.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/tests/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      112 2023-06-12 16:01:43.000000 easy_local_features-0.2.1/tests/test_dalf.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      112 2023-06-12 16:01:22.000000 easy_local_features-0.2.1/tests/test_deal.py
```

### Comparing `easy_local_features-0.2/README.md` & `easy_local_features-0.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -8,23 +8,30 @@
 pip install -r requirements.txt
 pip install .
 ```
 
 # How to use
 
 ```python
-from easy_local_features_baselines.baseline_r2d2 import R2D2_baseline
+from easy_local_features import DEAL
+# from easy_local_features import DALF, DISK, R2D2, SuperPoint, SuperGlue
 
+# Load an image
 img = cv2.imread("assets/notredame.png")
 
-extractor = R2D2_baseline()
+# Initialize the extractor
+extractor = DEAL()
 
+# Return keypoints and descriptors just like OpenCV
 keypoints, descriptors = extractor.detectAndCompute(img)
 
-...
 ```
 # TODO
 
 - [x] Add a setup.py to make it a pip package
 - [ ] Add a script to download some datasets
 - [ ] Add a download script for the pretrained models
-- [ ] Add more baselines :)
+- [ ] Add more baselines :)
+  - [ ] ASLFeat
+  - [ ] DELF
+  - [ ] LoFTR
+  - [ ] DKM
```

### Comparing `easy_local_features-0.2/easy_local_features/baseline_dalf.py` & `easy_local_features-0.2.1/easy_local_features/baseline_dalf.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import torchvision.transforms as transforms
 
 from thinplate import pytorch as TPS
 #from modules import utils
 import pyrootutils
 root = pyrootutils.find_root()
 
-class DALF_extractor:
+class DALF_baseline:
     """
     Class for extracting local features (keypoints and descriptors) using the DALF method.
 
     Args:
         model (str, optional): Path to the pre-trained DALF model file. Defaults to None, in which case the default
             pre-trained model shipped with the library will be used.
         dev (torch.device, optional): Device on which to run the model. Defaults to `torch.device('cpu')`.
@@ -903,15 +903,15 @@
       return {'map':out, 'feat':feat}
       
 ################################################################################################################
 
 
 if __name__ == "__main__":
     img = cv2.imread(str(root / "assets" / "notredame.png"))
-    extractor = DALF_extractor()
+    extractor = DALF_baseline()
 
     # Extract keypoints and descriptors
     kpts, descr = extractor.detectAndCompute(img)
 
     # Visualize keypoints
     img_kpts = cv2.drawKeypoints(img, kpts, None, color=(0, 255, 0), flags=0)
```

### Comparing `easy_local_features-0.2/easy_local_features/baseline_deal.py` & `easy_local_features-0.2.1/easy_local_features/baseline_deal.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2/easy_local_features/baseline_disk.py` & `easy_local_features-0.2.1/easy_local_features/baseline_disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2/easy_local_features/baseline_r2d2.py` & `easy_local_features-0.2.1/easy_local_features/baseline_r2d2.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2/easy_local_features/baseline_superglue.py` & `easy_local_features-0.2.1/easy_local_features/baseline_superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2/easy_local_features/baseline_superpoint.py` & `easy_local_features-0.2.1/easy_local_features/baseline_superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2/easy_local_features/datasets/download.py` & `easy_local_features-0.2.1/easy_local_features/datasets/download.py`

 * *Files identical despite different names*

