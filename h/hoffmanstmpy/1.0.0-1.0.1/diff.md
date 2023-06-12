# Comparing `tmp/hoffmanstmpy-1.0.0.tar.gz` & `tmp/hoffmanstmpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoffmanstmpy-1.0.0.tar", last modified: Thu May  4 01:59:31 2023, max compression
+gzip compressed data, was "hoffmanstmpy-1.0.1.tar", last modified: Mon Jun 12 20:08:27 2023, max compression
```

## Comparing `hoffmanstmpy-1.0.0.tar` & `hoffmanstmpy-1.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-05-04 01:59:31.214385 hoffmanstmpy-1.0.0/
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1065 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/LICENSE.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)       71 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/MANIFEST.in
--rw-r--r--   0 richardyuliu   (501) staff       (20)      621 2023-05-04 01:59:31.214683 hoffmanstmpy-1.0.0/PKG-INFO
--rw-r--r--   0 richardyuliu   (501) staff       (20)      570 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/README.md
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-05-04 01:59:31.188447 hoffmanstmpy-1.0.0/hoffmanstmpy.egg-info/
--rw-r--r--   0 richardyuliu   (501) staff       (20)      621 2023-05-04 01:59:31.000000 hoffmanstmpy-1.0.0/hoffmanstmpy.egg-info/PKG-INFO
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1139 2023-05-04 01:59:31.000000 hoffmanstmpy-1.0.0/hoffmanstmpy.egg-info/SOURCES.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:59:31.000000 hoffmanstmpy-1.0.0/hoffmanstmpy.egg-info/dependency_links.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)       50 2023-05-04 01:59:31.000000 hoffmanstmpy-1.0.0/hoffmanstmpy.egg-info/requires.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)        6 2023-05-04 01:59:31.000000 hoffmanstmpy-1.0.0/hoffmanstmpy.egg-info/top_level.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)       79 2023-05-04 01:59:31.215620 hoffmanstmpy-1.0.0/setup.cfg
--rw-r--r--   0 richardyuliu   (501) staff       (20)      922 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/setup.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-05-04 01:59:31.193295 hoffmanstmpy-1.0.0/stmpy/
--rw-r--r--   0 richardyuliu   (501) staff       (20)      670 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/__init__.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-05-04 01:59:31.195515 hoffmanstmpy-1.0.0/stmpy/color/
--rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/__init__.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     7611 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/colormap.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-05-04 01:59:31.207079 hoffmanstmpy-1.0.0/stmpy/color/maps/
--rw-r--r--   0 richardyuliu   (501) staff       (20)     8055 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/ALS-og.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)    19200 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/ALS.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1944 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Autumn.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     2251 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Blue1.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     2045 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Blue2.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1955 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Blue3.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1905 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Defect0.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1733 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Defect1.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1494 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Defect2.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1734 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Defect4.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1073 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Gray.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1536 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/GrayInverse.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)    25600 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/PuGn.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)    25585 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/Red_Blue.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1511 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/SailingMod2.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)      694 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/YH.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     2996 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/maps/mhblue.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     2410 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/color/palette.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1544 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.0/stmpy/cv.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    80698 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/driftcorr.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-05-04 01:59:31.209894 hoffmanstmpy-1.0.0/stmpy/hp/
--rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/hp/__init__.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     8939 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/hp/kondo_holes.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    20378 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/hp/tight_binding.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    18901 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/image.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    39756 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/io.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-05-04 01:59:31.213721 hoffmanstmpy-1.0.0/stmpy/mapviewer/
--rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/mapviewer/__init__.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    32564 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/mapviewer/gui_components.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)      886 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/mapviewer/helptext.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)     3393 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/mapviewer/misc.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     8131 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/mapviewer/view3ds.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     7015 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/matio.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1226 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/read_STMView.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    26985 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/read_all.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)   104436 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.0/stmpy/tools.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.063629 hoffmanstmpy-1.0.1/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1065 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/LICENSE.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)       71 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/MANIFEST.in
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      621 2023-06-12 20:08:27.063908 hoffmanstmpy-1.0.1/PKG-INFO
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1283 2023-05-25 15:46:08.000000 hoffmanstmpy-1.0.1/README.md
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.027938 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      621 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/PKG-INFO
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1139 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)       50 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/requires.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        6 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/top_level.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)       79 2023-06-12 20:08:27.064796 hoffmanstmpy-1.0.1/setup.cfg
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      922 2023-06-12 20:07:31.000000 hoffmanstmpy-1.0.1/setup.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.034884 hoffmanstmpy-1.0.1/stmpy/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      670 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/__init__.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.037292 hoffmanstmpy-1.0.1/stmpy/color/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/__init__.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     7611 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/colormap.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.053202 hoffmanstmpy-1.0.1/stmpy/color/maps/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     8055 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/ALS-og.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    19200 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/ALS.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1944 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Autumn.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     2251 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Blue1.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     2045 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Blue2.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1955 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Blue3.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1905 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Defect0.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1733 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Defect1.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1494 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Defect2.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1734 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Defect4.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1073 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Gray.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1536 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/GrayInverse.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    25600 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/PuGn.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    25585 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Red_Blue.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1511 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/SailingMod2.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      694 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/YH.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     2996 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/mhblue.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     2410 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/palette.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1544 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/cv.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    83396 2023-05-25 19:46:50.000000 hoffmanstmpy-1.0.1/stmpy/driftcorr.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.056792 hoffmanstmpy-1.0.1/stmpy/hp/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/hp/__init__.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     8939 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/hp/kondo_holes.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    20378 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/hp/tight_binding.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    19176 2023-05-25 20:07:07.000000 hoffmanstmpy-1.0.1/stmpy/image.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    39913 2023-05-18 21:06:25.000000 hoffmanstmpy-1.0.1/stmpy/io.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.062853 hoffmanstmpy-1.0.1/stmpy/mapviewer/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/__init__.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    32564 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/gui_components.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      886 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/helptext.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     3393 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/misc.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     8131 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/view3ds.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     7015 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/matio.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1226 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/read_STMView.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    26985 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/read_all.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)   104850 2023-05-25 19:30:41.000000 hoffmanstmpy-1.0.1/stmpy/tools.py
```

### Comparing `hoffmanstmpy-1.0.0/LICENSE.txt` & `hoffmanstmpy-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/PKG-INFO` & `hoffmanstmpy-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hoffmanstmpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scanning tunneling microscopy data analysis suite
 Home-page: https://github.com/hoffmanlabcoding/stmpy
 Author: Harris Pirie
 Author-email: hoffmanlabcoding@gmail.com
 License: MIT
 Download-URL: https://github.com/hoffmanlabcoding/stmpy.git
 Description: UNKNOWN
