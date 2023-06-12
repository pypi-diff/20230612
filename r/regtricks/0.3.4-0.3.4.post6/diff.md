# Comparing `tmp/regtricks-0.3.4.tar.gz` & `tmp/regtricks-0.3.4.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/regtricks-0.3.4.tar", last modified: Wed Jan  5 11:14:07 2022, max compression
+gzip compressed data, was "regtricks-0.3.4.post6.tar", last modified: Mon Jun 12 18:59:31 2023, max compression
```

## Comparing `regtricks-0.3.4.tar` & `regtricks-0.3.4.post6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2022-01-05 11:14:07.000000 regtricks-0.3.4/
--rw-r--r--   0 thomaskirk   (501) staff       (20)     1249 2022-01-05 11:14:07.000000 regtricks-0.3.4/PKG-INFO
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2022-01-05 11:14:07.000000 regtricks-0.3.4/regtricks.egg-info/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1249 2022-01-05 11:14:07.000000 regtricks-0.3.4/regtricks.egg-info/PKG-INFO
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2022-01-05 11:14:07.000000 regtricks-0.3.4/regtricks.egg-info/SOURCES.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2022-01-05 11:14:07.000000 regtricks-0.3.4/regtricks.egg-info/requires.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2022-01-05 11:14:07.000000 regtricks-0.3.4/regtricks.egg-info/top_level.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2022-01-05 11:14:07.000000 regtricks-0.3.4/regtricks.egg-info/dependency_links.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.4/LICENSE
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.4/requirements.txt
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.4/MANIFEST.in
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.4/README.md
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2022-01-05 11:14:07.000000 regtricks-0.3.4/regtricks/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14313 2022-01-05 10:37:03.000000 regtricks-0.3.4/regtricks/fnirt_coefficients.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)       70 2022-01-05 11:14:07.000000 regtricks-0.3.4/regtricks/_version.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11652 2022-01-05 10:40:50.000000 regtricks-0.3.4/regtricks/image_space.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     7508 2022-01-05 10:40:43.000000 regtricks-0.3.4/regtricks/application_helpers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.4/regtricks/__init__.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.4/regtricks/x5_interface.py
-drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2022-01-05 11:14:07.000000 regtricks-0.3.4/regtricks/transforms/
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14937 2020-11-23 18:51:42.000000 regtricks-0.3.4/regtricks/transforms/nonlinear.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11498 2021-03-17 16:20:16.000000 regtricks-0.3.4/regtricks/transforms/linear.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.4/regtricks/transforms/__init__.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8419 2022-01-05 10:40:51.000000 regtricks-0.3.4/regtricks/transforms/transform.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3258 2020-10-30 18:59:14.000000 regtricks-0.3.4/regtricks/wrappers.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.4/regtricks/multiplication.py
--rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3590 2020-10-22 13:00:54.000000 regtricks-0.3.4/setup.py
--rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2022-01-05 11:14:07.000000 regtricks-0.3.4/setup.cfg
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-06-12 18:59:31.916213 regtricks-0.3.4.post6/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1479 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/LICENSE
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       42 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/MANIFEST.in
+-rw-r--r--   0 thomaskirk   (501) staff       (20)     1102 2023-06-12 18:59:31.915964 regtricks-0.3.4.post6/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      790 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/README.md
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-06-12 18:59:31.913420 regtricks-0.3.4.post6/regtricks/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      425 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/regtricks/__init__.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       77 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks/_version.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     7508 2022-01-05 10:40:43.000000 regtricks-0.3.4.post6/regtricks/application_helpers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    15290 2022-02-12 22:48:27.000000 regtricks-0.3.4.post6/regtricks/fnirt_coefficients.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11764 2022-10-27 12:09:55.000000 regtricks-0.3.4.post6/regtricks/image_space.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8120 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/regtricks/multiplication.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-06-12 18:59:31.915620 regtricks-0.3.4.post6/regtricks/transforms/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      215 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/regtricks/transforms/__init__.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    11498 2021-03-17 16:20:16.000000 regtricks-0.3.4.post6/regtricks/transforms/linear.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)    14937 2020-11-23 18:51:42.000000 regtricks-0.3.4.post6/regtricks/transforms/nonlinear.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     8452 2022-05-09 11:26:49.000000 regtricks-0.3.4.post6/regtricks/transforms/transform.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     3258 2020-10-30 18:59:14.000000 regtricks-0.3.4.post6/regtricks/wrappers.py
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     4387 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/regtricks/x5_interface.py
+drwxr-xr-x   0 thomaskirk   (501) staff       (20)        0 2023-06-12 18:59:31.914602 regtricks-0.3.4.post6/regtricks.egg-info/
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)     1102 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/PKG-INFO
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)      561 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)        1 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       26 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/requires.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       10 2023-06-12 18:59:31.000000 regtricks-0.3.4.post6/regtricks.egg-info/top_level.txt
+-rwxrwxrwx   0 thomaskirk   (501) staff       (20)       25 2020-10-22 13:00:54.000000 regtricks-0.3.4.post6/requirements.txt
+-rw-r--r--   0 thomaskirk   (501) staff       (20)       38 2023-06-12 18:59:31.916260 regtricks-0.3.4.post6/setup.cfg
+-rwxr-xr-x   0 thomaskirk   (501) staff       (20)     3590 2022-02-12 22:43:08.000000 regtricks-0.3.4.post6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `regtricks-0.3.4/PKG-INFO` & `regtricks-0.3.4.post6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.4
+Version: 0.3.4.post6
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
 Author-email: thomas.kirk@eng.ox.ac.uk
 License: BSD-3-clause
-Description: # Regtricks
-        Tools for manipulating, combining and applying image transformations.
-        
-        Install via pip: `pip install regtricks`
-        
-        Documentation: https://regtricks.readthedocs.io/en/latest/
-        
-        
-        ## Further reading
-        An explanation of the FSL coordinate system: https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FLIRT/FAQ
-        
-        ## Acknowledgements 
-        The FLIRT matrix adjustment code was supplied by Tim Coalson and Martin Craig, adapted from (https://github.com/Washington-University/workbench/blob/9c34187281066519e78841e29dc14bef504776df/src/Nifti/NiftiHeader.cxx#L168) and (https://github.com/Washington-University/workbench/blob/335ad0c910ca9812907ea92ba0e5563225eee1e6/src/Files/AffineFile.cxx#L144)
-        
-        ## Contact 
-        Tom Kirk, 2020.
-        Institute of Biomedical Engineering, University of Oxford. 
-        thomas.kirk@eng.ox.ac.uk
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Regtricks
+Tools for manipulating, combining and applying image transformations.
+
+Install via pip: `pip install regtricks`
+
+Documentation: https://regtricks.readthedocs.io/en/latest/
+
+
+## Further reading
+An explanation of the FSL coordinate system: https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FLIRT/FAQ
+
+## Acknowledgements 
+The FLIRT matrix adjustment code was supplied by Tim Coalson and Martin Craig, adapted from (https://github.com/Washington-University/workbench/blob/9c34187281066519e78841e29dc14bef504776df/src/Nifti/NiftiHeader.cxx#L168) and (https://github.com/Washington-University/workbench/blob/335ad0c910ca9812907ea92ba0e5563225eee1e6/src/Files/AffineFile.cxx#L144)
+
+## Contact 
+Tom Kirk, 2020.
+Institute of Biomedical Engineering, University of Oxford. 
+thomas.kirk@eng.ox.ac.uk
```

