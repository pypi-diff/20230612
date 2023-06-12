# Comparing `tmp/topological-recursion-0.0a1.tar.gz` & `tmp/topological-recursion-0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topological-recursion-0.0a1.tar", last modified: Mon Jun 12 21:30:53 2023, max compression
+gzip compressed data, was "topological-recursion-0.0a2.tar", last modified: Mon Jun 12 21:35:25 2023, max compression
```

## Comparing `topological-recursion-0.0a1.tar` & `topological-recursion-0.0a2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-12 21:30:53.942231 topological-recursion-0.0a1/
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       35 2023-06-12 21:26:53.000000 topological-recursion-0.0a1/MANIFEST.in
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     2086 2023-06-12 21:30:53.942231 topological-recursion-0.0a1/PKG-INFO
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     1467 2023-06-12 21:28:26.000000 topological-recursion-0.0a1/README.rst
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)        6 2023-06-12 21:18:50.000000 topological-recursion-0.0a1/VERSION
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       38 2023-06-12 21:30:53.942231 topological-recursion-0.0a1/setup.cfg
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     1325 2023-06-12 21:29:07.000000 topological-recursion-0.0a1/setup.py
-drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-12 21:30:53.942231 topological-recursion-0.0a1/topological_recursion/
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)        0 2023-06-12 21:00:40.000000 topological-recursion-0.0a1/topological_recursion/__init__.py
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     4402 2023-06-12 21:00:40.000000 topological-recursion-0.0a1/topological_recursion/divisor.py
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    13958 2023-06-12 21:00:40.000000 topological-recursion-0.0a1/topological_recursion/intersection_numbers.py
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    48974 2023-06-12 21:00:40.000000 topological-recursion-0.0a1/topological_recursion/newton_polygon.py
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    21037 2023-06-12 21:00:40.000000 topological-recursion-0.0a1/topological_recursion/partitions.py
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     9430 2023-06-12 21:00:40.000000 topological-recursion-0.0a1/topological_recursion/permutations.py
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    23084 2023-06-12 21:00:40.000000 topological-recursion-0.0a1/topological_recursion/spectral_curve.py
-drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-12 21:30:53.942231 topological-recursion-0.0a1/topological_recursion.egg-info/
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     2086 2023-06-12 21:30:53.000000 topological-recursion-0.0a1/topological_recursion.egg-info/PKG-INFO
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)      486 2023-06-12 21:30:53.000000 topological-recursion-0.0a1/topological_recursion.egg-info/SOURCES.txt
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)        1 2023-06-12 21:30:53.000000 topological-recursion-0.0a1/topological_recursion.egg-info/dependency_links.txt
--rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       22 2023-06-12 21:30:53.000000 topological-recursion-0.0a1/topological_recursion.egg-info/top_level.txt
+drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-12 21:35:25.257631 topological-recursion-0.0a2/
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       35 2023-06-12 21:26:53.000000 topological-recursion-0.0a2/MANIFEST.in
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     2226 2023-06-12 21:35:25.257631 topological-recursion-0.0a2/PKG-INFO
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     1607 2023-06-12 21:34:05.000000 topological-recursion-0.0a2/README.rst
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)        6 2023-06-12 21:34:53.000000 topological-recursion-0.0a2/VERSION
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       38 2023-06-12 21:35:25.257631 topological-recursion-0.0a2/setup.cfg
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     1325 2023-06-12 21:29:07.000000 topological-recursion-0.0a2/setup.py
+drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-12 21:35:25.257631 topological-recursion-0.0a2/topological_recursion/
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)        0 2023-06-12 21:00:40.000000 topological-recursion-0.0a2/topological_recursion/__init__.py
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     4402 2023-06-12 21:00:40.000000 topological-recursion-0.0a2/topological_recursion/divisor.py
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    13958 2023-06-12 21:00:40.000000 topological-recursion-0.0a2/topological_recursion/intersection_numbers.py
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    48974 2023-06-12 21:00:40.000000 topological-recursion-0.0a2/topological_recursion/newton_polygon.py
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    21037 2023-06-12 21:00:40.000000 topological-recursion-0.0a2/topological_recursion/partitions.py
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     9430 2023-06-12 21:00:40.000000 topological-recursion-0.0a2/topological_recursion/permutations.py
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)    23084 2023-06-12 21:00:40.000000 topological-recursion-0.0a2/topological_recursion/spectral_curve.py
+drwxrwxr-x   0 doctorant  (1000) doctorant  (1000)        0 2023-06-12 21:35:25.257631 topological-recursion-0.0a2/topological_recursion.egg-info/
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)     2226 2023-06-12 21:35:25.000000 topological-recursion-0.0a2/topological_recursion.egg-info/PKG-INFO
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)      486 2023-06-12 21:35:25.000000 topological-recursion-0.0a2/topological_recursion.egg-info/SOURCES.txt
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)        1 2023-06-12 21:35:25.000000 topological-recursion-0.0a2/topological_recursion.egg-info/dependency_links.txt
+-rw-rw-r--   0 doctorant  (1000) doctorant  (1000)       22 2023-06-12 21:35:25.000000 topological-recursion-0.0a2/topological_recursion.egg-info/top_level.txt
```

### Comparing `topological-recursion-0.0a1/PKG-INFO` & `topological-recursion-0.0a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 Metadata-Version: 2.1
 Name: topological-recursion
