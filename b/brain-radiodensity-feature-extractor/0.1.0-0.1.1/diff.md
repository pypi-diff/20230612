# Comparing `tmp/brain-radiodensity-feature-extractor-0.1.0.tar.gz` & `tmp/brain-radiodensity-feature-extractor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brain-radiodensity-feature-extractor-0.1.0.tar", last modified: Sun Jun 11 23:31:11 2023, max compression
+gzip compressed data, was "brain-radiodensity-feature-extractor-0.1.1.tar", last modified: Mon Jun 12 00:00:24 2023, max compression
```

## Comparing `brain-radiodensity-feature-extractor-0.1.0.tar` & `brain-radiodensity-feature-extractor-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 23:31:11.884648 brain-radiodensity-feature-extractor-0.1.0/
--rw-rw-rw-   0        0        0     1779 2023-06-11 23:31:11.878693 brain-radiodensity-feature-extractor-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-06-11 23:20:00.000000 brain-radiodensity-feature-extractor-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 23:31:11.846361 brain-radiodensity-feature-extractor-0.1.0/brain_feature_extractor/
--rw-rw-rw-   0        0        0     5016 2023-06-11 23:02:40.000000 brain-radiodensity-feature-extractor-0.1.0/brain_feature_extractor/BrainFeatureExtractorGMM.py
--rw-rw-rw-   0        0        0     5847 2023-06-11 23:10:53.000000 brain-radiodensity-feature-extractor-0.1.0/brain_feature_extractor/ExtractorGMM.py
--rw-rw-rw-   0        0        0     3699 2023-06-11 21:00:24.000000 brain-radiodensity-feature-extractor-0.1.0/brain_feature_extractor/GaussianMixtureModel.py
--rw-rw-rw-   0        0        0       85 2023-06-11 23:10:56.000000 brain-radiodensity-feature-extractor-0.1.0/brain_feature_extractor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 23:31:11.873711 brain-radiodensity-feature-extractor-0.1.0/brain_radiodensity_feature_extractor.egg-info/
--rw-rw-rw-   0        0        0     1779 2023-06-11 23:31:11.000000 brain-radiodensity-feature-extractor-0.1.0/brain_radiodensity_feature_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2023-06-11 23:31:11.000000 brain-radiodensity-feature-extractor-0.1.0/brain_radiodensity_feature_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 23:31:11.000000 brain-radiodensity-feature-extractor-0.1.0/brain_radiodensity_feature_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-11 23:31:11.000000 brain-radiodensity-feature-extractor-0.1.0/brain_radiodensity_feature_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-11 23:31:11.000000 brain-radiodensity-feature-extractor-0.1.0/brain_radiodensity_feature_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 23:31:11.884648 brain-radiodensity-feature-extractor-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1540 2023-06-11 23:29:01.000000 brain-radiodensity-feature-extractor-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 00:00:24.348882 brain-radiodensity-feature-extractor-0.1.1/
+-rw-rw-rw-   0        0        0     1644 2023-06-12 00:00:24.345797 brain-radiodensity-feature-extractor-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      807 2023-06-11 23:55:28.000000 brain-radiodensity-feature-extractor-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 00:00:24.310031 brain-radiodensity-feature-extractor-0.1.1/brain_feature_extractor/
+-rw-rw-rw-   0        0        0     4504 2023-06-11 23:54:18.000000 brain-radiodensity-feature-extractor-0.1.1/brain_feature_extractor/BrainFeatureExtractorGMM.py
+-rw-rw-rw-   0        0        0     5511 2023-06-11 23:53:41.000000 brain-radiodensity-feature-extractor-0.1.1/brain_feature_extractor/ExtractorGMM.py
+-rw-rw-rw-   0        0        0     3699 2023-06-11 21:00:24.000000 brain-radiodensity-feature-extractor-0.1.1/brain_feature_extractor/GaussianMixtureModel.py
+-rw-rw-rw-   0        0        0       85 2023-06-11 23:10:56.000000 brain-radiodensity-feature-extractor-0.1.1/brain_feature_extractor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 00:00:24.337822 brain-radiodensity-feature-extractor-0.1.1/brain_radiodensity_feature_extractor.egg-info/
+-rw-rw-rw-   0        0        0     1644 2023-06-12 00:00:24.000000 brain-radiodensity-feature-extractor-0.1.1/brain_radiodensity_feature_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-06-12 00:00:24.000000 brain-radiodensity-feature-extractor-0.1.1/brain_radiodensity_feature_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 00:00:24.000000 brain-radiodensity-feature-extractor-0.1.1/brain_radiodensity_feature_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-06-12 00:00:24.000000 brain-radiodensity-feature-extractor-0.1.1/brain_radiodensity_feature_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-12 00:00:24.000000 brain-radiodensity-feature-extractor-0.1.1/brain_radiodensity_feature_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 00:00:24.348882 brain-radiodensity-feature-extractor-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1540 2023-06-11 23:53:01.000000 brain-radiodensity-feature-extractor-0.1.1/setup.py
```

### Comparing `brain-radiodensity-feature-extractor-0.1.0/PKG-INFO` & `brain-radiodensity-feature-extractor-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-radiodensity-feature-extractor
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple library that extracts brain features from a Brain Tomography.
 Home-page: https://brain-radiodensity-feature-extractor.readthedocs.io/
 Author: Williana Leite
 Author-email: willianaluziasousaleite@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,14 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# brain-radiodensity-feature-extractor
