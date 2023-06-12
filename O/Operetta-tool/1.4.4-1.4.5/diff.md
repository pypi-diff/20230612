# Comparing `tmp/Operetta_tool-1.4.4.tar.gz` & `tmp/Operetta_tool-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Operetta_tool-1.4.4.tar", last modified: Mon Jun 12 15:53:12 2023, max compression
+gzip compressed data, was "Operetta_tool-1.4.5.tar", last modified: Mon Jun 12 20:52:17 2023, max compression
```

## Comparing `Operetta_tool-1.4.4.tar` & `Operetta_tool-1.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 15:53:12.388142 Operetta_tool-1.4.4/
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.4.4/LICENSE
--rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.4.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-12 15:53:12.379589 Operetta_tool-1.4.4/Operetta_tool.egg-info/
--rw-rw-rw-   0        0        0      725 2023-06-12 15:53:11.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-12 15:53:12.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 15:53:11.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-06-12 15:53:12.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 15:53:12.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-06-12 15:53:12.387019 Operetta_tool-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 15:53:12.381605 Operetta_tool-1.4.4/operetta/
--rw-rw-rw-   0        0        0      153 2023-06-12 15:53:06.000000 Operetta_tool-1.4.4/operetta/__init__.py
--rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.4.4/operetta/jbsicon.ico
--rw-rw-rw-   0        0        0    59095 2023-06-12 15:51:54.000000 Operetta_tool-1.4.4/operetta/operetta_annotation.py
--rw-rw-rw-   0        0        0       42 2023-06-12 15:53:12.388142 Operetta_tool-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1276 2023-06-12 15:53:01.000000 Operetta_tool-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:52:17.616438 Operetta_tool-1.4.5/
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.4.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-12 20:52:17.597201 Operetta_tool-1.4.5/Operetta_tool.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-06-12 20:52:16.000000 Operetta_tool-1.4.5/Operetta_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-12 20:52:17.000000 Operetta_tool-1.4.5/Operetta_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 20:52:16.000000 Operetta_tool-1.4.5/Operetta_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-06-12 20:52:17.000000 Operetta_tool-1.4.5/Operetta_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 20:52:17.000000 Operetta_tool-1.4.5/Operetta_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-06-12 20:52:17.615916 Operetta_tool-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 20:52:17.612153 Operetta_tool-1.4.5/operetta/
+-rw-rw-rw-   0        0        0      153 2023-06-12 20:51:47.000000 Operetta_tool-1.4.5/operetta/__init__.py
+-rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.4.5/operetta/jbsicon.ico
+-rw-rw-rw-   0        0        0    61071 2023-06-12 20:48:47.000000 Operetta_tool-1.4.5/operetta/operetta_annotation.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 20:52:17.616438 Operetta_tool-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1276 2023-06-12 20:51:50.000000 Operetta_tool-1.4.5/setup.py
```

### Comparing `Operetta_tool-1.4.4/LICENSE` & `Operetta_tool-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.4/Operetta_tool.egg-info/PKG-INFO` & `Operetta_tool-1.4.5/Operetta_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta-tool
-Version: 1.4.4
+Version: 1.4.5
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.4.4/PKG-INFO` & `Operetta_tool-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta_tool
-Version: 1.4.4
+Version: 1.4.5
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.4.4/README.md` & `Operetta_tool-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.4/operetta/jbsicon.ico` & `Operetta_tool-1.4.5/operetta/jbsicon.ico`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.4/operetta/operetta_annotation.py` & `Operetta_tool-1.4.5/operetta/operetta_annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,114 +17,141 @@
 import gc
 import warnings
 import tkinter as tk 
 from tkinter import ttk, Text
 from skimage import io, filters
 import pkg_resources
 from PIL import ImageFont, ImageDraw, Image
+import copy
+
 
 
 
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 
 
 
-def resize_tiff(path_to_tiff:str, metadata, prefix = 'resized' , height = None, width = None, resize_factor = None):
+def resize_tiff(channels:list, metadata, prefix = 'resized' , height = None, width = None, resize_factor = None):
     
     if metadata == None:
         print('Metadata is required. Load metadata')
-    elif not os.path.exists(path_to_tiff):
-        print('\nImage does not exist. Check the correctness of the path to image')
     
     else:
         
         try:
-    
-            image = tiff.imread(path_to_tiff)
             
-            if height != None and  width == None:
-                h = image.shape[1]
-                w = image.shape[2]
-                
-                wh = int(height/h * w)
-                
+            
+            for ch in channels:
                 
+                res_metadata = copy.deepcopy(metadata)
                 
-                resized_image = np.empty((image.shape[0], height, wh))
+                path_to_tiff = str('channel_' + str(ch) + '.tiff')
                 
-                for n in range(image.shape[0]):
-                    resized_image[n] = cv2.resize(image[n], (wh, height))
+                if not os.path.exists(path_to_tiff):
+                    print('\nImage ' + path_to_tiff +  ' does not exist')
+                else:
+    
+                    image = tiff.imread(path_to_tiff)
                     
+                    if height != None and  width == None:
+                        h = image.shape[1]
+                        w = image.shape[2]
+                        
+                        wh = int(height/h * w)
+                        
+                        
+                        
+                        resized_image = np.empty((image.shape[0], height, wh)).astype(np.uint16)
+                        
+                        for n in range(image.shape[0]):
+                            resized_image[n] = cv2.resize(image[n], (wh, height))
+                            
+                            
+                        res_metadata['X_resolution[m]'][0] = res_metadata['X_resolution[m]'][0]*height/h
+                        res_metadata['Y_resolution[m]'][0] = res_metadata['Y_resolution[m]'][0]*height/h
+                        
+                        
+                        tiff.imsave(str(prefix + '_' + path_to_tiff), resized_image,
+                                        imagej=True,
+                                        resolution=(res_metadata['X_resolution[m]'][0]*1000000, res_metadata['Y_resolution[m]'][0]*1000000),
+                                        metadata={'spacing': res_metadata['z_spacing'], 'unit': 'um'}) 
+                            
+                        print('Resized succesfully')
+                        print('Current resolution is ' + str(resized_image.shape[2]) + 'x' + str(resized_image.shape[1]))
+                        
+                    elif width != None and height == None:
+                        h = image.shape[1]
+                        w = image.shape[2]
+                        
+                        wh = int(width/w * h)
+                        
+                        
+                        resized_image = np.empty((image.shape[0], wh, width)).astype(np.uint16)
+                        
+                        for n in range(image.shape[0]):
+                            resized_image[n] = cv2.resize(image[n], (width, wh))
+                            
+                
+                        res_metadata['X_resolution[m]'][0] = res_metadata['X_resolution[m]'][0]*width/w
+                        res_metadata['Y_resolution[m]'][0] = res_metadata['Y_resolution[m]'][0]*width/w
+                        
+                        tiff.imsave(str(prefix + '_' + path_to_tiff), resized_image,
+                                        imagej=True,
+                                        resolution=(res_metadata['X_resolution[m]'][0]*1000000, res_metadata['Y_resolution[m]'][0]*1000000),
+                                        metadata={'spacing': res_metadata['z_spacing'], 'unit': 'um'}) 
+                        
+                        print('Resized succesfully')
+                        print('Current resolution is ' + str(resized_image.shape[2]) + 'x' + str(resized_image.shape[1]))
+                        
+                    elif width == None and height == None and resize_factor != None:
+                        h = image.shape[1]
+                        w = image.shape[2]
+                        
+                        wh = int(w / resize_factor)
+                        hw = int(h / resize_factor)
+                        
+                        
+                        resized_image = np.empty((image.shape[0], hw, wh)).astype(np.uint16)
+                        
+                        for n in range(image.shape[0]):
+                            resized_image[n] = cv2.resize(image[n], (wh, hw))
+                        
+                
+                        res_metadata['X_resolution[m]'][0] = res_metadata['X_resolution[m]'][0]/resize_factor
+                        res_metadata['Y_resolution[m]'][0] = res_metadata['Y_resolution[m]'][0]/resize_factor
+                        
+                        tiff.imsave(str(prefix + '_' + path_to_tiff), resized_image,
+                                        imagej=True,
+                                        resolution=(res_metadata['X_resolution[m]'][0]*1000000, res_metadata['Y_resolution[m]'][0]*1000000),
+                                        metadata={'spacing': res_metadata['z_spacing'], 'unit': 'um'}) 
+                           
+                        print('Resized succesfully')
+                        print('Current resolution is ' + str(resized_image.shape[2]) + 'x' + str(resized_image.shape[1]))
+                        
+                    elif width != None and height != None:
+                        print('Resized with [width x hight] both parameters is not allowed')
+                        print('Choose one parameter and second will be scaled')
+                        print('Rescaling on both parameters without scale can modifie biological diversity')
                     
-                metadata['X_resolution[m]'][0] = metadata['X_resolution[m]'][0]*height/h
-                metadata['Y_resolution[m]'][0] = metadata['Y_resolution[m]'][0]*height/h
+                    else:
+                        print('Resized unsuccessfully')
+                        print('Provided wrong parameters or lack of parameters')
+                           
                     
-                print('Resized succesfully')
-                print('Current resolution is ' + str(image.shape[1]) + 'x' + str(image.shape[0]))
-                
-            elif width != None and height == None:
-                h = image.shape[1]
-                w = image.shape[2]
-                
-                wh = int(width/w * h)
-                
-                
-                resized_image = np.empty((image.shape[0], wh, width))
-                
-                for n in range(image.shape[0]):
-                    resized_image[n] = cv2.resize(image[n], (width, wh))
                     
-        
-                metadata['X_resolution[m]'][0] = metadata['X_resolution[m]'][0]*width/w
-                metadata['Y_resolution[m]'][0] = metadata['Y_resolution[m]'][0]*width/w
-                
-                print('Resized succesfully')
-                print('Current resolution is ' + str(image.shape[1]) + 'x' + str(image.shape[0]))
-                
-            elif width == None and height == None and resize_factor != None:
-                h = image.shape[1]
-                w = image.shape[2]
-                
-                wh = int(w / resize_factor)
-                hw = int(h / resize_factor)
-                
-                
-                resized_image = np.empty((image.shape[0], hw, wh))
-                
-                for n in range(image.shape[0]):
-                    resized_image[n] = cv2.resize(image[n], (wh, hw))
-                
-        
-                metadata['X_resolution[m]'][0] = metadata['X_resolution[m]'][0]/resize_factor
-                metadata['Y_resolution[m]'][0] = metadata['Y_resolution[m]'][0]/resize_factor
-                   
-                print('Resized succesfully')
-                print('Current resolution is ' + str(image.shape[1]) + 'x' + str(image.shape[0]))
-                
-            elif width != None and height != None:
-                print('Resized with [width x hight] both parameters is not allowed')
-                print('Choose one parameter and second will be scaled')
-                print('Rescaling on both parameters without scale can modifie biological diversity')
-            
-            else:
-                print('Resized unsuccessfully')
-                print('Provided wrong parameters or lack of parameters')
-                   
-            
-            tiff.imsave(str(prefix + '_' + path_to_tiff), resized_image,
-                            imagej=True,
-                            resolution=(metadata['X_resolution[m]'][0]*1000000, metadata['Y_resolution[m]'][0]*1000000),
-                            metadata={'spacing': metadata['z_spacing'], 'unit': 'um'}) 
-        
-            return metadata
+            
+            
+            return res_metadata
         
         except:
             print("Something went wrong. Check the function input data and try again!")
             
-            
+     
+
+     
 def resize_projection(image, metadata = None, height = None, width = None, resize_factor = None):
     
     try:
         if height != None and  width == None:
             h = image.shape[0]
             w = image.shape[1]
```

### Comparing `Operetta_tool-1.4.4/setup.py` & `Operetta_tool-1.4.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.4' 
+VERSION = '1.4.5' 
 DESCRIPTION = 'operetta_tool'
 LONG_DESCRIPTION = 'The Operetta_tool is a python library created for handling and annotation images from the Opera Phenix platform used for ML / AI applications. Instructions for use on github [https://github.com/jkubis96/Operetta_tool] '
 
 # Setting up
 setup(
         name="Operetta_tool", 
         version=VERSION,
```

