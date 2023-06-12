# Comparing `tmp/FileHarvester-0.0.tar.gz` & `tmp/FileHarvester-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileHarvester-0.0.tar", last modified: Mon Jun 12 09:03:44 2023, max compression
+gzip compressed data, was "FileHarvester-0.1.tar", last modified: Mon Jun 12 09:05:03 2023, max compression
```

## Comparing `FileHarvester-0.0.tar` & `FileHarvester-0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-12 09:03:44.072885 FileHarvester-0.0/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-12 09:03:44.072885 FileHarvester-0.0/FileHarvester/
--rw-r--r--   0 kali      (1000) kali      (1000)     4648 2018-06-19 23:16:08.000000 FileHarvester-0.0/FileHarvester/Binomialdistribution.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7787 2023-06-11 14:25:09.000000 FileHarvester-0.0/FileHarvester/Fharvester.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3631 2018-06-19 23:16:08.000000 FileHarvester-0.0/FileHarvester/Gaussiandistribution.py
--rw-r--r--   0 kali      (1000) kali      (1000)      932 2018-06-19 23:16:08.000000 FileHarvester-0.0/FileHarvester/Generaldistribution.py
--rw-r--r--   0 kali      (1000) kali      (1000)       86 2018-06-19 23:16:08.000000 FileHarvester-0.0/FileHarvester/__init__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-12 09:03:44.072885 FileHarvester-0.0/FileHarvester.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      124 2023-06-12 09:03:43.000000 FileHarvester-0.0/FileHarvester.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      369 2023-06-12 09:03:44.000000 FileHarvester-0.0/FileHarvester.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-06-12 09:03:43.000000 FileHarvester-0.0/FileHarvester.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-06-12 09:03:43.000000 FileHarvester-0.0/FileHarvester.egg-info/not-zip-safe
--rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-06-12 09:03:43.000000 FileHarvester-0.0/FileHarvester.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      124 2023-06-12 09:03:44.072885 FileHarvester-0.0/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-06-12 09:03:44.072885 FileHarvester-0.0/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      614 2023-06-12 09:03:40.000000 FileHarvester-0.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-12 09:05:03.452963 FileHarvester-0.1/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-12 09:05:03.448963 FileHarvester-0.1/FileHarvester/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4648 2018-06-19 23:16:08.000000 FileHarvester-0.1/FileHarvester/Binomialdistribution.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7787 2023-06-11 14:25:09.000000 FileHarvester-0.1/FileHarvester/Fharvester.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3631 2018-06-19 23:16:08.000000 FileHarvester-0.1/FileHarvester/Gaussiandistribution.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      932 2018-06-19 23:16:08.000000 FileHarvester-0.1/FileHarvester/Generaldistribution.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       86 2018-06-19 23:16:08.000000 FileHarvester-0.1/FileHarvester/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-06-12 09:05:03.452963 FileHarvester-0.1/FileHarvester.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      124 2023-06-12 09:05:03.000000 FileHarvester-0.1/FileHarvester.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      369 2023-06-12 09:05:03.000000 FileHarvester-0.1/FileHarvester.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-06-12 09:05:03.000000 FileHarvester-0.1/FileHarvester.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-06-12 09:03:43.000000 FileHarvester-0.1/FileHarvester.egg-info/not-zip-safe
+-rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-06-12 09:05:03.000000 FileHarvester-0.1/FileHarvester.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      124 2023-06-12 09:05:03.452963 FileHarvester-0.1/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-06-12 09:05:03.452963 FileHarvester-0.1/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      610 2023-06-12 09:05:00.000000 FileHarvester-0.1/setup.py
```

### Comparing `FileHarvester-0.0/FileHarvester/Binomialdistribution.py` & `FileHarvester-0.1/FileHarvester/Binomialdistribution.py`

 * *Files identical despite different names*

### Comparing `FileHarvester-0.0/FileHarvester/Fharvester.py` & `FileHarvester-0.1/FileHarvester/Fharvester.py`

 * *Files identical despite different names*

### Comparing `FileHarvester-0.0/FileHarvester/Gaussiandistribution.py` & `FileHarvester-0.1/FileHarvester/Gaussiandistribution.py`

 * *Files identical despite different names*

### Comparing `FileHarvester-0.0/FileHarvester/Generaldistribution.py` & `FileHarvester-0.1/FileHarvester/Generaldistribution.py`

 * *Files identical despite different names*

### Comparing `FileHarvester-0.0/setup.py` & `FileHarvester-0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from setuptools import setup
 
 setup(name='FileHarvester',
-      version='0.0',
+      version='0.1',
       description='''
 	Документация
-	
 	Список функций:
-	
 	Fharvester.create_file(name = "test.txt", text = "Hello \nworld \n!")
 	Fharvester.count_line_by_line(name = "test.txt")
 	Fharvester.overwrite_file(name = "test.txt", text = "Hello world !")
 	Fharvester.general_reading(name = "test.txt")
 	Fharvester.list_of_files("test.txt")
 	Fharvester.append_file(name = "test.txt", text = "Hello world !")
       ''',
```

