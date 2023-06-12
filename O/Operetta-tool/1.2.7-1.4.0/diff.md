# Comparing `tmp/Operetta_tool-1.2.7.tar.gz` & `tmp/Operetta_tool-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Operetta_tool-1.2.7.tar", last modified: Mon Mar 20 21:06:47 2023, max compression
+gzip compressed data, was "Operetta_tool-1.4.0.tar", last modified: Mon Jun 12 12:40:40 2023, max compression
```

## Comparing `Operetta_tool-1.2.7.tar` & `Operetta_tool-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 21:06:47.345867 Operetta_tool-1.2.7/
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.2.7/LICENSE
--rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.2.7/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-03-20 21:06:47.334081 Operetta_tool-1.2.7/Operetta_tool.egg-info/
--rw-rw-rw-   0        0        0      725 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-20 21:06:46.000000 Operetta_tool-1.2.7/Operetta_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-03-20 21:06:47.345867 Operetta_tool-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 21:06:47.344866 Operetta_tool-1.2.7/operetta/
--rw-rw-rw-   0        0        0      153 2023-03-20 21:02:36.000000 Operetta_tool-1.2.7/operetta/__init__.py
--rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.2.7/operetta/jbsicon.ico
--rw-rw-rw-   0        0        0    31809 2023-03-20 21:02:20.000000 Operetta_tool-1.2.7/operetta/operetta_annotation.py
--rw-rw-rw-   0        0        0       42 2023-03-20 21:06:47.346867 Operetta_tool-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1276 2023-03-20 21:02:40.000000 Operetta_tool-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:40:40.926566 Operetta_tool-1.4.0/
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.4.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-12 12:40:40.913465 Operetta_tool-1.4.0/Operetta_tool.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 12:40:40.000000 Operetta_tool-1.4.0/Operetta_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-06-12 12:40:40.925186 Operetta_tool-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 12:40:40.924075 Operetta_tool-1.4.0/operetta/
+-rw-rw-rw-   0        0        0      153 2023-06-12 12:33:03.000000 Operetta_tool-1.4.0/operetta/__init__.py
+-rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.4.0/operetta/jbsicon.ico
+-rw-rw-rw-   0        0        0    59099 2023-06-12 12:24:38.000000 Operetta_tool-1.4.0/operetta/operetta_annotation.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:40:40.926566 Operetta_tool-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1276 2023-06-12 12:33:10.000000 Operetta_tool-1.4.0/setup.py
```

### Comparing `Operetta_tool-1.2.7/LICENSE` & `Operetta_tool-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.2.7/Operetta_tool.egg-info/PKG-INFO` & `Operetta_tool-1.4.0/Operetta_tool.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta-tool
-Version: 1.2.7
+Version: 1.4.0
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.2.7/PKG-INFO` & `Operetta_tool-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta_tool
-Version: 1.2.7
+Version: 1.4.0
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.2.7/README.md` & `Operetta_tool-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.2.7/operetta/jbsicon.ico` & `Operetta_tool-1.4.0/operetta/jbsicon.ico`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.2.7/setup.py` & `Operetta_tool-1.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.7' 
+VERSION = '1.4.0' 
 DESCRIPTION = 'operetta_tool'
 LONG_DESCRIPTION = 'The Operetta_tool is a python library created for handling and annotation images from the Opera Phenix platform used for ML / AI applications. Instructions for use on github [https://github.com/jkubis96/Operetta_tool] '
 
 # Setting up
 setup(
         name="Operetta_tool", 
         version=VERSION,
```