```

### Comparing `hoffmanstmpy-1.0.0/hoffmanstmpy.egg-info/PKG-INFO` & `hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hoffmanstmpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scanning tunneling microscopy data analysis suite
 Home-page: https://github.com/hoffmanlabcoding/stmpy
 Author: Harris Pirie
 Author-email: hoffmanlabcoding@gmail.com
 License: MIT
 Download-URL: https://github.com/hoffmanlabcoding/stmpy.git
 Description: UNKNOWN
```

### Comparing `hoffmanstmpy-1.0.0/hoffmanstmpy.egg-info/SOURCES.txt` & `hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/setup.py` & `hoffmanstmpy-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'hoffmanstmpy',
-  version = '1.0.0',
+  version = '1.0.1',
   packages = find_packages(),
   package_data = {
     "":["*.txt", "*.mat"]
     },
   include_package_data=True,
   license='MIT',
   description = 'Scanning tunneling microscopy data analysis suite',
```

### Comparing `hoffmanstmpy-1.0.0/stmpy/__init__.py` & `hoffmanstmpy-1.0.1/stmpy/__init__.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/colormap.py` & `hoffmanstmpy-1.0.1/stmpy/color/colormap.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/ALS-og.txt` & `hoffmanstmpy-1.0.1/stmpy/color/maps/ALS-og.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/ALS.txt` & `hoffmanstmpy-1.0.1/stmpy/color/maps/ALS.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Autumn.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Autumn.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Blue1.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Blue1.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Blue2.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Blue2.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Blue3.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Blue3.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Defect0.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Defect0.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Defect1.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Defect1.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Defect2.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Defect2.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Defect4.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Defect4.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Gray.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Gray.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/GrayInverse.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/GrayInverse.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/PuGn.txt` & `hoffmanstmpy-1.0.1/stmpy/color/maps/PuGn.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/Red_Blue.txt` & `hoffmanstmpy-1.0.1/stmpy/color/maps/Red_Blue.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/SailingMod2.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/SailingMod2.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/YH.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/YH.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/maps/mhblue.mat` & `hoffmanstmpy-1.0.1/stmpy/color/maps/mhblue.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/color/palette.py` & `hoffmanstmpy-1.0.1/stmpy/color/palette.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/cv.py` & `hoffmanstmpy-1.0.1/stmpy/cv.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/driftcorr.py` & `hoffmanstmpy-1.0.1/stmpy/driftcorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -563,19 +563,18 @@
     History:
         06/23/2020  - RL : Initial commit.
     '''
     p = {}
     if cut1 is not None:
         A = cropedge_new(A, n=cut1)
 
-    # find the Bragg peak before the drift correction 
-    bp1 = findBraggs(A, r=r, w=w, mask3=mask3, show=show, **kwargs)
-    bp1 = sortBraggs(bp1, s=np.shape(A))
-
     if bp_c is None:
+        # find the Bragg peak before the drift correction 
+        bp1 = findBraggs(A, r=r, w=w, mask3=mask3, show=show, **kwargs)
+        bp1 = sortBraggs(bp1, s=np.shape(A))
         # Find the angle between each Bragg peaks
         if bp_angle is None:
             N = len(bp1)
             Q = bp_to_q(bp1, A)
             angles = []
             for i in range(N-1):
                 angles.append(np.arctan2(*Q[i+1]) - np.arctan2(*Q[i]))
@@ -584,14 +583,16 @@
             offset = np.absolute(np.mean(angles) - angle_list)
             index = np.argmin(offset)
             bp_angle = angle_list[index]
             if orient is None:
                 orient = np.arctan2(*Q[0][::-1])
         # Calculate the correction position of each Bragg peak
         bp_c = generate_bp(A, bp1, angle=bp_angle, orient= orient, even_out=even_out)
+    else:
+        bp1 = bp_c
     
     # Find the phasemap 
     thetax, thetay, Q1, Q2 = phasemap(A, bp=bp_c, method=method, sigma=sigma)
 
     phix = fixphaseslip(thetax, method='unwrap')
     phiy = fixphaseslip(thetay, method='unwrap')
     ux, uy = driftmap(phix, phiy, Q1, Q2, method=method)
@@ -1079,24 +1080,25 @@
     popt, pcov = opt.curve_fit(gauss, (X,Y), data.ravel(), p0=p0)
     return popt, gauss((X,Y),*popt).reshape(data.shape)
 
 # help function: custom mask to remove unwanted Bragg peaks
 def mask_bp(A, p):
 
     n, offset, thres, *_ = p
-    s = np.shape(A)[-1]
-    t = np.arange(s)
-    x, y = np.meshgrid(t, t)
-    center = (np.array([s, s])-1) // 2
+    s2, s1 = np.shape(A)[-2:]
+    t1 = np.arange(s1)
+    t2 = np.arange(s2)
+    x, y = np.meshgrid(t1, t2)
+    center = (np.array([s1, s2])-1) // 2
     mask = np.ones_like(x)
     theta = 2 * np.pi / n
     for i in range(n):
         angle = theta * i + offset
         index = np.where(np.absolute(np.cos(angle)*(y-center[1]) - \
-                                     np.sin(angle)*(x-center[0])) < thres)
+                                     np.sin(angle)*(x-center[0]) * s2 / s1) < thres)
         mask[index] = 0
     return mask
 
 # help function: make sure the Bragg peaks are located on even pixels
 def __even_bp(bp, s):
     '''
     This internal function rounds the Bragg peaks to their nearest even number of Q vectors.