-Repository responsible for extracting radiodensity characteristics from a brain CT scan.
-
 # Brain Feature Extractor
 A simple library that extracts brain features from a Brain Tomography. The constructed features refer to the regions: 
 - cerebrospinal fluid;
 - clacification;
 - gray matter;
 - white matter;
 - ischemic stroke;
```

### Comparing `brain-radiodensity-feature-extractor-0.1.0/README.md` & `brain-radiodensity-feature-extractor-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# brain-radiodensity-feature-extractor
-Repository responsible for extracting radiodensity characteristics from a brain CT scan.
-
 # Brain Feature Extractor
 A simple library that extracts brain features from a Brain Tomography. The constructed features refer to the regions: 
 - cerebrospinal fluid;
 - clacification;
 - gray matter;
 - white matter;
 - ischemic stroke;
```

### Comparing `brain-radiodensity-feature-extractor-0.1.0/brain_feature_extractor/BrainFeatureExtractorGMM.py` & `brain-radiodensity-feature-extractor-0.1.1/brain_feature_extractor/BrainFeatureExtractorGMM.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import pandas as pd
 import cv2
 import pydicom
 import time
-import logging
 from brain_feature_extractor.ExtractorGMM import ExtractorGMM
 
 
 class BrainFeatureExtractorGMM:
 
     """
     The instance extracts features related to brain regions from an entire brain scan.
@@ -22,30 +21,26 @@
     """
 
     def __init__(self, percentage: float = 0.3, pixel_level_feature: bool = False):
 
         self.percentage = percentage
         self.pixel_level_feature = pixel_level_feature
 
-        logging.basicConfig(filename = 'logs/main_logger.log', level = logging.DEBUG, format = '%(asctime)s:%(levelname)s:%(name)s:%(message)s', filemode='w')
-        self.logger = logging
-
     def _load_dcm(self, img_path: str):
 
         """
         Loading a DICOM image of a brain scan.
 
         :param img_path: Local path with DICOM file.
         :type img_path: str
 
         :return: Array with the radiodensities of the DICOM image.
         :rtype: np.array
         """
 
-        self.logger.info(f'Reading image from path: {img_path}')
         dcm = pydicom.read_file(img_path)
         rescale_intercept = int(dcm.data_element('RescaleIntercept').value)
         img = np.array(dcm.pixel_array, dtype=np.int16) + rescale_intercept
         return img
     
     def _extract_brain(self, src: np.array, inf_limit: int = 0, sup_limit: int = 100):
 
@@ -61,16 +56,14 @@
         :param inf_limit: Lower limit of Hounsfield Units (HU) that will be considered the skull region.
         :type inf_limit: np.array
 
         :return: Array with the radiodensities of the DICOM image without the skull region.
         :rtype: np.array
         """
 
-        self.logger.info('Extract brain from image CT')
-
         # Restrict the HU values to be between 0 and 255
         brain_image = np.where(src < inf_limit, 0, src)
         new_img = np.where(brain_image > sup_limit, 255, brain_image)
 
         # Get only the skull
         img = np.asarray(new_img, np.uint8)
         binary_image = np.where(img != 255, 0, img)
@@ -97,32 +90,30 @@
 
         return output
 
     def extract_features(self, path, verbose=False):
 
         """ Extract features of brain regions from a brain tomography DICOM file. """
 
-        self.logger.info('Start of feature extraction')
         brain_image = self._load_dcm(path)
         new_img = self._extract_brain(brain_image, inf_limit=0, sup_limit=120)
 
         new_img = cv2.resize(new_img, (0, 0), fx=self.percentage, fy=self.percentage) 
 
         left_img = new_img[0:new_img.shape[0], 0:int(new_img.shape[1] / 2)]
         right_img = new_img[0:new_img.shape[0], int(new_img.shape[1] / 2):int(new_img.shape[1])]
 
         init_time = time.time()
         
-        left_extractor = ExtractorGMM(left_img, self.pixel_level_feature, self.logger)
-        right_extractor = ExtractorGMM(right_img, self.pixel_level_feature, self.logger)
+        left_extractor = ExtractorGMM(left_img, self.pixel_level_feature)
+        right_extractor = ExtractorGMM(right_img, self.pixel_level_feature)
 
         left_feat = left_extractor.segmentation()
         right_feat = right_extractor.segmentation()
 
         final_time = time.time() - init_time
         if verbose:
             print(f'Extract feature of {path} - TIME: {round(final_time, 2)}, seconds ...')
 
         features = left_feat + right_feat
 
-        self.logger.info(f'Finishing feature extraction into {round(final_time, 2)} seconds')
         return [round(feat, 6) for feat in features]
```

### Comparing `brain-radiodensity-feature-extractor-0.1.0/brain_feature_extractor/ExtractorGMM.py` & `brain-radiodensity-feature-extractor-0.1.1/brain_feature_extractor/ExtractorGMM.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from numpy import ndarray
 import pandas as pd
 import yaml
 from brain_feature_extractor.GaussianMixtureModel import GaussianMixtureModel
-from logging import Logger
 import os
 
 
 class ExtractorGMM:
 
     """
     The instance extracts the features related to the brain regions of a hemisphere from the tomography.