### Comparing `regtricks-0.3.4/regtricks.egg-info/PKG-INFO` & `regtricks-0.3.4.post6/regtricks.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: regtricks
-Version: 0.3.4
+Version: 0.3.4.post6
 Summary: Tools for manipulating and applying registrations
 Home-page: https://github.com/tomfrankkirk/regtricks
 Author: Tom Kirk
 Author-email: thomas.kirk@eng.ox.ac.uk
 License: BSD-3-clause
-Description: # Regtricks
-        Tools for manipulating, combining and applying image transformations.
-        
-        Install via pip: `pip install regtricks`
-        
-        Documentation: https://regtricks.readthedocs.io/en/latest/
-        
-        
-        ## Further reading
-        An explanation of the FSL coordinate system: https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FLIRT/FAQ
-        
-        ## Acknowledgements 
-        The FLIRT matrix adjustment code was supplied by Tim Coalson and Martin Craig, adapted from (https://github.com/Washington-University/workbench/blob/9c34187281066519e78841e29dc14bef504776df/src/Nifti/NiftiHeader.cxx#L168) and (https://github.com/Washington-University/workbench/blob/335ad0c910ca9812907ea92ba0e5563225eee1e6/src/Files/AffineFile.cxx#L144)
-        
-        ## Contact 
-        Tom Kirk, 2020.
-        Institute of Biomedical Engineering, University of Oxford. 
-        thomas.kirk@eng.ox.ac.uk
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Regtricks
+Tools for manipulating, combining and applying image transformations.
+
+Install via pip: `pip install regtricks`
+
+Documentation: https://regtricks.readthedocs.io/en/latest/
+
+
+## Further reading
+An explanation of the FSL coordinate system: https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FLIRT/FAQ
+
+## Acknowledgements 
+The FLIRT matrix adjustment code was supplied by Tim Coalson and Martin Craig, adapted from (https://github.com/Washington-University/workbench/blob/9c34187281066519e78841e29dc14bef504776df/src/Nifti/NiftiHeader.cxx#L168) and (https://github.com/Washington-University/workbench/blob/335ad0c910ca9812907ea92ba0e5563225eee1e6/src/Files/AffineFile.cxx#L144)
+
+## Contact 
+Tom Kirk, 2020.
+Institute of Biomedical Engineering, University of Oxford. 
+thomas.kirk@eng.ox.ac.uk
```

### Comparing `regtricks-0.3.4/regtricks.egg-info/SOURCES.txt` & `regtricks-0.3.4.post6/regtricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4/LICENSE` & `regtricks-0.3.4.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4/README.md` & `regtricks-0.3.4.post6/README.md`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4/regtricks/fnirt_coefficients.py` & `regtricks-0.3.4.post6/regtricks/fnirt_coefficients.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from distutils.log import warn
 import tempfile 
 import subprocess
 import os.path as op 
 import warnings 
 
 import nibabel 
 import numpy as np 
@@ -343,14 +344,31 @@
     if not ((len(vec_field.shape) == 4) and (vec_field.shape[3] == 3)):
         raise ValueError("vec_field should be a 4D array with size 3 in "
             "the last dimension")
 
     if not len(vox_size) == 3: 
         raise ValueError("vox_size should be a 3-vector of dimensions") 
 
+    # One of the sneakiest bugs I have ever had the misfortune of dealing
+    # with.... If any of the coordinate axes have been flipped (due to FSL
+    # conventions, for example), then the absolute displacement vectors 
+    # will be strictly decreasing in that dimension (ie X, X-1, X-2 etc). 
+    # This means all partial derivatives in that dimension will also be 
+    # negative, which means a negative Jacobian determinant. So, check each
+    # dimension to see if it is ascending / descending, and flip the 
+    # corresponding voxel dimension to compensate if so. 
+    if (np.diff(vec_field[:,0,0,0]) < 0).all(): 
+        vox_size[0] *= -1 
+
+    if (np.diff(vec_field[0,:,0,1]) < 0).all(): 
+        vox_size[1] *= -1
+
+    if (np.diff(vec_field[0,0,:,2]) < 0).all(): 
+        vox_size[2] *= -1 
+
     # Calculate partial derivatives in each direction. Note that each of these
     # returns an array of size (X,Y,Z,3), arranged d/dx, d/dy, d/dz in the last
     # dimension. So dfx is a stack of arrays df(i)/dx, df(i)/dy, df(i)/dz. We
     # need to calculate the derivative with respect to each direction because
     # f is a vector field, ie, it contains i,j,k components, each of which are
     # independent functions of x,y,z
     dfi = np.gradient(vec_field, vox_size[0], axis=0)
@@ -366,9 +384,12 @@
                          [dfj[...,0], dfj[...,1], dfj[...,2]],
                          [dfk[...,0], dfk[...,1], dfk[...,2]]
                         ])
 
     # Reshape into a single stack of (N,3,3) arrays and calculate the det
     # Return an array of scalars sized (XYZ) again 
     jacobian = np.moveaxis(jacobian.reshape(3,3,-1), 2, 0)
-    jdet = np.linalg.det(jacobian)
-    return jdet.reshape(vec_field.shape[:3])
+    jdet = np.linalg.det(jacobian).reshape(vec_field.shape[:3])
+    if ((jdet < 0).sum() / jdet.size) > 0.1: 
+        warnings.warn('regtricks: numerous negative values returned for Jacobian determinant')
+
+    return jdet
```

### Comparing `regtricks-0.3.4/regtricks/image_space.py` & `regtricks-0.3.4.post6/regtricks/image_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,21 @@
     @property
     def fov_size(self):
         """FoV associated with image, in mm"""
 
         return self.size * self.vox_size
 
 
+    @property 
+    def n_vox(self): 
+        """Number of voxels in grid"""
+
+        return self.size.prod() 
+
+
     @property
     def bbox_origin(self): 
         """
         Origin of the image's bounding box, referenced to first voxel's 
         corner, not center (ie, -0.5, -0.5, -0.5)
         """
```

### Comparing `regtricks-0.3.4/regtricks/application_helpers.py` & `regtricks-0.3.4.post6/regtricks/application_helpers.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4/regtricks/x5_interface.py` & `regtricks-0.3.4.post6/regtricks/x5_interface.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4/regtricks/transforms/nonlinear.py` & `regtricks-0.3.4.post6/regtricks/transforms/nonlinear.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4/regtricks/transforms/linear.py` & `regtricks-0.3.4.post6/regtricks/transforms/linear.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4/regtricks/transforms/transform.py` & `regtricks-0.3.4.post6/regtricks/transforms/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,16 +192,16 @@
 
         if (superfactor < 1).any(): 
             raise ValueError("Superfactor must be integer > 0")
 
         if (superfactor != 1).any(): 
             ref = ref.resize_voxels(1 / superfactor, 'ceil')
 
-        if not (data.shape[:3] == src.size).all(): 
-            raise RuntimeError("Data shape {} does not match source space {}"
+        if not ((data.ndim in (3,4)) and (np.array_equal(src.size, data.shape[:3]))): 
+            raise ValueError("Data shape {} does not match source space {}"
                                 .format(data.shape, src.size))
 
         # Force to float data 
         if data.dtype.kind != 'f': 
             data = data.astype(float)
 
         # Only use multiprocessing on 4D data
```

### Comparing `regtricks-0.3.4/regtricks/wrappers.py` & `regtricks-0.3.4.post6/regtricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4/regtricks/multiplication.py` & `regtricks-0.3.4.post6/regtricks/multiplication.py`

 * *Files identical despite different names*

### Comparing `regtricks-0.3.4/setup.py` & `regtricks-0.3.4.post6/setup.py`

 * *Files identical despite different names*

