# Comparing `tmp/minidevice-1.0.9.tar.gz` & `tmp/minidevice-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.0.9.tar", last modified: Sun Jun 11 11:12:54 2023, max compression
+gzip compressed data, was "minidevice-1.1.0.tar", last modified: Mon Jun 12 12:58:19 2023, max compression
```

## Comparing `minidevice-1.0.9.tar` & `minidevice-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 11:12:54.718341 minidevice-1.0.9/
--rw-rw-rw-   0        0        0   181499 2023-06-10 03:07:02.000000 minidevice-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     2838 2023-06-11 11:12:54.717303 minidevice-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2523 2023-06-10 15:30:42.000000 minidevice-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 11:12:54.701040 minidevice-1.0.9/minidevice/
--rw-rw-rw-   0        0        0      105 2023-06-11 09:46:25.000000 minidevice-1.0.9/minidevice/__init__.py
--rw-rw-rw-   0        0        0    13769 2023-06-10 04:44:53.000000 minidevice-1.0.9/minidevice/adb.py
--rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.9/minidevice/config.py
--rw-rw-rw-   0        0        0     5113 2023-06-11 09:20:04.000000 minidevice-1.0.9/minidevice/device.py
--rw-rw-rw-   0        0        0    18480 2023-06-11 11:12:30.000000 minidevice-1.0.9/minidevice/images.py
--rw-rw-rw-   0        0        0     2266 2023-06-07 14:54:13.000000 minidevice-1.0.9/minidevice/minicap.py
--rw-rw-rw-   0        0        0      666 2023-06-07 15:41:47.000000 minidevice-1.0.9/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      265 2023-06-09 14:39:12.000000 minidevice-1.0.9/minidevice/utils.py
--rw-rw-rw-   0        0        0     1673 2023-06-11 07:12:03.000000 minidevice-1.0.9/minidevice/win.py
-drwxrwxrwx   0        0        0        0 2023-06-11 11:12:54.716306 minidevice-1.0.9/minidevice.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 11:12:54.000000 minidevice-1.0.9/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 11:12:54.719338 minidevice-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-06-11 11:12:15.000000 minidevice-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:58:19.356788 minidevice-1.1.0/
+-rw-rw-rw-   0        0        0   181499 2023-06-10 03:07:02.000000 minidevice-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2838 2023-06-12 12:58:19.355792 minidevice-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2523 2023-06-10 15:30:42.000000 minidevice-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 12:58:19.347779 minidevice-1.1.0/minidevice/
+-rw-rw-rw-   0        0        0      141 2023-06-12 12:43:29.000000 minidevice-1.1.0/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    13767 2023-06-12 12:55:22.000000 minidevice-1.1.0/minidevice/adb.py
+-rw-rw-rw-   0        0        0     2360 2023-06-12 12:45:18.000000 minidevice-1.1.0/minidevice/capture.py
+-rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.1.0/minidevice/config.py
+-rw-rw-rw-   0        0        0     3176 2023-06-12 12:56:12.000000 minidevice-1.1.0/minidevice/device.py
+-rw-rw-rw-   0        0        0    19850 2023-06-12 12:44:40.000000 minidevice-1.1.0/minidevice/images.py
+-rw-rw-rw-   0        0        0     2291 2023-06-12 12:33:40.000000 minidevice-1.1.0/minidevice/minicap.py
+-rw-rw-rw-   0        0        0      666 2023-06-07 15:41:47.000000 minidevice-1.1.0/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0     1675 2023-06-12 12:44:55.000000 minidevice-1.1.0/minidevice/wincap.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:58:19.354793 minidevice-1.1.0/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:58:19.356788 minidevice-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      729 2023-06-12 12:57:15.000000 minidevice-1.1.0/setup.py
```

### Comparing `minidevice-1.0.9/LICENSE` & `minidevice-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.9/PKG-INFO` & `minidevice-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.9
+Version: 1.1.0
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-1.0.9/README.md` & `minidevice-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.9/minidevice/adb.py` & `minidevice-1.1.0/minidevice/adb.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     # 遍历输出列表中的每一行，跳过表头和空行
     for line in result[1:]:
         if line.strip() != "":
             # 分割每一行，获取设备序号并添加到列表中
             device_list.append(line.split("\t")[0])
     if len(device_list) == 0:
         print("没有连接的设备")
