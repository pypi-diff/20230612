# Comparing `tmp/minidevice-1.1.0.tar.gz` & `tmp/minidevice-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.1.0.tar", last modified: Mon Jun 12 12:58:19 2023, max compression
+gzip compressed data, was "minidevice-1.1.1.tar", last modified: Mon Jun 12 14:21:54 2023, max compression
```

## Comparing `minidevice-1.1.0.tar` & `minidevice-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 12:58:19.356788 minidevice-1.1.0/
--rw-rw-rw-   0        0        0   181499 2023-06-10 03:07:02.000000 minidevice-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2838 2023-06-12 12:58:19.355792 minidevice-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2523 2023-06-10 15:30:42.000000 minidevice-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 12:58:19.347779 minidevice-1.1.0/minidevice/
--rw-rw-rw-   0        0        0      141 2023-06-12 12:43:29.000000 minidevice-1.1.0/minidevice/__init__.py
--rw-rw-rw-   0        0        0    13767 2023-06-12 12:55:22.000000 minidevice-1.1.0/minidevice/adb.py
--rw-rw-rw-   0        0        0     2360 2023-06-12 12:45:18.000000 minidevice-1.1.0/minidevice/capture.py
--rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.1.0/minidevice/config.py
--rw-rw-rw-   0        0        0     3176 2023-06-12 12:56:12.000000 minidevice-1.1.0/minidevice/device.py
--rw-rw-rw-   0        0        0    19850 2023-06-12 12:44:40.000000 minidevice-1.1.0/minidevice/images.py
--rw-rw-rw-   0        0        0     2291 2023-06-12 12:33:40.000000 minidevice-1.1.0/minidevice/minicap.py
--rw-rw-rw-   0        0        0      666 2023-06-07 15:41:47.000000 minidevice-1.1.0/minidevice/minitouch.py
--rw-rw-rw-   0        0        0     1675 2023-06-12 12:44:55.000000 minidevice-1.1.0/minidevice/wincap.py
-drwxrwxrwx   0        0        0        0 2023-06-12 12:58:19.354793 minidevice-1.1.0/minidevice.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 12:58:19.000000 minidevice-1.1.0/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 12:58:19.356788 minidevice-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-06-12 12:57:15.000000 minidevice-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:21:54.349197 minidevice-1.1.1/
+-rw-rw-rw-   0        0        0   181499 2023-06-10 03:07:02.000000 minidevice-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2838 2023-06-12 14:21:54.347721 minidevice-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2523 2023-06-10 15:30:42.000000 minidevice-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 14:21:54.340355 minidevice-1.1.1/minidevice/
+-rw-rw-rw-   0        0        0      141 2023-06-12 12:43:29.000000 minidevice-1.1.1/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    13767 2023-06-12 12:55:22.000000 minidevice-1.1.1/minidevice/adb.py
+-rw-rw-rw-   0        0        0     2360 2023-06-12 12:45:18.000000 minidevice-1.1.1/minidevice/capture.py
+-rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.1.1/minidevice/config.py
+-rw-rw-rw-   0        0        0     3176 2023-06-12 12:56:12.000000 minidevice-1.1.1/minidevice/device.py
+-rw-rw-rw-   0        0        0    19850 2023-06-12 12:44:40.000000 minidevice-1.1.1/minidevice/images.py
+-rw-rw-rw-   0        0        0     2291 2023-06-12 12:33:40.000000 minidevice-1.1.1/minidevice/minicap.py
+-rw-rw-rw-   0        0        0      666 2023-06-07 15:41:47.000000 minidevice-1.1.1/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0     1675 2023-06-12 12:44:55.000000 minidevice-1.1.1/minidevice/wincap.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:21:54.346211 minidevice-1.1.1/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 14:21:54.000000 minidevice-1.1.1/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:21:54.350178 minidevice-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      729 2023-06-12 14:21:38.000000 minidevice-1.1.1/setup.py
```

### Comparing `minidevice-1.1.0/LICENSE` & `minidevice-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minidevice-1.1.0/PKG-INFO` & `minidevice-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.1.0
+Version: 1.1.1
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-1.1.0/README.md` & `minidevice-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-1.1.0/minidevice/adb.py` & `minidevice-1.1.1/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.1.0/minidevice/capture.py` & `minidevice-1.1.1/minidevice/capture.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.1.0/minidevice/device.py` & `minidevice-1.1.1/minidevice/device.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.1.0/minidevice/images.py` & `minidevice-1.1.1/minidevice/images.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.1.0/minidevice/minicap.py` & `minidevice-1.1.1/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.1.0/minidevice/minitouch.py` & `minidevice-1.1.1/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.1.0/minidevice/wincap.py` & `minidevice-1.1.1/minidevice/wincap.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.1.0/minidevice.egg-info/PKG-INFO` & `minidevice-1.1.1/minidevice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.1.0
+Version: 1.1.1
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-1.1.0/setup.py` & `minidevice-1.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='1.1.0',
+      version='1.1.1',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

