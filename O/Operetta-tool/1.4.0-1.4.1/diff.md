# Comparing `tmp/Operetta_tool-1.4.0.tar.gz` & `tmp/Operetta_tool-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Operetta_tool-1.4.0.tar", last modified: Mon Jun 12 12:40:40 2023, max compression
+gzip compressed data, was "Operetta_tool-1.4.1.tar", last modified: Mon Jun 12 15:12:30 2023, max compression
```

## Comparing `Operetta_tool-1.4.0.tar` & `Operetta_tool-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 12:40:40.926566 Operetta_tool-1.4.0/
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.4.0/LICENSE
--rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.4.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-12 12:40:40.913465 Operetta_tool-1.4.0/Operetta_tool.egg-info/
--rw-rw-rw-   0        0        0      725 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-06-12 12:40:40.925186 Operetta_tool-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 12:40:40.924075 Operetta_tool-1.4.0/operetta/
--rw-rw-rw-   0        0        0      153 2023-06-12 12:33:03.000000 Operetta_tool-1.4.0/operetta/__init__.py
--rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.4.0/operetta/jbsicon.ico
--rw-rw-rw-   0        0        0    59099 2023-06-12 12:24:38.000000 Operetta_tool-1.4.0/operetta/operetta_annotation.py
--rw-rw-rw-   0        0        0       42 2023-06-12 12:40:40.926566 Operetta_tool-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1276 2023-06-12 12:33:10.000000 Operetta_tool-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:12:30.840678 Operetta_tool-1.4.1/
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.4.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-12 15:12:30.837145 Operetta_tool-1.4.1/Operetta_tool.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-06-12 15:12:30.000000 Operetta_tool-1.4.1/Operetta_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-12 15:12:30.000000 Operetta_tool-1.4.1/Operetta_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 15:12:30.000000 Operetta_tool-1.4.1/Operetta_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-06-12 15:12:30.000000 Operetta_tool-1.4.1/Operetta_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 15:12:30.000000 Operetta_tool-1.4.1/Operetta_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-06-12 15:12:30.840678 Operetta_tool-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 15:12:30.840678 Operetta_tool-1.4.1/operetta/
+-rw-rw-rw-   0        0        0      153 2023-06-12 12:33:03.000000 Operetta_tool-1.4.1/operetta/__init__.py
+-rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.4.1/operetta/jbsicon.ico
+-rw-rw-rw-   0        0        0    59095 2023-06-12 14:49:42.000000 Operetta_tool-1.4.1/operetta/operetta_annotation.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 15:12:30.843814 Operetta_tool-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1276 2023-06-12 15:12:21.000000 Operetta_tool-1.4.1/setup.py
```

### Comparing `Operetta_tool-1.4.0/LICENSE` & `Operetta_tool-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.0/Operetta_tool.egg-info/PKG-INFO` & `Operetta_tool-1.4.1/Operetta_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta-tool
-Version: 1.4.0
+Version: 1.4.1
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.4.0/PKG-INFO` & `Operetta_tool-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta_tool
-Version: 1.4.0
+Version: 1.4.1
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.4.0/README.md` & `Operetta_tool-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.0/operetta/jbsicon.ico` & `Operetta_tool-1.4.1/operetta/jbsicon.ico`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.0/operetta/operetta_annotation.py` & `Operetta_tool-1.4.1/operetta/operetta_annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
                 
                 resized_image = np.empty((image.shape[0], wh, width))
                 
                 for n in range(image.shape[0]):
                     resized_image[n] = cv2.resize(image[n], (width, wh))
                     
         
-                metadata['X_resolution[m]'][0] = metadata['X_resolution[m]'][0]*height/h
-                metadata['Y_resolution[m]'][0] = metadata['X_resolution[m]'][0]*height/h
+                metadata['X_resolution[m]'][0] = metadata['X_resolution[m]'][0]*width/w
+                metadata['Y_resolution[m]'][0] = metadata['X_resolution[m]'][0]*width/w
                 
                 print('Resized succesfully')
                 print('Current resolution is ' + str(image.shape[1]) + 'x' + str(image.shape[0]))
                 
             elif width == None and height == None and resize_factor != None:
                 h = image.shape[1]
                 w = image.shape[2]
@@ -145,16 +145,16 @@
             
             wh = int(width/w * h)
             
             
             image = cv2.resize(image, (width, wh))
             if metadata != None:
     
-                metadata['X_resolution[m]'][0] = metadata['X_resolution[m]'][0]*height/h
-                metadata['Y_resolution[m]'][0] = metadata['X_resolution[m]'][0]*height/h
+                metadata['X_resolution[m]'][0] = metadata['X_resolution[m]'][0]*width/w
+                metadata['Y_resolution[m]'][0] = metadata['X_resolution[m]'][0]*width/w
             
             print('Resized succesfully')
             print('Current resolution is ' + str(image.shape[1]) + 'x' + str(image.shape[0]))
             
         elif width == None and height == None and resize_factor != None:
             h = image.shape[0]
             w = image.shape[1]
```

### Comparing `Operetta_tool-1.4.0/setup.py` & `Operetta_tool-1.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.0' 
+VERSION = '1.4.1' 
 DESCRIPTION = 'operetta_tool'
 LONG_DESCRIPTION = 'The Operetta_tool is a python library created for handling and annotation images from the Opera Phenix platform used for ML / AI applications. Instructions for use on github [https://github.com/jkubis96/Operetta_tool] '
 
 # Setting up
 setup(
         name="Operetta_tool", 
         version=VERSION,
```

