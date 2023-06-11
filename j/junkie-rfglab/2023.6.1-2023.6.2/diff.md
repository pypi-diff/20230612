# Comparing `tmp/junkie-rfglab-2023.6.1.tar.gz` & `tmp/junkie-rfglab-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junkie-rfglab-2023.6.1.tar", last modified: Sun Jun 11 21:51:44 2023, max compression
+gzip compressed data, was "junkie-rfglab-2023.6.2.tar", last modified: Sun Jun 11 21:58:44 2023, max compression
```

## Comparing `junkie-rfglab-2023.6.1.tar` & `junkie-rfglab-2023.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:51:44.335533 junkie-rfglab-2023.6.1/
--rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.1/LICENSE
--rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-11 21:51:44.335412 junkie-rfglab-2023.6.1/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)     2949 2023-06-11 21:38:08.000000 junkie-rfglab-2023.6.1/README.md
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:51:44.334643 junkie-rfglab-2023.6.1/junkie/
--rw-r--r--   0 rodrigo    (501) staff       (20)       70 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.1/junkie/__init__.py
--rw-r--r--   0 rodrigo    (501) staff       (20)    11354 2023-06-11 21:36:16.000000 junkie-rfglab-2023.6.1/junkie/junkie.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:51:44.334748 junkie-rfglab-2023.6.1/junkie/tests/
--rw-r--r--   0 rodrigo    (501) staff       (20)        0 2023-05-14 00:28:03.000000 junkie-rfglab-2023.6.1/junkie/tests/__init__.py
-drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:51:44.335259 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/
--rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/PKG-INFO
--rw-r--r--   0 rodrigo    (501) staff       (20)      277 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/SOURCES.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/dependency_links.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)       75 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/requires.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-06-11 21:51:44.000000 junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/top_level.txt
--rw-r--r--   0 rodrigo    (501) staff       (20)      853 2023-06-11 21:50:33.000000 junkie-rfglab-2023.6.1/pyproject.toml
--rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-06-11 21:51:44.335566 junkie-rfglab-2023.6.1/setup.cfg
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:58:44.848105 junkie-rfglab-2023.6.2/
+-rw-r--r--   0 rodrigo    (501) staff       (20)    33148 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.2/LICENSE
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-11 21:58:44.847975 junkie-rfglab-2023.6.2/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)     2949 2023-06-11 21:38:08.000000 junkie-rfglab-2023.6.2/README.md
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:58:44.847218 junkie-rfglab-2023.6.2/junkie/
+-rw-r--r--   0 rodrigo    (501) staff       (20)       70 2023-05-12 19:44:56.000000 junkie-rfglab-2023.6.2/junkie/__init__.py
+-rw-r--r--   0 rodrigo    (501) staff       (20)    11354 2023-06-11 21:58:18.000000 junkie-rfglab-2023.6.2/junkie/junkie.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:58:44.847324 junkie-rfglab-2023.6.2/junkie/tests/
+-rw-r--r--   0 rodrigo    (501) staff       (20)        0 2023-05-14 00:28:03.000000 junkie-rfglab-2023.6.2/junkie/tests/__init__.py
+drwxr-xr-x   0 rodrigo    (501) staff       (20)        0 2023-06-11 21:58:44.847817 junkie-rfglab-2023.6.2/junkie_rfglab.egg-info/
+-rw-r--r--   0 rodrigo    (501) staff       (20)     3537 2023-06-11 21:58:44.000000 junkie-rfglab-2023.6.2/junkie_rfglab.egg-info/PKG-INFO
+-rw-r--r--   0 rodrigo    (501) staff       (20)      277 2023-06-11 21:58:44.000000 junkie-rfglab-2023.6.2/junkie_rfglab.egg-info/SOURCES.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        1 2023-06-11 21:58:44.000000 junkie-rfglab-2023.6.2/junkie_rfglab.egg-info/dependency_links.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)       69 2023-06-11 21:58:44.000000 junkie-rfglab-2023.6.2/junkie_rfglab.egg-info/requires.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)        7 2023-06-11 21:58:44.000000 junkie-rfglab-2023.6.2/junkie_rfglab.egg-info/top_level.txt
+-rw-r--r--   0 rodrigo    (501) staff       (20)      847 2023-06-11 21:57:47.000000 junkie-rfglab-2023.6.2/pyproject.toml
+-rw-r--r--   0 rodrigo    (501) staff       (20)       38 2023-06-11 21:58:44.848140 junkie-rfglab-2023.6.2/setup.cfg
```

### Comparing `junkie-rfglab-2023.6.1/LICENSE` & `junkie-rfglab-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `junkie-rfglab-2023.6.1/PKG-INFO` & `junkie-rfglab-2023.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `junkie-rfglab-2023.6.1/README.md` & `junkie-rfglab-2023.6.2/README.md`

 * *Files identical despite different names*

### Comparing `junkie-rfglab-2023.6.1/junkie/junkie.py` & `junkie-rfglab-2023.6.2/junkie/junkie.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import skimage
 import IPython.display as IPyd
 import ipywidgets as ipyw
 import matplotlib.pyplot as plt
 
-__version__: str = '2023.6.1'  # this must be here for pyproject.toml to find it.
+__version__: str = '2023.6.2'  # this must be here for pyproject.toml to find it.
 
 
 # You will need this line in your jupyter notebook: %matplotlib widget
 
 class junkie:
     """ 
     junkie: a JUpyter NotebooK Image Explorer
```

### Comparing `junkie-rfglab-2023.6.1/junkie_rfglab.egg-info/PKG-INFO` & `junkie-rfglab-2023.6.2/junkie_rfglab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junkie-rfglab
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: junkie is a JUpyter NotebooK Image Explorer
 Author-email: Rodrigo Fernandez-Gonzalez <rodrigo.fernandez.gonzalez@utoronto.ca>
 Project-URL: Homepage, https://bitbucket.com/rfg_lab/junkie
 Project-URL: Bug Tracker, https://bitbucket.com/rfg_lab/junkie/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `junkie-rfglab-2023.6.1/pyproject.toml` & `junkie-rfglab-2023.6.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "numpy>=1.23",
   "ipympl>=0.9",
   "ipywidgets>=8.0",
   "matplotlib>=3.7",
-  "scikit-image>=0.19",
+  "scikit-image",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "junkie.junkie.__version__"}
 
 [project.urls]
 "Homepage" = "https://bitbucket.com/rfg_lab/junkie"
```

