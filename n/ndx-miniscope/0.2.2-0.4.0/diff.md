# Comparing `tmp/ndx-miniscope-0.2.2.tar.gz` & `tmp/ndx-miniscope-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ndx-miniscope-0.2.2.tar", last modified: Wed Jun 26 21:01:48 2019, max compression
+gzip compressed data, was "ndx-miniscope-0.4.0.tar", last modified: Mon Jun 12 13:53:25 2023, max compression
```

## Comparing `ndx-miniscope-0.2.2.tar` & `ndx-miniscope-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,39 @@
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/
--rw-r--r--   0 bendichter   (501) staff       (20)      375 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/PKG-INFO
--rw-r--r--   0 bendichter   (501) staff       (20)       20 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/requirements.txt
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/spec/
--rw-r--r--   0 bendichter   (501) staff       (20)      269 2019-06-26 20:56:20.000000 ndx-miniscope-0.2.2/spec/ndx-miniscope.namespace.yaml
--rw-r--r--   0 bendichter   (501) staff       (20)      336 2019-06-26 20:56:20.000000 ndx-miniscope-0.2.2/spec/ndx-miniscope.extensions.yaml
--rw-r--r--   0 bendichter   (501) staff       (20)      264 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/MANIFEST.in
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/docs/
--rw-r--r--   0 bendichter   (501) staff       (20)     6600 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/Makefile
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/docs/source/
--rw-r--r--   0 bendichter   (501) staff       (20)      456 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/source/index.rst
--rw-r--r--   0 bendichter   (501) staff       (20)       88 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/source/release_notes.rst
--rw-r--r--   0 bendichter   (501) staff       (20)     7378 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/source/conf.py
--rw-r--r--   0 bendichter   (501) staff       (20)       76 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/source/description.rst
--rw-r--r--   0 bendichter   (501) staff       (20)      161 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/source/format.rst
--rw-r--r--   0 bendichter   (501) staff       (20)      167 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/source/credits.rst
--rw-r--r--   0 bendichter   (501) staff       (20)     3962 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/source/conf_doc_autogen.py
--rw-r--r--   0 bendichter   (501) staff       (20)     6193 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/README.md
--rw-r--r--   0 bendichter   (501) staff       (20)      785 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/docs/make.bat
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/docs/build/
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/docs/build/html/
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/docs/build/html/_static/
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/docs/build/html/_static/css/
--rw-r--r--   0 bendichter   (501) staff       (20)   112267 2018-03-26 17:36:57.000000 ndx-miniscope-0.2.2/docs/build/html/_static/css/theme.css
--rw-r--r--   0 bendichter   (501) staff       (20)     3376 2018-03-26 17:36:57.000000 ndx-miniscope-0.2.2/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0 bendichter   (501) staff       (20)    10362 2019-06-10 04:53:33.000000 ndx-miniscope-0.2.2/docs/build/html/_static/basic.css
--rw-r--r--   0 bendichter   (501) staff       (20)     4395 2019-06-10 04:53:33.000000 ndx-miniscope-0.2.2/docs/build/html/_static/pygments.css
--rw-r--r--   0 bendichter   (501) staff       (20)     2434 2019-06-26 18:06:22.000000 ndx-miniscope-0.2.2/README.md
--rw-r--r--   0 bendichter   (501) staff       (20)     1270 2019-06-26 20:59:44.000000 ndx-miniscope-0.2.2/setup.py
--rw-r--r--   0 bendichter   (501) staff       (20)       38 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/setup.cfg
--rw-r--r--   0 bendichter   (501) staff       (20)        0 2019-06-09 22:23:19.000000 ndx-miniscope-0.2.2/LICENSE.txt
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/src/
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/src/pynwb/
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope.egg-info/
--rw-r--r--   0 bendichter   (501) staff       (20)      375 2019-06-26 21:01:47.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope.egg-info/PKG-INFO
--rw-r--r--   0 bendichter   (501) staff       (20)        1 2019-06-26 21:01:47.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope.egg-info/not-zip-safe
--rw-r--r--   0 bendichter   (501) staff       (20)      972 2019-06-26 21:01:47.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope.egg-info/SOURCES.txt
--rw-r--r--   0 bendichter   (501) staff       (20)        6 2019-06-26 21:01:47.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope.egg-info/requires.txt
--rw-r--r--   0 bendichter   (501) staff       (20)       14 2019-06-26 21:01:47.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope.egg-info/top_level.txt
--rw-r--r--   0 bendichter   (501) staff       (20)        1 2019-06-26 21:01:47.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope.egg-info/dependency_links.txt
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope/
-drwxr-xr-x   0 bendichter   (501) staff       (20)        0 2019-06-26 21:01:48.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope/spec/
--rw-r--r--   0 bendichter   (501) staff       (20)      269 2019-06-26 20:56:20.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope/spec/ndx-miniscope.namespace.yaml
--rw-r--r--   0 bendichter   (501) staff       (20)      336 2019-06-26 20:56:20.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope/spec/ndx-miniscope.extensions.yaml
--rw-r--r--   0 bendichter   (501) staff       (20)       25 2019-06-26 16:10:42.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope/__init__.py
--rw-r--r--   0 bendichter   (501) staff       (20)     2239 2019-06-26 18:20:00.000000 ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope/miniscope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.741544 ndx-miniscope-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-12 13:53:25.741544 ndx-miniscope-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/conf_doc_autogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/docs/source/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:53:25.741544 ndx-miniscope-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/spec/ndx-miniscope.extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/spec/ndx-miniscope.namespace.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.733544 ndx-miniscope-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.733544 ndx-miniscope-0.4.0/src/pynwb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/miniscope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/spec/ndx-miniscope.extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-12 13:53:19.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/spec/ndx-miniscope.namespace.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:53:25.737544 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 13:53:25.000000 ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ndx-miniscope-0.2.2/docs/Makefile` & `ndx-miniscope-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.2.2/docs/source/conf.py` & `ndx-miniscope-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.2.2/docs/source/conf_doc_autogen.py` & `ndx-miniscope-0.4.0/docs/source/conf_doc_autogen.py`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.2.2/docs/README.md` & `ndx-miniscope-0.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.2.2/docs/make.bat` & `ndx-miniscope-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndx-miniscope-0.2.2/setup.py` & `ndx-miniscope-0.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,64 @@
 # -*- coding: utf-8 -*-
 
 import os
-
-from setuptools import setup, find_packages
+from pathlib import Path
 from shutil import copy2
 
+from setuptools import find_packages, setup
+
+path = Path(__file__).parent
+
+with open(os.path.join(path, "README.md")) as f:
+    long_description = f.read()
+
+with open(path / "requirements.txt") as f:
+    install_requires = f.readlines()
+
 setup_args = {
-    'name': 'ndx-miniscope',
-    'version': '0.2.2',
-    'description': 'holds metadata relevant for miniscope acquisition',
-    'author': 'Ben Dichter',
-    'author_email': 'ben.dichter@gmail.com',
-    'url': '',
-    'license': '',
-    'install_requires': [
-        'pynwb'
-    ],
-    'packages': find_packages('src/pynwb'),
-    'package_dir': {'': 'src/pynwb'},
-    'package_data': {'ndx_miniscope': [
-        'spec/ndx-miniscope.namespace.yaml',
-        'spec/ndx-miniscope.extensions.yaml',
-    ]},
-    'classifiers': [
+    "name": "ndx-miniscope",
+    "version": "0.4.0",
+    "description": "Represent metadata for Miniscope acquisition system.",
+    "long_description": long_description,
+    "long_description_content_type": "text/markdown",
+    "author": "Ben Dichter",
+    "author_email": "ben.dichter@catalystneuro.com",
+    "url": "https://github.com/catalystneuro/ndx-miniscope",
+    "license": "BSD-3",
+    "install_requires": install_requires,
+    "packages": find_packages("src/pynwb", exclude=["tests", "tests.*"]),
+    "package_dir": {"": "src/pynwb"},
+    "package_data": {
+        "ndx_miniscope": [
+            "spec/ndx-miniscope.namespace.yaml",
+            "spec/ndx-miniscope.extensions.yaml",
+        ]
+    },
+    "classifiers": [
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
     ],
-    'zip_safe': False
+    "keywords": [
+        "NeurodataWithoutBorders",
+        "NWB",
+        "nwb-extension",
+        "ndx-extension",
+    ],
+    "zip_safe": False,
 }
 
 
 def _copy_spec_files(project_dir):
-    ns_path = os.path.join(project_dir, 'spec', 'ndx-miniscope.namespace.yaml')
-    ext_path = os.path.join(project_dir, 'spec', 'ndx-miniscope.extensions.yaml')
+    ns_path = os.path.join(project_dir, "spec", "ndx-miniscope.namespace.yaml")
+    ext_path = os.path.join(project_dir, "spec", "ndx-miniscope.extensions.yaml")
 
-    dst_dir = os.path.join(project_dir, 'src', 'pynwb', 'ndx_miniscope', 'spec')
+    dst_dir = os.path.join(project_dir, "src", "pynwb", "ndx_miniscope", "spec")
     if not os.path.exists(dst_dir):
         os.mkdir(dst_dir)
 
     copy2(ns_path, dst_dir)
     copy2(ext_path, dst_dir)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     _copy_spec_files(os.path.dirname(__file__))
     setup(**setup_args)
```

