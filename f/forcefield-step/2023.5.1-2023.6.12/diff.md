# Comparing `tmp/forcefield_step-2023.5.1.tar.gz` & `tmp/forcefield_step-2023.6.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forcefield_step-2023.5.1.tar", last modified: Mon May  1 15:21:39 2023, max compression
+gzip compressed data, was "forcefield_step-2023.6.12.tar", last modified: Mon Jun 12 19:09:08 2023, max compression
```

## Comparing `forcefield_step-2023.5.1.tar` & `forcefield_step-2023.6.12.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.161509 forcefield_step-2023.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.161509 forcefield_step-2023.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.161509 forcefield_step-2023.5.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9604 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.165509 forcefield_step-2023.5.1/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.165509 forcefield_step-2023.5.1/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.165509 forcefield_step-2023.5.1/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/forcefield_step/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/forcefield_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/forcefield_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/data/lithium_battery.frc
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/data/nacl_water.frc
--rw-r--r--   0 runner    (1001) docker     (123)   474899 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/data/oplsaa.frc
--rw-r--r--   0 runner    (1001) docker     (123)   361764 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/data/pcff2018.frc
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/forcefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/forcefield_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/forcefield_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/forcefield_step/tk_forcefield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/forcefield_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 15:21:39.000000 forcefield_step-2023.5.1/forcefield_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:21:39.169509 forcefield_step-2023.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/tests/test_forcefield_step.py
--rw-r--r--   0 runner    (1001) docker     (123)   153001 2023-05-01 15:21:25.000000 forcefield_step-2023.5.1/tests/test_oplsaa_assignment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.865053 forcefield_step-2023.6.12/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-12 19:09:08.865053 forcefield_step-2023.6.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.857053 forcefield_step-2023.6.12/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.857053 forcefield_step-2023.6.12/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.857053 forcefield_step-2023.6.12/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9604 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.861053 forcefield_step-2023.6.12/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/developer_guide/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.861053 forcefield_step-2023.6.12/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.861053 forcefield_step-2023.6.12/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.865053 forcefield_step-2023.6.12/forcefield_step/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/forcefield_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-12 19:09:08.865053 forcefield_step-2023.6.12/forcefield_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.861053 forcefield_step-2023.6.12/forcefield_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/forcefield_step/data/lithium_battery.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/forcefield_step/data/nacl_water.frc
+-rw-r--r--   0 runner    (1001) docker     (123)   474899 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/forcefield_step/data/oplsaa.frc
+-rw-r--r--   0 runner    (1001) docker     (123)   361966 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/forcefield_step/data/pcff2018.frc
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/forcefield_step/forcefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/forcefield_step/forcefield_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/forcefield_step/forcefield_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/forcefield_step/tk_forcefield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.861053 forcefield_step-2023.6.12/forcefield_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-12 19:09:08.000000 forcefield_step-2023.6.12/forcefield_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-12 19:09:08.000000 forcefield_step-2023.6.12/forcefield_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:09:08.000000 forcefield_step-2023.6.12/forcefield_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 19:09:08.000000 forcefield_step-2023.6.12/forcefield_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 19:09:08.000000 forcefield_step-2023.6.12/forcefield_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 19:09:08.000000 forcefield_step-2023.6.12/forcefield_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-12 19:09:08.865053 forcefield_step-2023.6.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:09:08.865053 forcefield_step-2023.6.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/tests/test_forcefield_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153001 2023-06-12 19:08:41.000000 forcefield_step-2023.6.12/tests/test_oplsaa_assignment.py
```

### Comparing `forcefield_step-2023.5.1/CONTRIBUTING.rst` & `forcefield_step-2023.6.12/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/HISTORY.rst` & `forcefield_step-2023.6.12/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/LICENSE` & `forcefield_step-2023.6.12/LICENSE`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/PKG-INFO` & `forcefield_step-2023.6.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcefield_step
-Version: 2023.5.1
+Version: 2023.6.12
 Summary: A SEAMM plug-in for setting up a forcefield or EAM potentials for subsequent simulations.
 Home-page: https://github.com/molssi-seam/forcefield_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM
 Platform: Linux
```

