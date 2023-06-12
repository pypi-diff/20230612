# Comparing `tmp/qsm_forward-0.2.tar.gz` & `tmp/qsm_forward-0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsm_forward-0.2.tar", last modified: Mon Jun 12 06:45:29 2023, max compression
+gzip compressed data, was "qsm_forward-0.2.post1.tar", last modified: Mon Jun 12 07:02:25 2023, max compression
```

## Comparing `qsm_forward-0.2.tar` & `qsm_forward-0.2.post1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 06:45:29.364277 qsm_forward-0.2/
--rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm_forward-0.2/LICENSE
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-12 06:45:29.364277 qsm_forward-0.2/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm_forward-0.2/README.md
--rw-r--r--   0 ashley    (1000) ashley    (1000)      750 2023-06-12 05:21:02.000000 qsm_forward-0.2/pyproject.toml
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 06:45:29.364277 qsm_forward-0.2/qsm_forward/
--rw-r--r--   0 ashley    (1000) ashley    (1000)      397 2023-06-12 05:17:28.000000 qsm_forward-0.2/qsm_forward/__init__.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)    11979 2023-06-12 05:17:28.000000 qsm_forward-0.2/qsm_forward/qsm_forward.py
--rw-r--r--   0 ashley    (1000) ashley    (1000)     8139 2023-06-12 05:17:28.000000 qsm_forward-0.2/qsm_forward/visualisation.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 06:45:29.364277 qsm_forward-0.2/qsm_forward.egg-info/
--rw-r--r--   0 ashley    (1000) ashley    (1000)     1342 2023-06-12 06:45:29.000000 qsm_forward-0.2/qsm_forward.egg-info/PKG-INFO
--rw-r--r--   0 ashley    (1000) ashley    (1000)      321 2023-06-12 06:45:29.000000 qsm_forward-0.2/qsm_forward.egg-info/SOURCES.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-12 06:45:29.000000 qsm_forward-0.2/qsm_forward.egg-info/dependency_links.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       67 2023-06-12 06:45:29.000000 qsm_forward-0.2/qsm_forward.egg-info/requires.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-12 06:45:29.000000 qsm_forward-0.2/qsm_forward.egg-info/top_level.txt
--rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-12 06:45:29.364277 qsm_forward-0.2/setup.cfg
--rw-r--r--   0 ashley    (1000) ashley    (1000)      914 2023-06-12 06:43:30.000000 qsm_forward-0.2/setup.py
-drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 06:45:29.364277 qsm_forward-0.2/tests/
--rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm_forward-0.2/tests/test_qsm_forward.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    35149 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/LICENSE
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      571 2023-06-12 04:37:47.000000 qsm_forward-0.2.post1/README.md
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      752 2023-06-12 07:02:11.000000 qsm_forward-0.2.post1/pyproject.toml
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/qsm_forward/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      397 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/qsm_forward/__init__.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)    11979 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/qsm_forward/qsm_forward.py
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     8139 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/qsm_forward/visualisation.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/qsm_forward.egg-info/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)     1348 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/PKG-INFO
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      321 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        1 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       67 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/requires.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       12 2023-06-12 07:02:25.000000 qsm_forward-0.2.post1/qsm_forward.egg-info/top_level.txt
+-rw-r--r--   0 ashley    (1000) ashley    (1000)       38 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/setup.cfg
+-rw-r--r--   0 ashley    (1000) ashley    (1000)      916 2023-06-12 07:02:07.000000 qsm_forward-0.2.post1/setup.py
+drwxr-xr-x   0 ashley    (1000) ashley    (1000)        0 2023-06-12 07:02:25.984252 qsm_forward-0.2.post1/tests/
+-rw-r--r--   0 ashley    (1000) ashley    (1000)        6 2023-06-12 05:17:28.000000 qsm_forward-0.2.post1/tests/test_qsm_forward.py
```

### Comparing `qsm_forward-0.2/LICENSE` & `qsm_forward-0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2/PKG-INFO` & `qsm_forward-0.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qsm_forward
-Version: 0.2
+Version: 0.2.post1
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
-Home-page: https://github.com/astewartau/qsm_forward_model
+Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
-Project-URL: Homepage, https://github.com/astewartau/qsm_forward_model
-Project-URL: Bug Tracker, https://github.com/astewartau/qsm_forward_model/issues
+Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
+Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `qsm_forward-0.2/README.md` & `qsm_forward-0.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2/pyproject.toml` & `qsm_forward-0.2.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qsm_forward"
-version = "0.2"
+version = "0.2-1"
 authors = [
   { name="Ashley Stewart", email="a.stewart.au@gmail.com" },
 ]
 description = "A forward-model simulation for Quantitative Susceptibility Mapping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
@@ -16,9 +16,9 @@
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/astewartau/qsm_forward_model"
-"Bug Tracker" = "https://github.com/astewartau/qsm_forward_model/issues"
+"Homepage" = "https://github.com/astewartau/qsm-forward-model"
+"Bug Tracker" = "https://github.com/astewartau/qsm-forward-model/issues"
```

### Comparing `qsm_forward-0.2/qsm_forward/qsm_forward.py` & `qsm_forward-0.2.post1/qsm_forward/qsm_forward.py`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2/qsm_forward/visualisation.py` & `qsm_forward-0.2.post1/qsm_forward/visualisation.py`

 * *Files identical despite different names*

### Comparing `qsm_forward-0.2/qsm_forward.egg-info/PKG-INFO` & `qsm_forward-0.2.post1/qsm_forward.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qsm-forward
-Version: 0.2
+Version: 0.2.post1
 Summary: A forward-model simulation for Quantitative Susceptibility Mapping
-Home-page: https://github.com/astewartau/qsm_forward_model
+Home-page: https://github.com/astewartau/qsm-forward-model
 Author: Ashley Stewart
 Author-email: Ashley Stewart <a.stewart.au@gmail.com>
-Project-URL: Homepage, https://github.com/astewartau/qsm_forward_model
-Project-URL: Bug Tracker, https://github.com/astewartau/qsm_forward_model/issues
+Project-URL: Homepage, https://github.com/astewartau/qsm-forward-model
+Project-URL: Bug Tracker, https://github.com/astewartau/qsm-forward-model/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `qsm_forward-0.2/setup.py` & `qsm_forward-0.2.post1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='qsm_forward',
-    version='0.2',
+    version='0.2-2',
     packages=find_packages(),
-    url='https://github.com/astewartau/qsm_forward_model',
+    url='https://github.com/astewartau/qsm-forward-model',
     author='Ashley Stewart',
     author_email='a.stewart.au@gmail.com',
     description='A forward-model simulation for Quantitative Susceptibility Mapping',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'numpy',
```

