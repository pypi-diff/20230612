# Comparing `tmp/SmplML-1.0.1.tar.gz` & `tmp/SmplML-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SmplML-1.0.1.tar", last modified: Mon Jun 12 03:45:40 2023, max compression
+gzip compressed data, was "dist\SmplML-1.0.2.tar", last modified: Mon Jun 12 04:16:35 2023, max compression
```

## Comparing `SmplML-1.0.1.tar` & `SmplML-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 03:45:40.155224 SmplML-1.0.1/
--rw-rw-rw-   0        0        0       89 2023-06-12 03:45:01.000000 SmplML-1.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1086 2023-06-12 03:44:56.000000 SmplML-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       30 2023-06-12 03:44:54.000000 SmplML-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1659 2023-06-12 03:45:40.153593 SmplML-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      649 2023-06-12 03:44:53.000000 SmplML-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 03:45:40.130393 SmplML-1.0.1/SmplML.egg-info/
--rw-rw-rw-   0        0        0     1659 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 03:45:40.155224 SmplML-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-06-12 03:44:50.000000 SmplML-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:45:40.144677 SmplML-1.0.1/smpl_ml/
--rw-rw-rw-   0        0        0       46 2023-06-12 03:44:49.000000 SmplML-1.0.1/smpl_ml/__init__.py
--rw-rw-rw-   0        0        0     8081 2023-06-12 02:47:59.000000 SmplML-1.0.1/smpl_ml/classification_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:16:35.144250 SmplML-1.0.2/
+-rw-rw-rw-   0        0        0       91 2023-06-12 04:14:53.000000 SmplML-1.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-12 03:44:56.000000 SmplML-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-06-12 03:44:54.000000 SmplML-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2767 2023-06-12 04:16:35.143238 SmplML-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1755 2023-06-12 04:14:55.000000 SmplML-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 04:16:35.136645 SmplML-1.0.2/SmplML.egg-info/
+-rw-rw-rw-   0        0        0     2767 2023-06-12 04:16:34.000000 SmplML-1.0.2/SmplML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-12 04:16:35.000000 SmplML-1.0.2/SmplML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 04:16:34.000000 SmplML-1.0.2/SmplML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-12 04:16:34.000000 SmplML-1.0.2/SmplML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 04:16:34.000000 SmplML-1.0.2/SmplML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 04:16:35.145232 SmplML-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-06-12 04:15:12.000000 SmplML-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:16:35.140752 SmplML-1.0.2/smpl_ml/
+-rw-rw-rw-   0        0        0       46 2023-06-12 03:44:49.000000 SmplML-1.0.2/smpl_ml/__init__.py
+-rw-rw-rw-   0        0        0     8081 2023-06-12 02:47:59.000000 SmplML-1.0.2/smpl_ml/classification_helpers.py
```

### Comparing `SmplML-1.0.1/LICENSE` & `SmplML-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SmplML-1.0.1/setup.py` & `SmplML-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  
 dependencies = ['pandas', 
                 'numpy', 
                 'scikit-learn']
 
 setup(
   name='SmplML',
-  version='1.0.1',
+  version='1.0.2',
   description=desc,
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/JhunBrian/SmplML',  
   author='Jhun Brian Andam',
   author_email='brianandam123@gmail.com',
   license='MIT',
```

### Comparing `SmplML-1.0.1/smpl_ml/classification_helpers.py` & `SmplML-1.0.2/smpl_ml/classification_helpers.py`

 * *Files identical despite different names*

