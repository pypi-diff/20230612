# Comparing `tmp/baseImage-2.1.3.tar.gz` & `tmp/baseImage-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseImage-2.1.3.tar", last modified: Mon Sep 12 10:24:55 2022, max compression
+gzip compressed data, was "baseImage-2.1.4.tar", last modified: Mon Jun 12 06:08:52 2023, max compression
```

## Comparing `baseImage-2.1.3.tar` & `baseImage-2.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 10:24:55.871328 baseImage-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-12 10:24:43.000000 baseImage-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-12 10:24:43.000000 baseImage-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8798 2022-09-12 10:24:55.871328 baseImage-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8093 2022-09-12 10:24:43.000000 baseImage-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 10:24:55.867328 baseImage-2.1.3/baseImage/
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28204 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/base_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3864 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/base_image.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/constant.py
--rw-r--r--   0 runner    (1001) docker     (121)    12782 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 10:24:55.871328 baseImage-2.1.3/baseImage/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/utils/api.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 10:24:55.871328 baseImage-2.1.3/baseImage/utils/image_diff/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/utils/image_diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3464 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/utils/image_diff/ssim_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 10:24:55.871328 baseImage-2.1.3/baseImage/utils/ssim/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/utils/ssim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4690 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/utils/ssim/paddle.py
--rw-r--r--   0 runner    (1001) docker     (121)     7762 2022-09-12 10:24:43.000000 baseImage-2.1.3/baseImage/utils/ssim/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 10:24:55.871328 baseImage-2.1.3/baseImage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8798 2022-09-12 10:24:55.000000 baseImage-2.1.3/baseImage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-09-12 10:24:55.000000 baseImage-2.1.3/baseImage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 10:24:55.000000 baseImage-2.1.3/baseImage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-12 10:24:55.000000 baseImage-2.1.3/baseImage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-12 10:24:55.000000 baseImage-2.1.3/baseImage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-12 10:24:43.000000 baseImage-2.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-12 10:24:55.871328 baseImage-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-09-12 10:24:43.000000 baseImage-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 10:24:55.871328 baseImage-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-12 10:24:43.000000 baseImage-2.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-09-12 10:24:43.000000 baseImage-2.1.3/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:08:52.212783 baseImage-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 06:08:42.000000 baseImage-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-12 06:08:42.000000 baseImage-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-12 06:08:52.212783 baseImage-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-06-12 06:08:42.000000 baseImage-2.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:08:52.204783 baseImage-2.1.4/baseImage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31520 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/base_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/base_image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12782 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:08:52.208783 baseImage-2.1.4/baseImage/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/utils/api.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:08:52.208783 baseImage-2.1.4/baseImage/utils/image_diff/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/utils/image_diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/utils/image_diff/ssim_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:08:52.208783 baseImage-2.1.4/baseImage/utils/ssim/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/utils/ssim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/utils/ssim/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-12 06:08:42.000000 baseImage-2.1.4/baseImage/utils/ssim/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:08:52.208783 baseImage-2.1.4/baseImage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-12 06:08:52.000000 baseImage-2.1.4/baseImage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-12 06:08:52.000000 baseImage-2.1.4/baseImage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 06:08:52.000000 baseImage-2.1.4/baseImage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 06:08:52.000000 baseImage-2.1.4/baseImage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 06:08:52.000000 baseImage-2.1.4/baseImage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 06:08:42.000000 baseImage-2.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 06:08:52.212783 baseImage-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-12 06:08:42.000000 baseImage-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:08:52.212783 baseImage-2.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 06:08:42.000000 baseImage-2.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-12 06:08:42.000000 baseImage-2.1.4/tests/test_all.py
```

### Comparing `baseImage-2.1.3/LICENSE` & `baseImage-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `baseImage-2.1.3/PKG-INFO` & `baseImage-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: baseImage
-Version: 2.1.3
+Version: 2.1.4
 Summary: This is a secondary package of OpenCV,for manage image data
 Home-page: https://github.com/hakaboom/base_image
 Author: hakaboom
 Author-email: 1534225986@qq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6, <=3.10
+Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # base_image
 对opencv_python常用接口的二次开发
 
 建议 opencv version >= 4.5.5(不同opencv版本的python绑定,函数名可能会不同)
```

