# Comparing `tmp/mdreg-0.3.7.tar.gz` & `tmp/mdreg-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdreg-0.3.7.tar", last modified: Sun Jul  3 21:00:40 2022, max compression
+gzip compressed data, was "mdreg-0.3.8.tar", last modified: Mon Jun 12 15:20:18 2023, max compression
```

## Comparing `mdreg-0.3.7.tar` & `mdreg-0.3.8.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-07-03 21:00:40.302624 mdreg-0.3.7/
--rw-rw-rw-   0        0        0    11525 2022-06-06 13:00:34.000000 mdreg-0.3.7/LICENSE
--rw-rw-rw-   0        0        0    20120 2022-07-03 21:00:40.300629 mdreg-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     6076 2022-06-24 21:49:46.000000 mdreg-0.3.7/README.md
--rw-rw-rw-   0        0        0     1425 2022-07-03 20:57:36.000000 mdreg-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-03 21:00:40.303622 mdreg-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      215 2022-06-30 20:06:22.000000 mdreg-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-03 21:00:40.183919 mdreg-0.3.7/src/
-drwxrwxrwx   0        0        0        0 2022-07-03 21:00:40.209912 mdreg-0.3.7/src/mdreg/
--rw-rw-rw-   0        0        0       21 2022-06-30 21:05:00.000000 mdreg-0.3.7/src/mdreg/__init__.py
--rw-rw-rw-   0        0        0    18771 2022-06-24 21:49:46.000000 mdreg-0.3.7/src/mdreg/main.py
-drwxrwxrwx   0        0        0        0 2022-07-03 21:00:40.297650 mdreg-0.3.7/src/mdreg/models/
--rw-rw-rw-   0        0        0     2614 2022-06-06 13:13:38.000000 mdreg-0.3.7/src/mdreg/models/DCE_2CFM.py
--rw-rw-rw-   0        0        0     5753 2022-06-06 13:13:38.000000 mdreg-0.3.7/src/mdreg/models/DTI.py
--rw-rw-rw-   0        0        0     1733 2022-06-06 13:13:38.000000 mdreg-0.3.7/src/mdreg/models/DWI_simple.py
--rw-rw-rw-   0        0        0     2300 2022-06-06 13:13:38.000000 mdreg-0.3.7/src/mdreg/models/T1_simple.py
--rw-rw-rw-   0        0        0     1240 2022-06-06 13:13:38.000000 mdreg-0.3.7/src/mdreg/models/T2_simple.py
--rw-rw-rw-   0        0        0     1220 2022-06-06 13:13:38.000000 mdreg-0.3.7/src/mdreg/models/T2star_simple.py
--rw-rw-rw-   0        0        0        0 2022-07-02 07:13:36.000000 mdreg-0.3.7/src/mdreg/models/__init__.py
--rw-rw-rw-   0        0        0     1146 2022-06-06 13:13:38.000000 mdreg-0.3.7/src/mdreg/models/constant.py
--rw-rw-rw-   0        0        0     2058 2022-06-06 13:13:38.000000 mdreg-0.3.7/src/mdreg/models/exp_decay.py
-drwxrwxrwx   0        0        0        0 2022-07-03 21:00:40.264732 mdreg-0.3.7/src/mdreg.egg-info/
--rw-rw-rw-   0        0        0    20120 2022-07-03 21:00:39.000000 mdreg-0.3.7/src/mdreg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2022-07-03 21:00:40.000000 mdreg-0.3.7/src/mdreg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-03 21:00:39.000000 mdreg-0.3.7/src/mdreg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2022-07-03 21:00:39.000000 mdreg-0.3.7/src/mdreg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-07-03 21:00:39.000000 mdreg-0.3.7/src/mdreg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 15:20:18.942546 mdreg-0.3.8/
+-rw-rw-rw-   0        0        0    11525 2023-03-01 22:09:12.000000 mdreg-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0    20120 2023-06-12 15:20:18.938556 mdreg-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6076 2023-03-01 22:09:12.000000 mdreg-0.3.8/README.md
+-rw-rw-rw-   0        0        0     1425 2023-06-12 14:43:17.000000 mdreg-0.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 15:20:18.954513 mdreg-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      215 2023-03-01 22:09:12.000000 mdreg-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:20:18.618416 mdreg-0.3.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 15:20:18.695206 mdreg-0.3.8/src/mdreg/
+-rw-rw-rw-   0        0        0       21 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/__init__.py
+-rw-rw-rw-   0        0        0    25424 2023-03-16 23:43:14.000000 mdreg-0.3.8/src/mdreg/main.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:20:18.934568 mdreg-0.3.8/src/mdreg/models/
+-rw-rw-rw-   0        0        0     2614 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/models/DCE_2CFM.py
+-rw-rw-rw-   0        0        0     5844 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/models/DTI.py
+-rw-rw-rw-   0        0        0     6467 2023-03-11 18:25:45.000000 mdreg-0.3.8/src/mdreg/models/DWI_monoexponential_parallel.py
+-rw-rw-rw-   0        0        0     1733 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/models/DWI_simple.py
+-rw-rw-rw-   0        0        0     5109 2023-03-11 18:25:45.000000 mdreg-0.3.8/src/mdreg/models/T1_parallel.py
+-rw-rw-rw-   0        0        0     2516 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/models/T1_simple.py
+-rw-rw-rw-   0        0        0     4671 2023-03-11 18:25:45.000000 mdreg-0.3.8/src/mdreg/models/T2_parallel.py
+-rw-rw-rw-   0        0        0     1240 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/models/T2_simple.py
+-rw-rw-rw-   0        0        0     4854 2023-03-11 18:25:45.000000 mdreg-0.3.8/src/mdreg/models/T2star_parallel.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/models/T2star_simple.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/models/__init__.py
+-rw-rw-rw-   0        0        0     1146 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/models/constant.py
+-rw-rw-rw-   0        0        0     2058 2023-03-01 22:09:12.000000 mdreg-0.3.8/src/mdreg/models/exp_decay.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:20:18.831841 mdreg-0.3.8/src/mdreg.egg-info/
+-rw-rw-rw-   0        0        0    20120 2023-06-12 15:20:18.000000 mdreg-0.3.8/src/mdreg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      660 2023-06-12 15:20:18.000000 mdreg-0.3.8/src/mdreg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 15:20:18.000000 mdreg-0.3.8/src/mdreg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-06-12 15:20:18.000000 mdreg-0.3.8/src/mdreg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 15:20:18.000000 mdreg-0.3.8/src/mdreg.egg-info/top_level.txt
```

### Comparing `mdreg-0.3.7/LICENSE` & `mdreg-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mdreg-0.3.7/PKG-INFO` & `mdreg-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdreg
-Version: 0.3.7
+Version: 0.3.8
 Summary: Model-driven image registration
 Author-email: Kanishka Sharma <kanishka.sharma@sheffield.ac.uk>, Joao Almeida e Sousa <j.g.sousa@sheffield.ac.uk>, Steven Sourbron <s.sourbron@sheffield.ac.uk>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mdreg-0.3.7/README.md` & `mdreg-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `mdreg-0.3.7/pyproject.toml` & `mdreg-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0d0a 2320 6d69 6e69 6d61 6c20 7265 7175  ..# minimal requ
 00000010: 6972 6564 2069 6e66 6f72 6d61 7469 6f6e  ired information
 00000020: 0d0a 0d0a 5b70 726f 6a65 6374 5d0d 0a6e  ....[project]..n
 00000030: 616d 6520 3d20 226d 6472 6567 220d 0a76  ame = "mdreg"..v
-00000040: 6572 7369 6f6e 203d 2022 302e 332e 3722  ersion = "0.3.7"
+00000040: 6572 7369 6f6e 203d 2022 302e 332e 3822  ersion = "0.3.8"
 00000050: 0d0a 6465 7065 6e64 656e 6369 6573 203d  ..dependencies =
 00000060: 205b 0d0a 2020 2269 746b 2d65 6c61 7374   [..  "itk-elast
 00000070: 6978 222c 0d0a 2020 226d 6174 706c 6f74  ix",..  "matplot
 00000080: 6c69 6222 2c0d 0a20 2022 6e75 6d70 7922  lib",..  "numpy"
 00000090: 2c0d 0a20 2022 7061 6e64 6173 222c 0d0a  ,..  "pandas",..
 000000a0: 2020 2250 696c 6c6f 7722 2c0d 0a20 2022    "Pillow",..  "
 000000b0: 7363 6970 7922 2c0d 0a20 2022 5369 6d70  scipy",..  "Simp
```

