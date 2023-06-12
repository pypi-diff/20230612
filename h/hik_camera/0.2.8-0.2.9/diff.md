# Comparing `tmp/hik_camera-0.2.8.tar.gz` & `tmp/hik_camera-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hik_camera-0.2.8.tar", last modified: Sat Apr  2 06:03:48 2022, max compression
+gzip compressed data, was "dist/hik_camera-0.2.9.tar", last modified: Tue Apr 19 10:30:24 2022, max compression
```

## Comparing `hik_camera-0.2.8.tar` & `hik_camera-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2022-04-02 06:03:48.000000 hik_camera-0.2.8/
--rw-rw-r--   0 dl        (1000) dl        (1000)       65 2021-09-10 10:03:06.000000 hik_camera-0.2.8/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      678 2022-04-02 06:03:48.000000 hik_camera-0.2.8/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)     1071 2022-01-05 12:15:32.000000 hik_camera-0.2.8/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2022-04-02 06:03:48.000000 hik_camera-0.2.8/hik_camera/
--rw-r--r--   0 dl        (1000) dl        (1000)    19410 2021-05-06 05:57:01.000000 hik_camera-0.2.8/hik_camera/MvCameraNode-CH.csv
--rw-rw-r--   0 dl        (1000) dl        (1000)      221 2022-04-02 05:51:44.000000 hik_camera-0.2.8/hik_camera/__info__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)       93 2021-05-06 05:57:01.000000 hik_camera-0.2.8/hik_camera/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     5704 2021-05-06 05:57:01.000000 hik_camera-0.2.8/hik_camera/bandwidth.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    17463 2022-04-02 05:51:33.000000 hik_camera-0.2.8/hik_camera/hik_camera.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     2121 2022-01-27 13:20:26.000000 hik_camera-0.2.8/hik_camera/tmp_windows_debug.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2022-04-02 06:03:48.000000 hik_camera-0.2.8/hik_camera.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      678 2022-04-02 06:03:48.000000 hik_camera-0.2.8/hik_camera.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      449 2022-04-02 06:03:48.000000 hik_camera-0.2.8/hik_camera.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2022-04-02 06:03:48.000000 hik_camera-0.2.8/hik_camera.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       25 2022-04-02 06:03:48.000000 hik_camera-0.2.8/hik_camera.egg-info/requires.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       11 2022-04-02 06:03:48.000000 hik_camera-0.2.8/hik_camera.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       25 2022-01-10 13:37:08.000000 hik_camera-0.2.8/requirements.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2022-04-02 06:03:48.000000 hik_camera-0.2.8/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)     1004 2021-09-10 10:10:02.000000 hik_camera-0.2.8/setup.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2022-04-02 06:03:48.000000 hik_camera-0.2.8/test/
--rw-rw-r--   0 dl        (1000) dl        (1000)      142 2022-01-05 08:23:05.000000 hik_camera-0.2.8/test/test_base.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      673 2022-01-05 12:12:01.000000 hik_camera-0.2.8/test/test_continuous_adjust_exposure.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      662 2022-01-05 12:17:32.000000 hik_camera-0.2.8/test/test_raw.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2022-04-19 10:30:24.000000 hik_camera-0.2.9/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       65 2021-09-10 10:03:06.000000 hik_camera-0.2.9/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      678 2022-04-19 10:30:24.000000 hik_camera-0.2.9/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1071 2022-01-05 12:15:32.000000 hik_camera-0.2.9/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2022-04-19 10:30:24.000000 hik_camera-0.2.9/hik_camera/
+-rw-r--r--   0 dl        (1000) dl        (1000)    19410 2021-05-06 05:57:01.000000 hik_camera-0.2.9/hik_camera/MvCameraNode-CH.csv
+-rw-rw-r--   0 dl        (1000) dl        (1000)      221 2022-04-19 10:30:07.000000 hik_camera-0.2.9/hik_camera/__info__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)       93 2021-05-06 05:57:01.000000 hik_camera-0.2.9/hik_camera/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5704 2021-05-06 05:57:01.000000 hik_camera-0.2.9/hik_camera/bandwidth.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      184 2022-04-19 10:26:34.000000 hik_camera-0.2.9/hik_camera/get_all_ips.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    17665 2022-04-19 10:25:50.000000 hik_camera-0.2.9/hik_camera/hik_camera.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     2121 2022-01-27 13:20:26.000000 hik_camera-0.2.9/hik_camera/tmp_windows_debug.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2022-04-19 10:30:24.000000 hik_camera-0.2.9/hik_camera.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      678 2022-04-19 10:30:24.000000 hik_camera-0.2.9/hik_camera.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      475 2022-04-19 10:30:24.000000 hik_camera-0.2.9/hik_camera.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2022-04-19 10:30:24.000000 hik_camera-0.2.9/hik_camera.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       25 2022-04-19 10:30:24.000000 hik_camera-0.2.9/hik_camera.egg-info/requires.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       11 2022-04-19 10:30:24.000000 hik_camera-0.2.9/hik_camera.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       25 2022-01-10 13:37:08.000000 hik_camera-0.2.9/requirements.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2022-04-19 10:30:24.000000 hik_camera-0.2.9/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1004 2021-09-10 10:10:02.000000 hik_camera-0.2.9/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2022-04-19 10:30:24.000000 hik_camera-0.2.9/test/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      142 2022-01-05 08:23:05.000000 hik_camera-0.2.9/test/test_base.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      673 2022-01-05 12:12:01.000000 hik_camera-0.2.9/test/test_continuous_adjust_exposure.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      662 2022-01-05 12:17:32.000000 hik_camera-0.2.9/test/test_raw.py
```

### Comparing `hik_camera-0.2.8/PKG-INFO` & `hik_camera-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hik_camera
-Version: 0.2.8
+Version: 0.2.9
 Summary: Provides an easy-to-use API to control Hik industrial cameras. (supports Linux/Docker/Windows)
 Home-page: UNKNOWN
 Author: Lei Yang
 Author-email: 
 License: UNKNOWN
 Description: Provides an easy-to-use API to control Hik industrial cameras. (supports Linux/Docker/Windows)
 Platform: UNKNOWN