@@ -1356,15 +1358,15 @@
         A_x = A * np.exp(-1j*exponent_x)
         A_y = A * np.exp(-1j*exponent_y)
         # sx = sigma
         # sy = sigma * s1 / s2
         sx = sigmax
         sy = sigmay
         Amp = 1/(4*np.pi*sx*sy)
-        p0 = [int((s-1)/2), int((s-1)/2), sx, sy, Amp, np.pi/2]
+        p0 = [int((s1-1)/2), int((s2-1)/2), sx, sy, Amp, np.pi/2]
         G = stmpy.tools.gauss2d(t_x, t_y, p=p0, symmetric=True)
         T_x = sp.signal.fftconvolve(A_x, G, mode='same',)
         T_y = sp.signal.fftconvolve(A_y, G, mode='same',)
         R_x = np.abs(T_x)
         R_y = np.abs(T_y)
         phi_y = np.angle(T_y)
         phi_x = np.angle(T_x)
@@ -1891,15 +1893,16 @@
         if saveon is True:
             plt.savefig(
                 imgName + " along {}.{}".format(fname[i], extension), facecolor='w')
 
 # Quick show single images
 
 
-def quick_show_single(A, en, thres=5, fs=4, qscale=None, rspace=False, saveon=False, qlimit=1.2, imgName='', extension='png', dpi=400):
+def quick_show_single(A, en, thres=5, fs=4, qscale=None, rspace=False, saveon=False, 
+                        qlimit=1.2, imgName='', extension='png', dpi=400):
     layers = len(A)
     if rspace is False:
         if qscale is None:
             imgsize = np.shape(A)[-1]
             if len(np.shape(A)) == 3:
                 A_topo = np.mean(A, axis=0)
             else:
@@ -1953,7 +1956,74 @@
         if saveon is True:
             if extension == 'png':
                 plt.savefig("{} at {} mV.{}".format(imgName, int(
                     en), extension), dpi=dpi, bbox_inches='tight', pad_inches=0)
             else:
                 plt.savefig("{} at {} mV.{}".format(imgName, int(
                     en), extension), bbox_inches='tight', pad_inches=0)
+
+
+def quick_plot(A, rspace=True, thres=3, fs=4, qscale=None, qlimit=1.2,  clims=None, cmap=None,
+                      saveon=False, imgName=None, extension='png', dpi=400, **kwargs):
+    
+    '''
+    Display 2D real space and FT images with a set of standard settings.
+    
+    Inputs:
+        A           - Required : 2D arrays of real space or FT image to dispaly
+        rspace      - Optional : bool, flag to indicate if A is a real space or FT image
+        thres       - Optional : float, number of sigma to control the color limit
+        fs          - Optional : float, figure size 
+        qscale      - Optional : float, specify the extent for the FT image
+        qlimit      - Optional : float, specify the range to plot for the FT image
+        clims       - Optional : list, specify the color limit for imshow. If not give, clims will be computed based on mean and std of A.
+        imgName     - Optional : String, default None. If not None image will be saved with the name imgName
+        kwargs      - Optional : key word arguments used in imshow()
+    Returns:
+        No return 
+
+    Usage:
+        import stmpy
+        import stmpy.driftcorr as dfc
+        dfc.quick_plot(d.z)
+        d.z_ft = stmpy.tools.fft(d.z, zeroDC=True)
+        dfc.quick_plot(d.z_ft, rspace=False)
+
+    History:
+        05/25/2023        RL : Initial commit.
+    '''
+    
+    plt.figure(figsize=[fs, fs])
+    c = np.mean(A)
+    s = np.std(A)
+    
+    # compute the color limit if clims is not given
+    if clims == None:
+        if rspace == True:
+            clims = [c-thres*s, c+thres*s]
+        else:
+            clims = [0, c+thres*s]
+    
+    # compute the FT image qscale if qscale is not given
+    if qscale == None:
+        extents = None
+    else:
+        extents = [-qscale, qscale, -qscale, qscale, ]
+        
+    # Use the default color maps if cmap is not set
+    if cmap == None:
+        cmap = stmpy.cm.blue2 if rspace else stmpy.cm.gray_r
+        
+    if rspace == True:
+        plt.imshow(A, clim=[c-thres*s, c+thres*s], cmap=cmap, **kwargs)
+        plt.gca().set_aspect(1)
+    else:
+        plt.imshow(A, extent=extents, clim=[0, c+thres*s], cmap=cmap, **kwargs)
+    plt.gca().axes.get_xaxis().set_visible(False)
+    plt.gca().axes.get_yaxis().set_visible(False)
+    plt.gca().set_frame_on(False)
+    
+    if imgName != None:
+        if extension == 'png':
+            plt.savefig("{}.{}".format(imgName, extension), dpi=dpi, bbox_inches='tight', pad_inches=0)
+        else:
+            plt.savefig("{}.{}".format(imgName, extension), bbox_inches='tight', pad_inches=0)
```

### Comparing `hoffmanstmpy-1.0.0/stmpy/hp/kondo_holes.py` & `hoffmanstmpy-1.0.1/stmpy/hp/kondo_holes.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/hp/tight_binding.py` & `hoffmanstmpy-1.0.1/stmpy/hp/tight_binding.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/image.py` & `hoffmanstmpy-1.0.1/stmpy/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         write_animation(data, fileName, saturation=2, clims=(0,1), cmap=None,
                     label=None, label_caption='meV', speed=8, zoom=1, **kwargs)
 
     History:
         2017-06-08  -   HP  : Added **kwargs sent to imshow
         2017-06-23  -   HP  : Added support for MP4 export and made codec
                               choice automatic.