### Comparing `baseImage-2.1.3/README.md` & `baseImage-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `baseImage-2.1.3/baseImage/base_image.py` & `baseImage-2.1.4/baseImage/base_image.py`

 * *Files 21% similar despite different names*

```diff
@@ -766,14 +766,21 @@
             raise TypeError("Unknown place:'{}', image_data={}, image_data_type".format(self.place, self.data, type(self.data)))
         return data
 
     def calcHist(self, histSize, ranges, mask=None, accumulate=False, stream=None):
         """
         计算图像颜色直方图
 
+        Args:
+            histSize: 直方图每一个维度划分的柱条的数目
+            ranges: 取值区间
+            mask: 掩模
+            accumulate: 在多个图像时，是否累积计算像素值的个数
+            stream: cuda流
+
         Returns:
             各通道的直方图数组
         """
         hists = []
         data = self.data
 
         if self.place == Place.GpuMat:
@@ -784,7 +791,99 @@
             # stream = stream or self._stream
             # data = self.split(stream)
             # dst = [self._create_gpu_mat((1, 256), dtype=cv2.CV_32SC1) for i in range(self.channels)]
             # for i in range(self.channels):
             #     hists.append(cv2.cuda.calcHist(data[i], hist=dst[i], stream=stream))
             # [np.rot90(i.download(), 3) for i in hists]
         return hists
+
+    def inRange(self, lowerb, upperb, stream=None):
+        """
+        检查数组元素是否位于两个标量之间
+
+        Args:
+            lowerb: 下边界
+            upperb: 上边界
+            stream: cuda流
+
+        Returns:
+            二值化后的数组
+        """
+        if self.place in (Place.Ndarray, Place.UMat):
+            data = cv2.inRange(self.data, lowerb, upperb)
+        elif self.place == Place.GpuMat:
+            stream = stream or self._stream
+            dst = self._create_gpu_mat(data=self.data, dtype=cv2.CV_8UC1)
+            data = cv2.cuda.inRange(self.data, lowerb, upperb, dst=dst, stream=stream)
+        else:
+            raise TypeError("Unknown place:'{}', image_data={}, image_data_type".format(self.place, self.data, type(self.data)))
+
+        return self._clone_with_params(data, clone=False)
+
+    def multiply(self, src2, scale=1, dtype=-1, stream=None):
+        """
+        计算两个数组的每个元素缩放乘积
+
+        Args:
+            src2:
+            scale: 比例
+            dtype: 数组深度
+            stream: cuda流
+
+        Returns:
+            计算后的数组
+        """
+        if isinstance(src2, Image):
+            src2 = src2.data
+
+        if self.place in (Place.Ndarray, Place.UMat):
+            data = cv2.multiply(self.data, src2=src2, scale=scale, dtype=dtype)
+        elif self.place == Place.GpuMat:
+            stream = stream or self._stream
+            dst = self._create_gpu_mat(data=self.data, dtype=self.cv_dtype)
+            data = cv2.cuda.multiply(self.data, src2=src2, dst=dst, scale=scale, dtype=dtype, stream=stream)
+        else:
+            raise TypeError("Unknown place:'{}', image_data={}, image_data_type".format(self.place, self.data, type(self.data)))
+
+        return self._clone_with_params(data, clone=False)
+
+    def sqrt(self, stream=None):
+        """
+        开平方
+
+        Args:
+            stream: cuda流
+
+        Returns:
+            计算后的数组
+        """
+        if self.place in (Place.Ndarray, Place.UMat):
+            data = cv2.sqrt(self.data)
+        elif self.place == Place.GpuMat:
+            stream = stream or self._stream
+            dst = self._create_gpu_mat(data=self.data, dtype=self.cv_dtype)
+            data = cv2.cuda.sqrt(self.data, dst=dst, stream=stream)
+        else:
+            raise TypeError("Unknown place:'{}', image_data={}, image_data_type".format(self.place, self.data, type(self.data)))
+
+        return self._clone_with_params(data, clone=False)
+
+    def mean(self, mask=None):
+        """
+        计算数组平均数
+
+        Args:
+            mask: 掩码
+
+        Returns:
+            数组平均数
+        """
+        if self.place == Place.GpuMat:
+            data = self.data.download()
+        elif self.place in (Place.Ndarray, Place.UMat):
+            data = self.data
+        else:
+            raise TypeError("Unknown place:'{}', image_data={}, image_data_type".format(self.place, self.data, type(self.data)))
+
+        ret = cv2.mean(data, mask=mask)
+        return ret
+
```

