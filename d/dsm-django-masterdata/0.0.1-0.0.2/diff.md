# Comparing `tmp/dsm_django_masterdata-0.0.1.tar.gz` & `tmp/dsm_django_masterdata-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsm_django_masterdata-0.0.1.tar", last modified: Mon Jun 12 15:34:45 2023, max compression
+gzip compressed data, was "dsm_django_masterdata-0.0.2.tar", last modified: Mon Jun 12 15:36:22 2023, max compression
```

## Comparing `dsm_django_masterdata-0.0.1.tar` & `dsm_django_masterdata-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:34:45.957074 dsm_django_masterdata-0.0.1/
--rw-r--r--   0 naii       (501) staff       (20)      984 2023-06-12 15:34:45.956579 dsm_django_masterdata-0.0.1/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      375 2023-06-12 15:17:45.000000 dsm_django_masterdata-0.0.1/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:34:45.930282 dsm_django_masterdata-0.0.1/dsm_django_masterdata/
--rw-r--r--   0 naii       (501) staff       (20)      153 2023-06-12 15:33:11.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      165 2023-06-12 15:30:14.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata/apps.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:34:45.936498 dsm_django_masterdata-0.0.1/dsm_django_masterdata/hscode/
--rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:43:46.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata/hscode/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      327 2023-06-12 10:06:08.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata/hscode/admin.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:34:45.950304 dsm_django_masterdata-0.0.1/dsm_django_masterdata/hscode/migrations/
--rw-r--r--   0 naii       (501) staff       (20)     1093 2023-06-12 15:25:37.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata/hscode/migrations/0001_initial.py
--rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:50:06.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata/hscode/migrations/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      395 2023-06-12 11:19:07.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata/hscode/models.py
--rw-r--r--   0 naii       (501) staff       (20)       60 2023-06-12 09:43:33.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata/tests.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:34:45.933543 dsm_django_masterdata-0.0.1/dsm_django_masterdata.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)      984 2023-06-12 15:34:45.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      563 2023-06-12 15:34:45.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-06-12 15:34:45.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       15 2023-06-12 15:34:45.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       22 2023-06-12 15:34:45.000000 dsm_django_masterdata-0.0.1/dsm_django_masterdata.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-06-12 15:34:45.957219 dsm_django_masterdata-0.0.1/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1315 2023-06-12 15:34:26.000000 dsm_django_masterdata-0.0.1/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.201526 dsm_django_masterdata-0.0.2/
+-rw-r--r--   0 naii       (501) staff       (20)      995 2023-06-12 15:36:22.200716 dsm_django_masterdata-0.0.2/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      386 2023-06-12 15:35:40.000000 dsm_django_masterdata-0.0.2/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.192579 dsm_django_masterdata-0.0.2/dsm_django_masterdata/
+-rw-r--r--   0 naii       (501) staff       (20)      153 2023-06-12 15:36:06.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      165 2023-06-12 15:30:14.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/apps.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.198243 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/
+-rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:43:46.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      327 2023-06-12 10:06:08.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/admin.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.199945 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/migrations/
+-rw-r--r--   0 naii       (501) staff       (20)     1093 2023-06-12 15:25:37.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/migrations/0001_initial.py
+-rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:50:06.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/migrations/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      395 2023-06-12 11:19:07.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/models.py
+-rw-r--r--   0 naii       (501) staff       (20)       60 2023-06-12 09:43:33.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/tests.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.196671 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)      995 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      563 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       15 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       22 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-06-12 15:36:22.201715 dsm_django_masterdata-0.0.2/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     1315 2023-06-12 15:36:16.000000 dsm_django_masterdata-0.0.2/setup.py
```

### Comparing `dsm_django_masterdata-0.0.1/PKG-INFO` & `dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dsm_django_masterdata
-Version: 0.0.1
+Name: dsm-django-masterdata
+Version: 0.0.2
 Summary: A simple way to use Master Data in django project.
 Home-page: https://github.com/storemesh/masterdata/tree/django-app
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 ```
 pip install dsm_master
 ```
 1. install django app in `settings.py`
 ```python
 INSTALLED_APPS = [
     ...
-    'dsm_master.hscode',
+    'dsm_django_masterdata.hscode',
     ...
 ]
 ```
 
 2. migrate database
 ```
 python manage.py migrate
```

### Comparing `dsm_django_masterdata-0.0.1/dsm_django_masterdata/hscode/migrations/0001_initial.py` & `dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dsm_django_masterdata-0.0.1/dsm_django_masterdata.egg-info/PKG-INFO` & `dsm_django_masterdata-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dsm-django-masterdata
-Version: 0.0.1
+Name: dsm_django_masterdata
+Version: 0.0.2
 Summary: A simple way to use Master Data in django project.
 Home-page: https://github.com/storemesh/masterdata/tree/django-app
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 ```
 pip install dsm_master
 ```
 1. install django app in `settings.py`
 ```python
 INSTALLED_APPS = [
     ...
-    'dsm_master.hscode',
+    'dsm_django_masterdata.hscode',
     ...
 ]
 ```
 
 2. migrate database
 ```
 python manage.py migrate
```

### Comparing `dsm_django_masterdata-0.0.1/dsm_django_masterdata.egg-info/SOURCES.txt` & `dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsm_django_masterdata-0.0.1/setup.py` & `dsm_django_masterdata-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 setup(
     name='dsm_django_masterdata',
-    version='0.0.1',
+    version='0.0.2',
     url='https://github.com/storemesh/masterdata/tree/django-app',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple way to use Master Data in django project.',
     long_description=README,
     long_description_content_type='text/markdown',
```

