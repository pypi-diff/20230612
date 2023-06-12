# Comparing `tmp/napatrackmater-3.6.9.tar.gz` & `tmp/napatrackmater-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-ieczq_60/napatrackmater-3.6.9.tar", last modified: Mon Jun 12 07:53:42 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-tq39lcbp/napatrackmater-3.7.0.tar", last modified: Mon Jun 12 08:29:14 2023, max compression
```

## Comparing `napatrackmater-3.6.9.tar` & `napatrackmater-3.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:53:42.335665 napatrackmater-3.6.9/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.6.9/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 07:53:42.330946 napatrackmater-3.6.9/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.6.9/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:53:42.159171 napatrackmater-3.6.9/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.6.9/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.6.9/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.6.9/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.6.9/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.6.9/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13192 2023-06-12 07:52:43.000000 napatrackmater-3.6.9/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.6.9/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.6.9/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.6.9/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-12 07:53:02.000000 napatrackmater-3.6.9/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 07:53:42.308773 napatrackmater-3.6.9/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 07:53:41.000000 napatrackmater-3.6.9/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-12 07:53:41.000000 napatrackmater-3.6.9/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-12 07:53:41.000000 napatrackmater-3.6.9/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-12 07:53:41.000000 napatrackmater-3.6.9/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-12 07:53:41.000000 napatrackmater-3.6.9/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-12 07:53:41.000000 napatrackmater-3.6.9/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-12 07:53:42.336971 napatrackmater-3.6.9/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.6.9/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 08:29:14.535812 napatrackmater-3.7.0/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.0/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 08:29:14.530806 napatrackmater-3.7.0/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.0/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 08:29:14.311875 napatrackmater-3.7.0/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.0/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.0/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.0/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.0/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.0/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13192 2023-06-12 08:28:29.000000 napatrackmater-3.7.0/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.0/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.0/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.0/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-12 08:28:36.000000 napatrackmater-3.7.0/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 08:29:14.493132 napatrackmater-3.7.0/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 08:29:13.000000 napatrackmater-3.7.0/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-12 08:29:13.000000 napatrackmater-3.7.0/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-12 08:29:13.000000 napatrackmater-3.7.0/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-12 08:29:13.000000 napatrackmater-3.7.0/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-12 08:29:13.000000 napatrackmater-3.7.0/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-12 08:29:13.000000 napatrackmater-3.7.0/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-12 08:29:14.536814 napatrackmater-3.7.0/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.0/setup.py
```

### Comparing `napatrackmater-3.6.9/LICENSE` & `napatrackmater-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/PKG-INFO` & `napatrackmater-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.9
+Version: 3.7.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.9/README.md` & `napatrackmater-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.7.0/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.7.0/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/napatrackmater/Trackmate.py` & `napatrackmater-3.7.0/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/napatrackmater/Trackvector.py` & `napatrackmater-3.7.0/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/napatrackmater/__init__.py` & `napatrackmater-3.7.0/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/napatrackmater/clustering.py` & `napatrackmater-3.7.0/napatrackmater/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         
         pretrainer = Trainer(accelerator=accelerator, devices=devices)
         results = pretrainer.predict(model=model, dataloaders=dataloader)
         outputs = zip(*results)
         
         output_cluster_centroid = output_cluster_centroid +  [tuple(centroid_input) for centroid_input in centroids]
         output_labels = output_labels + [int(float(label_input)) for label_input in labels]
-        output_cloud_eccentricity = output_cloud_eccentricity +  [tuple(get_eccentricity(cloud_input)[0]) for cloud_input in outputs]
+        output_cloud_eccentricity = output_cloud_eccentricity +  [tuple(get_eccentricity(cloud_input))[0] for cloud_input in outputs]
         output_largest_eigenvector = output_largest_eigenvector + [get_eccentricity(cloud_input)[1] for cloud_input in outputs]
         output_largest_eigenvalue = output_largest_eigenvalue + [get_eccentricity(cloud_input)[2] for cloud_input in outputs]
         output_dimensions = output_dimensions + [get_eccentricity(cloud_input)[3] for cloud_input in outputs]
         output_cloud_surface_area = output_cloud_surface_area + [float(get_surface_area(cloud_input)) for cloud_input in outputs]
                 
         return output_labels, output_cluster_centroid, output_cloud_eccentricity, output_largest_eigenvector, output_largest_eigenvalue, output_dimensions, output_cloud_surface_area
```

### Comparing `napatrackmater-3.6.9/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.7.0/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/napatrackmater/fate_mapping.py` & `napatrackmater-3.7.0/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/napatrackmater/pretrained.py` & `napatrackmater-3.7.0/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.7.0/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.6.9
+Version: 3.7.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.6.9/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.7.0/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.6.9/setup.py` & `napatrackmater-3.7.0/setup.py`

 * *Files identical despite different names*

