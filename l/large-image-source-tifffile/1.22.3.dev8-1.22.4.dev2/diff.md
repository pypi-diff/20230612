# Comparing `tmp/large-image-source-tifffile-1.22.3.dev8.tar.gz` & `tmp/large-image-source-tifffile-1.22.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-tifffile-1.22.3.dev8.tar", last modified: Thu Jun  8 12:53:00 2023, max compression
+gzip compressed data, was "large-image-source-tifffile-1.22.4.dev2.tar", last modified: Mon Jun 12 21:05:47 2023, max compression
```

## Comparing `large-image-source-tifffile-1.22.3.dev8.tar` & `large-image-source-tifffile-1.22.4.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 12:53:00.420898 large-image-source-tifffile-1.22.3.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-08 12:53:00.000000 large-image-source-tifffile-1.22.3.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-08 12:53:00.420898 large-image-source-tifffile-1.22.3.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-08 12:53:00.000000 large-image-source-tifffile-1.22.3.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 12:53:00.416898 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20913 2023-06-08 12:51:10.000000 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-06-08 12:51:10.000000 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 12:53:00.420898 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-08 12:53:00.000000 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-08 12:53:00.000000 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 12:53:00.000000 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-08 12:53:00.000000 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-06-08 12:53:00.000000 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-08 12:53:00.000000 large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-08 12:53:00.420898 large-image-source-tifffile-1.22.3.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-06-08 12:51:10.000000 large-image-source-tifffile-1.22.3.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 21:05:47.846654 large-image-source-tifffile-1.22.4.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-12 21:05:47.000000 large-image-source-tifffile-1.22.4.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-12 21:05:47.846654 large-image-source-tifffile-1.22.4.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-12 21:05:47.000000 large-image-source-tifffile-1.22.4.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 21:05:47.846654 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20974 2023-06-12 21:03:44.000000 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-06-12 21:03:44.000000 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 21:05:47.846654 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-06-12 21:05:47.000000 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-12 21:05:47.000000 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-12 21:05:47.000000 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-12 21:05:47.000000 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2023-06-12 21:05:47.000000 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-12 21:05:47.000000 large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-12 21:05:47.846654 large-image-source-tifffile-1.22.4.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2023-06-12 21:03:44.000000 large-image-source-tifffile-1.22.4.dev2/setup.py
```

### Comparing `large-image-source-tifffile-1.22.3.dev8/LICENSE` & `large-image-source-tifffile-1.22.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.3.dev8/PKG-INFO` & `large-image-source-tifffile-1.22.4.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.22.3.dev8
+Version: 1.22.4.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.22.3.dev8/README.rst` & `large-image-source-tifffile-1.22.4.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile/__init__.py` & `large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         self.levels = int(max(1, math.ceil(math.log(
             float(max(self.sizeX, self.sizeY)) / self.tileWidth) / math.log(2)) + 1))
         self._findAssociatedImages()
         for key in dir(self._tf):
             if (key.startswith('is_') and hasattr(self, '_handle_' + key[3:]) and
                     getattr(self._tf, key)):
                 getattr(self, '_handle_' + key[3:])()
+        self._populatedLevels = len(self._baseSeries.levels)
 
     def _biggestSeries(self):
         """
         Find the series with the most pixels.  Use all series that have the
         same dimensionality and resolution.  They can differ in X, Y size.
 
         :returns: index of the largest series, number of pixels in a frame in
```

### Comparing `large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile/girder_source.py` & `large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.22.3.dev8/large_image_source_tifffile.egg-info/PKG-INFO` & `large-image-source-tifffile-1.22.4.dev2/large_image_source_tifffile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.22.3.dev8
+Version: 1.22.4.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.22.3.dev8/setup.py` & `large-image-source-tifffile-1.22.4.dev2/setup.py`

 * *Files identical despite different names*