-        return None
+        return []
     return device_list
 
 def restart_adb():
     """
     restart_adb 重启adb
     """
     subprocess.run([ADB_PATH, "kill-server"])
```

### Comparing `minidevice-1.0.9/minidevice/images.py` & `minidevice-1.1.0/minidevice/images.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import math
-import time
+import urllib.request
+
 import cv2
 import numpy as np
-import urllib.request
 
-from .utils import raw2opencv
 
 class Colors():
     BLACK = "#FF000000"#黑色
     DKGRAY = "#FF444444"#深灰色
     GRAY = "#FF888888"#灰色
     LTGRAY = "#FFCCCCCC"#亮灰色
     WHITE ="#FFFFFFFF"#白色
@@ -238,14 +237,25 @@
     else:
         h = (r - g) / diff + 4
     h = h / 6
     s = 0 if maxVal == 0 else diff / maxVal
     return [h, s]
 
 
+def raw2opencv(raw):
+    """raw to opencv
+
+    Args:
+        raw (byte): raw
+
+    Returns:
+        mat: opencv格式图像
+    """
+    return cv2.imdecode(np.frombuffer(raw, dtype=np.uint8), cv2.IMREAD_COLOR)
+
 class Images():
     def read(path,flag=cv2.IMREAD_COLOR):
         """
         read 读取图像
 
         Args:
             path (str): 图像路径
@@ -281,23 +291,23 @@
         Args:
             img (mat): opencv格式图像
             title (str, optional): 显示的标题. Defaults to "".
         """
         cv2.imshow(title,img)
         cv2.waitKey()
 
-    def save(path,img):
+    def save(img,path="save.png"):
         """
         save 保存图像到路径
 
         Args:
             path (str): 路径
-            img (mat): opencv格式图像
+            img (mat): opencv格式图像 默认保存到当前路径下save.png
         """
-        cv2.imwrite(path,img)
+        cv2.imwrite(img,path)
     
     def pixel(img,x,y):
         """
         pixel 返回图片image在点(x, y)处的像素的RGB值。
 
         Args:
             img (Mat): opencv图像
@@ -389,25 +399,25 @@
                    Colors.parse_color(target_color),
                     Colors.parse_color(Images.pixel(img,x+x0,y+y0)),
                     threshold=threshold):
                     break
             return x0,y0
         return None
 
-    def find_image(img, template, threshold=0.8, region=None, level=3):
+    def find_image(img, template, threshold=0.8, region=None, level=3,debug=False):
         """
         find_image 模板匹配
 
         Args:
             img (mat): opencv格式图像
             template (mat): opencv格式图像
             threshold (float, optional): 匹配度. Defaults to 0.8.
             region (list, optional): 范围[]. Defaults to None. 像素数量与查找效率几乎成正比
             level (int, optional): 图像金字塔等级. Defaults to 3. 全屏1080x2400查找情况下level3效率是level2的5倍,是level1的10倍,分辨率越低提升越不明显
-
+            debug (bool,optional): 调试模式(方框绘制并显示) Defaults to False.
         Returns:
             max_loc: (x,y)
         """
         # 设置查找区域
         x_min, y_min, x_max, y_max = region or (0, 0, img.shape[1], img.shape[0])
         img = img[y_min:y_max, x_min:x_max]
 
@@ -426,79 +436,92 @@
             # 选择相似度最高的一个结果
             min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(res)
             if max_val > threshold:
                 # 转换坐标系
                 max_loc = (max_loc[0]*(2**i), max_loc[1]*(2**i))
                 if region is not None:
                     max_loc = (max_loc[0] + x_min, max_loc[1] + y_min)
+                if debug:
+                    copy = img_array[0].copy()
+                    cv2.rectangle(copy,[max_loc[0],max_loc[1],template_array[0].shape[1],template_array[0].shape[0]] , (0, 255, 0), 2)
+                    Images.save(copy)
                 return max_loc
         return None
     
-    def detect_and_compute_features(img, grayscale=True,method='SIFT',region=None):
+    def detect_and_compute_features(img, grayscale=True, method='SIFT', region=None, scale=1):
         """
         detect_and_compute_features 计算特征点和描述值
 
         Args:
             img (mat): opencv格式图像
             grayscale (bool, optional): 是否灰度化图像. Defaults to True.
             method (str, optional): 特征点计算方法. Defaults to 'SIFT'.
