# Comparing `tmp/pyKVFinder-0.6.0.tar.gz` & `tmp/pyKVFinder-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyKVFinder-0.6.0.tar", last modified: Fri May 12 19:53:35 2023, max compression
+gzip compressed data, was "pyKVFinder-0.6.1.tar", last modified: Mon Jun 12 18:58:23 2023, max compression
```

## Comparing `pyKVFinder-0.6.0.tar` & `pyKVFinder-0.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.125694 pyKVFinder-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.117694 pyKVFinder-0.6.0/C/
--rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/C/numpy.i
--rw-r--r--   0 runner    (1001) docker     (123)    78654 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/C/pyKVFinder.c
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/C/pyKVFinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/C/pyKVFinder.i
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-05-12 19:53:35.125694 pyKVFinder-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.121694 pyKVFinder-0.6.0/pyKVFinder/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.121694 pyKVFinder-0.6.0/pyKVFinder/data/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/EisenbergWeiss.toml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/HessaHeijne.toml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/KyteDoolittle.toml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/MoonFleming.toml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/RadzickaWolfenden.toml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/WimleyWhite.toml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/ZhaoLondon.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.125694 pyKVFinder-0.6.0/pyKVFinder/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/ADN.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/ADN.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/ClO4.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/PKI.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/custom-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/tests/residues-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/data/vdw.dat
--rw-r--r--   0 runner    (1001) docker     (123)   107710 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    71046 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    63360 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyKVFinder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:53:35.121694 pyKVFinder-0.6.0/pyKVFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 19:53:35.000000 pyKVFinder-0.6.0/pyKVFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:53:35.125694 pyKVFinder-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-12 19:53:21.000000 pyKVFinder-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.513375 pyKVFinder-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.505375 pyKVFinder-0.6.1/C/
+-rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/C/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (123)    78654 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/C/pyKVFinder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/C/pyKVFinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/C/pyKVFinder.i
+-rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-06-12 18:58:23.513375 pyKVFinder-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.509375 pyKVFinder-0.6.1/pyKVFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.509375 pyKVFinder-0.6.1/pyKVFinder/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/EisenbergWeiss.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/HessaHeijne.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/KyteDoolittle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/MoonFleming.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/RadzickaWolfenden.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/WimleyWhite.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/ZhaoLondon.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.513375 pyKVFinder-0.6.1/pyKVFinder/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/ADN.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/ADN.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/ClO4.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/PKI.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/custom-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/tests/residues-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/data/vdw.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   107710 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71046 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63360 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyKVFinder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:58:23.509375 pyKVFinder-0.6.1/pyKVFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44189 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 18:58:23.000000 pyKVFinder-0.6.1/pyKVFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:58:23.513375 pyKVFinder-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-12 18:58:08.000000 pyKVFinder-0.6.1/setup.py
```

### Comparing `pyKVFinder-0.6.0/C/numpy.i` & `pyKVFinder-0.6.1/C/numpy.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/C/pyKVFinder.c` & `pyKVFinder-0.6.1/C/pyKVFinder.c`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/C/pyKVFinder.h` & `pyKVFinder-0.6.1/C/pyKVFinder.h`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/C/pyKVFinder.i` & `pyKVFinder-0.6.1/C/pyKVFinder.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/LICENSE.txt` & `pyKVFinder-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/PKG-INFO` & `pyKVFinder-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `pyKVFinder-0.6.0/README.rst` & `pyKVFinder-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/__init__.py` & `pyKVFinder-0.6.1/pyKVFinder/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,13 +27,13 @@
 --------
 * GitHub repository: https://github.com/LBC-LNBio/pyKVFinder
 
 * Documentation: https://lbc-lnbio.github.io/pyKVFinder
 """
 
 __name__ = "pyKVFinder"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 license = "GNU GPL-3.0 License"
 
 from .utils import *
 from .grid import *
 from .main import *
```

### Comparing `pyKVFinder-0.6.0/pyKVFinder/argparser.py` & `pyKVFinder-0.6.1/pyKVFinder/argparser.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb` & `pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.pdb` & `pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/data/tests/1FMO.xyz` & `pyKVFinder-0.6.1/pyKVFinder/data/tests/1FMO.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/data/tests/ADN.pdb` & `pyKVFinder-0.6.1/pyKVFinder/data/tests/ADN.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/data/tests/ADN.xyz` & `pyKVFinder-0.6.1/pyKVFinder/data/tests/ADN.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/data/tests/PKI.pdb` & `pyKVFinder-0.6.1/pyKVFinder/data/tests/PKI.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/data/vdw.dat` & `pyKVFinder-0.6.1/pyKVFinder/data/vdw.dat`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/grid.py` & `pyKVFinder-0.6.1/pyKVFinder/grid.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/main.py` & `pyKVFinder-0.6.1/pyKVFinder/main.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder/utils.py` & `pyKVFinder-0.6.1/pyKVFinder/utils.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyKVFinder.egg-info/PKG-INFO` & `pyKVFinder-0.6.1/pyKVFinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `pyKVFinder-0.6.0/pyKVFinder.egg-info/SOURCES.txt` & `pyKVFinder-0.6.1/pyKVFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.0/pyproject.toml` & `pyKVFinder-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,20 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "toml==0.10.2",
     "numpy==1.24.3",
     "matplotlib==3.7.1",
-    "plotly==5.14.1",
+    "plotly==5.15.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["pytest==7.3.1", "pytest-cov==4.0.0", "black==23.3.0", "flake8==6.0.0"]
+dev = ["pytest==7.3.2", "pytest-cov==4.1.0", "black==23.3.0", "flake8==6.0.0"]
 
 [project.urls]
 homepage = "https://github.com/LBC-LNBio/pyKVFinder/"
 documentation = "https://lbc-lnbio.github.io/pyKVFinder/"
 issues = "https://github.com/LBC-LNBio/pyKVFinder/issues"
 
 [project.scripts]
```

### Comparing `pyKVFinder-0.6.0/setup.py` & `pyKVFinder-0.6.1/setup.py`

 * *Files identical despite different names*

