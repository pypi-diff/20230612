# Comparing `tmp/large-image-source-rasterio-1.22.3.dev8.tar.gz` & `tmp/large-image-source-rasterio-1.22.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.22.3.dev8.tar", last modified: Thu Jun  8 12:52:46 2023, max compression
+gzip compressed data, was "large-image-source-rasterio-1.22.4.dev2.tar", last modified: Mon Jun 12 21:05:34 2023, max compression
```

## Comparing `large-image-source-rasterio-1.22.3.dev8.tar` & `large-image-source-rasterio-1.22.4.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 12:52:46.800842 large-image-source-rasterio-1.22.3.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-08 12:52:46.000000 large-image-source-rasterio-1.22.3.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-08 12:52:46.800842 large-image-source-rasterio-1.22.3.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-08 12:52:46.000000 large-image-source-rasterio-1.22.3.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 12:52:46.800842 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43052 2023-06-08 12:51:10.000000 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-06-08 12:51:10.000000 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 12:52:46.800842 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-08 12:52:46.000000 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-08 12:52:46.000000 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 12:52:46.000000 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-08 12:52:46.000000 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-06-08 12:52:46.000000 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-08 12:52:46.000000 large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-08 12:52:46.800842 large-image-source-rasterio-1.22.3.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-06-08 12:51:10.000000 large-image-source-rasterio-1.22.3.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 21:05:34.326660 large-image-source-rasterio-1.22.4.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-12 21:05:34.000000 large-image-source-rasterio-1.22.4.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-12 21:05:34.326660 large-image-source-rasterio-1.22.4.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-12 21:05:34.000000 large-image-source-rasterio-1.22.4.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 21:05:34.326660 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43289 2023-06-12 21:03:44.000000 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-06-12 21:03:44.000000 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 21:05:34.326660 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-12 21:05:34.000000 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-12 21:05:34.000000 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-12 21:05:34.000000 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-12 21:05:34.000000 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-06-12 21:05:34.000000 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-12 21:05:34.000000 large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-12 21:05:34.326660 large-image-source-rasterio-1.22.4.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-06-12 21:03:44.000000 large-image-source-rasterio-1.22.4.dev2/setup.py
```

### Comparing `large-image-source-rasterio-1.22.3.dev8/LICENSE` & `large-image-source-rasterio-1.22.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.3.dev8/PKG-INFO` & `large-image-source-rasterio-1.22.4.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.22.3.dev8
+Version: 1.22.4.dev2
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.22.3.dev8/README.rst` & `large-image-source-rasterio-1.22.4.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,17 +148,25 @@
         logX = math.log(float(self.sizeX) / self.tileWidth)
         logY = math.log(float(self.sizeY) / self.tileHeight)
         computedLevel = math.ceil(max(logX, logY) / math.log(2))
         self.sourceLevels = self.levels = int(max(0, computedLevel) + 1)
 
         self._unitsPerPixel = unitsPerPixel
         self.projection is None or self._initWithProjection(unitsPerPixel)
+        self._getPopulatedLevels()
         self._getTileLock = threading.Lock()
         self._setDefaultStyle()
 
+    def _getPopulatedLevels(self):
+        try:
+            with self._getDatasetLock:
+                self._populatedLevels = 1 + len(self.dataset.overviews(1))
+        except Exception:
+            pass
+
     def _scanForMinMax(self, dtype, frame=0, analysisSize=1024, onlyMinMax=True):
         """Update the band range of the data type to the end of the range list.
 
         This will change autocalling behavior, and for non-integer data types,
         this adds the range [0, 1].
 
         :param dtype: the dtype of the bands
@@ -236,16 +244,16 @@
             self.unitsAcrossLevel0 = ProjUnitsAcrossLevel0.get(
                 self.projection.to_string()
             )
             if self.unitsAcrossLevel0 is None:
                 # If unitsPerPixel is not specified, the horizontal distance
                 # between -180,0 and +180,0 is used.  Some projections (such as
                 # stereographic) will fail in this case; they must have a unitsPerPixel specified.
-                east, _ = warp.transform(srcCrs, dstCrs, [-180,], [0,])
-                west, _ = warp.transform(srcCrs, dstCrs, [180,], [0,])
+                east, _ = warp.transform(srcCrs, dstCrs, [-180], [0])
+                west, _ = warp.transform(srcCrs, dstCrs, [180], [0])
                 self.unitsAcrossLevel0 = abs(east[0] - west[0])
                 if not self.unitsAcrossLevel0:
                     raise TileSourceError(
                         'unitsPerPixel must be specified for this projection'
                     )
                 if len(ProjUnitsAcrossLevel0) >= ProjUnitsAcrossLevel0_MaxSize:
                     ProjUnitsAcrossLevel0.clear()
```

### Comparing `large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.3.dev8/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.22.4.dev2/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.22.3.dev8
+Version: 1.22.4.dev2
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.22.3.dev8/setup.py` & `large-image-source-rasterio-1.22.4.dev2/setup.py`

 * *Files identical despite different names*