-            region (list, optional): 特征点计算范围[x_min, y_min, x_max, y_max ]. Defaults to None.
+            region (list, optional): 特征点计算范围[x_min, y_min, x_max, y_max]. Defaults to None.
+            scale (int, optional): 图像缩放. Defaults to '1'. 分辨率较大时,计算效率与这个成正比
 
         Raises:
             ValueError: "Invalid feature detection method"
 
         Returns:
-            keypoints:特征点
+            keypoints: 特征点
             descriptors: 描述值
         """
         # 转换为灰度图像
         if grayscale:
-            if len(img.shape)==3:
+            if len(img.shape) == 3:
                 img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+
         # 选择特征计算方法
         if method == 'SIFT':
             feature_detector = cv2.SIFT_create()
         elif method == 'ORB':
             feature_detector = cv2.ORB_create()
         else:
             raise ValueError("Invalid feature detection method")
+
         x_min, y_min, x_max, y_max = region or (0, 0, img.shape[1], img.shape[0])
         img = img[y_min:y_max, x_min:x_max]
+        img_new = cv2.resize(img,None,fx=scale,fy=scale)
+        keypoints = feature_detector.detect(img_new)
 
-        keypoints = feature_detector.detect(img)
+        # 调整关键点坐标
         for kp in keypoints:
-            kp.pt = (kp.pt[0]+x_min, kp.pt[1]+y_min)  # 调整关键点坐标
+            kp.pt = ((kp.pt[0])*(1/scale) , (kp.pt[1])*(1/scale))
 
         _, descriptors = feature_detector.compute(img, keypoints)
+        # img = cv2.drawKeypoints(img,keypoints,img)
+        # Images.save(f"{random.randint(8,100)}.png",img)
         # 返回特征信息
-        return keypoints,descriptors
+        return keypoints, descriptors
         
-    def match_features(template, target,region=None,threshold = 0.75,method="FLANNBASED"):
+    def match_features(img,template,region=None,threshold = 0.75,method="FLANNBASED",debug=False,scale=1):
         """
         match_features 特征匹配 
         (计算小图花费不了多少资源,重要的是计算大图特,所以请务必区域特征计算)
         由于orb效果不尽人意,只采用sift计算特征
-        计算2400x1080的大图消耗0.6s 500x1080的图消耗0.1s,但需注意的是不要过度裁切图片(会导致匹配失败)
+        计算2400x1080的大图消耗0.6s 500x1080的图消耗0.1s
 
         Args:
+            img (mat): opencv格式图像 大图
             template (mat): opencv格式图像 小图
-            target (mat): opencv格式图像 大图
             region (list, optional): 大图特征范围[x_min, y_min, x_max, y_max ]. Defaults to None.
             threshold (float, optional): 相似度. Defaults to 0.75.
             method (str, optional): 特征匹配算法. Defaults to "FLANNBASED".其他可选"BRUTEFORCE","BRUTEFORCE_L1"
