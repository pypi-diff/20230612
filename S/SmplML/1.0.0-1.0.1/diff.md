# Comparing `tmp/SmplML-1.0.0.tar.gz` & `tmp/SmplML-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SmplML-1.0.0.tar", last modified: Mon Jun 12 03:32:10 2023, max compression
+gzip compressed data, was "dist\SmplML-1.0.1.tar", last modified: Mon Jun 12 03:45:40 2023, max compression
```

## Comparing `SmplML-1.0.0.tar` & `SmplML-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 03:32:10.270201 SmplML-1.0.0/
--rw-rw-rw-   0        0        0       89 2023-06-12 02:47:59.000000 SmplML-1.0.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1086 2023-06-12 03:31:27.000000 SmplML-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       30 2023-06-12 02:51:43.000000 SmplML-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1659 2023-06-12 03:32:10.269194 SmplML-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      649 2023-06-12 03:31:30.000000 SmplML-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 03:32:10.265205 SmplML-1.0.0/SmplML.egg-info/
--rw-rw-rw-   0        0        0     1659 2023-06-12 03:32:09.000000 SmplML-1.0.0/SmplML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-12 03:32:10.000000 SmplML-1.0.0/SmplML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 03:32:09.000000 SmplML-1.0.0/SmplML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-12 03:32:09.000000 SmplML-1.0.0/SmplML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 03:32:09.000000 SmplML-1.0.0/SmplML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 03:32:10.270201 SmplML-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-06-12 03:31:38.000000 SmplML-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:32:10.267233 SmplML-1.0.0/smpl_ml/
--rw-rw-rw-   0        0        0     8081 2023-06-12 02:47:59.000000 SmplML-1.0.0/smpl_ml/classification_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:45:40.155224 SmplML-1.0.1/
+-rw-rw-rw-   0        0        0       89 2023-06-12 03:45:01.000000 SmplML-1.0.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-12 03:44:56.000000 SmplML-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-06-12 03:44:54.000000 SmplML-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1659 2023-06-12 03:45:40.153593 SmplML-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      649 2023-06-12 03:44:53.000000 SmplML-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 03:45:40.130393 SmplML-1.0.1/SmplML.egg-info/
+-rw-rw-rw-   0        0        0     1659 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 03:45:39.000000 SmplML-1.0.1/SmplML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 03:45:40.155224 SmplML-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-06-12 03:44:50.000000 SmplML-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 03:45:40.144677 SmplML-1.0.1/smpl_ml/
+-rw-rw-rw-   0        0        0       46 2023-06-12 03:44:49.000000 SmplML-1.0.1/smpl_ml/__init__.py
+-rw-rw-rw-   0        0        0     8081 2023-06-12 02:47:59.000000 SmplML-1.0.1/smpl_ml/classification_helpers.py
```

### Comparing `SmplML-1.0.0/LICENSE` & `SmplML-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SmplML-1.0.0/PKG-INFO` & `SmplML-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmplML
-Version: 1.0.0
+Version: 1.0.1
 Summary: SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive modules for data preprocessing, feature engineering, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies classification tasks, enabling you to gain valuable insights from your data with ease.
 Home-page: https://github.com/JhunBrian/SmplML
 Author: Jhun Brian Andam
 Author-email: brianandam123@gmail.com
 License: MIT
 Keywords: Machine Learning,Classification
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,10 +24,10 @@
 - Data preprocessing: Easily handle encoding categorical variables.
 - Model training: Train various classification models with just a few lines of code.
 - Model evaluation: Evaluate model performance using common metrics and visualizations.
 
 Change Log
 ==================
 
-1.0.0 (06/12/2023)
+1.0.1 (06/12/2023)
 ------------------
 Initial Version
```

### Comparing `SmplML-1.0.0/README.md` & `SmplML-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `SmplML-1.0.0/SmplML.egg-info/PKG-INFO` & `SmplML-1.0.1/SmplML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmplML
-Version: 1.0.0
+Version: 1.0.1
 Summary: SmplML is a user-friendly Python library for streamlined machine learning classification. It offers intuitive modules for data preprocessing, feature engineering, model training, and evaluation. Ideal for beginners and experts alike, SmplML simplifies classification tasks, enabling you to gain valuable insights from your data with ease.
 Home-page: https://github.com/JhunBrian/SmplML
 Author: Jhun Brian Andam
 Author-email: brianandam123@gmail.com
 License: MIT
 Keywords: Machine Learning,Classification
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,10 +24,10 @@
 - Data preprocessing: Easily handle encoding categorical variables.
 - Model training: Train various classification models with just a few lines of code.
 - Model evaluation: Evaluate model performance using common metrics and visualizations.
 
 Change Log
 ==================
 
-1.0.0 (06/12/2023)
+1.0.1 (06/12/2023)
 ------------------
 Initial Version
```

### Comparing `SmplML-1.0.0/setup.py` & `SmplML-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  
 dependencies = ['pandas', 
                 'numpy', 
                 'scikit-learn']
 
 setup(
   name='SmplML',
-  version='1.0.0',
+  version='1.0.1',
   description=desc,
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/JhunBrian/SmplML',  
   author='Jhun Brian Andam',
   author_email='brianandam123@gmail.com',
   license='MIT',
```

### Comparing `SmplML-1.0.0/smpl_ml/classification_helpers.py` & `SmplML-1.0.1/smpl_ml/classification_helpers.py`

 * *Files identical despite different names*

