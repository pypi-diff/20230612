# Comparing `tmp/edxval-2.2.0.tar.gz` & `tmp/edxval-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edxval-2.2.0.tar", last modified: Tue Feb 22 10:33:49 2022, max compression
+gzip compressed data, was "edxval-2.3.0.tar", last modified: Mon Jun 12 11:15:24 2023, max compression
```

## Comparing `edxval-2.2.0.tar` & `edxval-2.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:33:49.545483 edxval-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35135 2022-02-22 10:33:43.000000 edxval-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-02-22 10:33:43.000000 edxval-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-02-22 10:33:49.545483 edxval-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-02-22 10:33:43.000000 edxval-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:33:49.541483 edxval-2.2.0/edxval/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    44550 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:33:49.541483 edxval-2.2.0/edxval/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/config/waffle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:33:49.541483 edxval-2.2.0/edxval/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    10986 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/migrations/0002_add_error_description_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/migrations/0003_delete_transcriptcredentials.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22828 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8154 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:33:49.545483 edxval-2.2.0/edxval/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10706 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)   129574 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2707 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5488 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3463 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/tests/test_transcript_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    42047 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     3768 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/transcript_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     8793 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14390 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-02-22 10:33:43.000000 edxval-2.2.0/edxval/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:33:49.541483 edxval-2.2.0/edxval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-02-22 10:33:49.000000 edxval-2.2.0/edxval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-02-22 10:33:49.000000 edxval-2.2.0/edxval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 10:33:49.000000 edxval-2.2.0/edxval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-22 10:33:49.000000 edxval-2.2.0/edxval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-22 10:33:49.000000 edxval-2.2.0/edxval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:33:49.545483 edxval-2.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-02-22 10:33:43.000000 edxval-2.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-02-22 10:33:43.000000 edxval-2.2.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-02-22 10:33:49.545483 edxval-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-02-22 10:33:43.000000 edxval-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-06-12 11:15:19.000000 edxval-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-12 11:15:19.000000 edxval-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-12 11:15:24.443369 edxval-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-06-12 11:15:19.000000 edxval-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.439369 edxval-2.3.0/edxval/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4084 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44550 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/edxval/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/config/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/edxval/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    10986 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/migrations/0002_add_error_description_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/migrations/0003_delete_transcriptcredentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22828 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/edxval/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10706 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)   129574 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5488 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3463 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_transcript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42047 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/transcript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8793 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14390 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/edxval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-12 11:15:19.000000 edxval-2.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-06-12 11:15:19.000000 edxval-2.3.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-12 11:15:24.443369 edxval-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-06-12 11:15:19.000000 edxval-2.3.0/setup.py
```

### Comparing `edxval-2.2.0/LICENSE` & `edxval-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/PKG-INFO` & `edxval-2.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: edxval
-Version: 2.2.0
+Version: 2.3.0
 Summary: edx-val
-Home-page: http://github.com/edx/edx-val
+Home-page: http://github.com/openedx/edx-val
 Author: edX
 License: AGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 edx-val
-
```

### Comparing `edxval-2.2.0/README.rst` & `edxval-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/admin.py` & `edxval-2.3.0/edxval/admin.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/api.py` & `edxval-2.3.0/edxval/api.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/config/waffle.py` & `edxval-2.3.0/edxval/config/waffle.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/exceptions.py` & `edxval-2.3.0/edxval/exceptions.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py` & `edxval-2.3.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/models.py` & `edxval-2.3.0/edxval/models.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/serializers.py` & `edxval-2.3.0/edxval/serializers.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/tests/__init__.py` & `edxval-2.3.0/edxval/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/tests/constants.py` & `edxval-2.3.0/edxval/tests/constants.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/tests/test_admin.py` & `edxval-2.3.0/edxval/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/tests/test_api.py` & `edxval-2.3.0/edxval/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/tests/test_models.py` & `edxval-2.3.0/edxval/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/tests/test_serializers.py` & `edxval-2.3.0/edxval/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/tests/test_transcript_utils.py` & `edxval-2.3.0/edxval/tests/test_transcript_utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/tests/test_utils.py` & `edxval-2.3.0/edxval/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/tests/test_views.py` & `edxval-2.3.0/edxval/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/transcript_utils.py` & `edxval-2.3.0/edxval/transcript_utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/urls.py` & `edxval-2.3.0/edxval/urls.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/utils.py` & `edxval-2.3.0/edxval/utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/views.py` & `edxval-2.3.0/edxval/views.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval/wsgi.py` & `edxval-2.3.0/edxval/wsgi.py`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/edxval.egg-info/PKG-INFO` & `edxval-2.3.0/edxval.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: edxval
-Version: 2.2.0
+Version: 2.3.0
 Summary: edx-val
-Home-page: http://github.com/edx/edx-val
+Home-page: http://github.com/openedx/edx-val
 Author: edX
 License: AGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 edx-val
-
```

### Comparing `edxval-2.2.0/edxval.egg-info/SOURCES.txt` & `edxval-2.3.0/edxval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/setup.cfg` & `edxval-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `edxval-2.2.0/setup.py` & `edxval-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     os.system("git push --tags")
     sys.exit()
 
 setup(
     name='edxval',
     version=VERSION,
     author='edX',
-    url='http://github.com/edx/edx-val',
+    url='http://github.com/openedx/edx-val',
     description='edx-val',
     long_description='edx-val',
     long_description_content_type='text/x-rst',
     license='AGPL',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

