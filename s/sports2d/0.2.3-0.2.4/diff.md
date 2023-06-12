# Comparing `tmp/sports2d-0.2.3.tar.gz` & `tmp/sports2d-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.2.3.tar", last modified: Mon Jun 12 07:12:29 2023, max compression
+gzip compressed data, was "sports2d-0.2.4.tar", last modified: Mon Jun 12 12:28:29 2023, max compression
```

## Comparing `sports2d-0.2.3.tar` & `sports2d-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.898589 sports2d-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-12 07:12:11.000000 sports2d-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-12 07:12:29.898589 sports2d-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-06-12 07:12:11.000000 sports2d-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.894589 sports2d-0.2.3/Sports2D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.894589 sports2d-0.2.3/Sports2D/Demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Demo/Config_demo.toml
--rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Demo/demo.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Sports2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.898589 sports2d-0.2.3/Sports2D/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/Blazepose_runsave.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/test_with_blazepose.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21939 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/compute_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/detect_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 07:12:11.000000 sports2d-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-12 07:12:29.898589 sports2d-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 07:12:11.000000 sports2d-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.898589 sports2d-0.2.3/sports2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.396700 sports2d-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-12 12:28:17.000000 sports2d-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-12 12:28:29.396700 sports2d-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-06-12 12:28:17.000000 sports2d-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.388700 sports2d-0.2.4/Sports2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.388700 sports2d-0.2.4/Sports2D/Demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Demo/Config_demo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Demo/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Sports2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.392700 sports2d-0.2.4/Sports2D/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/Utilities/test_with_blazepose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/compute_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-06-12 12:28:17.000000 sports2d-0.2.4/Sports2D/detect_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 12:28:17.000000 sports2d-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-12 12:28:29.396700 sports2d-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 12:28:17.000000 sports2d-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:28:29.396700 sports2d-0.2.4/sports2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 12:28:29.000000 sports2d-0.2.4/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.2.3/LICENSE` & `sports2d-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.3/PKG-INFO` & `sports2d-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.2.3
+Version: 0.2.4
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
```

### Comparing `sports2d-0.2.3/README.md` & `sports2d-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.3/Sports2D/Demo/Config_demo.toml` & `sports2d-0.2.4/Sports2D/Demo/Config_demo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
    	
 	
 
 # ADVANCED CONFIGURATION
 	
 [pose_advanced] # only for OPENPOSE
-load_pose = true # proceeds to detection only if pose files not found
+load_pose = true # If true, don't run openpose again if json pose files are found. If false, run it and overwrite pose files. 
 save_vid = true
 save_img = true
 interp_gap_smaller_than = 5 # do not interpolate bigger gaps
 filter = true
 show_plots = false
 filter_type = 'butterworth' # butterworth, gaussian, LOESS, median
    [pose_advanced.butterworth]
@@ -60,16 +60,16 @@
    [pose_advanced.loess]
    nb_values_used = 5 # = fraction of data used * nb frames
    [pose_advanced.median]
    kernel_size = 3
 
 
 [compute_angles_advanced] # for OPENPOSE and BLAZEPOSE
-save_img = true
-save_vid = true
+show_angles_on_img = true
+show_angles_on_vid = true
 filter = false
 show_plots = false
 filter_type = 'butterworth' # butterworth, gaussian, LOESS, median
    [compute_angles_advanced.butterworth]
    order = 4 
    cut_off_frequency = 6 # Hz
    [compute_angles_advanced.gaussian]
```

### Comparing `sports2d-0.2.3/Sports2D/Demo/demo.mp4` & `sports2d-0.2.4/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.3/Sports2D/Sports2D.py` & `sports2d-0.2.4/Sports2D/Sports2D.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.3/Sports2D/Utilities/Blazepose_runsave.py` & `sports2d-0.2.4/Sports2D/Utilities/Blazepose_runsave.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.3/Sports2D/Utilities/common.py` & `sports2d-0.2.4/Sports2D/Utilities/common.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.3/Sports2D/Utilities/filter.py` & `sports2d-0.2.4/Sports2D/Utilities/filter.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.3/Sports2D/Utilities/skeletons.py` & `sports2d-0.2.4/Sports2D/Utilities/skeletons.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.3/Sports2D/compute_angles.py` & `sports2d-0.2.4/Sports2D/compute_angles.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,16 +372,16 @@
     butterworth_filter_order = config_dict.get('compute_angles_advanced').get('butterworth').get('order')
     butterworth_filter_cutoff = config_dict.get('compute_angles_advanced').get('butterworth').get('cut_off_frequency')
     gaussian_filter_kernel = config_dict.get('compute_angles_advanced').get('gaussian').get('sigma_kernel')
     loess_filter_kernel = config_dict.get('compute_angles_advanced').get('loess').get('nb_values_used')
     median_filter_kernel = config_dict.get('compute_angles_advanced').get('median').get('kernel_size')
     filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
     
-    show_angles_img = config_dict.get('compute_angles_advanced').get('save_img')
-    show_angles_vid = config_dict.get('compute_angles_advanced').get('save_vid')
+    show_angles_img = config_dict.get('compute_angles_advanced').get('show_angles_on_img')
+    show_angles_vid = config_dict.get('compute_angles_advanced').get('show_angles_on_vid')
     
     # Find csv position files in video_dir, search pose_model and video_file.stem
     logging.info(f'Retrieving csv position files in {result_dir}...')
     csv_paths = list(result_dir.glob(f'*{video_file.stem}_{pose_model}_*points*.csv'))
     logging.info(f'{len(csv_paths)} persons found.')
 
     # Compute angles
@@ -491,15 +491,15 @@
                         if frame_nb==0: img_pose.mkdir(parents=True, exist_ok=True)
                         cv2.imwrite(str(img_pose / (video_base.stem + '_' + pose_model + '.' + str(frame_nb).zfill(5)+'.png')), frame)
                     if show_angles_vid:
                         writer.write(frame)
                     frame_nb+=1
                 else:
                     break
-        
+
         if show_angles_vid:
             cap.release()
             writer.release()
             if Path.exists(video_pose): os.remove(video_pose)
             os.rename(video_pose2,video_pose)
             if Path.exists(video_pose2): os.remove(video_pose2)
```

### Comparing `sports2d-0.2.3/Sports2D/detect_pose.py` & `sports2d-0.2.4/Sports2D/detect_pose.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.3/setup.cfg` & `sports2d-0.2.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sports2d
-version = 0.2.3
+version = 0.2.4
 author = David Pagnon
 author_email = contact@david-pagnon.com
 description = Detect pose and compute 2D joint angles from a video.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/davidpagnon/Sports2D
 keywords = markerless, kinematics, OpenPose, BlazePose, joint angles, 2D, biomechanics, sports, sports-analytics
```

### Comparing `sports2d-0.2.3/sports2d.egg-info/PKG-INFO` & `sports2d-0.2.4/sports2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.2.3
+Version: 0.2.4
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
```

### Comparing `sports2d-0.2.3/sports2d.egg-info/SOURCES.txt` & `sports2d-0.2.4/sports2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

