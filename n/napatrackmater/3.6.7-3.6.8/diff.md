# Comparing `tmp/napatrackmater-3.6.7.tar.gz` & `tmp/napatrackmater-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-94k0k8sz/napatrackmater-3.6.7.tar", last modified: Sun Jun 11 19:46:42 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-n9kq6jt4/napatrackmater-3.6.8.tar", last modified: Sun Jun 11 20:36:10 2023, max compression
```

## Comparing `napatrackmater-3.6.7.tar` & `napatrackmater-3.6.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 19:46:42.080200 napatrackmater-3.6.7/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.7/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 19:46:42.076941 napatrackmater-3.6.7/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.7/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 19:46:41.862095 napatrackmater-3.6.7/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.7/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.7/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.6.7/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.7/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.6.7/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13099 2023-06-11 19:45:59.000000 napatrackmater-3.6.7/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.7/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.7/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.7/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 19:46:07.000000 napatrackmater-3.6.7/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 19:46:42.054601 napatrackmater-3.6.7/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 19:46:41.000000 napatrackmater-3.6.7/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 19:46:41.000000 napatrackmater-3.6.7/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 19:46:41.000000 napatrackmater-3.6.7/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 19:46:41.000000 napatrackmater-3.6.7/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 19:46:41.000000 napatrackmater-3.6.7/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 19:46:41.000000 napatrackmater-3.6.7/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 19:46:42.081206 napatrackmater-3.6.7/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.7/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 20:36:10.386670 napatrackmater-3.6.8/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.8/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 20:36:10.378617 napatrackmater-3.6.8/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.8/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 20:36:10.095529 napatrackmater-3.6.8/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.8/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.8/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.6.8/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.8/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.6.8/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13268 2023-06-11 20:35:17.000000 napatrackmater-3.6.8/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.8/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.8/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.8/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-11 20:35:23.000000 napatrackmater-3.6.8/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-11 20:36:10.337908 napatrackmater-3.6.8/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-11 20:36:09.000000 napatrackmater-3.6.8/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-11 20:36:09.000000 napatrackmater-3.6.8/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-11 20:36:09.000000 napatrackmater-3.6.8/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-11 20:36:09.000000 napatrackmater-3.6.8/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-11 20:36:09.000000 napatrackmater-3.6.8/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-11 20:36:09.000000 napatrackmater-3.6.8/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-11 20:36:10.389642 napatrackmater-3.6.8/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.8/setup.py
```

### Comparing `napatrackmater-3.6.7/LICENSE` & `napatrackmater-3.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/PKG-INFO` & `napatrackmater-3.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.7
+Version: 3.6.8
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.7/README.md` & `napatrackmater-3.6.8/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.6.8/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.6.8/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/napatrackmater/Trackmate.py` & `napatrackmater-3.6.8/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/napatrackmater/Trackvector.py` & `napatrackmater-3.6.8/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/napatrackmater/__init__.py` & `napatrackmater-3.6.8/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/napatrackmater/clustering.py` & `napatrackmater-3.6.8/napatrackmater/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,19 +186,23 @@
                             if False not in valid:
                                     #Apply the model prediction for getting clusters
                                     vertices, faces, normals, values = marching_cubes(binary_image)
                                     mesh_obj = trimesh.Trimesh(
                                         vertices=vertices, faces=faces, process=False
                                     )
                                    
-                                    mesh_obj.sample(num_points)
-                                    x_coords = mesh_obj.vertices[:, 0]  # X coordinates
-                                    y_coords = mesh_obj.vertices[:, 1]  # Y coordinates
-                                    z_coords = mesh_obj.vertices[:, 2]  # Z coordinates
-                                    points = np.vstack((x_coords, y_coords, z_coords)).T
+
+                                    mesh_file = str(label) 
+                                    
+                                    with tempfile.TemporaryDirectory() as mesh_dir:
+                                                save_mesh_file = os.path.join(mesh_dir, mesh_file) + ".off"
+                                                mesh_obj.export(save_mesh_file) 
+                                                data = read_off(save_mesh_file)
+                                    
+                                    points = sample_points(data=data, num=num_points).numpy()
                                     if ndim == 2:
                                       cloud = get_panda_cloud_xy(points)
                                     if ndim == 3:
                                       cloud = get_panda_cloud_xyz(points)  
                                     else:
                                       cloud = get_panda_cloud_xyz(points)
```

### Comparing `napatrackmater-3.6.7/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.6.8/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/napatrackmater/fate_mapping.py` & `napatrackmater-3.6.8/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/napatrackmater/pretrained.py` & `napatrackmater-3.6.8/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.6.8/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.7
+Version: 3.6.8
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.7/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.6.8/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.7/setup.py` & `napatrackmater-3.6.8/setup.py`

 * *Files identical despite different names*

