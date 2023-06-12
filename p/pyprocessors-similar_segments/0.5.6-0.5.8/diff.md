# Comparing `tmp/pyprocessors_similar_segments-0.5.6.tar.gz` & `tmp/pyprocessors_similar_segments-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_similar_segments-0.5.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors_similar_segments-0.5.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprocessors_similar_segments-0.5.6.tar` & `pyprocessors_similar_segments-0.5.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       97 2023-06-07 12:32:02.131814 pyprocessors_similar_segments-0.5.6/.dockerignore
--rw-r--r--   0        0        0      167 2023-06-07 12:32:02.133814 pyprocessors_similar_segments-0.5.6/.gitignore
--rw-r--r--   0        0        0      448 2023-06-07 12:32:02.133814 pyprocessors_similar_segments-0.5.6/Dockerfile
--rw-r--r--   0        0        0    10223 2023-06-07 12:37:56.541204 pyprocessors_similar_segments-0.5.6/Jenkinsfile
--rw-r--r--   0        0        0      380 2023-06-07 12:32:02.134814 pyprocessors_similar_segments-0.5.6/README.md
--rw-r--r--   0        0        0     1559 2023-06-07 12:32:02.134814 pyprocessors_similar_segments-0.5.6/bumpversion.py
--rw-r--r--   0        0        0       55 2023-06-07 12:40:09.173750 pyprocessors_similar_segments-0.5.6/pyprocessors_similar_segments/__init__.py
--rw-r--r--   0        0        0     3689 2023-06-07 12:32:02.135814 pyprocessors_similar_segments-0.5.6/pyprocessors_similar_segments/similar_segments.py
--rw-r--r--   0        0        0     2560 2023-06-07 12:32:02.136814 pyprocessors_similar_segments-0.5.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 12:32:02.136814 pyprocessors_similar_segments-0.5.6/tests/__init__.py
--rw-r--r--   0        0        0     5070 2023-06-07 12:32:02.136814 pyprocessors_similar_segments-0.5.6/tests/data/question_segments.json
--rw-r--r--   0        0        0     1024 2023-06-07 12:32:02.137814 pyprocessors_similar_segments-0.5.6/tests/test_similar_segments.py
--rw-r--r--   0        0        0      951 2023-06-07 12:32:02.137814 pyprocessors_similar_segments-0.5.6/tox.ini
--rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 pyprocessors_similar_segments-0.5.6/setup.py
--rw-r--r--   0        0        0     2482 1970-01-01 00:00:00.000000 pyprocessors_similar_segments-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-06-07 12:32:02.131814 pyprocessors_similar_segments-0.5.8/.dockerignore
+-rw-r--r--   0        0        0      167 2023-06-07 12:32:02.133814 pyprocessors_similar_segments-0.5.8/.gitignore
+-rw-r--r--   0        0        0      448 2023-06-07 12:32:02.133814 pyprocessors_similar_segments-0.5.8/Dockerfile
+-rw-r--r--   0        0        0    10223 2023-06-07 12:37:56.541204 pyprocessors_similar_segments-0.5.8/Jenkinsfile
+-rw-r--r--   0        0        0      380 2023-06-07 12:32:02.134814 pyprocessors_similar_segments-0.5.8/README.md
+-rw-r--r--   0        0        0     1559 2023-06-07 12:32:02.134814 pyprocessors_similar_segments-0.5.8/bumpversion.py
+-rw-r--r--   0        0        0       55 2023-06-07 12:42:40.339792 pyprocessors_similar_segments-0.5.8/pyprocessors_similar_segments/__init__.py
+-rw-r--r--   0        0        0     3689 2023-06-07 12:32:02.135814 pyprocessors_similar_segments-0.5.8/pyprocessors_similar_segments/similar_segments.py
+-rw-r--r--   0        0        0     2560 2023-06-07 12:32:02.136814 pyprocessors_similar_segments-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 12:32:02.136814 pyprocessors_similar_segments-0.5.8/tests/__init__.py
+-rw-r--r--   0        0        0     5070 2023-06-07 12:32:02.136814 pyprocessors_similar_segments-0.5.8/tests/data/question_segments.json
+-rw-r--r--   0        0        0     1024 2023-06-07 12:32:02.137814 pyprocessors_similar_segments-0.5.8/tests/test_similar_segments.py
+-rw-r--r--   0        0        0      951 2023-06-07 12:32:02.137814 pyprocessors_similar_segments-0.5.8/tox.ini
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 pyprocessors_similar_segments-0.5.8/setup.py
+-rw-r--r--   0        0        0     2482 1970-01-01 00:00:00.000000 pyprocessors_similar_segments-0.5.8/PKG-INFO
```

### Comparing `pyprocessors_similar_segments-0.5.6/Jenkinsfile` & `pyprocessors_similar_segments-0.5.8/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors_similar_segments-0.5.6/bumpversion.py` & `pyprocessors_similar_segments-0.5.8/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_similar_segments-0.5.6/pyprocessors_similar_segments/similar_segments.py` & `pyprocessors_similar_segments-0.5.8/pyprocessors_similar_segments/similar_segments.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_similar_segments-0.5.6/pyproject.toml` & `pyprocessors_similar_segments-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors_similar_segments-0.5.6/tests/data/question_segments.json` & `pyprocessors_similar_segments-0.5.8/tests/data/question_segments.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_similar_segments-0.5.6/tests/test_similar_segments.py` & `pyprocessors_similar_segments-0.5.8/tests/test_similar_segments.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_similar_segments-0.5.6/tox.ini` & `pyprocessors_similar_segments-0.5.8/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors_similar_segments-0.5.6/setup.py` & `pyprocessors_similar_segments-0.5.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           'flask==2.1.3']}
 
 entry_points = \
 {'pyprocessors.plugins': ['similar_segments = '
                           'pyprocessors_similar_segments.similar_segments:SimilarSegmentsProcessor']}
 
 setup(name='pyprocessors-similar_segments',
-      version='0.5.6',
+      version='0.5.8',
       description='Similar segments processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyprocessors_similar_segments-0.5.6/PKG-INFO` & `pyprocessors_similar_segments-0.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-similar_segments
-Version: 0.5.6
+Version: 0.5.8
 Summary: Similar segments processor
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

