# Comparing `tmp/sports2d-0.2.2.tar.gz` & `tmp/sports2d-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.2.2.tar", last modified: Tue May 23 14:35:46 2023, max compression
+gzip compressed data, was "sports2d-0.2.3.tar", last modified: Mon Jun 12 07:12:29 2023, max compression
```

## Comparing `sports2d-0.2.2.tar` & `sports2d-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:35:46.383593 sports2d-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-23 14:35:35.000000 sports2d-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15786 2023-05-23 14:35:46.383593 sports2d-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-05-23 14:35:35.000000 sports2d-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:35:46.379593 sports2d-0.2.2/Sports2D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:35:46.379593 sports2d-0.2.2/Sports2D/Demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/Demo/Config_demo.toml
--rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/Demo/demo.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/Sports2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:35:46.383593 sports2d-0.2.2/Sports2D/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/Utilities/Blazepose_runsave.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/Utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/Utilities/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/Utilities/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/Utilities/test_with_blazepose.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21895 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/compute_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    24115 2023-05-23 14:35:35.000000 sports2d-0.2.2/Sports2D/detect_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 14:35:35.000000 sports2d-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-23 14:35:46.383593 sports2d-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 14:35:35.000000 sports2d-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:35:46.383593 sports2d-0.2.2/sports2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15786 2023-05-23 14:35:46.000000 sports2d-0.2.2/sports2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-23 14:35:46.000000 sports2d-0.2.2/sports2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:35:46.000000 sports2d-0.2.2/sports2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:35:46.000000 sports2d-0.2.2/sports2d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 14:35:46.000000 sports2d-0.2.2/sports2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 14:35:46.000000 sports2d-0.2.2/sports2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.898589 sports2d-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-12 07:12:11.000000 sports2d-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-12 07:12:29.898589 sports2d-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-06-12 07:12:11.000000 sports2d-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.894589 sports2d-0.2.3/Sports2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.894589 sports2d-0.2.3/Sports2D/Demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Demo/Config_demo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Demo/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Sports2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.898589 sports2d-0.2.3/Sports2D/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/Utilities/test_with_blazepose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21939 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/compute_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-06-12 07:12:11.000000 sports2d-0.2.3/Sports2D/detect_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 07:12:11.000000 sports2d-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-12 07:12:29.898589 sports2d-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 07:12:11.000000 sports2d-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:12:29.898589 sports2d-0.2.3/sports2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 07:12:29.000000 sports2d-0.2.3/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.2.2/LICENSE` & `sports2d-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.2/PKG-INFO` & `sports2d-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.2.2
+Version: 0.2.3
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -39,15 +39,15 @@
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
 [![status](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26/status.svg)](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26)
 -->
 
 
 # Sports2D
 
-**`Sports2D` lets you compute 2D joint and segment angles from a video.**
+**`Sports2D` lets you compute 2D joint positions, as well as joint and segment angles from a video.**
 
 </br>
 
 **`Announcement:` \
 User-friendly Colab version released!\
 Works on any smartphone!**\
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
```

### Comparing `sports2d-0.2.2/README.md` & `sports2d-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
 [![status](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26/status.svg)](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26)
 -->
 
 
 # Sports2D
 
-**`Sports2D` lets you compute 2D joint and segment angles from a video.**
+**`Sports2D` lets you compute 2D joint positions, as well as joint and segment angles from a video.**
 
 </br>
 
 **`Announcement:` \
 User-friendly Colab version released!\
 Works on any smartphone!**\
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
```

### Comparing `sports2d-0.2.2/Sports2D/Demo/Config_demo.toml` & `sports2d-0.2.3/Sports2D/Demo/Config_demo.toml`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.2/Sports2D/Demo/demo.mp4` & `sports2d-0.2.3/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.2/Sports2D/Sports2D.py` & `sports2d-0.2.3/Sports2D/Sports2D.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.2/Sports2D/Utilities/Blazepose_runsave.py` & `sports2d-0.2.3/Sports2D/Utilities/Blazepose_runsave.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.2/Sports2D/Utilities/common.py` & `sports2d-0.2.3/Sports2D/Utilities/common.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.2/Sports2D/Utilities/filter.py` & `sports2d-0.2.3/Sports2D/Utilities/filter.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.2/Sports2D/Utilities/skeletons.py` & `sports2d-0.2.3/Sports2D/Utilities/skeletons.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.2/Sports2D/compute_angles.py` & `sports2d-0.2.3/Sports2D/compute_angles.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,15 +472,16 @@
                 df_angles_list_frame = [df_angles_list[n].iloc[frame_nb,:] for n in range(len(df_angles_list))]
                 frame = cv2.imread(str(frames_img[frame_nb]))
                 frame = overlay_angles(frame, df_angles_list_frame)
                 if show_angles_img:
                     cv2.imwrite(str(frames_img[frame_nb]), frame)
                 if show_angles_vid:
                     writer.write(frame)
-            writer.release()
+            if show_angles_vid:
+                writer.release()
                 
         # Else from pose video (or base video if pose video does not exist)
         elif Path.exists(video_base) or Path.exists(video_pose):
             frame_nb = 0
             while cap.isOpened():
                 ret, frame = cap.read()
                 if ret == True:
@@ -491,15 +492,15 @@
                         cv2.imwrite(str(img_pose / (video_base.stem + '_' + pose_model + '.' + str(frame_nb).zfill(5)+'.png')), frame)
                     if show_angles_vid:
                         writer.write(frame)
                     frame_nb+=1
                 else:
                     break
         
-        cap.release()
-        writer.release()
         if show_angles_vid:
+            cap.release()
+            writer.release()
             if Path.exists(video_pose): os.remove(video_pose)
             os.rename(video_pose2,video_pose)
             if Path.exists(video_pose2): os.remove(video_pose2)
 
     logging.info(f'Done.')
```

