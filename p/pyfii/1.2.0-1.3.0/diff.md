# Comparing `tmp/pyfii-1.2.0.tar.gz` & `tmp/pyfii-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfii-1.2.0.tar", last modified: Mon Jun 12 15:13:12 2023, max compression
+gzip compressed data, was "pyfii-1.3.0.tar", last modified: Mon Jun 12 15:34:51 2023, max compression
```

## Comparing `pyfii-1.2.0.tar` & `pyfii-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.898677 pyfii-1.2.0/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    35149 2023-06-09 19:42:27.000000 pyfii-1.2.0/LICENSE
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2127 2023-06-12 15:13:12.897819 pyfii-1.2.0/PKG-INFO
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1578 2023-06-12 14:42:00.000000 pyfii-1.2.0/README.md
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)      687 2023-06-12 15:12:52.000000 pyfii-1.2.0/pyproject.toml
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)       38 2023-06-12 15:13:12.898963 pyfii-1.2.0/setup.cfg
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.858571 pyfii-1.2.0/src/
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.875986 pyfii-1.2.0/src/pyfii/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)      132 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/__init__.py
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.895746 pyfii-1.2.0/src/pyfii/cv3d/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     5441 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/cv3d/IIID.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3978 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/cv3d/IIID2.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1426 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/cv3d/transfer.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16682 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/drone.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3190 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/fii.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16559 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/read.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    21818 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/show.py
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.885609 pyfii-1.2.0/src/pyfii.egg-info/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2127 2023-06-12 15:13:12.000000 pyfii-1.2.0/src/pyfii.egg-info/PKG-INFO
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)      332 2023-06-12 15:13:12.000000 pyfii-1.2.0/src/pyfii.egg-info/SOURCES.txt
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)        1 2023-06-12 15:13:12.000000 pyfii-1.2.0/src/pyfii.egg-info/dependency_links.txt
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)        6 2023-06-12 15:13:12.000000 pyfii-1.2.0/src/pyfii.egg-info/top_level.txt
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:34:51.204299 pyfii-1.3.0/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    35149 2023-06-09 19:42:27.000000 pyfii-1.3.0/LICENSE
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2127 2023-06-12 15:34:51.203242 pyfii-1.3.0/PKG-INFO
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1578 2023-06-12 14:42:00.000000 pyfii-1.3.0/README.md
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      687 2023-06-12 15:34:31.000000 pyfii-1.3.0/pyproject.toml
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)       38 2023-06-12 15:34:51.204692 pyfii-1.3.0/setup.cfg
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:34:51.165972 pyfii-1.3.0/src/
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:34:51.187604 pyfii-1.3.0/src/pyfii/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      152 2023-06-12 15:21:41.000000 pyfii-1.3.0/src/pyfii/__init__.py
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:34:51.201517 pyfii-1.3.0/src/pyfii/cv3d/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     5441 2023-06-09 19:42:27.000000 pyfii-1.3.0/src/pyfii/cv3d/IIID.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3978 2023-06-09 19:42:27.000000 pyfii-1.3.0/src/pyfii/cv3d/IIID2.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:32:24.000000 pyfii-1.3.0/src/pyfii/cv3d/__init__.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1426 2023-06-09 19:42:27.000000 pyfii-1.3.0/src/pyfii/cv3d/transfer.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16682 2023-06-09 19:42:27.000000 pyfii-1.3.0/src/pyfii/drone.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3190 2023-06-09 19:42:27.000000 pyfii-1.3.0/src/pyfii/fii.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16559 2023-06-09 19:42:27.000000 pyfii-1.3.0/src/pyfii/read.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    21817 2023-06-12 15:24:40.000000 pyfii-1.3.0/src/pyfii/show.py
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:34:51.194730 pyfii-1.3.0/src/pyfii.egg-info/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2127 2023-06-12 15:34:51.000000 pyfii-1.3.0/src/pyfii.egg-info/PKG-INFO
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      359 2023-06-12 15:34:51.000000 pyfii-1.3.0/src/pyfii.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)        1 2023-06-12 15:34:51.000000 pyfii-1.3.0/src/pyfii.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)        6 2023-06-12 15:34:51.000000 pyfii-1.3.0/src/pyfii.egg-info/top_level.txt
```

### Comparing `pyfii-1.2.0/LICENSE` & `pyfii-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfii-1.2.0/PKG-INFO` & `pyfii-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfii
-Version: 1.2.0
+Version: 1.3.0
 Summary: 这个库可以让我们用python写Fii的无人机程序，有三视图模拟飞行的功能，模拟飞行更方便观看
 Author-email: Kevin0412 <kevin0412_xlt@qq.com>
 Project-URL: Homepage, https://github.com/Kevin0412/pyfii
 Project-URL: Bug Tracker, https://github.com/Kevin0412/pyfii/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyfii-1.2.0/README.md` & `pyfii-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfii-1.2.0/pyproject.toml` & `pyfii-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyfii"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
   { name="Kevin0412", email="kevin0412_xlt@qq.com" },
 ]
 description = "这个库可以让我们用python写Fii的无人机程序，有三视图模拟飞行的功能，模拟飞行更方便观看"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyfii-1.2.0/src/pyfii/cv3d/IIID.py` & `pyfii-1.3.0/src/pyfii/cv3d/IIID.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.2.0/src/pyfii/cv3d/IIID2.py` & `pyfii-1.3.0/src/pyfii/cv3d/IIID2.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.2.0/src/pyfii/cv3d/transfer.py` & `pyfii-1.3.0/src/pyfii/cv3d/transfer.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.2.0/src/pyfii/drone.py` & `pyfii-1.3.0/src/pyfii/drone.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.2.0/src/pyfii/fii.py` & `pyfii-1.3.0/src/pyfii/fii.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.2.0/src/pyfii/read.py` & `pyfii-1.3.0/src/pyfii/read.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.2.0/src/pyfii/show.py` & `pyfii-1.3.0/src/pyfii/show.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import warnings
 
 import cv2
 import numpy as np
 import pygame
 from ffmpy import FFmpeg
 
-from .cv3d import IIID,IIID2
+from cv3d import IIID,IIID2
 
 # 视频添加音频
 def video_add_audio(video_path: str, audio_path: str,output_path:str):
     _ext_video = os.path.basename(video_path).strip().split('.')[-1]
     _ext_audio = os.path.basename(audio_path).strip().split('.')[-1]
     if _ext_audio not in ['mp3', 'wav']:
         raise Exception('audio format not support')
```

### Comparing `pyfii-1.2.0/src/pyfii.egg-info/PKG-INFO` & `pyfii-1.3.0/src/pyfii.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfii
-Version: 1.2.0
+Version: 1.3.0
 Summary: 这个库可以让我们用python写Fii的无人机程序，有三视图模拟飞行的功能，模拟飞行更方便观看
 Author-email: Kevin0412 <kevin0412_xlt@qq.com>
 Project-URL: Homepage, https://github.com/Kevin0412/pyfii
 Project-URL: Bug Tracker, https://github.com/Kevin0412/pyfii/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