+        2023-05-25  -   RL  : Added support for different color limit for different layers
     '''
     boxProperties = dict(boxstyle='square', facecolor='w', alpha=0.8, linewidth=0.0)
     textOptions = dict(fontsize=14, color='k', bbox=boxProperties, ha='right', va='center')
 
     if cmap is None:
         cmap = cm.bone_r
     fig = plt.figure(figsize=[4,4])
@@ -105,30 +106,36 @@
     im = plt.imshow(data[0], cmap=cmap, extent=[-1,1,-1,1], origin='lower',
                     **kwargs)
     ax.set_xlim(-1.0/zoom, 1.0/zoom)
     ax.set_ylim(-1.0/zoom, 1.0/zoom)
     if saturation is not None:
         saturate(saturation, im=im)
     else:
-        plt.clim(clims)
+        if len(np.shape(clims)) > 1:
+            plt.clim(clims[0])
+        else:
+            plt.clim(clims)
 
     if label is not None:
         tx = ax.text(0.95,0.95,'{:2.1f} {:}'.format(label[0], label_caption),
                   transform=ax.transAxes, **textOptions)
     def init():
         im.set_array(data[0])
         ax.text(20,200,'')
         return [im]
 
     def animate(i):
         im.set_array(data[i])
         if saturation is not None:
             saturate(saturation, im=im)
         else:
-            plt.clim(clims)
+            if len(np.shape(clims)) > 1:
+                plt.clim(clims[i])
+            else:
+                plt.clim(clims)
         if label is not None:
             tx.set_text('{:2.1f} {:}'.format(label[i], label_caption))
         return [im]
     fig.tight_layout()
     ani = FuncAnimation(fig, animate, init_func=init, frames=data.shape[0])
     if fileName.endswith('.mov'):
         ani.save(fileName, codec='prores', dpi=200, fps=speed)
```

### Comparing `hoffmanstmpy-1.0.0/stmpy/io.py` & `hoffmanstmpy-1.0.1/stmpy/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         2018-11-07  - HP : Add byte support to SPY files.
         2018-11-13  - HP : Add nice_units to .dat files
         2019-01-09  - BB : Generalize file extension extraction
         2019-02-28  - HP : Loads multisweep .dat files even if missing header.
         2020-07-12  - WT : Added support for sm4 file from rhk system.
         2022-06-22  - HP : Added support for Cornell files: .2FL .1FL .TFR .1FR
         2022-02-15  - HP : Added support for STM1 Cornell .FFL files
+        2023-05-18  - RL : Loads sxm scan files even if missing header.
 
     '''
     try:
         filename, extension = os.path.splitext(filePath)
         extension = extension.replace(".","")
     except IndexError:
         raise IOError('Please include file extension in path.')
@@ -631,15 +632,18 @@
             tagname = line[1:-1]
         else:
             if 'Z-CONTROLLER' == tagname:
                 keys = line.split('\t')
                 values = fileObj.readline().strip().decode('utf-8').split('\t')
                 self.header['z-controller'] = dict(zip(keys, values))
             elif tagname in ('BIAS', 'REC_TEMP', 'ACQ_TIME', 'SCAN_ANGLE'):
