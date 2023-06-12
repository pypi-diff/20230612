# Comparing `tmp/napatrackmater-3.7.1.tar.gz` & `tmp/napatrackmater-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-yt3w20sc/napatrackmater-3.7.1.tar", last modified: Mon Jun 12 09:11:04 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-btysop2f/napatrackmater-3.7.2.tar", last modified: Mon Jun 12 12:02:17 2023, max compression
```

## Comparing `napatrackmater-3.7.1.tar` & `napatrackmater-3.7.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 09:11:04.955763 napatrackmater-3.7.1/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.1/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 09:11:04.950247 napatrackmater-3.7.1/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.1/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 09:11:04.783078 napatrackmater-3.7.1/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.1/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.1/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.1/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.1/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.1/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13199 2023-06-12 09:10:28.000000 napatrackmater-3.7.1/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.1/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.1/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.1/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-12 09:10:36.000000 napatrackmater-3.7.1/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 09:11:04.929188 napatrackmater-3.7.1/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 09:11:04.000000 napatrackmater-3.7.1/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-12 09:11:04.000000 napatrackmater-3.7.1/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-12 09:11:04.000000 napatrackmater-3.7.1/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-12 09:11:04.000000 napatrackmater-3.7.1/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-12 09:11:04.000000 napatrackmater-3.7.1/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-12 09:11:04.000000 napatrackmater-3.7.1/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-12 09:11:04.956759 napatrackmater-3.7.1/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.1/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 12:02:17.837670 napatrackmater-3.7.2/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.2/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 12:02:17.835448 napatrackmater-3.7.2/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.2/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 12:02:17.672942 napatrackmater-3.7.2/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.2/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.2/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.2/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.2/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.2/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13264 2023-06-12 12:01:31.000000 napatrackmater-3.7.2/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.2/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.2/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.2/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-12 12:01:36.000000 napatrackmater-3.7.2/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 12:02:17.810264 napatrackmater-3.7.2/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 12:02:16.000000 napatrackmater-3.7.2/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-12 12:02:17.000000 napatrackmater-3.7.2/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-12 12:02:16.000000 napatrackmater-3.7.2/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-12 12:02:16.000000 napatrackmater-3.7.2/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-12 12:02:16.000000 napatrackmater-3.7.2/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-12 12:02:16.000000 napatrackmater-3.7.2/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-12 12:02:17.839022 napatrackmater-3.7.2/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.2/setup.py
```

### Comparing `napatrackmater-3.7.1/LICENSE` & `napatrackmater-3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/PKG-INFO` & `napatrackmater-3.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.1
+Version: 3.7.2
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.1/README.md` & `napatrackmater-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.7.2/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.7.2/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/napatrackmater/Trackmate.py` & `napatrackmater-3.7.2/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/napatrackmater/Trackvector.py` & `napatrackmater-3.7.2/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/napatrackmater/__init__.py` & `napatrackmater-3.7.2/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/napatrackmater/clustering.py` & `napatrackmater-3.7.2/napatrackmater/clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,22 +130,21 @@
         output_dimensions = []
         dataset = PointCloudDataset(clouds, scale_z=scale_z, scale_xy=scale_xy)
         dataloader = DataLoader(dataset, batch_size = batch_size)
         model.eval()
         
         pretrainer = Trainer(accelerator=accelerator, devices=devices)
         outputs = pretrainer.predict(model=model, dataloaders=dataloader)
-        outputs = outputs.detach().cpu().numpy()
         output_cluster_centroid = output_cluster_centroid +  [tuple(centroid_input) for centroid_input in centroids]
         output_labels = output_labels + [int(float(label_input)) for label_input in labels]
-        output_cloud_eccentricity = output_cloud_eccentricity +  [tuple(get_eccentricity(cloud_input))[0] for cloud_input in outputs]
-        output_largest_eigenvector = output_largest_eigenvector + [get_eccentricity(cloud_input)[1] for cloud_input in outputs]
-        output_largest_eigenvalue = output_largest_eigenvalue + [get_eccentricity(cloud_input)[2] for cloud_input in outputs]
-        output_dimensions = output_dimensions + [get_eccentricity(cloud_input)[3] for cloud_input in outputs]
-        output_cloud_surface_area = output_cloud_surface_area + [float(get_surface_area(cloud_input)) for cloud_input in outputs]
+        output_cloud_eccentricity = output_cloud_eccentricity +  [tuple(get_eccentricity(cloud_input.detach().cpu().numpy()))[0] for cloud_input in outputs]
+        output_largest_eigenvector = output_largest_eigenvector + [get_eccentricity(cloud_input.detach().cpu().numpy())[1] for cloud_input in outputs]
+        output_largest_eigenvalue = output_largest_eigenvalue + [get_eccentricity(cloud_input.detach().cpu().numpy())[2] for cloud_input in outputs]
+        output_dimensions = output_dimensions + [get_eccentricity(cloud_input.detach().cpu().numpy())[3] for cloud_input in outputs]
+        output_cloud_surface_area = output_cloud_surface_area + [float(get_surface_area(cloud_input.detach().cpu().numpy())) for cloud_input in outputs]
                 
         return output_labels, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area             
 
 
        
 
 def _label_cluster(label_image, num_points, min_size, ndim):
```

### Comparing `napatrackmater-3.7.1/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.7.2/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/napatrackmater/fate_mapping.py` & `napatrackmater-3.7.2/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/napatrackmater/pretrained.py` & `napatrackmater-3.7.2/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.7.2/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.1
+Version: 3.7.2
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.1/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.7.2/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.1/setup.py` & `napatrackmater-3.7.2/setup.py`

 * *Files identical despite different names*