-Version: 0.0a1
+Version: 0.0a2
 Summary: Topological recursion
 Home-page: https://gitlab.com/toprec/toprec
 Author: Vincent Delecroix, Bertrand Eynard, Dimitrios Mitsios
 Author-email: bertrand.eynard@ipht.fr
 License: GPLv2+
 Keywords: topological-recursion surfaces geometry
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 
-# Topological Recursion
+Topological Recursion
+=====================
 
 `topological-recursion` is a Python module to compute with topological
 recursion.
 
-## Installation
+Installation
+------------
 
-### Prerequisites
+Prerequisites
+^^^^^^^^^^^^^
 
 Make sure that Python 3 is installed in version 3.8 or later.
 
-### Pip installation
+Pip installation
+^^^^^^^^^^^^^^^^
 
 To install the module on your system, simply run::
 
       $ pip install topological-recursion
 
 The above command will download the code from
 [PyPI](https://pypi.org/project/topological-recursion/) and then
 install on your system.
 
-### Editable installation of the development version
+Editable installation of the development version
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Alternatively, if you want to install the development version, you
 need versioning software ``git`` installed. You first need to clone the
 project::
 
     $ git clone https://gitlab.com/toprec/toprec.git
 
@@ -54,25 +59,28 @@
 
 To check whether the installation worked, change repository and try to load
 the module with::
 
     $ python
     >>> import topological_recursion
 
-## Authors and acknowledgment
+Authors and acknowledgment
+--------------------------
 
 - V. Delecroix
 - B. Eynard
 - D. Mitsios
 
-## Aknowledgements
+Aknowledgements
+---------------
 
 - ERC ReNewQuantum
 
-## License
+License
+-------
 
 `topological-recursion` is distributed under the terms of the GNU General
 Public License (GPL) published by the Free Software Foundation; either version
 2 of the License, or (at your option) any later version.
 See http://www.gnu.org/licenses/.
```

### Comparing `topological-recursion-0.0a1/README.rst` & `topological-recursion-0.0a2/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-# Topological Recursion
+Topological Recursion
+=====================
 
 `topological-recursion` is a Python module to compute with topological
 recursion.
 
-## Installation
+Installation
+------------
 
-### Prerequisites
+Prerequisites
+^^^^^^^^^^^^^
 
 Make sure that Python 3 is installed in version 3.8 or later.
 
-### Pip installation
+Pip installation
+^^^^^^^^^^^^^^^^
 
 To install the module on your system, simply run::
 
       $ pip install topological-recursion
 
 The above command will download the code from
 [PyPI](https://pypi.org/project/topological-recursion/) and then
 install on your system.
 
-### Editable installation of the development version
+Editable installation of the development version
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Alternatively, if you want to install the development version, you
 need versioning software ``git`` installed. You first need to clone the
 project::
 
     $ git clone https://gitlab.com/toprec/toprec.git
 
@@ -38,23 +43,26 @@
 
 To check whether the installation worked, change repository and try to load
 the module with::
 
     $ python
     >>> import topological_recursion
 
-## Authors and acknowledgment
+Authors and acknowledgment
+--------------------------
 
 - V. Delecroix
 - B. Eynard
 - D. Mitsios
 
-## Aknowledgements
+Aknowledgements
+---------------
 
 - ERC ReNewQuantum
 
-## License
+License
+-------
 
 `topological-recursion` is distributed under the terms of the GNU General
 Public License (GPL) published by the Free Software Foundation; either version
 2 of the License, or (at your option) any later version.
 See http://www.gnu.org/licenses/.
```

### Comparing `topological-recursion-0.0a1/setup.py` & `topological-recursion-0.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `topological-recursion-0.0a1/topological_recursion/divisor.py` & `topological-recursion-0.0a2/topological_recursion/divisor.py`

 * *Files identical despite different names*

### Comparing `topological-recursion-0.0a1/topological_recursion/intersection_numbers.py` & `topological-recursion-0.0a2/topological_recursion/intersection_numbers.py`

 * *Files identical despite different names*

### Comparing `topological-recursion-0.0a1/topological_recursion/newton_polygon.py` & `topological-recursion-0.0a2/topological_recursion/newton_polygon.py`

 * *Files identical despite different names*

### Comparing `topological-recursion-0.0a1/topological_recursion/partitions.py` & `topological-recursion-0.0a2/topological_recursion/partitions.py`

 * *Files identical despite different names*

### Comparing `topological-recursion-0.0a1/topological_recursion/permutations.py` & `topological-recursion-0.0a2/topological_recursion/permutations.py`

 * *Files identical despite different names*

### Comparing `topological-recursion-0.0a1/topological_recursion/spectral_curve.py` & `topological-recursion-0.0a2/topological_recursion/spectral_curve.py`

 * *Files identical despite different names*

### Comparing `topological-recursion-0.0a1/topological_recursion.egg-info/PKG-INFO` & `topological-recursion-0.0a2/topological_recursion.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 Metadata-Version: 2.1
 Name: topological-recursion
-Version: 0.0a1
+Version: 0.0a2
 Summary: Topological recursion
 Home-page: https://gitlab.com/toprec/toprec
 Author: Vincent Delecroix, Bertrand Eynard, Dimitrios Mitsios
 Author-email: bertrand.eynard@ipht.fr
 License: GPLv2+
 Keywords: topological-recursion surfaces geometry
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 
-# Topological Recursion
+Topological Recursion
+=====================
 
 `topological-recursion` is a Python module to compute with topological
 recursion.
 
-## Installation
+Installation
+------------
 
-### Prerequisites
+Prerequisites
+^^^^^^^^^^^^^
 
 Make sure that Python 3 is installed in version 3.8 or later.
 
-### Pip installation
+Pip installation
+^^^^^^^^^^^^^^^^
 
 To install the module on your system, simply run::
 
       $ pip install topological-recursion
 
 The above command will download the code from
 [PyPI](https://pypi.org/project/topological-recursion/) and then
 install on your system.
 
-### Editable installation of the development version
+Editable installation of the development version
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Alternatively, if you want to install the development version, you
 need versioning software ``git`` installed. You first need to clone the
 project::
 
     $ git clone https://gitlab.com/toprec/toprec.git
 
@@ -54,25 +59,28 @@
 
 To check whether the installation worked, change repository and try to load
 the module with::
 
     $ python
     >>> import topological_recursion
 
-## Authors and acknowledgment
+Authors and acknowledgment
+--------------------------
 
 - V. Delecroix
 - B. Eynard
 - D. Mitsios
 
-## Aknowledgements
+Aknowledgements
+---------------
 
 - ERC ReNewQuantum
 
-## License
+License
+-------
 
 `topological-recursion` is distributed under the terms of the GNU General
 Public License (GPL) published by the Free Software Foundation; either version
 2 of the License, or (at your option) any later version.
 See http://www.gnu.org/licenses/.
```

