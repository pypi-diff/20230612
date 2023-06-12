# Comparing `tmp/teenstudy-0.2.0rc1.tar.gz` & `tmp/teenstudy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teenstudy-0.2.0rc1.tar", max compression
+gzip compressed data, was "teenstudy-0.2.1.tar", max compression
```

## Comparing `teenstudy-0.2.0rc1.tar` & `teenstudy-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1063 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/LICENSE
--rw-r--r--   0        0        0    11355 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/README.md
--rw-r--r--   0        0        0      766 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/TeenStudy/__init__.py
--rw-r--r--   0        0        0       27 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/TeenStudy/models/__init__.py
--rw-r--r--   0        0        0     3438 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/TeenStudy/models/accuont.py
--rw-r--r--   0        0        0     2770 2023-06-12 02:32:00.308969 teenstudy-0.2.0rc1/TeenStudy/models/dxx.py
--rw-r--r--   0        0        0  7977480 2023-06-12 02:32:00.368970 teenstudy-0.2.0rc1/TeenStudy/resource/MiSans-Light.ttf
--rw-r--r--   0        0        0   881164 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/answer.png
--rw-r--r--   0        0        0    52240 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud1.jpg
--rw-r--r--   0        0        0    52119 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud2.jpg
--rw-r--r--   0        0        0    52136 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud3.jpg
--rw-r--r--   0        0        0    51874 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud4.jpg
--rw-r--r--   0        0        0    51634 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/resource/backgroud5.jpg
--rw-r--r--   0        0        0      116 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/__init__.py
--rw-r--r--   0        0        0    56096 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/dxx.py
--rw-r--r--   0        0        0    18464 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/handle.py
--rw-r--r--   0        0        0     4195 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/path.py
--rw-r--r--   0        0        0     2354 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/rule.py
--rw-r--r--   0        0        0    10171 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/update.py
--rw-r--r--   0        0        0    20971 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/utils/utils.py
--rw-r--r--   0        0        0     2209 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/__init__.py
--rw-r--r--   0        0        0      456 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/__init__.py
--rw-r--r--   0        0        0    38486 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/add.py
--rw-r--r--   0        0        0    11593 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/admin.py
--rw-r--r--   0        0        0     4927 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/home.py
--rw-r--r--   0        0        0     1403 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/log.py
--rw-r--r--   0        0        0     5192 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/api/login.py
--rw-r--r--   0        0        0      111 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/__init__.py
--rw-r--r--   0        0        0    29300 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/add.py
--rw-r--r--   0        0        0    44883 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/addArea.py
--rw-r--r--   0        0        0    23125 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/admin.py
--rw-r--r--   0        0        0    18037 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/home.py
--rw-r--r--   0        0        0     2038 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/log.py
--rw-r--r--   0        0        0     1982 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/pages/login.py
--rw-r--r--   0        0        0       24 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/utils/__init__.py
--rw-r--r--   0        0        0     2158 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/utils/add.py
--rw-r--r--   0        0        0     2175 2023-06-12 02:32:00.372970 teenstudy-0.2.0rc1/TeenStudy/web/utils/status.py
--rw-r--r--   0        0        0      988 2023-06-12 02:32:00.376970 teenstudy-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0    12903 1970-01-01 00:00:00.000000 teenstudy-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-12 02:38:41.554950 teenstudy-0.2.1/LICENSE
+-rw-r--r--   0        0        0    11355 2023-06-12 02:38:41.554950 teenstudy-0.2.1/README.md
+-rw-r--r--   0        0        0      766 2023-06-12 02:38:41.554950 teenstudy-0.2.1/TeenStudy/__init__.py
+-rw-r--r--   0        0        0       27 2023-06-12 02:38:41.554950 teenstudy-0.2.1/TeenStudy/models/__init__.py
+-rw-r--r--   0        0        0     3438 2023-06-12 02:38:41.554950 teenstudy-0.2.1/TeenStudy/models/accuont.py
+-rw-r--r--   0        0        0     2770 2023-06-12 02:38:41.554950 teenstudy-0.2.1/TeenStudy/models/dxx.py
+-rw-r--r--   0        0        0  7977480 2023-06-12 02:38:41.622950 teenstudy-0.2.1/TeenStudy/resource/MiSans-Light.ttf
+-rw-r--r--   0        0        0   881164 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/resource/answer.png
+-rw-r--r--   0        0        0    52240 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/resource/backgroud1.jpg
+-rw-r--r--   0        0        0    52119 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/resource/backgroud2.jpg
+-rw-r--r--   0        0        0    52136 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/resource/backgroud3.jpg
+-rw-r--r--   0        0        0    51874 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/resource/backgroud4.jpg
+-rw-r--r--   0        0        0    51634 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/resource/backgroud5.jpg
+-rw-r--r--   0        0        0      116 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/utils/__init__.py
+-rw-r--r--   0        0        0    56096 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/utils/dxx.py
+-rw-r--r--   0        0        0    18464 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/utils/handle.py
+-rw-r--r--   0        0        0     4195 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/utils/path.py
+-rw-r--r--   0        0        0     2354 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/utils/rule.py
+-rw-r--r--   0        0        0    10171 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/utils/update.py
+-rw-r--r--   0        0        0    20971 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/utils/utils.py
+-rw-r--r--   0        0        0     2209 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/web/__init__.py
+-rw-r--r--   0        0        0      456 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/web/api/__init__.py
+-rw-r--r--   0        0        0    38486 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/web/api/add.py
+-rw-r--r--   0        0        0    11593 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/web/api/admin.py
+-rw-r--r--   0        0        0     4927 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/web/api/home.py
+-rw-r--r--   0        0        0     1403 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/web/api/log.py
+-rw-r--r--   0        0        0     5192 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/web/api/login.py
+-rw-r--r--   0        0        0      111 2023-06-12 02:38:41.626950 teenstudy-0.2.1/TeenStudy/web/pages/__init__.py
+-rw-r--r--   0        0        0    29300 2023-06-12 02:38:41.630950 teenstudy-0.2.1/TeenStudy/web/pages/add.py
+-rw-r--r--   0        0        0    44883 2023-06-12 02:38:41.630950 teenstudy-0.2.1/TeenStudy/web/pages/addArea.py
+-rw-r--r--   0        0        0    23125 2023-06-12 02:38:41.630950 teenstudy-0.2.1/TeenStudy/web/pages/admin.py
+-rw-r--r--   0        0        0    18037 2023-06-12 02:38:41.630950 teenstudy-0.2.1/TeenStudy/web/pages/home.py
+-rw-r--r--   0        0        0     2038 2023-06-12 02:38:41.630950 teenstudy-0.2.1/TeenStudy/web/pages/log.py
+-rw-r--r--   0        0        0     1982 2023-06-12 02:38:41.630950 teenstudy-0.2.1/TeenStudy/web/pages/login.py
+-rw-r--r--   0        0        0       24 2023-06-12 02:38:41.630950 teenstudy-0.2.1/TeenStudy/web/utils/__init__.py
+-rw-r--r--   0        0        0     2158 2023-06-12 02:38:41.630950 teenstudy-0.2.1/TeenStudy/web/utils/add.py
+-rw-r--r--   0        0        0     2175 2023-06-12 02:38:41.630950 teenstudy-0.2.1/TeenStudy/web/utils/status.py
+-rw-r--r--   0        0        0      985 2023-06-12 02:38:41.630950 teenstudy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12900 1970-01-01 00:00:00.000000 teenstudy-0.2.1/PKG-INFO
```

### Comparing `teenstudy-0.2.0rc1/LICENSE` & `teenstudy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/README.md` & `teenstudy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/__init__.py` & `teenstudy-0.2.1/TeenStudy/__init__.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/models/accuont.py` & `teenstudy-0.2.1/TeenStudy/models/accuont.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/models/dxx.py` & `teenstudy-0.2.1/TeenStudy/models/dxx.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/resource/MiSans-Light.ttf` & `teenstudy-0.2.1/TeenStudy/resource/MiSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/resource/answer.png` & `teenstudy-0.2.1/TeenStudy/resource/answer.png`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud1.jpg` & `teenstudy-0.2.1/TeenStudy/resource/backgroud1.jpg`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud2.jpg` & `teenstudy-0.2.1/TeenStudy/resource/backgroud2.jpg`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud3.jpg` & `teenstudy-0.2.1/TeenStudy/resource/backgroud3.jpg`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud4.jpg` & `teenstudy-0.2.1/TeenStudy/resource/backgroud4.jpg`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/resource/backgroud5.jpg` & `teenstudy-0.2.1/TeenStudy/resource/backgroud5.jpg`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/utils/dxx.py` & `teenstudy-0.2.1/TeenStudy/utils/dxx.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/utils/handle.py` & `teenstudy-0.2.1/TeenStudy/utils/handle.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/utils/path.py` & `teenstudy-0.2.1/TeenStudy/utils/path.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/utils/rule.py` & `teenstudy-0.2.1/TeenStudy/utils/rule.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/utils/update.py` & `teenstudy-0.2.1/TeenStudy/utils/update.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/utils/utils.py` & `teenstudy-0.2.1/TeenStudy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/__init__.py` & `teenstudy-0.2.1/TeenStudy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/api/add.py` & `teenstudy-0.2.1/TeenStudy/web/api/add.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/api/admin.py` & `teenstudy-0.2.1/TeenStudy/web/api/admin.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/api/home.py` & `teenstudy-0.2.1/TeenStudy/web/api/home.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/api/log.py` & `teenstudy-0.2.1/TeenStudy/web/api/log.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/api/login.py` & `teenstudy-0.2.1/TeenStudy/web/api/login.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/pages/add.py` & `teenstudy-0.2.1/TeenStudy/web/pages/add.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/pages/addArea.py` & `teenstudy-0.2.1/TeenStudy/web/pages/addArea.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/pages/admin.py` & `teenstudy-0.2.1/TeenStudy/web/pages/admin.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/pages/home.py` & `teenstudy-0.2.1/TeenStudy/web/pages/home.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/pages/log.py` & `teenstudy-0.2.1/TeenStudy/web/pages/log.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/pages/login.py` & `teenstudy-0.2.1/TeenStudy/web/pages/login.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/utils/add.py` & `teenstudy-0.2.1/TeenStudy/web/utils/add.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/TeenStudy/web/utils/status.py` & `teenstudy-0.2.1/TeenStudy/web/utils/status.py`

 * *Files identical despite different names*

### Comparing `teenstudy-0.2.0rc1/pyproject.toml` & `teenstudy-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "TeenStudy"
-version = "0.2.0rc1"
+version = "0.2.1"
 description = "基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图"
 authors = ["ZM25XC <xingling25@qq.com>"]
 license="MIT"
 readme="README.md"
 homepage="https://github.com/ZM25XC/TeenStudy"
 packages = [
   { include = "TeenStudy" },
```

### Comparing `teenstudy-0.2.0rc1/PKG-INFO` & `teenstudy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teenstudy
-Version: 0.2.0rc1
+Version: 0.2.1
 Summary: 基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图
 Home-page: https://github.com/ZM25XC/TeenStudy
 License: MIT
 Author: ZM25XC
 Author-email: xingling25@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: teenstudy Version: 0.2.0rc1 Summary:
+Metadata-Version: 2.1 Name: teenstudy Version: 0.2.1 Summary:
 åºäºnonebot2å¼æ­¥æ¡æ¶çéå¹´å¤§å­¦èªå¨æäº¤æä»¶åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 Home-page: https://github.com/ZM25XC/TeenStudy License: MIT Author: ZM25XC
 Author-email: xingling25@qq.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Jinja2
```

