# Comparing `tmp/uframe-0.0.0.tar.gz` & `tmp/uframe-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uframe-0.0.0.tar", last modified: Sun Jun 11 21:14:57 2023, max compression
+gzip compressed data, was "uframe-0.0.1.tar", last modified: Mon Jun 12 11:53:12 2023, max compression
```

## Comparing `uframe-0.0.0.tar` & `uframe-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 21:14:57.809442 uframe-0.0.0/
--rw-rw-rw-   0        0        0     1069 2023-06-05 09:22:12.000000 uframe-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      619 2023-06-11 21:14:57.810439 uframe-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1751 2023-06-08 12:19:36.000000 uframe-0.0.0/README.md
--rw-rw-rw-   0        0        0      475 2023-06-05 11:37:08.000000 uframe-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      790 2023-06-11 21:14:57.813806 uframe-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-06-05 09:25:12.000000 uframe-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:14:57.713840 uframe-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 21:14:57.766572 uframe-0.0.0/src/uframe/
--rw-rw-rw-   0        0        0      183 2023-05-25 10:35:48.000000 uframe-0.0.0/src/uframe/__init__.py
--rw-rw-rw-   0        0        0    56754 2023-06-11 11:52:12.000000 uframe-0.0.0/src/uframe/uframe.py
--rw-rw-rw-   0        0        0    12104 2023-06-10 14:36:03.000000 uframe-0.0.0/src/uframe/uframe_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-11 21:14:57.798170 uframe-0.0.0/src/uframe.egg-info/
--rw-rw-rw-   0        0        0      619 2023-06-11 21:14:57.000000 uframe-0.0.0/src/uframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-11 21:14:57.000000 uframe-0.0.0/src/uframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 21:14:57.000000 uframe-0.0.0/src/uframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 11:38:57.000000 uframe-0.0.0/src/uframe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       85 2023-06-11 21:14:57.000000 uframe-0.0.0/src/uframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 21:14:57.000000 uframe-0.0.0/src/uframe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 21:14:57.804823 uframe-0.0.0/tests/
--rw-rw-rw-   0        0        0      224 2023-06-08 10:23:39.000000 uframe-0.0.0/tests/test_uframe.py
--rw-rw-rw-   0        0        0     2711 2023-06-09 08:18:37.000000 uframe-0.0.0/tests/test_uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:53:12.310210 uframe-0.0.1/
+-rw-rw-rw-   0        0        0     1069 2023-06-05 09:22:12.000000 uframe-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2353 2023-06-12 11:53:12.310848 uframe-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1751 2023-06-08 12:19:36.000000 uframe-0.0.1/README.md
+-rw-rw-rw-   0        0        0     1010 2023-06-12 09:04:04.000000 uframe-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      462 2023-06-12 11:53:12.312060 uframe-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-06-05 09:25:12.000000 uframe-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:53:12.243032 uframe-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 11:53:12.283867 uframe-0.0.1/src/uframe/
+-rw-rw-rw-   0        0        0      441 2023-06-12 08:57:00.000000 uframe-0.0.1/src/uframe/__init__.py
+-rw-rw-rw-   0        0        0    56755 2023-06-12 10:47:09.000000 uframe-0.0.1/src/uframe/uframe.py
+-rw-rw-rw-   0        0        0    12104 2023-06-10 14:36:03.000000 uframe-0.0.1/src/uframe/uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:53:12.301625 uframe-0.0.1/src/uframe.egg-info/
+-rw-rw-rw-   0        0        0     2353 2023-06-12 11:53:12.000000 uframe-0.0.1/src/uframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-12 11:53:12.000000 uframe-0.0.1/src/uframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 11:53:12.000000 uframe-0.0.1/src/uframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-05 11:38:57.000000 uframe-0.0.1/src/uframe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       85 2023-06-12 11:53:12.000000 uframe-0.0.1/src/uframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 11:53:12.000000 uframe-0.0.1/src/uframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 11:53:12.308161 uframe-0.0.1/tests/
+-rw-rw-rw-   0        0        0      224 2023-06-08 10:23:39.000000 uframe-0.0.1/tests/test_uframe.py
+-rw-rw-rw-   0        0        0     2711 2023-06-09 08:18:37.000000 uframe-0.0.1/tests/test_uframe_instance.py
```

### Comparing `uframe-0.0.0/LICENSE` & `uframe-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uframe-0.0.0/README.md` & `uframe-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `uframe-0.0.0/src/uframe/uframe.py` & `uframe-0.0.1/src/uframe/uframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from uframe_instance import uframe_instance
+from .uframe_instance import uframe_instance
 import scipy
 from scipy import stats
 from sklearn.neighbors import KernelDensity
 import sklearn.neighbors
 from sklearn.preprocessing import LabelEncoder, OneHotEncoder, MinMaxScaler
 import miceforest as mf
 import math
```

### Comparing `uframe-0.0.0/src/uframe/uframe_instance.py` & `uframe-0.0.1/src/uframe/uframe_instance.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.0/tests/test_uframe_instance.py` & `uframe-0.0.1/tests/test_uframe_instance.py`

 * *Files identical despite different names*

