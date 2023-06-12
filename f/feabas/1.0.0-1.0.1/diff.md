# Comparing `tmp/feabas-1.0.0.tar.gz` & `tmp/feabas-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feabas-1.0.0.tar", last modified: Fri May 26 20:28:17 2023, max compression
+gzip compressed data, was "feabas-1.0.1.tar", last modified: Mon Jun 12 15:55:46 2023, max compression
```

## Comparing `feabas-1.0.0.tar` & `feabas-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.287808 feabas-1.0.0/
--rw-rw-rw-   0        0        0     1132 2023-05-25 22:40:48.000000 feabas-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      102 2023-05-25 03:23:35.000000 feabas-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    24991 2023-05-26 20:28:17.284803 feabas-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    24305 2023-05-26 20:12:32.000000 feabas-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.090378 feabas-1.0.0/configs/
--rw-rw-rw-   0        0        0     4397 2023-05-26 02:02:16.000000 feabas-1.0.0/configs/default_alignment_configs.yaml
--rw-rw-rw-   0        0        0     1769 2023-05-26 04:06:57.000000 feabas-1.0.0/configs/default_material_table.json
--rw-rw-rw-   0        0        0     3926 2023-05-23 22:12:10.000000 feabas-1.0.0/configs/default_stitching_configs.yaml
--rw-rw-rw-   0        0        0     1417 2023-05-25 22:40:48.000000 feabas-1.0.0/configs/default_thumbnail_configs.yaml
--rw-rw-rw-   0        0        0      422 2023-05-25 22:40:48.000000 feabas-1.0.0/configs/general_configs.yaml
-drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.233806 feabas-1.0.0/feabas/
--rw-rw-rw-   0        0        0       23 2022-12-26 00:25:37.000000 feabas-1.0.0/feabas/__init__.py
--rw-rw-rw-   0        0        0    30628 2023-05-26 19:32:01.000000 feabas-1.0.0/feabas/aligner.py
--rw-rw-rw-   0        0        0    17351 2023-05-15 02:09:34.000000 feabas-1.0.0/feabas/caching.py
--rw-rw-rw-   0        0        0    21850 2023-05-25 22:40:48.000000 feabas-1.0.0/feabas/common.py
--rw-rw-rw-   0        0        0     3938 2023-05-25 22:40:48.000000 feabas-1.0.0/feabas/config.py
--rw-rw-rw-   0        0        0     1659 2023-03-16 01:55:19.000000 feabas-1.0.0/feabas/constant.py
--rw-rw-rw-   0        0        0    42661 2023-05-22 19:15:16.000000 feabas-1.0.0/feabas/dal.py
--rw-rw-rw-   0        0        0     3919 2023-05-19 01:45:40.000000 feabas-1.0.0/feabas/logging.py
--rw-rw-rw-   0        0        0    39736 2023-05-24 22:57:21.000000 feabas-1.0.0/feabas/matcher.py
--rw-rw-rw-   0        0        0    16701 2023-05-26 04:06:28.000000 feabas-1.0.0/feabas/material.py
--rw-rw-rw-   0        0        0   108574 2023-05-26 19:06:46.000000 feabas-1.0.0/feabas/mesh.py
--rw-rw-rw-   0        0        0    11316 2023-05-26 16:05:44.000000 feabas-1.0.0/feabas/mipmap.py
--rw-rw-rw-   0        0        0    61117 2023-05-26 18:36:13.000000 feabas-1.0.0/feabas/optimizer.py
--rw-rw-rw-   0        0        0    26598 2023-05-19 01:53:53.000000 feabas-1.0.0/feabas/renderer.py
--rw-rw-rw-   0        0        0    51419 2023-05-23 06:03:53.000000 feabas-1.0.0/feabas/spatial.py
--rw-rw-rw-   0        0        0    68921 2023-05-19 15:37:02.000000 feabas-1.0.0/feabas/stitcher.py
--rw-rw-rw-   0        0        0    34402 2023-05-26 17:34:14.000000 feabas-1.0.0/feabas/thumbnail.py
--rw-rw-rw-   0        0        0     7662 2023-03-16 01:55:19.000000 feabas-1.0.0/feabas/visualization.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.250805 feabas-1.0.0/feabas.egg-info/
--rw-rw-rw-   0        0        0    24991 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 20:28:16.000000 feabas-1.0.0/feabas.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.266805 feabas-1.0.0/scripts/
--rw-rw-rw-   0        0        0    21378 2023-05-26 19:32:11.000000 feabas-1.0.0/scripts/align_main.py
--rw-rw-rw-   0        0        0    12888 2023-05-26 16:09:49.000000 feabas-1.0.0/scripts/stitch_main.py
--rw-rw-rw-   0        0        0    15004 2023-05-26 18:06:49.000000 feabas-1.0.0/scripts/thumbnail_main.py
--rw-rw-rw-   0        0        0       42 2023-05-26 20:28:17.288805 feabas-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-05-26 19:43:57.000000 feabas-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:28:17.279805 feabas-1.0.0/tools/
--rw-rw-rw-   0        0        0     1670 2023-05-26 18:17:21.000000 feabas-1.0.0/tools/convert_manual_thumbnail_matches.py
--rw-rw-rw-   0        0        0     3797 2023-05-24 22:25:49.000000 feabas-1.0.0/tools/visualize_align_match_coverage.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:55:46.072080 feabas-1.0.1/
+-rw-rw-rw-   0        0        0     1132 2023-05-25 22:40:48.000000 feabas-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      102 2023-05-25 03:23:35.000000 feabas-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    24991 2023-06-12 15:55:46.072080 feabas-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    24305 2023-05-26 20:12:32.000000 feabas-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 15:55:45.962705 feabas-1.0.1/configs/
+-rw-rw-rw-   0        0        0     4397 2023-06-12 14:22:12.000000 feabas-1.0.1/configs/default_alignment_configs.yaml
+-rw-rw-rw-   0        0        0     1769 2023-05-26 04:06:57.000000 feabas-1.0.1/configs/default_material_table.json
+-rw-rw-rw-   0        0        0     4057 2023-06-06 06:04:44.000000 feabas-1.0.1/configs/default_stitching_configs.yaml
+-rw-rw-rw-   0        0        0     1417 2023-06-06 06:27:36.000000 feabas-1.0.1/configs/default_thumbnail_configs.yaml
+-rw-rw-rw-   0        0        0      463 2023-06-12 14:25:18.000000 feabas-1.0.1/configs/general_configs.yaml
+drwxrwxrwx   0        0        0        0 2023-06-12 15:55:46.025200 feabas-1.0.1/feabas/
+-rw-rw-rw-   0        0        0       23 2022-12-26 00:25:37.000000 feabas-1.0.1/feabas/__init__.py
+-rw-rw-rw-   0        0        0    30628 2023-05-26 19:32:01.000000 feabas-1.0.1/feabas/aligner.py
+-rw-rw-rw-   0        0        0    17351 2023-05-15 02:09:34.000000 feabas-1.0.1/feabas/caching.py
+-rw-rw-rw-   0        0        0    21850 2023-05-25 22:40:48.000000 feabas-1.0.1/feabas/common.py
+-rw-rw-rw-   0        0        0     4697 2023-06-12 14:33:29.000000 feabas-1.0.1/feabas/config.py
+-rw-rw-rw-   0        0        0     1659 2023-03-16 01:55:19.000000 feabas-1.0.1/feabas/constant.py
+-rw-rw-rw-   0        0        0    42731 2023-06-06 06:28:05.000000 feabas-1.0.1/feabas/dal.py
+-rw-rw-rw-   0        0        0     3919 2023-05-19 01:45:40.000000 feabas-1.0.1/feabas/logging.py
+-rw-rw-rw-   0        0        0    39736 2023-05-24 22:57:21.000000 feabas-1.0.1/feabas/matcher.py
+-rw-rw-rw-   0        0        0    16701 2023-05-26 04:06:28.000000 feabas-1.0.1/feabas/material.py
+-rw-rw-rw-   0        0        0   108574 2023-05-26 19:06:46.000000 feabas-1.0.1/feabas/mesh.py
+-rw-rw-rw-   0        0        0    11320 2023-06-03 22:24:34.000000 feabas-1.0.1/feabas/mipmap.py
+-rw-rw-rw-   0        0        0    61117 2023-05-26 18:36:13.000000 feabas-1.0.1/feabas/optimizer.py
+-rw-rw-rw-   0        0        0    26598 2023-05-19 01:53:53.000000 feabas-1.0.1/feabas/renderer.py
+-rw-rw-rw-   0        0        0    51419 2023-05-23 06:03:53.000000 feabas-1.0.1/feabas/spatial.py
+-rw-rw-rw-   0        0        0    68921 2023-05-19 15:37:02.000000 feabas-1.0.1/feabas/stitcher.py
+-rw-rw-rw-   0        0        0    34402 2023-05-26 17:34:14.000000 feabas-1.0.1/feabas/thumbnail.py
+-rw-rw-rw-   0        0        0     7662 2023-03-16 01:55:19.000000 feabas-1.0.1/feabas/visualization.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:55:46.040829 feabas-1.0.1/feabas.egg-info/
+-rw-rw-rw-   0        0        0    24991 2023-06-12 15:55:45.000000 feabas-1.0.1/feabas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2023-06-12 15:55:45.000000 feabas-1.0.1/feabas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 15:55:45.000000 feabas-1.0.1/feabas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-06-12 15:55:45.000000 feabas-1.0.1/feabas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 15:55:45.000000 feabas-1.0.1/feabas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 15:55:46.056452 feabas-1.0.1/scripts/
+-rw-rw-rw-   0        0        0    21378 2023-05-26 19:32:11.000000 feabas-1.0.1/scripts/align_main.py
+-rw-rw-rw-   0        0        0    12927 2023-06-06 04:21:22.000000 feabas-1.0.1/scripts/stitch_main.py
+-rw-rw-rw-   0        0        0    15364 2023-06-12 14:40:06.000000 feabas-1.0.1/scripts/thumbnail_main.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 15:55:46.072080 feabas-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-06-06 06:07:48.000000 feabas-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:55:46.056452 feabas-1.0.1/tools/
+-rw-rw-rw-   0        0        0     1670 2023-05-26 18:17:21.000000 feabas-1.0.1/tools/convert_manual_thumbnail_matches.py
+-rw-rw-rw-   0        0        0     3797 2023-05-24 22:25:49.000000 feabas-1.0.1/tools/visualize_align_match_coverage.py
```

### Comparing `feabas-1.0.0/LICENSE` & `feabas-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/PKG-INFO` & `feabas-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feabas
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library for stitching & alignment of connectome datasets using finite-element method.
 Author: Yuelong Wu
 Author-email: yuelong.wu.2017@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feabas-1.0.0/README.md` & `feabas-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/configs/default_alignment_configs.yaml` & `feabas-1.0.1/configs/default_alignment_configs.yaml`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/configs/default_material_table.json` & `feabas-1.0.1/configs/default_material_table.json`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/configs/default_stitching_configs.yaml` & `feabas-1.0.1/configs/default_stitching_configs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     out_dir: null # directory to save the stitched images. if set to null, default to working_directory/stitched_sections
     num_workers: 5
     tile_size: [4096, 4096] # output tile size
     scale: 1.0
     resolution: null    # if null, use the intrinsic image resolution; otherwise scale to this resolution
     loader_settings: # see dal.AbstractImageLoader for details
         cache_size: 150