### Comparing `mdreg-0.3.7/src/mdreg/main.py` & `mdreg-0.3.8/src/mdreg/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,33 +2,38 @@
 
 import time, os, copy
 from tqdm import tqdm
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.animation as animation
+#import dask
 import itk
-import SimpleITK as sitk
+import multiprocessing
+#from multiprocessing import shared_memory
+#import psutil
+import gc
 
 from .models import constant
 
 default_path = os.path.dirname(__file__)
 
 class MDReg:
 
     def __init__(self):
 
-        # input
+        # input DEFAULT
         self.array = None
         self.coreg_mask = None
         self.signal_parameters = None
         self.pixel_spacing = 1.0
-        self.signal_model = constant
-        self.elastix = default_bspline()
+        #self.signal_model = constant
+        self.elastix = default_bspline('2')
         self.log = False
+        self.parallel = True
 
         # mdr optimization
         self.max_iterations = 5
         self.precision = 1.0
 
         # output
         self.coreg = None
@@ -54,109 +59,173 @@
         return np.prod(shape[:-1]), len(shape)-1, shape[-1]
 
     def set_array(self, array):
         self.array = array
         self.coreg = array
         n = self._npdt
         self.coreg = np.reshape(self.coreg, (n[0],n[2]))
+        if n[1] == 3:
+            self.elastix = default_bspline('3')
     
     def set_mask(self, mask_array):
         self.coreg_mask = mask_array
         n = self._npdt
         self.coreg_mask = np.reshape(self.coreg_mask, (n[0],n[2]))
 
     def read_elastix(self, file):
         self.elastix.AddParameterFile(file)
     
     def set_elastix(self, **kwargs):
         for tag, value in kwargs.items():
             self.elastix.SetParameter(tag, str(value))       
 
     def fit(self):
