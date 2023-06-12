# Comparing `tmp/epubs-0.0.1.tar.gz` & `tmp/epubs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubs-0.0.1.tar", last modified: Mon Jun 12 04:24:55 2023, max compression
+gzip compressed data, was "epubs-0.0.2.tar", last modified: Mon Jun 12 04:29:47 2023, max compression
```

## Comparing `epubs-0.0.1.tar` & `epubs-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-12 04:24:55.674020 epubs-0.0.1/
--rw-r--r--   0 bo         (501) staff       (20)    11357 2023-06-09 08:36:54.000000 epubs-0.0.1/LICENSE
--rw-r--r--   0 bo         (501) staff       (20)      736 2023-06-12 04:24:55.673903 epubs-0.0.1/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      282 2023-06-12 04:23:58.000000 epubs-0.0.1/README.md
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-12 04:24:55.673197 epubs-0.0.1/epubs/
--rw-r--r--   0 bo         (501) staff       (20)      411 2023-06-12 04:23:41.000000 epubs-0.0.1/epubs/__init__.py
--rw-r--r--   0 bo         (501) staff       (20)     1668 2023-06-09 09:38:35.000000 epubs-0.0.1/epubs/epub_to_html.py
--rw-r--r--   0 bo         (501) staff       (20)     2417 2023-06-12 04:01:23.000000 epubs-0.0.1/epubs/epub_to_text.py
-drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-12 04:24:55.673750 epubs-0.0.1/epubs.egg-info/
--rw-r--r--   0 bo         (501) staff       (20)      736 2023-06-12 04:24:55.000000 epubs-0.0.1/epubs.egg-info/PKG-INFO
--rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-12 04:24:55.000000 epubs-0.0.1/epubs.egg-info/SOURCES.txt
--rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-12 04:24:55.000000 epubs-0.0.1/epubs.egg-info/dependency_links.txt
--rw-r--r--   0 bo         (501) staff       (20)       27 2023-06-12 04:24:55.000000 epubs-0.0.1/epubs.egg-info/requires.txt
--rw-r--r--   0 bo         (501) staff       (20)        6 2023-06-12 04:24:55.000000 epubs-0.0.1/epubs.egg-info/top_level.txt
--rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-12 04:24:55.674056 epubs-0.0.1/setup.cfg
--rw-r--r--   0 bo         (501) staff       (20)      804 2023-06-12 04:15:30.000000 epubs-0.0.1/setup.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-12 04:29:47.120336 epubs-0.0.2/
+-rw-r--r--   0 bo         (501) staff       (20)    11357 2023-06-09 08:36:54.000000 epubs-0.0.2/LICENSE
+-rw-r--r--   0 bo         (501) staff       (20)      743 2023-06-12 04:29:47.120210 epubs-0.0.2/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      289 2023-06-12 04:29:36.000000 epubs-0.0.2/README.md
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-12 04:29:47.119257 epubs-0.0.2/epubs/
+-rw-r--r--   0 bo         (501) staff       (20)      423 2023-06-12 04:29:08.000000 epubs-0.0.2/epubs/__init__.py
+-rw-r--r--   0 bo         (501) staff       (20)     1668 2023-06-09 09:38:35.000000 epubs-0.0.2/epubs/epub_to_html.py
+-rw-r--r--   0 bo         (501) staff       (20)     2417 2023-06-12 04:01:23.000000 epubs-0.0.2/epubs/epub_to_text.py
+drwxr-xr-x   0 bo         (501) staff       (20)        0 2023-06-12 04:29:47.120047 epubs-0.0.2/epubs.egg-info/
+-rw-r--r--   0 bo         (501) staff       (20)      743 2023-06-12 04:29:46.000000 epubs-0.0.2/epubs.egg-info/PKG-INFO
+-rw-r--r--   0 bo         (501) staff       (20)      232 2023-06-12 04:29:47.000000 epubs-0.0.2/epubs.egg-info/SOURCES.txt
+-rw-r--r--   0 bo         (501) staff       (20)        1 2023-06-12 04:29:46.000000 epubs-0.0.2/epubs.egg-info/dependency_links.txt
+-rw-r--r--   0 bo         (501) staff       (20)       27 2023-06-12 04:29:47.000000 epubs-0.0.2/epubs.egg-info/requires.txt
+-rw-r--r--   0 bo         (501) staff       (20)        6 2023-06-12 04:29:47.000000 epubs-0.0.2/epubs.egg-info/top_level.txt
+-rw-r--r--   0 bo         (501) staff       (20)       38 2023-06-12 04:29:47.120372 epubs-0.0.2/setup.cfg
+-rw-r--r--   0 bo         (501) staff       (20)      804 2023-06-12 04:29:36.000000 epubs-0.0.2/setup.py
```

### Comparing `epubs-0.0.1/LICENSE` & `epubs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epubs-0.0.1/PKG-INFO` & `epubs-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Conversion Tool for EPUB
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -26,22 +26,29 @@
 
 
 ## 使用
 
 - epub 转 html
 
 
+
     import epubs
     
     epubs.to_html('xxxxx.epub', save_path='./xxxxx')
 
 
+
+
 - epub 转 text
-    
+   
+
+ 
 
     import epubs
     
     text = epubs.to_text('xxxxx.epub')
     print(text)
 
 
 
+
+
```

### Comparing `epubs-0.0.1/epubs/epub_to_html.py` & `epubs-0.0.2/epubs/epub_to_html.py`

 * *Files identical despite different names*

### Comparing `epubs-0.0.1/epubs/epub_to_text.py` & `epubs-0.0.2/epubs/epub_to_text.py`

 * *Files identical despite different names*

### Comparing `epubs-0.0.1/epubs.egg-info/PKG-INFO` & `epubs-0.0.2/epubs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubs
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Conversion Tool for EPUB
 Home-page: https://gitee.com/maxbanana
 Author: hongbo liu
 Author-email: 782027465@qq.com
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -26,22 +26,29 @@
 
 
 ## 使用
 
 - epub 转 html
 
 
+
     import epubs
     
     epubs.to_html('xxxxx.epub', save_path='./xxxxx')
 
 
+
+
 - epub 转 text
-    
+   
+
+ 
 
     import epubs
     
     text = epubs.to_text('xxxxx.epub')
     print(text)
 
 
 
+
+
```

### Comparing `epubs-0.0.1/setup.py` & `epubs-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='epubs',
-    version='0.0.1',
+    version='0.0.2',
     packages=setuptools.find_packages(),
     url='https://gitee.com/maxbanana',
     license='Apache',
     author='hongbo liu',
     author_email='782027465@qq.com',
     description='A Conversion Tool for EPUB',
     long_description=long_description,
```