-        apply_CLAHE: true
+        apply_CLAHE: true # opencv clahe not properly working for 16-bit
         inverse: true
         fillval: 0
+        dtype: null # can be uint8, uint16 etc. to use the src dtype, set to null 
     render_settings:
         blend: PYRAMID  # options: LINEAR, NEAREST, PYRAMID, MAX, MIN, NONE
     filename_settings:  # see stitcher.MontageRenderer.plan_render_series for details
         pattern: _tr{ROW_IND}-tc{COL_IND}.png
         one_based: true # zero-based or one-based row/colume indexing
```

### Comparing `feabas-1.0.0/configs/default_thumbnail_configs.yaml` & `feabas-1.0.1/configs/default_thumbnail_configs.yaml`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/aligner.py` & `feabas-1.0.1/feabas/aligner.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/caching.py` & `feabas-1.0.1/feabas/caching.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/common.py` & `feabas-1.0.1/feabas/common.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/config.py` & `feabas-1.0.1/feabas/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+import math
 import os
 import yaml
 from feabas import constant
 
+if os.path.isfile(os.path.join(os.getcwd(), 'configs', 'general_configs.yaml')):
+    _default_configuration_folder = os.path.join(os.getcwd(), 'configs')
+elif os.path.isfile(os.path.join(os.path.dirname(os.getcwd()), 'configs', 'general_configs.yaml')):
+    _default_configuration_folder = os.path.join(os.path.dirname(os.getcwd()), 'configs')
+else:
+    _default_configuration_folder = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'configs')
 
-_default_configuration_folder = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'configs')
 
 def general_settings():
     config_file = os.path.join(_default_configuration_folder, 'general_configs.yaml')
     if os.path.isfile(config_file):
         with open(config_file, 'r') as f:
             conf = yaml.safe_load(f)
     else:
@@ -66,14 +72,19 @@
         assert(os.path.isfile(config_file))
     return config_file
 
 
 def align_configs():
     with open(align_config_file(), 'r') as f:
         conf = yaml.safe_load(f)
+    section_thickness = general_settings().get('section_thickness', None)
+    if (section_thickness is not None) and (conf.get('matching', {}).get('working_mip_level', None) is None):
+        align_mip = max(0, math.floor(math.log2(section_thickness / DEFAULT_RESOLUTION)))
+        conf.setdefault('matching', {})
+        conf['matching'].setdefault('working_mip_level', align_mip)
     return conf
 
 
 def thumbnail_config_file():
     work_dir = get_work_dir()
     config_file = os.path.join(work_dir, 'configs', 'thumbnail_configs.yaml')
     if not os.path.isfile(config_file):
```

