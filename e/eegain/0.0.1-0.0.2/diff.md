# Comparing `tmp/eegain-0.0.1.tar.gz` & `tmp/eegain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eegain-0.0.1.tar", last modified: Sun May 28 12:13:20 2023, max compression
+gzip compressed data, was "dist/eegain-0.0.2.tar", last modified: Mon Jun 12 06:57:57 2023, max compression
```

## Comparing `eegain-0.0.1.tar` & `eegain-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-28 12:13:20.755289 eegain-0.0.1/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      863 2023-05-28 12:13:20.755289 eegain-0.0.1/PKG-INFO
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       12 2023-05-28 12:05:25.000000 eegain-0.0.1/README.md
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-28 12:13:20.755289 eegain-0.0.1/eegain/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       99 2023-05-28 12:05:26.000000 eegain-0.0.1/eegain/__init__.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-28 12:13:20.755289 eegain-0.0.1/eegain/data/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       36 2023-05-28 00:17:16.000000 eegain-0.0.1/eegain/data/__init__.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       78 2023-05-28 12:08:09.000000 eegain-0.0.1/eegain/data/factory.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-28 12:13:20.755289 eegain-0.0.1/eegain/models/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       34 2023-05-28 11:04:36.000000 eegain-0.0.1/eegain/models/__init__.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       76 2023-05-28 12:08:09.000000 eegain-0.0.1/eegain/models/factory.py
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       22 2023-05-28 12:08:09.000000 eegain-0.0.1/eegain/version.py
-drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-05-28 12:13:20.755289 eegain-0.0.1/eegain.egg-info/
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      863 2023-05-28 12:13:20.000000 eegain-0.0.1/eegain.egg-info/PKG-INFO
--rw-rw-r--   0 raphael   (1000) raphael   (1000)      273 2023-05-28 12:13:20.000000 eegain-0.0.1/eegain.egg-info/SOURCES.txt
--rw-rw-r--   0 raphael   (1000) raphael   (1000)        1 2023-05-28 12:13:20.000000 eegain-0.0.1/eegain.egg-info/dependency_links.txt
--rw-rw-r--   0 raphael   (1000) raphael   (1000)        7 2023-05-28 12:13:20.000000 eegain-0.0.1/eegain.egg-info/top_level.txt
--rw-rw-r--   0 raphael   (1000) raphael   (1000)       38 2023-05-28 12:13:20.755289 eegain-0.0.1/setup.cfg
--rw-rw-r--   0 raphael   (1000) raphael   (1000)     1174 2023-05-28 12:12:18.000000 eegain-0.0.1/setup.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-06-12 06:57:57.828747 eegain-0.0.2/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      863 2023-06-12 06:57:57.828747 eegain-0.0.2/PKG-INFO
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       12 2023-05-28 12:05:25.000000 eegain-0.0.2/README.md
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-06-12 06:57:57.828747 eegain-0.0.2/eegain/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      102 2023-06-11 16:48:58.000000 eegain-0.0.2/eegain/__init__.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-06-12 06:57:57.828747 eegain-0.0.2/eegain/data/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       34 2023-06-02 21:40:19.000000 eegain-0.0.2/eegain/data/__init__.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3572 2023-06-11 16:48:58.000000 eegain-0.0.2/eegain/data/datasets.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3049 2023-06-11 16:48:58.000000 eegain-0.0.2/eegain/data/loader.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-06-12 06:57:57.828747 eegain-0.0.2/eegain/models/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      175 2023-06-11 16:48:58.000000 eegain-0.0.2/eegain/models/__init__.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      171 2023-06-11 15:47:06.000000 eegain-0.0.2/eegain/models/_registry.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     4932 2023-06-12 06:36:10.000000 eegain-0.0.2/eegain/models/conformer.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3320 2023-06-11 16:42:27.000000 eegain-0.0.2/eegain/models/deepconvnet.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3762 2023-06-11 16:42:27.000000 eegain-0.0.2/eegain/models/eegnet.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2134 2023-06-11 16:42:27.000000 eegain-0.0.2/eegain/models/shallowconvnet.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     2703 2023-06-11 16:48:58.000000 eegain-0.0.2/eegain/models/tsception.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-06-12 06:57:57.828747 eegain-0.0.2/eegain/transforms/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       26 2023-06-03 11:26:43.000000 eegain-0.0.2/eegain/transforms/__init__.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     3736 2023-06-11 16:48:58.000000 eegain-0.0.2/eegain/transforms/transforms.py
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       22 2023-06-12 06:57:54.000000 eegain-0.0.2/eegain/version.py
+drwxrwxr-x   0 raphael   (1000) raphael   (1000)        0 2023-06-12 06:57:57.828747 eegain-0.0.2/eegain.egg-info/
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      863 2023-06-12 06:57:57.000000 eegain-0.0.2/eegain.egg-info/PKG-INFO
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)      499 2023-06-12 06:57:57.000000 eegain-0.0.2/eegain.egg-info/SOURCES.txt
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)        1 2023-06-12 06:57:57.000000 eegain-0.0.2/eegain.egg-info/dependency_links.txt
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)        7 2023-06-12 06:57:57.000000 eegain-0.0.2/eegain.egg-info/top_level.txt
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)       38 2023-06-12 06:57:57.828747 eegain-0.0.2/setup.cfg
+-rw-rw-r--   0 raphael   (1000) raphael   (1000)     1175 2023-06-06 16:39:25.000000 eegain-0.0.2/setup.py
```

### Comparing `eegain-0.0.1/PKG-INFO` & `eegain-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eegain
-Version: 0.0.1
+Version: 0.0.2
 Summary: EEG emotion recognition package for standardization
 Home-page: https://github.com/RRaphaell/EEGain
 Author: GAIN Team
 Author-email: 
 Keywords: EEG,emotion recognition,framework,package,standardized
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `eegain-0.0.1/eegain.egg-info/PKG-INFO` & `eegain-0.0.2/eegain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eegain
-Version: 0.0.1
+Version: 0.0.2
 Summary: EEG emotion recognition package for standardization
 Home-page: https://github.com/RRaphaell/EEGain
 Author: GAIN Team
 Author-email: 
 Keywords: EEG,emotion recognition,framework,package,standardized
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `eegain-0.0.1/setup.py` & `eegain-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 
 from setuptools import setup
 
 FILE = Path(__file__).resolve()
 PARENT = FILE.parent  # root directory
+
 README = (PARENT / "README.md").read_text(encoding="utf-8")
 
 exec(open("eegain/version.py").read())
 setup(
     name="eegain",
     version=__version__,
     description="EEG emotion recognition package for standardization",
```