+            debug (bool,optional): 调试模式(方框绘制并显示) Defaults to False.
+            scale (int, optional): 图像缩放. Defaults to '1'. 分辨率较大时,计算效率与这个成正比
 
         Raises:
             ValueError: 算法不存在
 
         Returns:
             list: 小图在大图中的范围[x, y, w, h ]
         """
         # 计算关键点和描述符
-        kp_template, des_template = Images.detect_and_compute_features(template)
-        kp_target, des_target = Images.detect_and_compute_features(target,region=region)
+        kp_template, des_template = Images.detect_and_compute_features(template,scale=scale)
+        kp_target, des_target = Images.detect_and_compute_features(img,region=region,scale=scale)
 
         if method == "FLANNBASED":
             matcher = cv2.FlannBasedMatcher()
         elif method == "BRUTEFORCE_L1":
             matcher = cv2.BFMatcher(cv2.NORM_L1)
         elif method == "BRUTEFORCE":
             matcher = cv2.BFMatcher(cv2.NORM_L2)
@@ -521,23 +544,27 @@
             # 计算单应性矩阵
             M, mask = cv2.findHomography(src_pts, dst_pts, cv2.RANSAC, 5.0)
 
             # 将模板图像的角点映射到目标图像中的相应位置
             h, w = template.shape[:2]
             pts = np.float32([[0, 0], [0, h - 1], [w - 1, h - 1], [w - 1, 0]]).reshape(-1, 1, 2)
             dst = cv2.perspectiveTransform(pts, M)
+
+            x_min, y_min, x_max, y_max = region or (0, 0, img.shape[1], img.shape[0])
             # 计算矩形区域坐标
             x, y, w, h = cv2.boundingRect(dst)
-
-            return [x, y, w, h]
+            if debug:
+                    copy = img.copy()
+                    cv2.rectangle(copy,[x+x_min,y+y_min,w,h] , (0, 255, 0), 2)
+                    Images.save(copy)
+            return [x+x_min,y+y_min, w, h]
 
         else:
-            print("Not enough matches are found - %d/%d" % (len(good_matches), 10))
+            print("Not enough matches are found - {}/{}".format(len(good_matches), 10))
             return None
 
 
 
 
 
 if __name__=="__main__":
-
-    pass
+    pass
```

### Comparing `minidevice-1.0.9/minidevice/minicap.py` & `minidevice-1.1.0/minidevice/minicap.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,34 +6,34 @@
     if sdk >= 24:
         line_breaker = LINESEQ
     else:
         line_breaker = '\r' + LINESEQ
     return line_breaker.encode("ascii")
 
 
-def minicap_screen(device, sdk, vm_size):
+def minicap_screen(device, sdk, vm_size,quality=100):
     """minicap 0.15~0.25s
     """
     raw_data = subprocess.check_output([ADB_PATH, "-s", device, "shell",
                                         "LD_LIBRARY_PATH=/data/local/tmp",
-                                        "/data/local/tmp/minicap", "-P", f"{vm_size}@{vm_size}/0", "-s"],
+                                        "/data/local/tmp/minicap", "-P", f"{vm_size}@{vm_size}/0","-Q",str(quality),"-s"],
                                        stderr=subprocess.DEVNULL)
     jpg_data = raw_data.split(b"for JPG encoder\n"+line_breaker(sdk))[-1]
     jpg_data = jpg_data.replace(line_breaker(sdk), b"\n")
     return jpg_data
 
 
 def minicap_install(device, sdk, abi):
     """minicap
 
     Args:
         device (_type_): _description_
     """
     #在x86_64上运行32位minicap可正常运行
-    if sdk >= 31 and abi == "x86_64":
+    if sdk == 32 and abi == "x86_64":
         abi = "x86"
 
 
     MNC_HOME = "/data/local/tmp/minicap"
     MNC_SO_HOME = "/data/local/tmp/minicap.so"
 
     subprocess.run([
@@ -66,9 +66,7 @@
                                           "LD_LIBRARY_PATH=/data/local/tmp",
                                           "/data/local/tmp/minicap", "-P", f"{vm_size}@{vm_size}/0", "-t"], stderr=subprocess.DEVNULL)
         if "OK" in result.decode('utf-8'):
             return True
         return False
     except subprocess.CalledProcessError:
         return False
-
-
```

### Comparing `minidevice-1.0.9/minidevice/minitouch.py` & `minidevice-1.1.0/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.9/minidevice/win.py` & `minidevice-1.1.0/minidevice/wincap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #ocr文字识别
-from ctypes import windll, byref, c_ubyte
-from ctypes.wintypes import RECT, HWND
+from ctypes import byref, c_ubyte, windll
+from ctypes.wintypes import HWND, RECT
+
 import numpy as np
 
 GetDC = windll.user32.GetDC
 CreateCompatibleDC = windll.gdi32.CreateCompatibleDC
 GetClientRect = windll.user32.GetClientRect
 CreateCompatibleBitmap = windll.gdi32.CreateCompatibleBitmap
 SelectObject = windll.gdi32.SelectObject
```

### Comparing `minidevice-1.0.9/minidevice.egg-info/PKG-INFO` & `minidevice-1.1.0/minidevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.9
+Version: 1.1.0
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-1.0.9/setup.py` & `minidevice-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='1.0.9',
+      version='1.1.0',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