### Comparing `feabas-1.0.0/feabas/constant.py` & `feabas-1.0.1/feabas/constant.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/dal.py` & `feabas-1.0.1/feabas/dal.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,17 +359,17 @@
 
 
     def _read_image(self, imgpath, **kwargs):
         number_of_channels = kwargs.get('number_of_channels', self._number_of_channels)
         dtype = kwargs.get('dtype', self._dtype)
         apply_CLAHE = kwargs.get('apply_CLAHE', self._apply_CLAHE)
         inverse = kwargs.get('inverse', self._inverse)
-        if number_of_channels == 3:
+        if (number_of_channels == 3) and (np.dtype(dtype) == np.uint8):
             img = common.imread(imgpath, flag=cv2.IMREAD_COLOR)
-        elif number_of_channels == 1:
+        elif (number_of_channels == 1) and np.dtype(dtype) == np.uint8:
             img = common.imread(imgpath, flag=cv2.IMREAD_GRAYSCALE)
         else:
             img = common.imread(imgpath, flag=cv2.IMREAD_UNCHANGED)
         self._read_counter += 1
         if img is None:
             raise RuntimeError(f'Image file {imgpath} not valid!')
         if dtype is None:
```

### Comparing `feabas-1.0.0/feabas/logging.py` & `feabas-1.0.1/feabas/logging.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/matcher.py` & `feabas-1.0.1/feabas/matcher.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/material.py` & `feabas-1.0.1/feabas/material.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/mesh.py` & `feabas-1.0.1/feabas/mesh.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/mipmap.py` & `feabas-1.0.1/feabas/mipmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
     hist_num = kwargs.get('hist_num', 3000)
     right_lower_bound = kwargs.get('r_lower_bound', 0.7)
     right_upper_bound = kwargs.get('r_upper_bound', 1.0)
     left_lower_bound = kwargs.get('l_lower_bound', 0.0)
     left_upper_bound = kwargs.get('l_upper_bound', 0.3)
     num_gain = 50
     data0 = img[(img > img.min()) & (img < img.max())]