### Comparing `ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope.egg-info/SOURCES.txt` & `ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 docs/Makefile
 docs/README.md
 docs/make.bat
-docs/build/html/_static/basic.css
-docs/build/html/_static/pygments.css
-docs/build/html/_static/css/badge_only.css
-docs/build/html/_static/css/theme.css
 docs/source/conf.py
 docs/source/conf_doc_autogen.py
 docs/source/credits.rst
 docs/source/description.rst
 docs/source/format.rst
 docs/source/index.rst
 docs/source/release_notes.rst
```

### Comparing `ndx-miniscope-0.2.2/src/pynwb/ndx_miniscope/miniscope.py` & `ndx-miniscope-0.4.0/src/pynwb/ndx_miniscope/miniscope.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import os
 
 import pandas as pd
-from pynwb import load_namespaces, get_class
 from pynwb.misc import AnnotationSeries
 
-name = 'ndx-miniscope'
+from pynwb import get_class, load_namespaces
+
+name = "ndx-miniscope"
 
 here = os.path.abspath(os.path.dirname(__file__))
-ns_path = os.path.join(here, 'spec', name + '.namespace.yaml')
+ns_path = os.path.join(here, "spec", name + ".namespace.yaml")
 
 load_namespaces(ns_path)
 
-Miniscope = get_class('Miniscope', name)
+Miniscope = get_class("Miniscope", name)
 
 
-def load_miniscope_timestamps(fpath, cam_num=1):
+def read_miniscope_timestamps(fpath, cam_num=1):
     """Reads timestamp.dat and outputs a list of times in seconds
 
     Parameters
     ----------
     fpath: str
         data directory or path to timestamp.dat
     cam_num: int
         number of feed
 
     Returns
     -------
     numpy.ndarray list if times in seconds
 
     """
