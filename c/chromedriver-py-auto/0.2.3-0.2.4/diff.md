# Comparing `tmp/chromedriver-py-auto-0.2.3.tar.gz` & `tmp/chromedriver-py-auto-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chromedriver-py-auto-0.2.3.tar", last modified: Sun Jun 11 15:40:33 2023, max compression
+gzip compressed data, was "chromedriver-py-auto-0.2.4.tar", last modified: Mon Jun 12 14:07:30 2023, max compression
```

## Comparing `chromedriver-py-auto-0.2.3.tar` & `chromedriver-py-auto-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 roshanzamir  (1000) roshanzamir  (1000)        0 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     1076 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/LICENSE
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)      115 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/MANIFEST.in
--rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)     1663 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/PKG-INFO
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     1008 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/README.md
-drwxrwxr-x   0 roshanzamir  (1000) roshanzamir  (1000)        0 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)       52 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/__init__.py
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)       84 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/binary_path.py
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)      647 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/chrome.py
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)       27 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/chromedriver
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     2687 2023-06-11 15:22:43.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/chromedriver_py.py
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)        0 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/py.typed
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     1097 2023-06-11 15:16:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto/version.py
-drwxrwxr-x   0 roshanzamir  (1000) roshanzamir  (1000)        0 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/
--rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)     1663 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/PKG-INFO
--rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)      450 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/SOURCES.txt
--rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)        1 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/dependency_links.txt
--rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)       21 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/top_level.txt
--rw-rw-r--   0 roshanzamir  (1000) roshanzamir  (1000)       38 2023-06-11 15:40:33.000000 chromedriver-py-auto-0.2.3/setup.cfg
--rw-r--r--   0 roshanzamir  (1000) roshanzamir  (1000)     1134 2023-06-11 15:22:57.000000 chromedriver-py-auto-0.2.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 14:07:30.191960 chromedriver-py-auto-0.2.4/
+-rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-06-12 10:30:46.000000 chromedriver-py-auto-0.2.4/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      115 2023-06-12 10:30:46.000000 chromedriver-py-auto-0.2.4/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     1663 2023-06-12 14:07:30.187960 chromedriver-py-auto-0.2.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-06-12 10:30:46.000000 chromedriver-py-auto-0.2.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 14:07:30.187960 chromedriver-py-auto-0.2.4/chromedriver_py_auto/
+-rw-rw-r--   0 user      (1000) user      (1000)       52 2023-06-12 14:07:13.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       84 2023-06-12 10:30:46.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto/binary_path.py
+-rw-rw-r--   0 user      (1000) user      (1000)      647 2023-06-12 10:30:46.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto/chrome.py
+-rw-rw-r--   0 user      (1000) user      (1000)       27 2023-06-12 14:07:04.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto/chromedriver
+-rw-------   0 user      (1000) user      (1000)     1001 2023-06-12 13:13:18.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto/chromedriver_py.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-12 10:30:46.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto/py.typed
+-rw-rw-r--   0 user      (1000) user      (1000)     1097 2023-06-12 10:30:46.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 14:07:30.187960 chromedriver-py-auto-0.2.4/chromedriver_py_auto.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     1663 2023-06-12 14:07:30.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      450 2023-06-12 14:07:30.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 14:07:30.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       21 2023-06-12 14:07:30.000000 chromedriver-py-auto-0.2.4/chromedriver_py_auto.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 14:07:30.191960 chromedriver-py-auto-0.2.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1091 2023-06-12 12:58:21.000000 chromedriver-py-auto-0.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `chromedriver-py-auto-0.2.3/LICENSE` & `chromedriver-py-auto-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.3/PKG-INFO` & `chromedriver-py-auto-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-py-auto
-Version: 0.2.3
+Version: 0.2.4
 Summary: A wrapper around chromedriver-py library. Detects the Chrome version and installs the most suitable chromedriver-py version.
 Home-page: https://github.com/AlirezaRoshanzamir/chromedriver-py-auto
 Author: Alireza Roshanzamir
 Author-email: a.roshanzamir1996@gmail.com
 License: MIT License
 Description: # chromdriver-py-auto
         A wrapper around [chromedriver-py](https://github.com/breuerfelix/chromedriver-py)
```

### Comparing `chromedriver-py-auto-0.2.3/README.md` & `chromedriver-py-auto-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.3/chromedriver_py_auto/chrome.py` & `chromedriver-py-auto-0.2.4/chromedriver_py_auto/chrome.py`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.3/chromedriver_py_auto/version.py` & `chromedriver-py-auto-0.2.4/chromedriver_py_auto/version.py`

 * *Files identical despite different names*

### Comparing `chromedriver-py-auto-0.2.3/chromedriver_py_auto.egg-info/PKG-INFO` & `chromedriver-py-auto-0.2.4/chromedriver_py_auto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromedriver-py-auto
-Version: 0.2.3
+Version: 0.2.4
 Summary: A wrapper around chromedriver-py library. Detects the Chrome version and installs the most suitable chromedriver-py version.
 Home-page: https://github.com/AlirezaRoshanzamir/chromedriver-py-auto
 Author: Alireza Roshanzamir
 Author-email: a.roshanzamir1996@gmail.com
 License: MIT License
 Description: # chromdriver-py-auto
         A wrapper around [chromedriver-py](https://github.com/breuerfelix/chromedriver-py)
```

### Comparing `chromedriver-py-auto-0.2.3/setup.py` & `chromedriver-py-auto-0.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from asyncio import subprocess
 import logging
 from pathlib import Path
 
 import setuptools
 from setuptools.command.build_py import build_py
 
-from chromedriver_py_auto.chromedriver_py import copy_binary, extract_suitable_version
+from chromedriver_py_auto.chromedriver_py import (
+    copy_binary,
+    extract_requirement_specifier,
+)
 
 logging.basicConfig(level=logging.INFO)
 
 
 class CopyChromedriverPyBinary(setuptools.command.build_py.build_py):
     def run(self) -> None:
         copy_binary()
         build_py.run(self)
 
 
 setuptools.setup(
     name="chromedriver-py-auto",
-    version="0.2.3",
+    version="0.2.4",
     description="A wrapper around chromedriver-py library. Detects the Chrome version "
     "and installs the most suitable chromedriver-py version.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Alireza Roshanzamir",
     author_email="a.roshanzamir1996@gmail.com",
     url="https://github.com/AlirezaRoshanzamir/chromedriver-py-auto",
     packages=setuptools.find_packages(),
-    setup_requires=["chromedriver-py=={}".format(str(extract_suitable_version()))],
+    setup_requires=[extract_requirement_specifier()],
     include_package_data=True,
     cmdclass={"build_py": CopyChromedriverPyBinary},
 )
```