-
         n = self._npdt
         self.coreg = copy.deepcopy(self.array)
         self.coreg = np.reshape(self.coreg, (n[0],n[2]))
         self.deformation = np.zeros(n)
         start = time.time()
         improvement = []
         converged = False
         self.iteration = 1
         while not converged: 
             startit = time.time()
-            self.fit_signal()
+            self.fit_signal() 
             if self.export_unregistered:
                 if self.iteration == 1: 
                     self.export_fit(name='_unregistered')
             deformation = self.fit_deformation()
+            #reshape for maxnorm
+            deformation  = np.reshape(deformation,[n[0],n[1],n[2]])
             improvement.append(_maxnorm(self.deformation-deformation))
             self.deformation = deformation
             converged = improvement[-1] <= self.precision 
             if self.iteration == self.max_iterations: 
                 converged=True
             calctime = (time.time()-startit)/60
             print('Finished MDR iteration ' + str(self.iteration) + ' after ' + str(calctime) + ' min') 
             print('Improvement after MDR iteration ' + str(self.iteration) + ': ' + str(improvement[-1]) + ' pixels')  
+            del deformation
+            gc.collect()
             self.iteration += 1 
 
         self.fit_signal()
         shape = self.array.shape
         self.coreg = np.reshape(self.coreg, shape)
         nd = len(shape)-1
         self.deformation = np.reshape(self.deformation, shape[:-1]+(nd,)+(shape[-1],))
         self.iter = pd.DataFrame({'Maximum deformation': improvement}) 
 
         print('Total calculation time: ' + str((time.time()-start)/60) + ' min')
+        gc.collect()
 
     def fit_signal(self):
 
         msg = self.pinned_message + ', fitting signal model (iteration ' + str(self.iteration) + ')'
         print(msg)
         if self.status is not None:
             self.status.message(msg)
         start = time.time()
         fit, pars = self.signal_model.main(self.coreg, self.signal_parameters)
         shape = self.array.shape
-        self.model_fit = np.reshape(fit, shape)
+        self.model_fit = np.reshape(fit, shape) 
         self.pars = np.reshape(pars, shape[:-1] + (pars.shape[-1],))
+       
         print('Model fitting time: ' + str((time.time()-start)/60) + ' min')
 
+
     def fit_deformation(self):
 
         msg = self.pinned_message + ', fitting deformation field (iteration ' + str(self.iteration) + ')'
         if self.status is not None:
             self.status.message(msg)
         start = time.time()
         nt = self._npdt[-1]
+
         deformation = np.empty(self._npdt)
+        dict_param = _elastix2dict(self.elastix)
+
+        # reshape the deformation field 
+        if self._npdt[1] == 2: #2D
+            deformation = np.reshape(deformation,(self.array.shape[0], self.array.shape[1], 2, self.array.shape[2])) 
+        else: #3D
+            deformation = np.reshape(deformation,(self.array.shape[0], self.array.shape[1], self.array.shape[2], 3, self.array.shape[3])) 
+
         # If mask isn't same shape as images, then don't use it
         if isinstance(self.coreg_mask, np.ndarray):
             if np.shape(self.coreg_mask) != self.array.shape: 
                 mask = None
+                print("using mask shape: If mask isn't same shape as images, then don't use it")
             else: 
                 mask = self.coreg_mask
         else: 
             mask = None
-        
-        for t in tqdm(range(nt), desc=msg): # dynamics
-            if self.status is not None:
-                self.status.progress(t, nt)
-            if mask is not None:
-                mask_t = mask[...,t]
-            else: 
-                mask_t = None
-            self.coreg[:,t], deformation[:,:,t] = _coregister(
-                self.array[...,t], 
-                self.model_fit[...,t], 
-                self.elastix, 
-                self.pixel_spacing, 
-                self.log, 
-                mask_t,
-            )
+        # coregistration per dynamic (i.e. image time-point)
+
+        if self.parallel == False:
+
+            for t in tqdm(range(nt), desc=msg): 
+                if self.status is not None:
+                    self.status.progress(t, nt)
+
+                if mask is not None:
+                    mask_t = mask[...,t]
+                else: 
+                    mask_t = None
+                
+                self.coreg[:,t], deformation[...,t] = _coregister(
+                    self.array[...,t], 
+                    self.model_fit[...,t], 
+                    self.elastix, 
+                    self.pixel_spacing, 
+                    self.log, 
+                    mask_t,
+                )
+
+        if self.parallel == True:
+            #print("Part 1 before multiprocessing: " + str(psutil.virtual_memory()[3]/1000000000))
+
+            if mask is None:
+                args = [(self.array[...,t], self.model_fit[...,t], dict_param, self.pixel_spacing, self.log, mask) for t in range(nt)] #dynamics
+            else:
+                args = [(self.array[...,t], self.model_fit[...,t], dict_param, self.pixel_spacing, self.log, mask[...,t]) for t in range(nt)] #dynamics
+
+            #print("Part 1_2 after args before multiprocessing: " + str(psutil.virtual_memory()[3]/1000000000))
+            #args = shared_memory.ShareableList(args)
+
+            try: 
+                num_workers = int(len(os.sched_getaffinity(0)))
+            except: 
+                num_workers = int(os.cpu_count())
+            
+            pool = multiprocessing.Pool(processes=num_workers)
+            
+            #print("Part 2 after multiprocessing but before results: " + str(psutil.virtual_memory()[3]/1000000000))
+            
+            results = list(tqdm(pool.imap(_coregister_par, args), total=nt, desc=msg))
+            #print("Part 3 after multiprocessing after results: " + str(psutil.virtual_memory()[3]/1000000000))
+
+            pool.close()
+            pool.join()
+
+            #print("Part 4 after closing multiprocessing before unpacking results: " + str(psutil.virtual_memory()[3]/1000000000))
+
+            for t in range(nt):
+                self.coreg[:,t] = results[t][0]
+                deformation[...,t] = results[t][1]
+
+            #print("Part 5 after unpacking results: " + str(psutil.virtual_memory()[3]/1000000000))
+
+            del args
+            gc.collect()
+
+            #print("Part 6 after setting args to None: " + str(psutil.virtual_memory()[3]/1000000000))
+
         print('Coregistration time: ' + str((time.time()-start)/60) +' min')
