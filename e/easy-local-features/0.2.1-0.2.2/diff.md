# Comparing `tmp/easy_local_features-0.2.1.tar.gz` & `tmp/easy_local_features-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_local_features-0.2.1.tar", last modified: Mon Jun 12 16:09:28 2023, max compression
+gzip compressed data, was "easy_local_features-0.2.2.tar", last modified: Mon Jun 12 16:13:21 2023, max compression
```

## Comparing `easy_local_features-0.2.1.tar` & `easy_local_features-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      927 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      773 2023-06-12 16:04:27.000000 easy_local_features-0.2.1/README.md
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.757359 easy_local_features-0.2.1/easy_local_features/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      327 2023-06-12 16:00:57.000000 easy_local_features-0.2.1/easy_local_features/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    34250 2023-06-12 15:41:05.000000 easy_local_features-0.2.1/easy_local_features/baseline_dalf.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2496 2023-06-12 15:18:17.000000 easy_local_features-0.2.1/easy_local_features/baseline_deal.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6102 2023-06-09 08:29:10.000000 easy_local_features-0.2.1/easy_local_features/baseline_disk.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4458 2023-06-09 08:29:10.000000 easy_local_features-0.2.1/easy_local_features/baseline_r2d2.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3979 2023-06-09 08:29:10.000000 easy_local_features-0.2.1/easy_local_features/baseline_superglue.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2063 2023-06-09 08:29:10.000000 easy_local_features-0.2.1/easy_local_features/baseline_superpoint.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/easy_local_features/datasets/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 07:43:29.000000 easy_local_features-0.2.1/easy_local_features/datasets/__init__.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3034 2023-06-12 07:45:31.000000 easy_local_features-0.2.1/easy_local_features/datasets/download.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.757359 easy_local_features-0.2.1/easy_local_features.egg-info/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      927 2023-06-12 16:09:28.000000 easy_local_features-0.2.1/easy_local_features.egg-info/PKG-INFO
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      575 2023-06-12 16:09:28.000000 easy_local_features-0.2.1/easy_local_features.egg-info/SOURCES.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-06-12 16:09:28.000000 easy_local_features-0.2.1/easy_local_features.egg-info/dependency_links.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       20 2023-06-12 16:09:28.000000 easy_local_features-0.2.1/easy_local_features.egg-info/top_level.txt
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       38 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/setup.cfg
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      548 2023-06-12 16:09:23.000000 easy_local_features-0.2.1/setup.py
-drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:09:28.761359 easy_local_features-0.2.1/tests/
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      112 2023-06-12 16:01:43.000000 easy_local_features-0.2.1/tests/test_dalf.py
--rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      112 2023-06-12 16:01:22.000000 easy_local_features-0.2.1/tests/test_deal.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:13:21.610086 easy_local_features-0.2.2/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      927 2023-06-12 16:13:21.610086 easy_local_features-0.2.2/PKG-INFO
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      773 2023-06-12 16:04:27.000000 easy_local_features-0.2.2/README.md
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:13:21.610086 easy_local_features-0.2.2/easy_local_features/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      327 2023-06-12 16:00:57.000000 easy_local_features-0.2.2/easy_local_features/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)    34250 2023-06-12 15:41:05.000000 easy_local_features-0.2.2/easy_local_features/baseline_dalf.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2496 2023-06-12 15:18:17.000000 easy_local_features-0.2.2/easy_local_features/baseline_deal.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     6102 2023-06-09 08:29:10.000000 easy_local_features-0.2.2/easy_local_features/baseline_disk.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     4458 2023-06-09 08:29:10.000000 easy_local_features-0.2.2/easy_local_features/baseline_r2d2.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3979 2023-06-09 08:29:10.000000 easy_local_features-0.2.2/easy_local_features/baseline_superglue.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     2063 2023-06-09 08:29:10.000000 easy_local_features-0.2.2/easy_local_features/baseline_superpoint.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:13:21.610086 easy_local_features-0.2.2/easy_local_features/datasets/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 07:43:29.000000 easy_local_features-0.2.2/easy_local_features/datasets/__init__.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)     3034 2023-06-12 07:45:31.000000 easy_local_features-0.2.2/easy_local_features/datasets/download.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:13:21.610086 easy_local_features-0.2.2/easy_local_features.egg-info/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      927 2023-06-12 16:13:21.000000 easy_local_features-0.2.2/easy_local_features.egg-info/PKG-INFO
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      575 2023-06-12 16:13:21.000000 easy_local_features-0.2.2/easy_local_features.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)        1 2023-06-12 16:13:21.000000 easy_local_features-0.2.2/easy_local_features.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       20 2023-06-12 16:13:21.000000 easy_local_features-0.2.2/easy_local_features.egg-info/top_level.txt
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)       38 2023-06-12 16:13:21.610086 easy_local_features-0.2.2/setup.cfg
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      760 2023-06-12 16:13:02.000000 easy_local_features-0.2.2/setup.py
+drwxrwxr-x   0 felipecadar  (1002) felipecadar  (1002)        0 2023-06-12 16:13:21.610086 easy_local_features-0.2.2/tests/
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      112 2023-06-12 16:01:43.000000 easy_local_features-0.2.2/tests/test_dalf.py
+-rw-rw-r--   0 felipecadar  (1002) felipecadar  (1002)      112 2023-06-12 16:01:22.000000 easy_local_features-0.2.2/tests/test_deal.py
```

### Comparing `easy_local_features-0.2.1/PKG-INFO` & `easy_local_features-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_local_features
-Version: 0.2.1
+Version: 0.2.2
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
 
 # easy-local-features-baselines
 
 Just some scripts to make things easier for the local features baselines.