-                self.header[tagname.lower()] = float(line)
+                try:
+                    self.header[tagname.lower()] = float(line)
+                except ValueError:
+                    pass
             elif tagname in ('SCAN_PIXELS', 'SCAN_TIME', 'SCAN_RANGE', 'SCAN_OFFSET'):
                 self.header[tagname.lower()] = [ float(i) for i in re.split('\s+', line) ]
             elif 'DATA_INFO' == tagname:
                 if 1 == self.header['version']:
                     keys = re.split('\s\s+',line)
                 else:
                     keys = line.split('\t')
```

### Comparing `hoffmanstmpy-1.0.0/stmpy/mapviewer/gui_components.py` & `hoffmanstmpy-1.0.1/stmpy/mapviewer/gui_components.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/mapviewer/helptext.txt` & `hoffmanstmpy-1.0.1/stmpy/mapviewer/helptext.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/mapviewer/misc.py` & `hoffmanstmpy-1.0.1/stmpy/mapviewer/misc.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/mapviewer/view3ds.py` & `hoffmanstmpy-1.0.1/stmpy/mapviewer/view3ds.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/matio.py` & `hoffmanstmpy-1.0.1/stmpy/matio.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/read_STMView.py` & `hoffmanstmpy-1.0.1/stmpy/read_STMView.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/read_all.py` & `hoffmanstmpy-1.0.1/stmpy/read_all.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.0/stmpy/tools.py` & `hoffmanstmpy-1.0.1/stmpy/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,37 +507,40 @@
     G = np.array([x0, y0])
     K = np.array([a1, b1])
     M = np.array([(a1+a2)/2, (b1+b2)/2])
     hexagon = mpl.patches.Polygon(xy=[(a1, b1),(a2, b2),(a3, b3),(a4, b4),(a5, b5),(a6, b6)],\
                                   closed=True, fill=None, ec=ec, lw=lw)
     return G, M, K, hexagon
 
-def symmetrize(data, n, bp=(1.,1.), diag=False):
+def symmetrize(data, n, bp=(1.,1.), mirrorOnly=False, diag=False):
     '''
     Applies n-fold symmetrization to the image by rotating clockwise and
     anticlockwise by an angle 2pi/n, then applying a mirror line.  Works on 2D
     and 3D data sets, in the case of 3D each layer is symmetrzed.
     p is the location of one Bragg peak.
 
     Inputs:
         data    - Required : A 2D or 3D numpy array.
         n       - Required : Integer describing the degree of symmetrization.
         bp      - Optional : Pixel coordinates of the Bragg peak to define the
                              mirror line.
         diag    - Optional : Boolean to assert whether the mirror line is left
                              on the diagonal.
+        mirrorOnly - Optional : Boolean, if True only mirror symmetry along bp 
+                             direction is used
 
     Returns:
         dataSymm - A 2D or 3D numpy array containing symmetrized data.
 
     History:
         2017-05-04  - JG : Initial commit.
         2017-06-05  - HP : Modified default bp-value to be on diagonal.
         2017-08-15  - HP : Added flag to leave mirror line on the diagonal.
                            Code will not line mirror unsquare data.
+        2023-05-25  - RL : Add support for mirror only symmetrize 
      '''
     def sym2d(F, n):
         angle = 360.0/n
         out = np.zeros_like(F)
         for ix in range(n):
             out += snd.rotate(F, angle*ix, reshape=False)
             out += snd.rotate(F, -angle*ix, reshape=False)
@@ -558,19 +561,25 @@
             else:
                 Ffr = snd.rotate(Ff, alpha/np.pi*180, reshape=False) # rotate back
                 return (Ffr+F)/2.0
         else:
             return F
     p = np.array(bp, dtype=np.float64)
     if len(data.shape) is 2:
+        if mirrorOnly == False:
             return linmirr(sym2d(data, n), p[0], p[1])
+        else:
+            return linmirr(data, p[0], p[1])
     if len(data.shape) is 3:
         out = np.zeros_like(data)
         for ix, layer in enumerate(data):
-            out[ix] = linmirr(sym2d(layer, n), p[0], p[1])
+            if mirrorOnly == False:
+                out[ix] = linmirr(sym2d(layer, n), p[0], p[1])
+            else:
+                out[ix] = linmirr(layer, p[0], p[1])
         return out
     else:
         print('ERR: Input must be 2D or 3D numpy array.')
 
 
 def gauss2d(x, y, p, symmetric=False):
     '''Create a two dimensional Gaussian.
```