### Comparing `baseImage-2.1.3/baseImage/base_image.pyi` & `baseImage-2.1.4/baseImage/base_image.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -105,8 +105,16 @@
 
     def imshow(self, title: str = None, flags: int = cv2.WINDOW_KEEPRATIO) -> None: ...
 
     def imwrite(self, fileName: str) -> None: ...
 
     def split(self, stream: Stream = None) -> Tuple[Union[np.ndarray, cv2.cuda.GpuMat, cv2.UMat], ...]: ...
 
-    def calcHist(self, histSize: List[int, ...], ranges: Union[Tuple[int, ...], List[int, ...]], mask=None, accumulate: bool = False, stream: Stream = None) -> List[npt.NDArray[np.float32], ...]: ...
+    def calcHist(self, histSize: List[int, ...], ranges: Union[Tuple[int, ...], List[int, ...]], mask=None, accumulate: bool = False, stream: Stream = None) -> List[npt.NDArray[np.float32], ...]: ...
+
+    def inRange(self, lowerb: Union[Tuple[int, ...], List[int, ...]], upperb: Union[Tuple[int, ...], List[int, ...]], stream=None) -> Image: ...
+
+    def multiply(self, src: Union[Image, Tuple[Union[int, float], ...], float, int], scale: Union[int, float] = 1, dtype: int = -1, stream: Stream = None) -> Image: ...
+
+    def sqrt(self, stream: Stream = None) -> Image: ...
+
+    def mean(self, mask: ImageType) -> Union[float, int]: ...
```

### Comparing `baseImage-2.1.3/baseImage/constant.py` & `baseImage-2.1.4/baseImage/constant.py`

 * *Files identical despite different names*

### Comparing `baseImage-2.1.3/baseImage/coordinate.py` & `baseImage-2.1.4/baseImage/coordinate.py`

 * *Files identical despite different names*

### Comparing `baseImage-2.1.3/baseImage/exceptions.py` & `baseImage-2.1.4/baseImage/exceptions.py`

 * *Files identical despite different names*

### Comparing `baseImage-2.1.3/baseImage/utils/api.py` & `baseImage-2.1.4/baseImage/utils/api.py`

 * *Files identical despite different names*

### Comparing `baseImage-2.1.3/baseImage/utils/image_diff/ssim_diff.py` & `baseImage-2.1.4/baseImage/utils/image_diff/ssim_diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,27 @@
         self.ssim = SSIM(resize=resize)
 
     @classmethod
     def _image_check(cls, im1, im2):
         if im1.place != im2.place:
             im2 = Image(im2, place=im1.place, dtype=np.float32)
 
-        if im1.dtype != np.float32:
-            im1 = Image(im1, place=im1.place, dtype=np.float32)
+        if im1.dtype != np.float64:
+            im1 = Image(im1, place=im1.place, dtype=np.float64)
 
-        if im2.dtype != np.float32:
-            im2 = Image(im2, place=im2.place, dtype=np.float32)
+        if im2.dtype != np.float64:
+            im2 = Image(im2, place=im2.place, dtype=np.float64)
 
         return im1, im2
 
     def diff(self, im1: Image, im2: Image):
-        im1, im2 = self._image_check(im1, im2)
+        # im1, im2 = self._image_check(im1, im2)
         return self._diff(im1, im2)
 