+
         return deformation
 
     def export(self):
 
         self.export_data()
         self.export_fit()
         self.export_registered()
@@ -169,45 +238,56 @@
         _export_animation(self.array, path, 'images')
 
     def export_fit(self, name=''):
 
         print('Exporting fit..' + name)
         path = self.export_path 
         pars = self.signal_model.pars()
+    
         if not os.path.exists(path): os.mkdir(path)
         lower, upper = self.signal_model.bounds()
         for i in range(len(pars)):
             _export_imgs(self.pars[...,i], path, pars[i] + name, bounds=[lower[i],upper[i]])
         _export_animation(self.model_fit, path, 'modelfit' + name)
+        
 
     def export_registered(self):
 
         print('Exporting registration..')
         path = self.export_path 
         if not os.path.exists(path): os.mkdir(path)
-        defx = np.squeeze(self.deformation[:,:,0,:])
-        defy = np.squeeze(self.deformation[:,:,1,:])
         _export_animation(self.coreg, path, 'coregistered')
+        defx = np.squeeze(self.deformation[...,0,:])
+        defy = np.squeeze(self.deformation[...,1,:])
         _export_animation(defx, path, 'deformation_field_x')
         _export_animation(defy, path, 'deformation_field_y')
-        _export_animation(np.sqrt(defx**2 + defy**2), path, 'deformation_field')
+        if self._npdt[1] == 3: #3D
+            defz = np.squeeze(self.deformation[...,2,:])
+            _export_animation(defz, path, 'deformation_field_z')
+            _export_animation(np.sqrt(defx**2 + defy**2 + defz**2), path, 'deformation_field')
+        else: #2D
+            _export_animation(np.sqrt(defx**2 + defy**2), path, 'deformation_field')
         self.iter.to_csv(os.path.join(path, 'largest_deformations.csv'))
 
 
-def default_bspline():
+def default_bspline(d):
     param_obj = itk.ParameterObject.New()
     parameter_map_bspline = param_obj.GetDefaultParameterMap('bspline')
-    param_obj.AddParameterMap(parameter_map_bspline) #why??
+    ## add parameter map file to the parameter object: required in itk-elastix
+    param_obj.AddParameterMap(parameter_map_bspline) 
+    #OPTIONAL: Write the default parameter file to output file
+    # param_obj.WriteParameterFile(parameter_map_bspline, "bspline.default.txt")
     # *********************
     # * ImageTypes
     # *********************
     param_obj.SetParameter("FixedInternalImagePixelType", "float")
     param_obj.SetParameter("MovingInternalImagePixelType", "float")
-    param_obj.SetParameter("FixedImageDimension", "2")
-    param_obj.SetParameter("MovingImageDimension", "2")
+    ## selection based on 3D or 2D image data: newest elastix version does not require input image dimension
+    param_obj.SetParameter("FixedImageDimension", d) 
+    param_obj.SetParameter("MovingImageDimension", d) 
     param_obj.SetParameter("UseDirectionCosines", "true")
     # *********************
     # * Components
     # *********************
     param_obj.SetParameter("Registration", "MultiResolutionRegistration")
     # Image intensities are sampled using an ImageSampler, Interpolator and ResampleInterpolator.
     # Image sampler is responsible for selecting points in the image to sample. 
@@ -265,15 +345,16 @@
     # unrealistic deformations.
     # By default the grid spacing is halved after every resolution,
     # such that the final grid spacing is obtained in the last 
     # resolution level.
     # The grid spacing here is specified in voxel units.
     #(FinalGridSpacingInPhysicalUnits 10.0 10.0)
     #(FinalGridSpacingInVoxels 8)
-    param_obj.SetParameter("FinalGridSpacingInPhysicalUnits", ["50.0", "50.0"])
+    #param_obj.SetParameter("FinalGridSpacingInPhysicalUnits", ["50.0", "50.0"])
+    param_obj.SetParameter("FinalGridSpacingInPhysicalUnits", "50.0")
     # *********************
     # * Optimizer settings
     # *********************
     # The number of resolutions. 1 Is only enough if the expected
     # deformations are small. 3 or 4 mostly works fine. For large
     # images and large deformations, 5 or 6 may even be useful.
     param_obj.SetParameter("NumberOfResolutions", "4")
