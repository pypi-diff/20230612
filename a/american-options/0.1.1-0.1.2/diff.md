# Comparing `tmp/american_options-0.1.1.tar.gz` & `tmp/american_options-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\american_options-0.1.1.tar", last modified: Mon Jun 12 01:41:53 2023, max compression
+gzip compressed data, was "dist\american_options-0.1.2.tar", last modified: Mon Jun 12 10:11:25 2023, max compression
```

## Comparing `american_options-0.1.1.tar` & `american_options-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 01:41:53.000000 american_options-0.1.1/
--rw-rw-rw-   0        0        0     2510 2023-06-12 01:41:53.000000 american_options-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2023-06-12 01:21:26.000000 american_options-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options/
--rw-rw-rw-   0        0        0    34917 2023-06-12 00:23:55.000000 american_options-0.1.1/american_options/AMoption.py
--rw-rw-rw-   0        0        0      191 2023-06-12 00:46:34.000000 american_options-0.1.1/american_options/__init__.py
--rw-rw-rw-   0        0        0     4524 2023-06-11 22:01:15.000000 american_options-0.1.1/american_options/jump_diffusion.py
--rw-rw-rw-   0        0        0     4198 2023-06-11 22:50:46.000000 american_options-0.1.1/american_options/payoffs.py
--rw-rw-rw-   0        0        0     2333 2023-06-10 14:04:25.000000 american_options-0.1.1/american_options/próby.py
--rw-rw-rw-   0        0        0     2638 2023-06-11 17:41:22.000000 american_options-0.1.1/american_options/sobol.py
--rw-rw-rw-   0        0        0    10287 2023-06-11 22:52:35.000000 american_options-0.1.1/american_options/underlying.py
-drwxrwxrwx   0        0        0        0 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/
--rw-rw-rw-   0        0        0     2510 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 01:41:53.000000 american_options-0.1.1/american_options.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 01:41:53.000000 american_options-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1425 2023-06-12 01:41:05.000000 american_options-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:11:25.000000 american_options-0.1.2/
+-rw-rw-rw-   0        0        0     2510 2023-06-12 10:11:25.000000 american_options-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2023-06-12 01:21:26.000000 american_options-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options/
+-rw-rw-rw-   0        0        0    34934 2023-06-12 10:08:26.000000 american_options-0.1.2/american_options/AMoption.py
+-rw-rw-rw-   0        0        0      191 2023-06-12 00:46:34.000000 american_options-0.1.2/american_options/__init__.py
+-rw-rw-rw-   0        0        0     4524 2023-06-11 22:01:15.000000 american_options-0.1.2/american_options/jump_diffusion.py
+-rw-rw-rw-   0        0        0     4198 2023-06-11 22:50:46.000000 american_options-0.1.2/american_options/payoffs.py
+-rw-rw-rw-   0        0        0     2333 2023-06-10 14:04:25.000000 american_options-0.1.2/american_options/próby.py
+-rw-rw-rw-   0        0        0     2638 2023-06-11 17:41:22.000000 american_options-0.1.2/american_options/sobol.py
+-rw-rw-rw-   0        0        0    10287 2023-06-11 22:52:35.000000 american_options-0.1.2/american_options/underlying.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/
+-rw-rw-rw-   0        0        0     2510 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-12 10:11:25.000000 american_options-0.1.2/american_options.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:11:25.000000 american_options-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2023-06-12 10:08:26.000000 american_options-0.1.2/setup.py
```

### Comparing `american_options-0.1.1/PKG-INFO` & `american_options-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: american_options
-Version: 0.1.1
+Version: 0.1.2
 Summary: library T-28h
 Home-page: https://american_options.readthedocs.io/
 Author: Przemysław Adamski, Katarzyna Hasal, Kacper Toczek
 Author-email: kat.hasal99@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `american_options-0.1.1/README.md` & `american_options-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `american_options-0.1.1/american_options/AMoption.py` & `american_options-0.1.2/american_options/AMoption.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas
 from scipy.stats import norm
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from tqdm import tqdm
-from underlying import Underlying
+from american_options.underlying import Underlying
 from scipy import interpolate, stats
 from itertools import product
 from operator import itemgetter
 from sklearn import linear_model
 import warnings
 import chaospy
 #from payoffs import *
```

### Comparing `american_options-0.1.1/american_options/jump_diffusion.py` & `american_options-0.1.2/american_options/jump_diffusion.py`

 * *Files identical despite different names*

### Comparing `american_options-0.1.1/american_options/payoffs.py` & `american_options-0.1.2/american_options/payoffs.py`

 * *Files identical despite different names*

### Comparing `american_options-0.1.1/american_options/próby.py` & `american_options-0.1.2/american_options/próby.py`

 * *Files identical despite different names*

### Comparing `american_options-0.1.1/american_options/sobol.py` & `american_options-0.1.2/american_options/sobol.py`

 * *Files identical despite different names*

### Comparing `american_options-0.1.1/american_options/underlying.py` & `american_options-0.1.2/american_options/underlying.py`

 * *Files identical despite different names*

### Comparing `american_options-0.1.1/american_options.egg-info/PKG-INFO` & `american_options-0.1.2/american_options.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: american-options
-Version: 0.1.1
+Version: 0.1.2
 Summary: library T-28h
 Home-page: https://american_options.readthedocs.io/
 Author: Przemysław Adamski, Katarzyna Hasal, Kacper Toczek
 Author-email: kat.hasal99@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `american_options-0.1.1/setup.py` & `american_options-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Get the long description on pypi from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="american_options",
-    version="0.1.1",
+    version="0.1.2",
     description="library T-28h",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://american_options.readthedocs.io/",
     author="Przemysław Adamski, Katarzyna Hasal, Kacper Toczek",
     author_email="kat.hasal99@gmail.com",
     classifiers=[
```