### Comparing `sports2d-0.2.2/Sports2D/detect_pose.py` & `sports2d-0.2.3/Sports2D/detect_pose.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         bodyparts = ['Time']+[item for sublist in bodyparts for item in sublist]
         coords = ['seconds']+['x', 'y', 'likelihood']*keypoints_nb
         tuples = list(zip(scorer, individuals, bodyparts, coords))
         index_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'bodyparts', 'coords'])
 
         # Create dataframe
         df_list=[]
-        time = np.expand_dims( np.arange(0,len(Coords[i])/frame_rate, 1/frame_rate), axis=0 )
+        time = np.expand_dims( np.arange(0,len(Coords[i]), 1)/frame_rate, axis=0 )
         time_coords = np.concatenate(( time, Coords[i].T ))
         df_list += [pd.DataFrame(time_coords, index=index_csv).T]
 
         # Interpolate
         logging.info(f'Person {i}: Interpolating missing sequences if they are smaller than {interp_gap_smaller_than} frames.')
         df_list[0] = df_list[0].apply(common.interpolate_zeros_nans, axis=0, args = [interp_gap_smaller_than, 'linear'])
         
@@ -569,14 +569,15 @@
 
     if pose_algo == 'OPENPOSE':
         pose_model = config_dict.get('pose').get('OPENPOSE').get('openpose_model')
         json_path = result_dir / '_'.join((video_file_stem,pose_model,'json'))
 
         # Pose detection skipped if load existing json files
         if load_pose and len(list(json_path.glob('*')))>0:
+            logging.info(f'2D joint positions have already been detected. To run the analysis over again from the beginning, set "load_pose" to false in Advanced pose settings.')
             pass
         else:
             logging.info(f'Detecting 2D joint positions with OpenPose model {pose_model}, for {video_file}.')
             json_path.mkdir(parents=True, exist_ok=True)
             openpose_path = config_dict.get('pose').get('OPENPOSE').get('openpose_path')
             os.chdir(openpose_path)
             if platform =="win32":
@@ -601,8 +602,8 @@
             save_imgvid_reID(video_path, video_result_path, save_vid, save_img, pose_model)
    
      
     elif pose_algo == 'BLAZEPOSE':
         model_complexity = config_dict.get('pose').get('BLAZEPOSE').get('model_complexity')
         Blazepose_runsave.blazepose_detec_func(input_file=video_path, save_images=save_img, to_json=True, save_video=save_vid, to_csv=True, output_folder=result_dir, model_complexity=model_complexity)
 
-    logging.info(f'Done.')
+    logging.info(f'Done.')
```

### Comparing `sports2d-0.2.2/setup.cfg` & `sports2d-0.2.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sports2d
-version = 0.2.2
+version = 0.2.3
 author = David Pagnon
 author_email = contact@david-pagnon.com
 description = Detect pose and compute 2D joint angles from a video.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/davidpagnon/Sports2D
 keywords = markerless, kinematics, OpenPose, BlazePose, joint angles, 2D, biomechanics, sports, sports-analytics
```

### Comparing `sports2d-0.2.2/sports2d.egg-info/PKG-INFO` & `sports2d-0.2.3/sports2d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.2.2
+Version: 0.2.3
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -39,15 +39,15 @@
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
 [![status](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26/status.svg)](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26)
 -->
 
 
 # Sports2D
 
-**`Sports2D` lets you compute 2D joint and segment angles from a video.**
+**`Sports2D` lets you compute 2D joint positions, as well as joint and segment angles from a video.**
 
 </br>
 
 **`Announcement:` \
 User-friendly Colab version released!\
 Works on any smartphone!**\
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
```

### Comparing `sports2d-0.2.2/sports2d.egg-info/SOURCES.txt` & `sports2d-0.2.3/sports2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