-    if not fpath[-4:] == '.dat':
-        fpath = os.path.join(fpath, 'timestamp.dat')
-    df = pd.read_csv(fpath, sep='\t')
-    df_cam = df[df['camNum'] == cam_num]
-    tt = df_cam['sysClock'].values/1000
+    if not fpath[-4:] == ".dat":
+        fpath = os.path.join(fpath, "timestamp.dat")
+    df = pd.read_csv(fpath, sep="\t")
+    df_cam = df[df["camNum"] == cam_num]
+    tt = df_cam["sysClock"].values / 1000
     tt[0] = 0
     return tt
 
 
 def read_settings(fpath):
     """Reads the settings_and_notes.dat and creates a Miniscope object with leaded settings
 
@@ -48,21 +49,23 @@
 
     Returns
     -------
     ndx_miniscope.Miniscope
         with settings from settings_and_notes.dat
 
     """
-    if not fpath[-4:] == '.dat':
-        fpath = os.path.join(fpath, 'settings_and_notes.dat')
-    df = pd.read_csv(fpath, sep='\t').loc[0]
-
-    return Miniscope(name='Miniscope',
-                     excitation=int(df['excitation']),
-                     msCamExposure=int(df['msCamExposure']))
+    if not fpath[-4:] == ".dat":
+        fpath = os.path.join(fpath, "settings_and_notes.dat")
+    df = pd.read_csv(fpath, sep="\t").loc[0]
+
+    return Miniscope(
+        name="Miniscope",
+        excitation=int(df["excitation"]),
+        msCamExposure=int(df["msCamExposure"]),
+    )
 
 
 def read_notes(fpath):
     """Reads the notes from the settings_and_notes.dat file and creates a pynwb.misc.AnnotationSeries
 
     Parameters
     ----------
@@ -70,16 +73,29 @@
         data dir or path to settings_and_notes.dat
 
     Returns
     -------
     None or pynwb.misc.AnnotationSeries
 
     """
-    if not fpath[-4:] == '.dat':
-        fpath = os.path.join(fpath, 'settings_and_notes.dat')
-    df = pd.read_csv(fpath, skiprows=3, delimiter='\t')
+    if not fpath[-4:] == ".dat":
+        fpath = os.path.join(fpath, "settings_and_notes.dat")
+    df = pd.read_csv(fpath, skiprows=3, delimiter="\t")
     if len(df):
-        return AnnotationSeries(name='notes', data=df['Note'].values,
-                                timestamps=df['elapsedTime'].values / 1000,
-                                description='read from miniscope settings_and_notes.dat file')
-    else:
-        return
+        return AnnotationSeries(
+            name="notes",
+            data=df["Note"].values,
+            timestamps=df["elapsedTime"].values / 1000,
+            description="read from miniscope settings_and_notes.dat file",
+        )
+
+
+def get_starting_frames(video_files):
+    import cv2
+
+    out = [0]
+    for video_file in video_files[:-1]:
+        cap = cv2.VideoCapture(video_file)
+        length = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+        out.append(length)
+
+    return out
```