-    def _diff(self, im1: Image, im2: Image, threshold: float = 0.95):
+    def _diff(self, im1: Image, im2: Image, threshold: float = 0.70):
         """
         ssim对比,并找到差异区域
 
         Args:
             im1: 对比图片1
             im2: 对比图片2
             threshold: 允许的阈值,用于二值化时过滤部分像素,计算公式:thresh=int(255 * (1-threshold))
@@ -47,19 +47,18 @@
         if score.channels == 3:
             gary = score.cvtColor(cv2.COLOR_BGR2GRAY)
         else:
             gary = score
 
         # 反色
         gary = gary.bitwise_not()
-        # Image(gary).imshow('gary')
 
         # 二值化
         thresh = gary.threshold(code=cv2.THRESH_BINARY, thresh=int(255 * (1 - threshold)), maxval=255)
-
+        # thresh.imshow('thresh')
         # 闭运算
         kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (9, 9))
         erosion = cv2.morphologyEx(thresh.data, cv2.MORPH_CLOSE, kernel)
         Image(erosion).imshow('erosion')
         # 寻找轮廓
         cnts, hierarchy = cv2.findContours(erosion, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
```

### Comparing `baseImage-2.1.3/baseImage/utils/ssim/paddle.py` & `baseImage-2.1.4/baseImage/utils/ssim/paddle.py`

 * *Files identical despite different names*

### Comparing `baseImage-2.1.3/baseImage/utils/ssim/ssim.py` & `baseImage-2.1.4/baseImage/utils/ssim/ssim.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,42 +3,44 @@
 
 import cv2
 import numpy as np
 from typing import Union, Optional, Tuple
 
 
 class SSIM(object):
-    def __init__(self, win_size: int = 11, data_range: int = 255, sigma: Union[int, float] = 1.5,
+    def __init__(self, win_size: int = 7, data_range: int = 255, sigma: Union[int, float] = 1.5,
                  use_sample_covariance=True, resize=(500, 500)):
         """
         使用ssim计算两张图片的相似度
 
         Args:
             win_size(int): 高斯核大小
             data_range(int): 图片的取值范围 (1.0 or 255)
             sigma(float): 高斯核标准差
             use_sample_covariance: 如果为真，则通过 N-1 而不是 N 归一化
             resize: 输入图片的缩放大小(h, w)
         """
         self.win_size = win_size
         self.data_range = data_range
         self.sigma = sigma
-        self.dtype = np.float32
+        self.dtype = np.float64
         self.K1 = 0.01
         self.K2 = 0.03
         self.C1 = (self.K1 * self.data_range) ** 2
         self.C2 = (self.K2 * self.data_range) ** 2
         self.resize = resize
 
         NP = win_size ** 2
+
         # filter has already normalized by NP
         if use_sample_covariance:
             cov_norm = NP / (NP - 1)  # sample covariance
         else:
             cov_norm = 1.0  # population covariance to match Wang et. al. 2004
+
         self.cov_norm = cov_norm
         self.gaussian_args = {'size': (win_size, win_size), 'sigma': sigma, 'borderType': cv2.BORDER_REFLECT}
 
     #     if Setting.CUDA_Flag:
     #         self._buffer_cuda_mat()
     #
     # def _buffer_cuda_mat(self):
@@ -68,21 +70,21 @@
         if im1.channels != im2.channels:
             raise ValueError('图片通道数量必须一致, im1:{}, im2:{}'.format(im1.place, im2.place))
 
         if im1.size != im2.size:
             raise ValueError('图片大小一致, im1:{}, im2:{}'.format(im1.size, im2.size))
 
         if im1.place != im2.place:
-            im2 = Image(im2, place=im1.place, dtype=np.float32)
+            im2 = Image(im2, place=im1.place, dtype=np.float64)
 
-        if im1.dtype != np.float32:
-            im1 = Image(im1, place=im1.place, dtype=np.float32)
+        if im1.dtype != np.float64:
+            im1 = Image(im1, place=im1.place, dtype=np.float64)
 
-        if im2.dtype != np.float32:
-            im2 = Image(im2, place=im2.place, dtype=np.float32)
+        if im2.dtype != np.float64:
+            im2 = Image(im2, place=im2.place, dtype=np.float64)
         return im1, im2
 
     def ssim(self, im1: Image, im2: Image, full: bool = False) -> Tuple[float, Optional[Image]]:
         """
         计算两张图片的相似度
 
         Args:
