# Comparing `tmp/SmoobuExtractorFormatter-1.2.1.tar.gz` & `tmp/SmoobuExtractorFormatter-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.2.1.tar", last modified: Wed Jun  7 17:17:41 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.2.2.tar", last modified: Mon Jun 12 01:17:12 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.2.1.tar` & `SmoobuExtractorFormatter-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 17:17:41.706864 SmoobuExtractorFormatter-1.2.1/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-07 17:17:41.705900 SmoobuExtractorFormatter-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 17:17:41.686382 SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0     8173 2023-06-07 17:17:24.000000 SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-07 17:17:41.703866 SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-07 17:17:41.000000 SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-07 17:17:41.000000 SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 17:17:41.000000 SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-07 17:17:41.000000 SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-07 17:17:41.000000 SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 17:17:41.706864 SmoobuExtractorFormatter-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-07 17:17:31.000000 SmoobuExtractorFormatter-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:17:11.997194 SmoobuExtractorFormatter-1.2.2/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-12 01:17:11.996197 SmoobuExtractorFormatter-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 01:17:11.971011 SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0    11097 2023-06-12 01:16:03.000000 SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:17:11.994229 SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-12 01:17:11.000000 SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-12 01:17:11.000000 SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 01:17:11.000000 SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-12 01:17:11.000000 SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-12 01:17:11.000000 SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 01:17:11.997194 SmoobuExtractorFormatter-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-12 01:15:57.000000 SmoobuExtractorFormatter-1.2.2/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.2.1/LICENSE.txt` & `SmoobuExtractorFormatter-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.2.1/PKG-INFO` & `SmoobuExtractorFormatter-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.1
+Version: 1.2.2
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.1/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.2.2/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.1
+Version: 1.2.2
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.1/setup.py` & `SmoobuExtractorFormatter-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.2.1',
+    version='1.2.2',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