```

### Comparing `easy_local_features-0.2.1/README.md` & `easy_local_features-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.1/easy_local_features/baseline_dalf.py` & `easy_local_features-0.2.2/easy_local_features/baseline_dalf.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.1/easy_local_features/baseline_deal.py` & `easy_local_features-0.2.2/easy_local_features/baseline_deal.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.1/easy_local_features/baseline_disk.py` & `easy_local_features-0.2.2/easy_local_features/baseline_disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.1/easy_local_features/baseline_r2d2.py` & `easy_local_features-0.2.2/easy_local_features/baseline_r2d2.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.1/easy_local_features/baseline_superglue.py` & `easy_local_features-0.2.2/easy_local_features/baseline_superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.1/easy_local_features/baseline_superpoint.py` & `easy_local_features-0.2.2/easy_local_features/baseline_superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.1/easy_local_features/datasets/download.py` & `easy_local_features-0.2.2/easy_local_features/datasets/download.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.1/easy_local_features.egg-info/PKG-INFO` & `easy_local_features-0.2.2/easy_local_features.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-local-features
-Version: 0.2.1
+Version: 0.2.2
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
 
 # easy-local-features-baselines
 
 Just some scripts to make things easier for the local features baselines.
```

### Comparing `easy_local_features-0.2.1/easy_local_features.egg-info/SOURCES.txt` & `easy_local_features-0.2.2/easy_local_features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.2.1/setup.py` & `easy_local_features-0.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+import sys
 from setuptools import setup, find_packages
 
-try:
-    import pypandoc
-    long_description = pypandoc.convert_file('README.md', 'rst')
-except(IOError, ImportError):
-    long_description = open('README.md').read()
+# try:
+#     import pypandoc
+#     long_description = pypandoc.convert_file('README.md', 'rst')
+# except(IOError, ImportError):
+#     long_description = open('README.md').read()
+
+if sys.version_info[0] < 3:
+    with open('README.md') as f:
+        long_description = f.read()
+else:
+    with open('README.md', encoding='utf-8') as f:
+        long_description = f.read()
 
 setup(
     name='easy_local_features',
-    version='0.2.1',
+    version='0.2.2',
     author='eucadar',
     author_email='python@eucadar.com',
     packages=find_packages(exclude=('tests', 'docs', 'assets')),
     include_package_data=True,
     install_requires=[],
-    long_description=long_description,
     long_description_content_type='text/markdown',
+    long_description=long_description,
 )
```