@@ -323,117 +404,201 @@
     # Choose whether to generate the deformed moving image.
     # You can save some time by setting this to false, if you are
     # not interested in the final deformed moving image, but only
     # want to analyze the deformation field for example.
     param_obj.SetParameter("WriteResultImage", "true")
     # The pixel type and format of the resulting deformed moving image
     param_obj.SetParameter("ResultImagePixelType", "float")
-    param_obj.SetParameter("ResultImageFormat", "mhd")
+    param_obj.SetParameter("ResultImageFormat", "nii")
+    
     return param_obj
 
 
 def _export_animation(array, path, filename):
 
     file = os.path.join(path, filename + '.gif')
     array[np.isnan(array)] = 0
-    fig = plt.figure()
-    im = plt.imshow(np.squeeze(array[:,:,0]).T, animated=True)
-    def updatefig(i):
-        im.set_array(np.squeeze(array[:,:,i]).T)
-    anim = animation.FuncAnimation(fig, updatefig, interval=50, frames=array.shape[2])
-    anim.save(file)
-    #plt.show()
+    shape = np.shape(array)
+
+    if len(shape)==4: ##save 3D data
+        fig = plt.figure()
+        file_3D_save = os.path.join(path, filename)
+        for k in range(shape[2]): 
+            im = plt.imshow(np.squeeze(array[:,:,k,0]).T, animated=True) 
+            def updatefig(i):
+                im.set_array(np.squeeze(array[:,:,k,i]).T) # export each slice all dynamics
+            anim = animation.FuncAnimation(fig, updatefig, interval=50, frames=array.shape[3])
+            anim.save(file_3D_save + '_' + str(k) + ".gif")
+
+    else: # save 2D data   
+        fig = plt.figure()
+        im = plt.imshow(np.squeeze(array[:,:,0]).T, animated=True) 
+        def updatefig(i):
+            im.set_array(np.squeeze(array[:,:,i]).T) 
+        anim = animation.FuncAnimation(fig, updatefig, interval=50, frames=array.shape[2])
+        anim.save(file) 
 
 
 def _export_imgs(array, path, filename, bounds=[-np.inf, np.inf]):
 
     file = os.path.join(path, filename + '.png')
-    array[np.isnan(array)] = 0
+    array[np.isnan(array)] = 0 
     array[np.isinf(array)] = 0
     array = np.clip(array, bounds[0], bounds[1])
-    plt.imshow(array.T)
-    plt.clim(np.amin(array), np.amax(array))
-    cBar = plt.colorbar()
-    cBar.minorticks_on()
-    plt.savefig(fname=file)
-    plt.close()
+    shape_arr = np.shape(array)
 
+    if len(shape_arr) == 2: #2D data save
+        plt.imshow((array).T)
+        plt.clim(np.amin(array), np.amax(array))
+        cBar = plt.colorbar()
+        cBar.minorticks_on()
+        plt.savefig(fname=file)
+        plt.close()
+    else: #3D data save
+        file_3D = os.path.join(path, filename)
+        for i in range(shape_arr[2]):
+            plt.imshow((array[:,:,i]).T)
+            plt.clim(np.amin(array), np.amax(array))
+            cBar = plt.colorbar()
+            cBar.minorticks_on()
+            plt.savefig(fname=[file_3D + '_' + str(i) + ".png"])
+            plt.close()
+   
 
 def _maxnorm(d):
     """This function calculates diagnostics from the registration process.
 
     It takes as input the original deformation field and the new deformation field
     and returns the maximum deformation per pixel (in mm).
     The maximum deformation per pixel is calculated as 
     the euclidean distance of difference between the old and new deformation field. 
     """
-    d = d[:,0,:]**2 + d[:,1,:]**2
+    shape_deformation = np.shape(d) 
+    if (shape_deformation[1] == 3): #3D
+       d = d[:,0,:]**2 + d[:,1,:]**2 + d[:,2,:]**2
+    else: #2D
+       d = d[:,0,:]**2 + d[:,1,:]**2
+
     return np.nanmax(np.sqrt(d))
 
+def _coregister_par(args):
+    """
+    Coregister two arrays and return coregistered + deformation field 
+    """
+    target, source, elastix_model_parameters, spacing, log, mask = args
+
+    elastix_model_parameters = _dict2elastix(elastix_model_parameters)
+
+    shape_source = np.shape(source)
+    #shape_target = np.shape(target)
+    source = itk.GetImageFromArray(np.array(source, np.float32)) 
+    source.SetSpacing(spacing)
+ 
+    target = itk.GetImageFromArray(np.array(target, np.float32))
+    target.SetSpacing(spacing)
+
+    ## TODO: mask not included TBC
+    ## read the source and target images ## removed: NOT USING anymore: SET MOVING IMG; SET FIXED IMAGE
+    #elastixImageFilter = itk.ElastixRegistrationMethod.New() 
+    
+    # Call registration function: NEW
+    coregistered, result_transform_parameters = itk.elastix_registration_method(
+    source, target,
+    parameter_object=elastix_model_parameters)
+
+    # OPTIONAL:print the resulting transform parameters and the elastix bspline paramter file
+    # print(result_transform_parameters)
+    
+    ## RUN ELASTIX using ITK-Elastix filters
+    coregistered = itk.GetArrayFromImage(coregistered).flatten()
+
+    # Load Transformix Object
+    transformix_object = itk.TransformixFilter.New(target)
+    transformix_object.SetTransformParameterObject(result_transform_parameters)
+    
+    # Update object (required)
+    transformix_object.UpdateLargestPossibleRegion()
+    # Compute the deformation field
+    transformix_object.ComputeDeformationFieldOn() 
+    deformation_field = itk.GetArrayFromImage(transformix_object.GetOutputDeformationField()).flatten()
+
+    # Results of Transformation # optional
+    # result_image_transformix = transformix_object.GetOutput()
+  
+    if len(shape_source) == 2: # 2D
+        deformation_field = np.reshape(deformation_field,(shape_source[0], shape_source[1], 2)) 
+    else: #3D 
+        deformation_field = np.reshape(deformation_field,(shape_source[0], shape_source[1], shape_source[2], 3)) 
+
+    return coregistered, deformation_field
 
 
 def _coregister(target, source, elastix_model_parameters, spacing, log, mask):
     """
     Coregister two arrays and return coregistered + deformation field 
     """
     shape_source = np.shape(source)