@@ -173,17 +175,18 @@
 
         uxx = Image(data=multiply(im1.data, im1.data), **new_image_args).gaussianBlur(**self.gaussian_args).data
         uyy = Image(data=multiply(im2.data, im2.data), **new_image_args).gaussianBlur(**self.gaussian_args).data
         uxy = Image(data=multiply(im1.data, im2.data), **new_image_args).gaussianBlur(**self.gaussian_args).data
 
         # 官方的cuda python绑定有问题,目前没有修复, 需要用下面的commit才能使用
         # https://github.com/hakaboom/opencv_contrib/commit/ed0a7d567ff4775fc933c889cf856146a3ea79be
-        vx = multiply(subtract(multiply(ux, ux), uxx), cov_norm)
-        vy = multiply(subtract(multiply(uy, uy), uyy), cov_norm)
-        vxy = multiply(subtract(multiply(ux, uy), uxy), cov_norm)
+
+        vx = multiply(subtract(uxx, multiply(ux, ux)), cov_norm)
+        vy = multiply(subtract(uyy, multiply(uy, uy)), cov_norm)
+        vxy = multiply(subtract(uxy, multiply(ux, uy)), cov_norm)
 
         A1 = add(multiply(multiply(ux, uy), 2), C1)
         A2 = add(multiply(vxy, 2), C2)
         B1 = add(add(pow(ux, 2), pow(uy, 2)), C1)
         B2 = add(add(vx, vy), C2)
         D = multiply(B1, B2)
         S = divide(multiply(A1, A2), D)
```

### Comparing `baseImage-2.1.3/baseImage.egg-info/PKG-INFO` & `baseImage-2.1.4/baseImage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: baseImage
-Version: 2.1.3
+Version: 2.1.4
 Summary: This is a secondary package of OpenCV,for manage image data
 Home-page: https://github.com/hakaboom/base_image
 Author: hakaboom
 Author-email: 1534225986@qq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6, <=3.10
+Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # base_image
 对opencv_python常用接口的二次开发
 
 建议 opencv version >= 4.5.5(不同opencv版本的python绑定,函数名可能会不同)