-    bin_edges = np.linspace(img.min(), img.max(), num=hist_num, endpoint=True)
+    bin_edges = np.linspace(data0.min(), data0.max(), num=hist_num, endpoint=True)
     edge_cntrs = (bin_edges[:-1] + bin_edges[1:]) / 2
     hist, _ = np.histogram(data0, bins=bin_edges)
     cdf = np.cumsum(hist, axis=None)
     if right_upper_bound == 1.0:
         ru = np.max(data0)
     else:
         ru = np.quantile(data0, right_upper_bound)
```

### Comparing `feabas-1.0.0/feabas/optimizer.py` & `feabas-1.0.1/feabas/optimizer.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/renderer.py` & `feabas-1.0.1/feabas/renderer.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/spatial.py` & `feabas-1.0.1/feabas/spatial.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/stitcher.py` & `feabas-1.0.1/feabas/stitcher.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/thumbnail.py` & `feabas-1.0.1/feabas/thumbnail.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas/visualization.py` & `feabas-1.0.1/feabas/visualization.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/feabas.egg-info/PKG-INFO` & `feabas-1.0.1/feabas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feabas
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library for stitching & alignment of connectome datasets using finite-element method.
 Author: Yuelong Wu
 Author-email: yuelong.wu.2017@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feabas-1.0.0/feabas.egg-info/SOURCES.txt` & `feabas-1.0.1/feabas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/scripts/align_main.py` & `feabas-1.0.1/scripts/align_main.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/scripts/stitch_main.py` & `feabas-1.0.1/scripts/stitch_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,15 @@
     root_dir = config.get_work_dir()
     generate_settings = config.general_settings()
     num_cpus = generate_settings['cpu_budget']
 
     stitch_configs = config.stitch_configs()
     if args.mode.lower().startswith('r'):
         stitch_configs = stitch_configs['rendering']