```

### Comparing `hik_camera-0.2.8/README.md` & `hik_camera-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `hik_camera-0.2.8/hik_camera/MvCameraNode-CH.csv` & `hik_camera-0.2.9/hik_camera/MvCameraNode-CH.csv`

 * *Files identical despite different names*

### Comparing `hik_camera-0.2.8/hik_camera/bandwidth.py` & `hik_camera-0.2.9/hik_camera/bandwidth.py`

 * *Files identical despite different names*

### Comparing `hik_camera-0.2.8/hik_camera/hik_camera.py` & `hik_camera-0.2.9/hik_camera/hik_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import boxx
 from boxx import *
 
 import os
+import sys
 import time
 import ctypes
 import numpy as np
 from threading import Lock, Thread
 from ctypes import byref, POINTER, cast, sizeof, memset
 
 with boxx.impt("/opt/MVS/Samples/64/Python/MvImport"), boxx.impt(
@@ -68,16 +69,16 @@
         self._ip = ip
         self.host_ip = host_ip
         self._init()
         self.is_open = False
         self.last_time_get_frame = 0
 
     def _init(self):
-        # self._init_by_spec_ip()
-        self._init_by_enum()
+        self._init_by_spec_ip()
+        # self._init_by_enum()
 
     def setting(self):
         # self.setitem("GevSCPD", 200)  # 包延时, 单位 ns, 防止丢包, 6 个百万像素相机推荐 15000
         # self.set_OptimalPacketSize()  # 最优包大小
 
         self.set_rgb()  # 取 RGB 图
         # self.set_raw() # 取 raw 图
@@ -160,16 +161,18 @@
         while not self._ping():
             boxx.sleep(0.1)
             if time.time() - begin > timeout:
                 raise TimeoutError(f"Lost connection to {self.ip} for {timeout}s!")
 
     @classmethod
     def get_all_ips(cls):
-        ip_to_dev_info = cls._get_dev_info()
-        return sorted(ip_to_dev_info)
+        # 通过新的线程, 绕过 hik sdk 枚举后无法 "无枚举连接相机"(使用 ip 直连)的 bug
+        get_all_ips_py = boxx.relfile("./get_all_ips.py")
+        ips = boxx.execmd(f'"{sys.executable}" "{get_all_ips_py}"').strip().split(" ")
+        return ips
 
     @classmethod
     def get_cams(cls, ips=None):
         if ips is None:
             ips = cls.get_all_ips()
         else:
             ips = sorted(ips)
```

### Comparing `hik_camera-0.2.8/hik_camera/tmp_windows_debug.py` & `hik_camera-0.2.9/hik_camera/tmp_windows_debug.py`

 * *Files identical despite different names*

### Comparing `hik_camera-0.2.8/hik_camera.egg-info/PKG-INFO` & `hik_camera-0.2.9/hik_camera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hik-camera
-Version: 0.2.8
+Version: 0.2.9
 Summary: Provides an easy-to-use API to control Hik industrial cameras. (supports Linux/Docker/Windows)
 Home-page: UNKNOWN
 Author: Lei Yang
 Author-email: 
 License: UNKNOWN
 Description: Provides an easy-to-use API to control Hik industrial cameras. (supports Linux/Docker/Windows)
 Platform: UNKNOWN
```

### Comparing `hik_camera-0.2.8/setup.py` & `hik_camera-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `hik_camera-0.2.8/test/test_continuous_adjust_exposure.py` & `hik_camera-0.2.9/test/test_continuous_adjust_exposure.py`

 * *Files identical despite different names*

### Comparing `hik_camera-0.2.8/test/test_raw.py` & `hik_camera-0.2.9/test/test_raw.py`

 * *Files identical despite different names*

