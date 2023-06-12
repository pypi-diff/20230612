# Comparing `tmp/radvis-0.2.3.tar.gz` & `tmp/radvis-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radvis-0.2.3.tar", last modified: Mon Jun  5 03:40:46 2023, max compression
+gzip compressed data, was "radvis-0.2.4.tar", last modified: Mon Jun 12 06:19:52 2023, max compression
```

## Comparing `radvis-0.2.3.tar` & `radvis-0.2.4.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.318421 radvis-0.2.3/
--rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     3768 2023-06-05 03:40:46.317422 radvis-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3467 2023-06-05 03:40:01.000000 radvis-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.278073 radvis-0.2.3/radvis/
--rw-rw-rw-   0        0        0      357 2023-05-29 05:35:20.000000 radvis-0.2.3/radvis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.300665 radvis-0.2.3/radvis/image/
--rw-rw-rw-   0        0        0       78 2023-05-29 02:23:29.000000 radvis-0.2.3/radvis/image/__init__.py
--rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.2.3/radvis/image/load.py
--rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.2.3/radvis/image/rad_dicom_image.py
--rw-rw-rw-   0        0        0     3673 2023-05-29 02:54:49.000000 radvis-0.2.3/radvis/image/rad_image.py
--rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.2.3/radvis/image/rad_nifti_image.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.302661 radvis-0.2.3/radvis/mesh/
--rw-rw-rw-   0        0        0      130 2023-05-29 03:00:11.000000 radvis-0.2.3/radvis/mesh/__init__.py
--rw-rw-rw-   0        0        0     1618 2023-05-29 03:00:19.000000 radvis-0.2.3/radvis/mesh/compute_mesh.py
--rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.2.3/radvis/mesh/rad_mesh.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.306172 radvis-0.2.3/radvis/processing/
--rw-rw-rw-   0        0        0      171 2023-05-29 03:20:54.000000 radvis-0.2.3/radvis/processing/__init__.py
--rw-rw-rw-   0        0        0     3165 2023-05-29 03:04:44.000000 radvis-0.2.3/radvis/processing/image.py
--rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.2.3/radvis/processing/registration.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.309176 radvis-0.2.3/radvis/visualize/
--rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.2.3/radvis/visualize/__init__.py
--rw-rw-rw-   0        0        0     9409 2023-06-05 03:35:02.000000 radvis-0.2.3/radvis/visualize/rad_slicer.py
--rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.2.3/radvis/visualize/rad_slicer_group.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.295655 radvis-0.2.3/radvis.egg-info/
--rw-rw-rw-   0        0        0     3768 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      874 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 03:40:46.000000 radvis-0.2.3/radvis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 03:40:46.318421 radvis-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-06-05 03:29:31.000000 radvis-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.310176 radvis-0.2.3/tests/
--rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.2.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.311238 radvis-0.2.3/tests/mocks/
--rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.2.3/tests/mocks/__init__.py
--rw-rw-rw-   0        0        0      455 2023-05-29 02:42:01.000000 radvis-0.2.3/tests/mocks/mock_rad_image.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.313245 radvis-0.2.3/tests/test_mesh/
--rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.2.3/tests/test_mesh/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.2.3/tests/test_mesh/test_compute_mesh.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.315245 radvis-0.2.3/tests/test_processing/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:40:16.000000 radvis-0.2.3/tests/test_processing/__init__.py
--rw-rw-rw-   0        0        0     1645 2023-05-29 02:59:47.000000 radvis-0.2.3/tests/test_processing/test_image.py
-drwxrwxrwx   0        0        0        0 2023-06-05 03:40:46.316421 radvis-0.2.3/tests/test_visualize/
--rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.2.3/tests/test_visualize/__init__.py
--rw-rw-rw-   0        0        0      837 2023-05-29 02:59:35.000000 radvis-0.2.3/tests/test_visualize/test_rad_slicer.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.408033 radvis-0.2.4/
+-rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     4135 2023-06-12 06:19:52.408033 radvis-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3834 2023-06-12 06:17:24.000000 radvis-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.352033 radvis-0.2.4/radvis/
+-rw-rw-rw-   0        0        0      357 2023-05-29 05:35:20.000000 radvis-0.2.4/radvis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.376033 radvis-0.2.4/radvis/image/
+-rw-rw-rw-   0        0        0      134 2023-06-12 06:10:13.000000 radvis-0.2.4/radvis/image/__init__.py
+-rw-rw-rw-   0        0        0     1266 2023-06-12 06:17:42.000000 radvis-0.2.4/radvis/image/instantiate.py
+-rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.2.4/radvis/image/rad_dicom_image.py
+-rw-rw-rw-   0        0        0     4024 2023-06-12 06:12:48.000000 radvis-0.2.4/radvis/image/rad_image.py
+-rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.2.4/radvis/image/rad_nifti_image.py
+-rw-rw-rw-   0        0        0     1219 2023-06-12 06:17:56.000000 radvis-0.2.4/radvis/image/rad_numpy_image.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.379034 radvis-0.2.4/radvis/mesh/
+-rw-rw-rw-   0        0        0      130 2023-05-29 03:00:11.000000 radvis-0.2.4/radvis/mesh/__init__.py
+-rw-rw-rw-   0        0        0     1618 2023-05-29 03:00:19.000000 radvis-0.2.4/radvis/mesh/compute_mesh.py
+-rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.2.4/radvis/mesh/rad_mesh.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.382033 radvis-0.2.4/radvis/processing/
+-rw-rw-rw-   0        0        0      171 2023-05-29 03:20:54.000000 radvis-0.2.4/radvis/processing/__init__.py
+-rw-rw-rw-   0        0        0     3165 2023-05-29 03:04:44.000000 radvis-0.2.4/radvis/processing/image.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.2.4/radvis/processing/registration.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.388034 radvis-0.2.4/radvis/visualize/
+-rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.2.4/radvis/visualize/__init__.py
+-rw-rw-rw-   0        0        0     9409 2023-06-05 03:35:02.000000 radvis-0.2.4/radvis/visualize/rad_slicer.py
+-rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.2.4/radvis/visualize/rad_slicer_group.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.370033 radvis-0.2.4/radvis.egg-info/
+-rw-rw-rw-   0        0        0     4135 2023-06-12 06:19:52.000000 radvis-0.2.4/radvis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      979 2023-06-12 06:19:52.000000 radvis-0.2.4/radvis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:19:52.000000 radvis-0.2.4/radvis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-12 06:19:52.000000 radvis-0.2.4/radvis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 06:19:52.000000 radvis-0.2.4/radvis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 06:19:52.409033 radvis-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-06-12 06:15:27.000000 radvis-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.392033 radvis-0.2.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.2.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.395034 radvis-0.2.4/tests/mocks/
+-rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.2.4/tests/mocks/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-05-29 02:42:01.000000 radvis-0.2.4/tests/mocks/mock_rad_image.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.398033 radvis-0.2.4/tests/test_image/
+-rw-rw-rw-   0        0        0        0 2023-06-12 06:14:11.000000 radvis-0.2.4/tests/test_image/__init__.py
+-rw-rw-rw-   0        0        0      774 2023-06-12 06:18:24.000000 radvis-0.2.4/tests/test_image/test_instantiate.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.403034 radvis-0.2.4/tests/test_mesh/
+-rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.2.4/tests/test_mesh/__init__.py
+-rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.2.4/tests/test_mesh/test_compute_mesh.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.405034 radvis-0.2.4/tests/test_processing/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:40:16.000000 radvis-0.2.4/tests/test_processing/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-05-29 02:59:47.000000 radvis-0.2.4/tests/test_processing/test_image.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:19:52.407033 radvis-0.2.4/tests/test_visualize/
+-rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.2.4/tests/test_visualize/__init__.py
+-rw-rw-rw-   0        0        0      837 2023-05-29 02:59:35.000000 radvis-0.2.4/tests/test_visualize/test_rad_slicer.py
```

### Comparing `radvis-0.2.3/LICENSE` & `radvis-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/PKG-INFO` & `radvis-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.2.3
+Version: 0.2.4
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,22 +24,40 @@
 ## RadSlice Viewer
 
 Loading an image and displaying it with a slider
 ```python
 import radvis as rv
 
 # Creates a 'RadImage' object containing the image data
-image = rv.load_image('path/to/image.nii.gz')
+image = rv.load_image('path/to/image.nii.gz') # Can also load from DICOM or Numpy files
 
 slicer = rv.RadSlicer(image, axis=0)
 
 slicer.display()
 ```
 ![](https://raw.githubusercontent.com/medlee-code/RadVis/main/images/example_0.gif?token=GHSAT0AAAAAACBJZC7OUK4KUWZ4QWBJIGJ6ZC7T4HA)
 
+
+Create a `RadImage` from a numpy array
+```python
+import radvis as rv
+import numpy as np
+
+# Creating a numpy array
+image_data = np.random.rand(100, 100, 100)
+
+# Creating a 'RadImage' object from the numpy array
+image = rv.from_numpy(image_data)
+
+slicer = rv.RadSlicer(image, axis=0)
+
+slicer.display()
+```
+
+
 Adding masks to the image
 ```python
 import radvis as rv
 import numpy as np
 
 image = rv.load_image('path/to/image.nii.gz')
```

### Comparing `radvis-0.2.3/README.md` & `radvis-0.2.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -13,22 +13,40 @@
 ## RadSlice Viewer
 
 Loading an image and displaying it with a slider
 ```python
 import radvis as rv
 
 # Creates a 'RadImage' object containing the image data
-image = rv.load_image('path/to/image.nii.gz')
+image = rv.load_image('path/to/image.nii.gz') # Can also load from DICOM or Numpy files
 
 slicer = rv.RadSlicer(image, axis=0)
 
 slicer.display()
 ```
 ![](https://raw.githubusercontent.com/medlee-code/RadVis/main/images/example_0.gif?token=GHSAT0AAAAAACBJZC7OUK4KUWZ4QWBJIGJ6ZC7T4HA)
 
+
+Create a `RadImage` from a numpy array
+```python
+import radvis as rv
+import numpy as np
+
+# Creating a numpy array
+image_data = np.random.rand(100, 100, 100)
+
+# Creating a 'RadImage' object from the numpy array
+image = rv.from_numpy(image_data)
+
+slicer = rv.RadSlicer(image, axis=0)
+
+slicer.display()
+```
+
+
 Adding masks to the image
 ```python
 import radvis as rv
 import numpy as np
 
 image = rv.load_image('path/to/image.nii.gz')
```

### Comparing `radvis-0.2.3/radvis/image/rad_dicom_image.py` & `radvis-0.2.4/radvis/image/rad_dicom_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/radvis/image/rad_image.py` & `radvis-0.2.4/radvis/image/rad_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,28 @@
         # Get the header information
         header_str = ""
         if self.metadata is not None:
             for key, value in self.metadata.items():
                 header_str += f"{key}: {value}\n"
 
         return f"{shape_str}\n{header_str}"
+    
+    def get_image_data(self) -> np.ndarray:
+        """
+        Return the image data.
+        """
+        return self.image_data
+
+    def set_image_data(self, image_data: np.ndarray) -> None:
+        """
+        Set the image data.
+
+        :param image_data: The image data to set
+        """
+        self.image_data = image_data
 
     def get_slice(self, index: int, axis: int = 0) -> np.ndarray:
         """
         Get a 2D slice of the image data along the specified axis and index.
 
         :param index: The index of the slice to take
         :param axis: The axis along which to take the slice
```

### Comparing `radvis-0.2.3/radvis/image/rad_nifti_image.py` & `radvis-0.2.4/radvis/image/rad_nifti_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/radvis/mesh/compute_mesh.py` & `radvis-0.2.4/radvis/mesh/compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/radvis/mesh/rad_mesh.py` & `radvis-0.2.4/radvis/mesh/rad_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/radvis/processing/image.py` & `radvis-0.2.4/radvis/processing/image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/radvis/visualize/rad_slicer.py` & `radvis-0.2.4/radvis/visualize/rad_slicer.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/radvis/visualize/rad_slicer_group.py` & `radvis-0.2.4/radvis/visualize/rad_slicer_group.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/radvis.egg-info/PKG-INFO` & `radvis-0.2.4/radvis.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.2.3
+Version: 0.2.4
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,22 +24,40 @@
 ## RadSlice Viewer
 
 Loading an image and displaying it with a slider
 ```python
 import radvis as rv
 
 # Creates a 'RadImage' object containing the image data
-image = rv.load_image('path/to/image.nii.gz')
+image = rv.load_image('path/to/image.nii.gz') # Can also load from DICOM or Numpy files
 
 slicer = rv.RadSlicer(image, axis=0)
 
 slicer.display()
 ```
 ![](https://raw.githubusercontent.com/medlee-code/RadVis/main/images/example_0.gif?token=GHSAT0AAAAAACBJZC7OUK4KUWZ4QWBJIGJ6ZC7T4HA)
 
+
+Create a `RadImage` from a numpy array
+```python
+import radvis as rv
+import numpy as np
+
+# Creating a numpy array
+image_data = np.random.rand(100, 100, 100)
+
+# Creating a 'RadImage' object from the numpy array
+image = rv.from_numpy(image_data)
+
+slicer = rv.RadSlicer(image, axis=0)
+
+slicer.display()
+```
+
+
 Adding masks to the image
 ```python
 import radvis as rv
 import numpy as np
 
 image = rv.load_image('path/to/image.nii.gz')
```

### Comparing `radvis-0.2.3/radvis.egg-info/SOURCES.txt` & `radvis-0.2.4/radvis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 radvis/__init__.py
 radvis.egg-info/PKG-INFO
 radvis.egg-info/SOURCES.txt
 radvis.egg-info/dependency_links.txt
 radvis.egg-info/requires.txt
 radvis.egg-info/top_level.txt
 radvis/image/__init__.py
-radvis/image/load.py
+radvis/image/instantiate.py
 radvis/image/rad_dicom_image.py
 radvis/image/rad_image.py
 radvis/image/rad_nifti_image.py
+radvis/image/rad_numpy_image.py
 radvis/mesh/__init__.py
 radvis/mesh/compute_mesh.py
 radvis/mesh/rad_mesh.py
 radvis/processing/__init__.py
 radvis/processing/image.py
 radvis/processing/registration.py
 radvis/visualize/__init__.py
 radvis/visualize/rad_slicer.py
 radvis/visualize/rad_slicer_group.py
 tests/__init__.py
 tests/mocks/__init__.py
 tests/mocks/mock_rad_image.py
+tests/test_image/__init__.py
+tests/test_image/test_instantiate.py
 tests/test_mesh/__init__.py
 tests/test_mesh/test_compute_mesh.py
 tests/test_processing/__init__.py
 tests/test_processing/test_image.py
 tests/test_visualize/__init__.py
 tests/test_visualize/test_rad_slicer.py
```

### Comparing `radvis-0.2.3/setup.py` & `radvis-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='radvis',
-    version='0.2.3',
+    version='0.2.4',
     url='https://github.com/medlee-code/RadVis',
     author='Matthew lee',
     author_email='matthewlee@medlee.io',
     description='A visualization tool for medical images',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `radvis-0.2.3/tests/test_mesh/test_compute_mesh.py` & `radvis-0.2.4/tests/test_mesh/test_compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/tests/test_processing/test_image.py` & `radvis-0.2.4/tests/test_processing/test_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.3/tests/test_visualize/test_rad_slicer.py` & `radvis-0.2.4/tests/test_visualize/test_rad_slicer.py`

 * *Files identical despite different names*