@@ -15,24 +14,20 @@
 
     :param image: The input image.
     :type image: ndarray
 
     :param pixel_level_feature: If true, the segmentation returns the brain region of each pixel (MGABTD-pixel extractor).
                                 If false returns the percentage of pixels in each brain region (MGABTD-percent).
     :type pixel_level_feature: bool
-
-    :param logger: The main logging.
-    :type logger: Logger
     """
     
-    def __init__(self, image: ndarray, pixel_level_feature: bool, logger: Logger):
+    def __init__(self, image: ndarray, pixel_level_feature: bool):
 
         self.image = image
         self.pixel_level_feature = pixel_level_feature
-        self.logger = logger
         self.read_config()
         self.fit()
 
     def read_config(self):
 
         """ This function determines the value of the constants used to determine brain regions and to train the GMM. """
 
@@ -66,19 +61,17 @@
             self.GRAY_MATTER = list(range(int(gray_matter_threshold[0]), int(gray_matter_threshold[1]) + 1))
 
             stroke_hemorrhagic_threshold = config.get('STROKE_HEMORRHAGIC').split('-')
             self.STROKE_HEMORRHAGIC = list(range(int(stroke_hemorrhagic_threshold[0]), int(stroke_hemorrhagic_threshold[1]) + 1))
             
             calcification_threshold = config.get('CALCIFICATION').split('-')
             self.CALCIFICATION = list(range(int(calcification_threshold[0]), int(calcification_threshold[1]) + 1))
-            self.logger.info('Configuration variables read from configuration file')
 
         except:
 
-            self.logger.warning('There is something wrong with the configuration file, read default values')
             self.N_COMPONENTS_PER_CLASS = {0:2, 1:2, 2:3, 3:2, 4:2, 5:3, 6:4}
             self.N_ITER = 5
             self.NUMBER_REGIONS = 7
             self.BACKGROUND = list(range(0, 2))
             self.CEREBROSPINAL_FLUID = list(range(0, 6))
             self.STROKE_ISCHEMIC = list(range(6, 22))
             self.WHITE_MATTER = list(range(23, 35))
```

### Comparing `brain-radiodensity-feature-extractor-0.1.0/brain_feature_extractor/GaussianMixtureModel.py` & `brain-radiodensity-feature-extractor-0.1.1/brain_feature_extractor/GaussianMixtureModel.py`

 * *Files identical despite different names*

### Comparing `brain-radiodensity-feature-extractor-0.1.0/brain_radiodensity_feature_extractor.egg-info/PKG-INFO` & `brain-radiodensity-feature-extractor-0.1.1/brain_radiodensity_feature_extractor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brain-radiodensity-feature-extractor
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple library that extracts brain features from a Brain Tomography.
 Home-page: https://brain-radiodensity-feature-extractor.readthedocs.io/
 Author: Williana Leite
 Author-email: willianaluziasousaleite@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,14 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# brain-radiodensity-feature-extractor
-Repository responsible for extracting radiodensity characteristics from a brain CT scan.
-
 # Brain Feature Extractor
 A simple library that extracts brain features from a Brain Tomography. The constructed features refer to the regions: 
 - cerebrospinal fluid;
 - clacification;
 - gray matter;
 - white matter;
 - ischemic stroke;
```

### Comparing `brain-radiodensity-feature-extractor-0.1.0/setup.py` & `brain-radiodensity-feature-extractor-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Read all requeriments
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="brain-radiodensity-feature-extractor",
-    version="0.1.0",
+    version="0.1.1",
     description="A simple library that extracts brain features from a Brain Tomography.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://brain-radiodensity-feature-extractor.readthedocs.io/",
     author="Williana Leite",
     author_email="willianaluziasousaleite@gmail.com",
     license="MIT",
```