+        stitch_configs.pop('out_dir')
         mode = 'rendering'
     elif args.mode.lower().startswith('o'):
         stitch_configs = stitch_configs['optimization']
         mode = 'optimization'
     else:
         stitch_configs = stitch_configs['matching']
         mode = 'matching'
```

### Comparing `feabas-1.0.0/scripts/thumbnail_main.py` & `feabas-1.0.1/scripts/thumbnail_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,31 +223,38 @@
     manual_dir = os.path.join(thumbnail_dir, 'manual_matches')
     match_dir = os.path.join(thumbnail_dir, 'matches')
     feature_match_dir = os.path.join(thumbnail_dir, 'feature_matches')
     if mode == 'downsample':
         logger_info = logging.initialize_main_logger(logger_name='stitch_mipmap', mp=num_workers>1)
         thumbnail_configs['logger'] = logger_info[0]
         logger= logging.get_logger(logger_info[0])
-        max_mip = thumbnail_configs.pop('max_mip', thumbnail_mip_lvl-1)
+        max_mip = thumbnail_configs.pop('max_mip', max(0, thumbnail_mip_lvl-1))
+        align_mip = config.align_configs['matching']['working_mip_level']
+        max_mip = max(align_mip, max_mip)
         src_dir0 = config.stitch_render_dir()
         stitch_conf = config.stitch_configs()['rendering']
         pattern = stitch_conf['filename_settings']['pattern']
         one_based = stitch_conf['filename_settings']['one_based']
         fillval = stitch_conf['loader_settings'].get('fillval', 0)
         thumbnail_configs.setdefault('pattern', pattern)
         thumbnail_configs.setdefault('one_based', one_based)
         thumbnail_configs.setdefault('fillval', fillval)
         generate_stitched_mipmaps(src_dir0, max_mip, **thumbnail_configs)
         if thumbnail_configs.get('thumbnail_highpass', True):
-            src_dir = os.path.join(src_dir0, 'mip'+str(thumbnail_mip_lvl-2))
-            downsample = 4
-            highpass = True
+            src_mip = max(0, thumbnail_mip_lvl-2)
+            src_dir = os.path.join(src_dir0, 'mip'+str(src_mip))
+            downsample = 2 ** (thumbnail_mip_lvl - src_mip)
+            if downsample >= 4:
+                highpass = True
+            else:
+                highpass = False
         else:
-            src_dir = os.path.join(src_dir0, 'mip'+str(thumbnail_mip_lvl-1))
-            downsample = 2
+            src_mip = max(0, thumbnail_mip_lvl-1)
+            src_dir = os.path.join(src_dir0, 'mip'+str(src_mip))
+            downsample = 2 ** (thumbnail_mip_lvl - src_mip)
             highpass = False
         thumbnail_configs.setdefault('downsample', downsample)
         thumbnail_configs.setdefault('highpass', highpass)
         slist = generate_thumbnails(src_dir, img_dir, **thumbnail_configs)
         mask_scale = 1 / (2 ** thumbnail_mip_lvl)
         generate_thumbnail_masks(stitch_tform_dir, mat_mask_dir, seclist=slist, scale=mask_scale, 
                                  img_dir=img_dir, **thumbnail_configs)
```

### Comparing `feabas-1.0.0/setup.py` & `feabas-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name='feabas',
```

### Comparing `feabas-1.0.0/tools/convert_manual_thumbnail_matches.py` & `feabas-1.0.1/tools/convert_manual_thumbnail_matches.py`

 * *Files identical despite different names*

### Comparing `feabas-1.0.0/tools/visualize_align_match_coverage.py` & `feabas-1.0.1/tools/visualize_align_match_coverage.py`

 * *Files identical despite different names*

