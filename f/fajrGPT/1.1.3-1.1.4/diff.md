# Comparing `tmp/fajrGPT-1.1.3.tar.gz` & `tmp/fajrGPT-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.1.3.tar", last modified: Mon Jun 12 01:12:22 2023, max compression
+gzip compressed data, was "fajrGPT-1.1.4.tar", last modified: Mon Jun 12 01:14:39 2023, max compression
```

## Comparing `fajrGPT-1.1.3.tar` & `fajrGPT-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:12:22.833497 fajrGPT-1.1.3/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.1.3/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:12:22.833320 fajrGPT-1.1.3/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.1.3/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:12:22.831897 fajrGPT-1.1.3/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.1.3/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)     8174 2023-06-12 00:57:29.000000 fajrGPT-1.1.3/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:12:22.833093 fajrGPT-1.1.3/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:12:22.000000 fajrGPT-1.1.3/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      256 2023-06-12 01:12:22.000000 fajrGPT-1.1.3/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-12 01:12:22.000000 fajrGPT-1.1.3/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-06-12 01:12:22.000000 fajrGPT-1.1.3/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-06-12 01:12:22.000000 fajrGPT-1.1.3/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-12 01:12:22.000000 fajrGPT-1.1.3/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-06-12 01:12:22.833538 fajrGPT-1.1.3/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-06-12 01:11:16.000000 fajrGPT-1.1.3/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:39.850556 fajrGPT-1.1.4/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.1.4/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:14:39.850360 fajrGPT-1.1.4/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.1.4/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:39.848515 fajrGPT-1.1.4/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.1.4/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-05-15 07:45:19.000000 fajrGPT-1.1.4/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)     8174 2023-06-12 00:57:29.000000 fajrGPT-1.1.4/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:39.850113 fajrGPT-1.1.4/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-06-12 01:14:39.000000 fajrGPT-1.1.4/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-06-12 01:14:39.000000 fajrGPT-1.1.4/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-06-12 01:14:39.000000 fajrGPT-1.1.4/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-06-12 01:14:39.000000 fajrGPT-1.1.4/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-06-12 01:14:39.000000 fajrGPT-1.1.4/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-06-12 01:14:39.000000 fajrGPT-1.1.4/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-06-12 01:14:39.850609 fajrGPT-1.1.4/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-06-12 01:14:37.000000 fajrGPT-1.1.4/setup.py
```

### Comparing `fajrGPT-1.1.3/LICENSE` & `fajrGPT-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.3/PKG-INFO` & `fajrGPT-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.1.3/README.md` & `fajrGPT-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.3/fajrGPT/quran_metadata.py` & `fajrGPT-1.1.4/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.3/fajrGPT/wake.py` & `fajrGPT-1.1.4/fajrGPT/wake.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.1.3/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.1.4/fajrGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.1.3/setup.py` & `fajrGPT-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.1.3",
+    version="1.1.4",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