-    shape_target = np.shape(target)
-
-    source = sitk.GetImageFromArray(source)
+    #shape_target = np.shape(target)
+    source = itk.GetImageFromArray(np.array(source, np.float32)) 
     source.SetSpacing(spacing)
-    source.__SetPixelAsUInt16__
-    source = np.nan_to_num(np.reshape(source, [shape_source[0], shape_source[1]]))
-    
-    target = sitk.GetImageFromArray(target)
+ 
+    target = itk.GetImageFromArray(np.array(target, np.float32))
     target.SetSpacing(spacing)
-    target.__SetPixelAsUInt16__
-    target = np.nan_to_num(np.reshape(target, [shape_target[0], shape_target[1]]))
+
+    ## TODO: mask not included TBC
+    ## read the source and target images ## removed: NOT USING anymore: SET MOVING IMG; SET FIXED IMAGE
+    #elastixImageFilter = itk.ElastixRegistrationMethod.New() 
     
-    ## read the source and target images
-    elastixImageFilter = itk.ElastixRegistrationMethod.New()
-    elastixImageFilter.SetFixedImage(itk.GetImageFromArray(np.array(source, np.float32)))
-    elastixImageFilter.SetMovingImage(itk.GetImageFromArray(np.array(target, np.float32)))
-    if mask is not None:
-        shape_mask = np.shape(mask)
-        mask = sitk.GetImageFromArray(mask)
-        mask.SetSpacing(spacing)
-        mask.__SetPixelAsUInt8__
-        mask = np.nan_to_num(np.reshape(mask, [shape_mask[0], shape_mask[1]]))
-        elastixImageFilter.SetFixedMask(itk.GetImageFromArray(np.array(mask, np.uint8)))
-        elastixImageFilter.SetMovingMask(itk.GetImageFromArray(np.array(mask, np.uint8)))
+    # Call registration function: NEW
+    coregistered, result_transform_parameters = itk.elastix_registration_method(
+    source, target,
+    parameter_object=elastix_model_parameters)
 
-    ## call the parameter map file specifying the registration parameters
-    elastixImageFilter.SetParameterObject(elastix_model_parameters)
+    # OPTIONAL:print the resulting transform parameters and the elastix bspline paramter file
+    # print(result_transform_parameters)
+    
+    ## RUN ELASTIX using ITK-Elastix filters
+    coregistered = itk.GetArrayFromImage(coregistered).flatten()
 
-    ## set additional options
-    elastixImageFilter.SetNumberOfThreads(os.cpu_count()-1)
+    # Load Transformix Object
+    transformix_object = itk.TransformixFilter.New(target)
+    transformix_object.SetTransformParameterObject(result_transform_parameters)
     
-    # logging; note that nothing is printed in Jupyter Notebooks
-    elastixImageFilter.SetLogToFile(log)
-    elastixImageFilter.SetLogToConsole(log)
-    if log == True:
-        print("Parameter Map: ")
-        print(elastix_model_parameters)
-        output_dir = os.path.join(os.getcwd(), "Elastix Log")
-        os.makedirs(output_dir, exist_ok=True)
-        #log_filename = "ITK-Elastix.log"
-        i = 0
-        while os.path.exists(os.path.join(output_dir, f"ITK-Elastix_{i}.log")): i += 1
-        log_filename = f"ITK-Elastix_{i}.log"
-        elastixImageFilter.SetOutputDirectory(output_dir)
-        elastixImageFilter.SetLogFileName(log_filename)
+    # Update object (required)
+    transformix_object.UpdateLargestPossibleRegion()
+    # Compute the deformation field
+    transformix_object.ComputeDeformationFieldOn() 
+    deformation_field = itk.GetArrayFromImage(transformix_object.GetOutputDeformationField()).flatten()
+
+    # Results of Transformation # optional
+    # result_image_transformix = transformix_object.GetOutput()
+  
+    if len(shape_source) == 2: # 2D
+        deformation_field = np.reshape(deformation_field,(shape_source[0], shape_source[1], 2)) 
+    else: #3D 
+        deformation_field = np.reshape(deformation_field,(shape_source[0], shape_source[1], shape_source[2], 3)) 
 
