# Comparing `tmp/Multi-Template-Matching-1.6.4.tar.gz` & `tmp/Multi-Template-Matching-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Multi-Template-Matching-1.6.4.tar", last modified: Fri Mar  3 10:39:17 2023, max compression
+gzip compressed data, was "Multi-Template-Matching-1.6.5.tar", last modified: Mon Jun 12 14:43:11 2023, max compression
```

## Comparing `Multi-Template-Matching-1.6.4.tar` & `Multi-Template-Matching-1.6.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 10:39:17.209905 Multi-Template-Matching-1.6.4/
--rw-rw-rw-   0        0        0    35823 2023-03-03 09:53:22.000000 Multi-Template-Matching-1.6.4/LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-03 10:39:17.209905 Multi-Template-Matching-1.6.4/MTM/
--rw-rw-rw-   0        0        0     4032 2023-03-03 09:53:22.000000 Multi-Template-Matching-1.6.4/MTM/NMS.py
--rw-rw-rw-   0        0        0    16111 2023-03-03 10:06:23.000000 Multi-Template-Matching-1.6.4/MTM/__init__.py
--rw-rw-rw-   0        0        0      215 2023-03-03 09:53:31.000000 Multi-Template-Matching-1.6.4/MTM/version.py
-drwxrwxrwx   0        0        0        0 2023-03-03 10:39:17.209905 Multi-Template-Matching-1.6.4/Multi_Template_Matching.egg-info/
--rw-rw-rw-   0        0        0     5808 2023-03-03 10:39:17.000000 Multi-Template-Matching-1.6.4/Multi_Template_Matching.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-03-03 10:39:17.000000 Multi-Template-Matching-1.6.4/Multi_Template_Matching.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 10:39:17.000000 Multi-Template-Matching-1.6.4/Multi_Template_Matching.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-03-03 10:39:17.000000 Multi-Template-Matching-1.6.4/Multi_Template_Matching.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-03 10:39:17.000000 Multi-Template-Matching-1.6.4/Multi_Template_Matching.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5808 2023-03-03 10:39:17.209905 Multi-Template-Matching-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     5108 2023-03-03 10:13:24.000000 Multi-Template-Matching-1.6.4/README.md
--rw-rw-rw-   0        0        0      108 2023-03-03 09:53:22.000000 Multi-Template-Matching-1.6.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-03 10:39:17.209905 Multi-Template-Matching-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1038 2023-03-03 09:53:22.000000 Multi-Template-Matching-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:43:11.094475 Multi-Template-Matching-1.6.5/
+-rw-rw-rw-   0        0        0    35823 2023-03-03 09:53:22.000000 Multi-Template-Matching-1.6.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-12 14:43:11.083456 Multi-Template-Matching-1.6.5/MTM/
+-rw-rw-rw-   0        0        0     4032 2023-03-03 09:53:22.000000 Multi-Template-Matching-1.6.5/MTM/NMS.py
+-rw-rw-rw-   0        0        0    16786 2023-06-01 16:08:23.000000 Multi-Template-Matching-1.6.5/MTM/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-06-12 14:37:31.000000 Multi-Template-Matching-1.6.5/MTM/version.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:43:11.093456 Multi-Template-Matching-1.6.5/Multi_Template_Matching.egg-info/
+-rw-rw-rw-   0        0        0     5808 2023-06-12 14:43:10.000000 Multi-Template-Matching-1.6.5/Multi_Template_Matching.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-06-12 14:43:11.000000 Multi-Template-Matching-1.6.5/Multi_Template_Matching.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:43:10.000000 Multi-Template-Matching-1.6.5/Multi_Template_Matching.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-12 14:43:10.000000 Multi-Template-Matching-1.6.5/Multi_Template_Matching.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-12 14:43:10.000000 Multi-Template-Matching-1.6.5/Multi_Template_Matching.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5808 2023-06-12 14:43:11.094475 Multi-Template-Matching-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5108 2023-03-03 10:13:24.000000 Multi-Template-Matching-1.6.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-03 09:53:22.000000 Multi-Template-Matching-1.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:43:11.095455 Multi-Template-Matching-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-03-03 09:53:22.000000 Multi-Template-Matching-1.6.5/setup.py
```

### Comparing `Multi-Template-Matching-1.6.4/LICENSE` & `Multi-Template-Matching-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Multi-Template-Matching-1.6.4/MTM/NMS.py` & `Multi-Template-Matching-1.6.5/MTM/NMS.py`

 * *Files identical despite different names*

### Comparing `Multi-Template-Matching-1.6.4/MTM/__init__.py` & `Multi-Template-Matching-1.6.5/MTM/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,33 +117,51 @@
 
     Returns
     -------
     - Pandas DataFrame with 1 row per hit and column "TemplateName"(string), "BBox":(X, Y, Width, Height), "Score":float
     """
     if N_object != float("inf") and not isinstance(N_object, int):
         raise TypeError("N_object must be an integer")
-
+    
+    ## Check image has not 0-width or height
+    if image.shape[0] == 0:
+        raise ValueError("Image has a height of 0.")
+    
+    if image.shape[1] == 0:
+        raise ValueError("Image has a width of 0.")
+    
     ## Crop image to search region if provided
     if searchBox is not None:
         xOffset, yOffset, searchWidth, searchHeight = searchBox
         image = image[yOffset : yOffset+searchHeight, xOffset : xOffset+searchWidth]
     else:
         xOffset=yOffset=0
 
     # Check that the template are all smaller are equal to the image (original, or cropped if there is a search region)
     for index, tempTuple in enumerate(listTemplates):
 
-        if not isinstance(tempTuple, tuple) or len(tempTuple)==1:
+        if not isinstance(tempTuple, tuple) or len(tempTuple)<2:
             raise ValueError("listTemplates should be a list of tuples as ('name','array') or ('name', 'array', 'mask')")
-
-        templateSmallerThanImage = all(templateDim <= imageDim for templateDim, imageDim in zip(tempTuple[1].shape, image.shape))
+        
+        tempName = tempTuple[0]
+        tempImage = tempTuple[1]
+        
+        # Check that template is not 0-width or height
+        if tempImage.shape[0] == 0:
+            raise ValueError(f"Template '{tempName}' has a height of 0.")
+        
+        if tempImage.shape[1] == 0:
+            raise ValueError(f"Template '{tempName}' has a width of 0.")
+        
+        
+        templateSmallerThanImage = all(templateDim <= imageDim for templateDim, imageDim in zip(tempImage.shape, image.shape)) # check both width/height smaller than image or search region
 
         if not templateSmallerThanImage :
             fitIn = "searchBox" if (searchBox is not None) else "image"
-            raise ValueError("Template '{}' at index {} in the list of templates is larger than {}.".format(tempTuple[0], index, fitIn) )
+            raise ValueError("Template '{}' at index {} in the list of templates is larger than {}.".format(tempName, index, fitIn) )
 
     listHit = []
     ## Use multi-threading to iterate through all templates, using half the number of cpu cores available.
     with ThreadPoolExecutor(max_workers=round(os.cpu_count()*.5)) as executor:
         futures = [executor.submit(_multi_compute, tempTuple, image, method, N_object, score_threshold, xOffset, yOffset, listHit) for tempTuple in listTemplates]
         for future in as_completed(futures):
             _ = future.result()
```

### Comparing `Multi-Template-Matching-1.6.4/Multi_Template_Matching.egg-info/PKG-INFO` & `Multi-Template-Matching-1.6.5/Multi_Template_Matching.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multi-Template-Matching
-Version: 1.6.4
+Version: 1.6.5
 Summary: Object-recognition in images using multiple templates
 Home-page: https://github.com/multi-template-matching/MultiTemplateMatching-Python
 Author: Laurent Thomas
 Author-email: laurent132.thomas@laposte.net
 Keywords: object-recognition object-localization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Multi-Template-Matching-1.6.4/PKG-INFO` & `Multi-Template-Matching-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multi-Template-Matching
-Version: 1.6.4
+Version: 1.6.5
 Summary: Object-recognition in images using multiple templates
 Home-page: https://github.com/multi-template-matching/MultiTemplateMatching-Python
 Author: Laurent Thomas
 Author-email: laurent132.thomas@laposte.net
 Keywords: object-recognition object-localization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Multi-Template-Matching-1.6.4/README.md` & `Multi-Template-Matching-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `Multi-Template-Matching-1.6.4/setup.py` & `Multi-Template-Matching-1.6.5/setup.py`

 * *Files identical despite different names*

