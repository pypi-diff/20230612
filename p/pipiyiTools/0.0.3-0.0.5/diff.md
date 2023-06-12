# Comparing `tmp/pipiyiTools-0.0.3.tar.gz` & `tmp/pipiyiTools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pipiyiTools-0.0.3.tar", last modified: Tue Jun  6 09:02:38 2023, max compression
+gzip compressed data, was "dist/pipiyiTools-0.0.5.tar", last modified: Mon Jun 12 14:18:33 2023, max compression
```

## Comparing `pipiyiTools-0.0.3.tar` & `pipiyiTools-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/
--rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/PKG-INFO
--rw-r--r--   0 xiaopipi   (501) staff       (20)      314 2023-06-06 08:59:34.000000 pipiyiTools-0.0.3/README.md
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools/
--rw-r--r--   0 xiaopipi   (501) staff       (20)     2589 2023-05-23 08:46:36.000000 pipiyiTools-0.0.3/pipiyiTools/EpubSpliter.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1058 2023-05-25 05:43:31.000000 pipiyiTools-0.0.3/pipiyiTools/FileOperation.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1385 2023-06-06 09:02:18.000000 pipiyiTools-0.0.3/pipiyiTools/ListQueue.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1928 2023-05-26 09:49:22.000000 pipiyiTools-0.0.3/pipiyiTools/Log.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     2070 2023-05-23 06:29:36.000000 pipiyiTools-0.0.3/pipiyiTools/MyRequest.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)     6711 2023-05-28 14:14:08.000000 pipiyiTools-0.0.3/pipiyiTools/PooledBase.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)      972 2023-05-23 04:18:08.000000 pipiyiTools-0.0.3/pipiyiTools/Storage.py
--rw-r--r--   0 xiaopipi   (501) staff       (20)        0 2023-05-30 10:06:54.000000 pipiyiTools-0.0.3/pipiyiTools/__init__.py
-drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/
--rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/PKG-INFO
--rw-r--r--   0 xiaopipi   (501) staff       (20)      390 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/SOURCES.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)        1 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/dependency_links.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       43 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/requires.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       12 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/pipiyiTools.egg-info/top_level.txt
--rw-r--r--   0 xiaopipi   (501) staff       (20)       38 2023-06-06 09:02:38.000000 pipiyiTools-0.0.3/setup.cfg
--rw-r--r--   0 xiaopipi   (501) staff       (20)     1005 2023-06-06 09:02:25.000000 pipiyiTools-0.0.3/setup.py
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/PKG-INFO
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      314 2023-06-06 08:59:34.000000 pipiyiTools-0.0.5/README.md
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/pipiyiTools/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     2589 2023-05-23 08:46:36.000000 pipiyiTools-0.0.5/pipiyiTools/EpubSpliter.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1058 2023-05-25 05:43:31.000000 pipiyiTools-0.0.5/pipiyiTools/FileOperation.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1385 2023-06-06 09:02:18.000000 pipiyiTools-0.0.5/pipiyiTools/ListQueue.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1918 2023-06-12 14:17:44.000000 pipiyiTools-0.0.5/pipiyiTools/Log.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     2070 2023-05-23 06:29:36.000000 pipiyiTools-0.0.5/pipiyiTools/MyRequest.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     6711 2023-05-28 14:14:08.000000 pipiyiTools-0.0.5/pipiyiTools/PooledBase.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      972 2023-05-23 04:18:08.000000 pipiyiTools-0.0.5/pipiyiTools/Storage.py
+-rw-r--r--   0 xiaopipi   (501) staff       (20)        0 2023-05-30 10:06:54.000000 pipiyiTools-0.0.5/pipiyiTools/__init__.py
+drwxr-xr-x   0 xiaopipi   (501) staff       (20)        0 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/pipiyiTools.egg-info/
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      975 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/pipiyiTools.egg-info/PKG-INFO
+-rw-r--r--   0 xiaopipi   (501) staff       (20)      390 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/pipiyiTools.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)        1 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/pipiyiTools.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       43 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/pipiyiTools.egg-info/requires.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       12 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/pipiyiTools.egg-info/top_level.txt
+-rw-r--r--   0 xiaopipi   (501) staff       (20)       38 2023-06-12 14:18:33.000000 pipiyiTools-0.0.5/setup.cfg
+-rw-r--r--   0 xiaopipi   (501) staff       (20)     1005 2023-06-12 14:17:59.000000 pipiyiTools-0.0.5/setup.py
```

### Comparing `pipiyiTools-0.0.3/PKG-INFO` & `pipiyiTools-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipiyiTools
-Version: 0.0.3
+Version: 0.0.5
 Summary: Personal tool library
 Home-page: UNKNOWN
 Author: pipiyi
 Author-email: smallpoliao@gmail.com
 License: UNKNOWN
 Description: 
         # 一个小工具合集
```

### Comparing `pipiyiTools-0.0.3/pipiyiTools/EpubSpliter.py` & `pipiyiTools-0.0.5/pipiyiTools/EpubSpliter.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.3/pipiyiTools/FileOperation.py` & `pipiyiTools-0.0.5/pipiyiTools/FileOperation.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.3/pipiyiTools/ListQueue.py` & `pipiyiTools-0.0.5/pipiyiTools/ListQueue.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.3/pipiyiTools/Log.py` & `pipiyiTools-0.0.5/pipiyiTools/Log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 import colorlog
 
+
 class Log:
     # 设置日志格式
     formatter = colorlog.ColoredFormatter(
-        "%(log_color)s%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+        "%(log_color)s%(asctime)s - %(levelname)s - %(message)s",
         log_colors={
-            'DEBUG': 'cyan',
-            'INFO': 'green',
-            'WARNING': 'yellow',
-            'ERROR': 'red',
-            'CRITICAL': 'red,bg_white',
+            "DEBUG": "cyan",
+            "INFO": "green",
+            "WARNING": "yellow",
+            "ERROR": "red",
+            "CRITICAL": "red,bg_white",
         },
     )
 
     def __init__(self, filename="log"):
         # 它会自动获取当前模块的名称作为 logger 的名称。
         # 这样可以在日志中标识出日志消息来自哪个模块
         self.logger = logging.getLogger(__name__)
```

### Comparing `pipiyiTools-0.0.3/pipiyiTools/MyRequest.py` & `pipiyiTools-0.0.5/pipiyiTools/MyRequest.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.3/pipiyiTools/PooledBase.py` & `pipiyiTools-0.0.5/pipiyiTools/PooledBase.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.3/pipiyiTools/Storage.py` & `pipiyiTools-0.0.5/pipiyiTools/Storage.py`

 * *Files identical despite different names*

### Comparing `pipiyiTools-0.0.3/pipiyiTools.egg-info/PKG-INFO` & `pipiyiTools-0.0.5/pipiyiTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipiyiTools
-Version: 0.0.3
+Version: 0.0.5
 Summary: Personal tool library
 Home-page: UNKNOWN
 Author: pipiyi
 Author-email: smallpoliao@gmail.com
 License: UNKNOWN
 Description: 
         # 一个小工具合集
```

### Comparing `pipiyiTools-0.0.3/setup.py` & `pipiyiTools-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.3"
+VERSION = "0.0.5"
 DESCRIPTION = "Personal tool library"
 
 # Setting up
 setup(
     name="pipiyiTools",
     version=VERSION,
     author="pipiyi",
```