-    ## update filter object (required)
-    elastixImageFilter.UpdateLargestPossibleRegion()
+    return coregistered, deformation_field
 
-    ## RUN ELASTIX using ITK-Elastix filters
-    coregistered = itk.GetArrayFromImage(elastixImageFilter.GetOutput()).flatten()
+def _elastix2dict(elastix_model_parameters):
+    """
+    Hack to allow parallel processing
+    """
+    list_dictionaries_parameters = []
+    for index in range(elastix_model_parameters.GetNumberOfParameterMaps()):
+        parameter_map = elastix_model_parameters.GetParameterMap(index)
+        one_parameter_map_dict = {}
+        for i in parameter_map:
+            one_parameter_map_dict[i] = parameter_map[i]
+        list_dictionaries_parameters.append(one_parameter_map_dict)
+    return list_dictionaries_parameters
 
-    transformixImageFilter = itk.TransformixFilter.New()
-    transformixImageFilter.SetTransformParameterObject(elastixImageFilter.GetTransformParameterObject())
-    transformixImageFilter.ComputeDeformationFieldOn()
-    transformixImageFilter.SetMovingImage(itk.GetImageFromArray(np.array(target, np.float32)))
-    deformation_field = itk.GetArrayFromImage(transformixImageFilter.GetOutputDeformationField()).flatten()
-    deformation_field = np.reshape(deformation_field, [int(len(deformation_field)/2), 2])
 
-    return coregistered, deformation_field
+def _dict2elastix(list_dictionaries_parameters):
+    """
+    Hack to allow parallel processing
+    """
+    elastix_model_parameters = itk.ParameterObject.New()
+    for one_map in list_dictionaries_parameters:
+        elastix_model_parameters.AddParameterMap(one_map)
+    return elastix_model_parameters
```

### Comparing `mdreg-0.3.7/src/mdreg/models/DCE_2CFM.py` & `mdreg-0.3.8/src/mdreg/models/DCE_2CFM.py`

 * *Files identical despite different names*

### Comparing `mdreg-0.3.7/src/mdreg/models/DTI.py` & `mdreg-0.3.8/src/mdreg/models/DTI.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 iBEAt study DTI model fit for mdreg   
 2021 
 """
 
 import numpy as np
 
 def pars():
-    return ['FA', 'ADC']
+    return ['FA', 'ADC','S0']
 
 def bounds():
     lower = [0,0]
     upper = [1.0, 10]
     return lower, upper
 
 
@@ -66,23 +66,27 @@
     
     # Add another column to Bv to handle the constant term:
     # Slog = Bv * M + log(S0)
     # becomes:
     # Slog = [Bv, -1] * [M; -log(S0)]
     minus_one_column = -np.ones((np.shape(Bv)[0]))
     Bv_new = np.c_[Bv, minus_one_column]
+    
     assert method=='linear', "Wrong method as argument!!!"
     M = np.linalg.lstsq(Bv_new, -imlog.T, rcond=None)
     M = M[0].T
+    S0_log = M[:,6]
+    S0 = np.exp(S0_log)
     
     M[np.isnan(M)]=0
     M[np.isinf(M)]=0
     
     ### Initialize Variables
     npixels = np.shape(M)[0]
+   
     FA_mask = np.empty(npixels) 
     ADC_mask = np.empty(npixels) 
 
     for i in range(npixels):
         
         # The DiffusionTensor (Remember it is a symetric matrix,
         # thus for instance Dxy == Dyx)
@@ -117,18 +121,19 @@
             FA_mask[i] = 0
         else:    
             FA_mask[i]=np.sqrt(1.5)*(np.sqrt((EigenValues[0]-ADCv)**2+(EigenValues[1]-ADCv)**2+(EigenValues[2]-ADCv)**2)/denominator)
         ADC_mask[i]=ADCv
 
     Bv_new_times_M_new = np.moveaxis(np.dot(Bv_new, M.T),0,-1).reshape(sz) 
     fit = np.exp(-Bv_new_times_M_new)
-    
-    par = np.empty((npixels, 2))
+       
+    par = np.empty((npixels, 3))
     par[:,0] = FA_mask
     par[:,1] = ADC_mask
+    par[:,2] = S0
     
     return fit, par
 
 
 def main(images_to_be_fitted, signal_model_parameters):
     """ main function to perform DTI model fit. 
 
@@ -138,18 +143,19 @@
     signal_model_parameters (list): list containing 'b-values', 'b-vectors' and 'image_orientation_patient' as list elements.    
 
     Returns
     -------
     fit (numpy.ndarray): signal model fit at all time-series (i.e. at each b-value and direction) with shape [x-dim*y-dim, total time-series].   
     fitted_parameters (numpy.ndarray): output signal model fit parameters 'FA' and 'ADC' stored in a single nd-array with shape [2, x-dim*y-dim].   
     """
+  
     b_values = signal_model_parameters[0]
     bVec_original = signal_model_parameters[1]
     image_orientation_patient = signal_model_parameters[2]
- 
+    
     R1 = image_orientation_patient[0][3:6]
     R1 = [-float(x) for x in R1] 
 
     R2 = image_orientation_patient[0][0:3]
     R2 = [-float(x) for x in R2]
 
     R3 = np.cross(R1, R2)
```

### Comparing `mdreg-0.3.7/src/mdreg/models/DWI_simple.py` & `mdreg-0.3.8/src/mdreg/models/DWI_simple.py`

 * *Files identical despite different names*

### Comparing `mdreg-0.3.7/src/mdreg/models/T1_simple.py` & `mdreg-0.3.8/src/mdreg/models/exp_decay.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,79 @@
-""" 
+#!/ur/bin/python
+# -*- coding: utf-8 -*-
+"""
 @author: Steven Sourbron 
-T1-MOLLI model fit  
-2022  
-Messroghli DR, Radjenovic A, Kozerke S, Higgins DM, Sivananthan MU, Ridgway JP. 
-Modified Look-Locker inversion recovery (MOLLI) for high-resolution T1 mapping of the heart. 
-Magn Reson Med. 2004 Jul;52(1):141-6. doi: 10.1002/mrm.20110. PMID: 15236377. 
+Pixel-by-pixel exponential decay fit 
+2022
 """