```

### Comparing `baseImage-2.1.3/baseImage.egg-info/SOURCES.txt` & `baseImage-2.1.4/baseImage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseImage-2.1.3/setup.py` & `baseImage-2.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             'opencv-python>=4.5.5.64',
             'pydantic'
         ]
 
 
 setup(
     name='baseImage',
-    version='2.1.3',
+    version='2.1.4',
     author='hakaboom',
     author_email='1534225986@qq.com',
     license='Apache License 2.0',
     description='This is a secondary package of OpenCV,for manage image data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/hakaboom/base_image',
@@ -35,9 +35,9 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6, <=3.10',
-)
+    python_requires='>=3.6, <3.11',
+)
```

### Comparing `baseImage-2.1.3/tests/test_all.py` & `baseImage-2.1.4/tests/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -471,33 +471,62 @@
 00001d60: 2020 2020 2020 696d 6720 3d20 496d 6167        img = Imag
 00001d70: 6528 6461 7461 3d6f 732e 7061 7468 2e6a  e(data=os.path.j
 00001d80: 6f69 6e28 494d 4147 4544 4952 2c20 2730  oin(IMAGEDIR, '0
 00001d90: 2e70 6e67 2729 2c20 706c 6163 653d 706c  .png'), place=pl
 00001da0: 6163 6529 0a20 2020 2020 2020 2020 2020  ace).           
 00001db0: 2069 6d67 2e63 616c 6348 6973 7428 6869   img.calcHist(hi
 00001dc0: 7374 5369 7a65 2c20 7261 6e67 6573 290a  stSize, ranges).
-00001dd0: 0a20 2020 2064 6566 2074 6573 745f 7373  .    def test_ss
-00001de0: 696d 2873 656c 6629 3a0a 2020 2020 2020  im(self):.      
-00001df0: 2020 666f 7220 706c 6163 6520 696e 2073    for place in s
-00001e00: 656c 662e 706c 6163 655f 6c69 7374 3a0a  elf.place_list:.
-00001e10: 2020 2020 2020 2020 2020 2020 696d 3120              im1 
-00001e20: 3d20 496d 6167 6528 6461 7461 3d6f 732e  = Image(data=os.
-00001e30: 7061 7468 2e6a 6f69 6e28 494d 4147 4544  path.join(IMAGED
-00001e40: 4952 2c20 2731 2e70 6e67 2729 2c20 6474  IR, '1.png'), dt
-00001e50: 7970 653d 6e70 2e66 6c6f 6174 3332 2c20  ype=np.float32, 
-00001e60: 706c 6163 653d 706c 6163 6529 0a20 2020  place=place).   
-00001e70: 2020 2020 2020 2020 2069 6d32 203d 2049           im2 = I
-00001e80: 6d61 6765 2864 6174 613d 6f73 2e70 6174  mage(data=os.pat
-00001e90: 682e 6a6f 696e 2849 4d41 4745 4449 522c  h.join(IMAGEDIR,
-00001ea0: 2027 312e 706e 6727 292c 2064 7479 7065   '1.png'), dtype
-00001eb0: 3d6e 702e 666c 6f61 7433 322c 2070 6c61  =np.float32, pla
-00001ec0: 6365 3d70 6c61 6365 290a 0a20 2020 2020  ce=place)..     
-00001ed0: 2020 2020 2020 2073 7369 6d20 3d20 5353         ssim = SS
-00001ee0: 494d 2829 0a20 2020 2020 2020 2020 2020  IM().           
-00001ef0: 206d 2c20 5320 3d20 7373 696d 2e73 7369   m, S = ssim.ssi
-00001f00: 6d28 696d 312c 2069 6d32 2c20 6675 6c6c  m(im1, im2, full
-00001f10: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00001f20: 2020 2073 656c 662e 6173 7365 7274 4973     self.assertIs
-00001f30: 4e6f 744e 6f6e 6528 6d29 0a0a 0a69 6620  NotNone(m)...if 
-00001f40: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
-00001f50: 6169 6e5f 5f27 3a0a 2020 2020 756e 6974  ain__':.    unit
-00001f60: 7465 7374 2e6d 6169 6e28 290a            test.main().
+00001dd0: 0a20 2020 2064 6566 2074 6573 745f 696e  .    def test_in
+00001de0: 5261 6e67 6528 7365 6c66 293a 0a20 2020  Range(self):.   
+00001df0: 2020 2020 206c 6f77 6572 6220 3d20 2830       lowerb = (0
+00001e00: 2c20 302c 2030 290a 2020 2020 2020 2020  , 0, 0).        
+00001e10: 7570 7065 7262 203d 2028 3235 352c 2032  upperb = (255, 2
+00001e20: 3535 2c20 3235 3529 0a20 2020 2020 2020  55, 255).       
+00001e30: 2066 6f72 2070 6c61 6365 2069 6e20 7365   for place in se
+00001e40: 6c66 2e70 6c61 6365 5f6c 6973 743a 0a20  lf.place_list:. 
+00001e50: 2020 2020 2020 2020 2020 2069 6d67 203d             img =
+00001e60: 2049 6d61 6765 2864 6174 613d 6f73 2e70   Image(data=os.p
+00001e70: 6174 682e 6a6f 696e 2849 4d41 4745 4449  ath.join(IMAGEDI
+00001e80: 522c 2027 302e 706e 6727 292c 2070 6c61  R, '0.png'), pla
+00001e90: 6365 3d70 6c61 6365 290a 2020 2020 2020  ce=place).      
+00001ea0: 2020 2020 2020 6e65 775f 696d 6720 3d20        new_img = 
+00001eb0: 696d 672e 696e 5261 6e67 6528 6c6f 7765  img.inRange(lowe
+00001ec0: 7262 2c20 7570 7065 7262 290a 0a20 2020  rb, upperb)..   
+00001ed0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00001ee0: 7365 7274 4571 7561 6c28 6e65 775f 696d  sertEqual(new_im
+00001ef0: 672e 7369 7a65 2c20 696d 672e 7369 7a65  g.size, img.size
+00001f00: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00001f10: 6c66 2e61 7373 6572 7449 6d61 6765 5074  lf.assertImagePt
+00001f20: 724e 6f74 4571 7561 6c28 696d 672c 206e  rNotEqual(img, n
+00001f30: 6577 5f69 6d67 290a 2020 2020 2020 2020  ew_img).        
+00001f40: 2020 2020 7365 6c66 2e61 7373 6572 7450      self.assertP
+00001f50: 6c61 6365 4571 7561 6c28 6e65 775f 696d  laceEqual(new_im
+00001f60: 672c 2070 6c61 6365 290a 2020 2020 2020  g, place).      
+00001f70: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00001f80: 7444 5479 7065 4571 7561 6c28 6e65 775f  tDTypeEqual(new_
+00001f90: 696d 672c 206e 702e 7569 6e74 3829 0a0a  img, np.uint8)..
+00001fa0: 2020 2020 6465 6620 7465 7374 5f73 7369      def test_ssi
+00001fb0: 6d28 7365 6c66 293a 0a20 2020 2020 2020  m(self):.       
+00001fc0: 2066 6f72 2070 6c61 6365 2069 6e20 7365   for place in se
+00001fd0: 6c66 2e70 6c61 6365 5f6c 6973 743a 0a20  lf.place_list:. 
+00001fe0: 2020 2020 2020 2020 2020 2069 6d31 203d             im1 =
+00001ff0: 2049 6d61 6765 2864 6174 613d 6f73 2e70   Image(data=os.p
+00002000: 6174 682e 6a6f 696e 2849 4d41 4745 4449  ath.join(IMAGEDI
+00002010: 522c 2027 312e 706e 6727 292c 2064 7479  R, '1.png'), dty
+00002020: 7065 3d6e 702e 666c 6f61 7433 322c 2070  pe=np.float32, p
+00002030: 6c61 6365 3d70 6c61 6365 290a 2020 2020  lace=place).    
+00002040: 2020 2020 2020 2020 696d 3220 3d20 496d          im2 = Im
+00002050: 6167 6528 6461 7461 3d6f 732e 7061 7468  age(data=os.path
+00002060: 2e6a 6f69 6e28 494d 4147 4544 4952 2c20  .join(IMAGEDIR, 
+00002070: 2731 2e70 6e67 2729 2c20 6474 7970 653d  '1.png'), dtype=
+00002080: 6e70 2e66 6c6f 6174 3332 2c20 706c 6163  np.float32, plac
+00002090: 653d 706c 6163 6529 0a0a 2020 2020 2020  e=place)..      
+000020a0: 2020 2020 2020 7373 696d 203d 2053 5349        ssim = SSI
+000020b0: 4d28 290a 2020 2020 2020 2020 2020 2020  M().            
+000020c0: 6d2c 2053 203d 2073 7369 6d2e 7373 696d  m, S = ssim.ssim
+000020d0: 2869 6d31 2c20 696d 322c 2066 756c 6c3d  (im1, im2, full=
+000020e0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+000020f0: 2020 7365 6c66 2e61 7373 6572 7449 734e    self.assertIsN
+00002100: 6f74 4e6f 6e65 286d 290a 0a0a 6966 205f  otNone(m)...if _
+00002110: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
+00002120: 696e 5f5f 273a 0a20 2020 2075 6e69 7474  in__':.    unitt
+00002130: 6573 742e 6d61 696e 2829 0a              est.main().
```