### Comparing `forcefield_step-2023.5.1/README.rst` & `forcefield_step-2023.6.12/README.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/Makefile` & `forcefield_step-2023.6.12/docs/Makefile`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/_static/SEAMM inverted.png` & `forcefield_step-2023.6.12/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/_static/SEAMM logo.png` & `forcefield_step-2023.6.12/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/_static/molssi_main_logo.png` & `forcefield_step-2023.6.12/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/_static/molssi_main_logo_inverted_white.png` & `forcefield_step-2023.6.12/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/_static/molssi_square.png` & `forcefield_step-2023.6.12/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/_static/nsf.png` & `forcefield_step-2023.6.12/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/conf.py` & `forcefield_step-2023.6.12/docs/conf.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/developer_guide/installation.rst` & `forcefield_step-2023.6.12/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/getting_started/index.rst` & `forcefield_step-2023.6.12/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/index.rst` & `forcefield_step-2023.6.12/docs/index.rst`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/docs/make.bat` & `forcefield_step-2023.6.12/docs/make.bat`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/forcefield_step/__init__.py` & `forcefield_step-2023.6.12/forcefield_step/__init__.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/forcefield_step/data/lithium_battery.frc` & `forcefield_step-2023.6.12/forcefield_step/data/lithium_battery.frc`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/forcefield_step/data/nacl_water.frc` & `forcefield_step-2023.6.12/forcefield_step/data/nacl_water.frc`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/forcefield_step/data/oplsaa.frc` & `forcefield_step-2023.6.12/forcefield_step/data/oplsaa.frc`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/forcefield_step/data/pcff2018.frc` & `forcefield_step-2023.6.12/forcefield_step/data/pcff2018.frc`

 * *Files 0% similar despite different names*

```diff
@@ -6158,14 +6158,23 @@
         "2022.05.29": {
             "smarts": [
                 "[SX2:1]"
             ],
             "description": "Generic SP3 sulfur",
             "overrides": []
         }
+    },
+    "si": {
+        "2023.05.29": {
+            "smarts": [
+                "[SiX4:1]"
+            ],
+            "description": "generic SP3 silicon atom",
+            "overrides": []
+        }
     }
 }
 
 
 #reference 1
 @Author Biosym Technologies inc
 @Date 25-December-91
```

### Comparing `forcefield_step-2023.5.1/forcefield_step/forcefield.py` & `forcefield_step-2023.6.12/forcefield_step/forcefield.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/forcefield_step/forcefield_parameters.py` & `forcefield_step-2023.6.12/forcefield_step/forcefield_parameters.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/forcefield_step/forcefield_step.py` & `forcefield_step-2023.6.12/forcefield_step/forcefield_step.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/forcefield_step/tk_forcefield.py` & `forcefield_step-2023.6.12/forcefield_step/tk_forcefield.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/forcefield_step.egg-info/PKG-INFO` & `forcefield_step-2023.6.12/forcefield_step.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcefield-step
-Version: 2023.5.1
+Version: 2023.6.12
 Summary: A SEAMM plug-in for setting up a forcefield or EAM potentials for subsequent simulations.
 Home-page: https://github.com/molssi-seam/forcefield_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM
 Platform: Linux
```

### Comparing `forcefield_step-2023.5.1/forcefield_step.egg-info/SOURCES.txt` & `forcefield_step-2023.6.12/forcefield_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/setup.py` & `forcefield_step-2023.6.12/setup.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/tests/conftest.py` & `forcefield_step-2023.6.12/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/tests/test_forcefield_step.py` & `forcefield_step-2023.6.12/tests/test_forcefield_step.py`

 * *Files identical despite different names*

### Comparing `forcefield_step-2023.5.1/tests/test_oplsaa_assignment.py` & `forcefield_step-2023.6.12/tests/test_oplsaa_assignment.py`

 * *Files identical despite different names*