-
+from tqdm import tqdm
 import numpy as np
 from scipy.optimize import curve_fit
 
 def pars():
-    return ['S0', 'alpha', 'T1']
+    return ['S0', 'R']
 
 def bounds():
-    lower = [0, 1, 1.0] 
-    upper = [np.inf, 2.0, 3000.0]
+    lower = [0,0]
+    upper = [np.inf, np.inf]
     return lower, upper
 
 
-def func(TI, S0, alpha, T1):
-    """ exponential function for T1-fitting.
+def func(t, S, R):
+    """Mono-exponential decay function.  
 
     Args
     ----
-    x (numpy.ndarray): Inversion times (TI) in the T1-mapping sequence as input for the signal model fit.    
-    
+    t (numpy.ndarray): x-values.  
+
     Returns
     -------
-    a, b, T1 (numpy.ndarray): signal model fitted parameters.  
+    numpy.ndarray: S*exp(-t*R)
+
     """
-    mz = 1 - alpha * np.exp(-TI*(alpha-1)/T1)
-    return np.abs(S0 * mz) 
+    return S*np.exp(-t*R)
 
 
-def main(images, TI):
+def main(images, t, 
+    lower_bounds = [0,0], 
+    upper_bounds = [np.inf, np.inf], 
+    initial_value = [1,1], 
+    method = 'trf', 
+    maxfev = 500, 
+    ):
     """ main function that performs the T2*-map signal model-fit for input 2D image at multiple time-points (TEs).
 
     Args
     ----
     images (numpy.ndarray): input image at all time-series (i.e. at each TE time) with shape [x-dim*y-dim, total time-series].  
     t (list): list containing time points of exponential.  
 
     Returns
     -------
     fit (numpy.ndarray): signal model fit per pixel for whole image with shape [x-dim*y-dim, total time-series].  
     par (numpy.ndarray): output signal model fit parameters 'S' and 'R' stored in a single nd-array with shape [2, x-dim*y-dim].      
     """
 
-    TI = np.array(TI)
+    t = np.array(t)
     shape = np.shape(images)
-    par = np.empty((shape[0], 3)) # pixels should be first for consistency
+    par = np.empty((shape[0], 2)) 
     fit = np.empty(shape)
 
-    for x in range(shape[0]):
+    for x in tqdm(range(shape[0]), desc='Fitting exponential decay'):
 
         signal = images[x,:]
-        p0 = [np.max(signal), 1.9, 1500.0]
+        p0 = [np.max(signal)*initial_value[0], initial_value[1]]
         try:
             par[x,:], _ = curve_fit(func, 
-                xdata = TI, 
+                xdata = t, 
                 ydata = signal, 
                 p0 = p0, 
-                bounds = ([0, 1, 1.0], [np.inf, 2.0, 3000.0]), 
-                method = 'trf', 
-                maxfev = 500, 
+                bounds = (lower_bounds, upper_bounds), 
+                method = method, 
+                maxfev = maxfev, 
             )
-        except RuntimeError: #optimum not found.
+        except RuntimeError:
             par[x,:] = p0
-
-        fit[x,:] = func(TI, par[x,0], par[x,1], par[x,2])
+        fit[x,:] = func(t, par[x,0], par[x,1])
   
-    return fit, par
+    return fit, par
+
```

### Comparing `mdreg-0.3.7/src/mdreg/models/T2_simple.py` & `mdreg-0.3.8/src/mdreg/models/T2_simple.py`

 * *Files identical despite different names*

### Comparing `mdreg-0.3.7/src/mdreg/models/T2star_simple.py` & `mdreg-0.3.8/src/mdreg/models/T2star_simple.py`

 * *Files identical despite different names*

### Comparing `mdreg-0.3.7/src/mdreg/models/constant.py` & `mdreg-0.3.8/src/mdreg/models/constant.py`

 * *Files identical despite different names*

### Comparing `mdreg-0.3.7/src/mdreg.egg-info/PKG-INFO` & `mdreg-0.3.8/src/mdreg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdreg
-Version: 0.3.7
+Version: 0.3.8
 Summary: Model-driven image registration
 Author-email: Kanishka Sharma <kanishka.sharma@sheffield.ac.uk>, Joao Almeida e Sousa <j.g.sousa@sheffield.ac.uk>, Steven Sourbron <s.sourbron@sheffield.ac.uk>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

