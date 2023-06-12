# Comparing `tmp/pymodaq_plugins_thorlabs-1.0.0.tar.gz` & `tmp/pymodaq_plugins_thorlabs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_thorlabs-1.0.0.tar", last modified: Tue Apr 25 16:29:49 2023, max compression
+gzip compressed data, was "pymodaq_plugins_thorlabs-1.0.1.tar", last modified: Mon Jun 12 15:28:57 2023, max compression
```

## Comparing `pymodaq_plugins_thorlabs-1.0.0.tar` & `pymodaq_plugins_thorlabs-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis_Flipper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-04-25 16:29:36.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/hardware/powermeter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:29:49.250679 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 16:29:49.000000 pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.575821 pymodaq_plugins_thorlabs-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.579820 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisFlipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisIntegratedStepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/powermeter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.579820 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_thorlabs-1.0.0/LICENSE` & `pymodaq_plugins_thorlabs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.0/PKG-INFO` & `pymodaq_plugins_thorlabs-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_thorlabs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Set of PyMoDAQ plugins for instruments from Thorlabs (Kinesis K10CR1 (stepper rotation actuator), Kinesis Flipper, Kinesis KSP100, DCx camera...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_thorlabs
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_thorlabs-1.0.0/README.rst` & `pymodaq_plugins_thorlabs-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.0/setup.py` & `pymodaq_plugins_thorlabs-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main
-from pymodaq.control_modules.move_utility_classes import comon_parameters
+from pymodaq.control_modules.move_utility_classes import comon_parameters_fun
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
 from pymodaq.utils.logger import set_logger, get_module_name
 import clr
 from qtpy import QtWidgets
 import sys
 from easydict import EasyDict as edict
 
@@ -37,15 +37,15 @@
 
         See Also
         --------
         daq_utils.ThreadCommand
 
     """
     _controller_units = 'degrees'
-
+    _epsilon = 0.05
 
     try:
 
         Device.DeviceManagerCLI.BuildDeviceList()
         serialnumbers = [str(ser) for ser in Device.DeviceManagerCLI.GetDeviceList(Integrated.CageRotator.DevicePrefix)]
 
     except:
@@ -53,29 +53,20 @@
     is_multiaxes = False
 
     stage_names = []
 
     params = [{'title': 'Kinesis library:', 'name': 'kinesis_lib', 'type': 'browsepath', 'value': kinesis_path},
               {'title': 'Controller ID:', 'name': 'controller_id', 'type': 'str', 'value': '', 'readonly': True},
               {'title': 'Serial number:', 'name': 'serial_number', 'type': 'list', 'limits': serialnumbers},
-              {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group', 'visible': is_multiaxes, 'children': [
-                  {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes,
-                   'default': False},
-                  {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master',
-                   'limits': ['Master', 'Slave']},
-                  {'title': 'Axis:', 'name': 'axis', 'type': 'list', 'limits': stage_names},
-
-              ]}] + comon_parameters
+              ] + comon_parameters_fun(is_multiaxes, epsilon=_epsilon)
 
-    def __init__(self, parent=None, params_state=None):
-        super().__init__(parent, params_state)
 
+    def ini_attributes(self):
 
-        self.controller = None
-        self.settings.child('epsilon').setValue(0.005)
+        self.controller: Integrated.CageRotator.CreateCageRotator = None
 
         try:
             if MOVEDONEACTION:
                 self.move_done_action = Action[UInt64](self.someaction)  # if selected wil trigger
                 # self.someaction when move is done
 
             else:
@@ -83,15 +74,15 @@
 
 
         except Exception as e:
             self.emit_status(ThreadCommand("Update_Status", [getLineInfo() + str(e), 'log']))
             raise Exception(getLineInfo() + str(e))
 
     def someaction(self, pos_action):
-        position = self.check_position()
+        position = self.get_actuator_value()
         logger.debug(f'posaction is {pos_action} and position is {position}')
 
     def commit_settings(self, param):
         """
             | Activate any parameter changes on the hardware.
             | Called after a param_tree_changed signal received from DAQ_Move_main.
 
@@ -108,77 +99,42 @@
 
             except:
                 serialnumbers = []
             self.settings.child('serial_number').setOpts(limits=serialnumbers)
 
     def ini_stage(self, controller=None):
         """
-            Initialize the controller and stages (axes) with given parameters.
-
-            =============== ================================================ =========================================================================================
-            **Parameters**   **Type**                                         **Description**
-            *controller*     instance of the specific controller object       If defined this hardware will use it and will not initialize its own controller instance
-            *stage*          instance of the stage (axis or whatever) object  ???
-            =============== ================================================ =========================================================================================
-
-            Returns
-            -------
-            Easydict
-                dictionnary containing keys:
-                 * *info* : string displaying various info
-                 * *controller*: instance of the controller object in order to control other axes without the need to init the same controller twice
-                 * *stage*: instance of the stage (axis or whatever) object
-                 * *initialized*: boolean indicating if initialization has been done corretly
-
-            See Also
-            --------
-            daq_utils.ThreadCommand
         """
-        try:
-            self.status.update(edict(info="", controller=None, initialized=False))
 
-            # check whether this stage is controlled by a multiaxe controller (to be defined for each plugin)
-
-            # if mutliaxes then init the controller here if Master state otherwise use external controller
-            if self.settings.child('multiaxes', 'ismultiaxes').value() and self.settings.child('multiaxes',
-                                                                                               'multi_status').value() == "Slave":
-                if controller is None:
-                    raise Exception('no controller has been defined externally while this axe is a slave one')
-                else:
-                    self.controller = controller
-            else:  # Master stage
+        Device.DeviceManagerCLI.BuildDeviceList()
+        serialnumbers = Device.DeviceManagerCLI.GetDeviceList(Integrated.CageRotator.DevicePrefix)
+        ser_bool = self.settings['serial_number'] in serialnumbers
+        if ser_bool:
+            self.controller = self.ini_stage_init(controller,
+                                                  Integrated.CageRotator.CreateCageRotator(
+                                                      self.settings['serial_number']))
+        else:
+            raise Exception("Not valid serial number")
+
+        if self.settings['multiaxes', 'multi_status'] == "Master":
+
+            self.controller.Connect(self.settings['serial_number'])
+            self.controller.WaitForSettingsInitialized(5000)
+            self.controller.StartPolling(250)
+
+        info = self.controller.GetDeviceInfo().Name
+        self.settings.child('controller_id').setValue(info)
+        if not (self.controller.IsSettingsInitialized()):
+            raise (Exception("no Stage Connected"))
+        else:
+            self.controller.LoadMotorConfiguration(self.settings['serial_number'])
+        self.controller.SetBacklash(Decimal(0))
 
-                Device.DeviceManagerCLI.BuildDeviceList()
-                serialnumbers = Device.DeviceManagerCLI.GetDeviceList(Integrated.CageRotator.DevicePrefix)
-                ser_bool = self.settings.child('serial_number').value() in serialnumbers
-                if ser_bool:
-                    self.controller = Integrated.CageRotator.CreateCageRotator(
-                        self.settings.child('serial_number').value())
-                    self.controller.Connect(self.settings.child('serial_number').value())
-                    self.controller.WaitForSettingsInitialized(5000)
-                    self.controller.StartPolling(250)
-                else:
-                    raise Exception("Not valid serial number")
-
-            info = self.controller.GetDeviceInfo().Name
-            self.settings.child('controller_id').setValue(info)
-            if not (self.controller.IsSettingsInitialized()):
-                raise (Exception("no Stage Connected"))
-            self.motorSettings = self.controller.GetMotorConfiguration(self.settings.child('serial_number').value(), 2)
-            self.controller.SetBacklash(Decimal(0))
-            self.status.info = info
-            self.status.controller = self.controller
-            self.status.initialized = True
-            return self.status
-
-        except Exception as e:
-            self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
-            self.status.info = getLineInfo() + str(e)
-            self.status.initialized = False
-            return self.status
+        initialized = True
+        return info, initialized
 
     def close(self):
         """
             close the current instance of Kinesis instrument.
         """
         self.controller.StopPolling()
         self.controller.Disconnect()
@@ -190,30 +146,30 @@
             See Also
             --------
             DAQ_Move_base.move_done
         """
         self.controller.stop(0)
         self.move_done()
 
-    def check_position(self):
+    def get_actuator_value(self):
         """
             Get the current hardware position with scaling conversion of the Kinsesis insrument provided by get_position_with_scaling
 
             See Also
             --------
             DAQ_Move_base.get_position_with_scaling, daq_utils.ThreadCommand
         """
 
         pos = Decimal.ToDouble(self.controller.ContinuousRotationPosition)
         logger.debug(f'Motor state is {self.controller.State} and position is {pos}')
         pos = self.get_position_with_scaling(pos)
         self.emit_status(ThreadCommand('check_position', [pos]))
         return pos
 
-    def move_Abs(self, position):
+    def move_abs(self, position):
         """
             Make the hardware absolute move from the given position of the Kinesis instrument after thread command signal was received in DAQ_Move_main.
 
             =============== ========= =======================
             **Parameters**  **Type**   **Description**
 
             *position*       float     The absolute position
@@ -228,15 +184,15 @@
         self.target_position = position
 
         position = self.set_position_with_scaling(position)
         logger.debug(f'Should move to {position} but decimal gets {Decimal.ToDouble(Decimal(position))}')
         self.controller.MoveTo(Decimal(position), self.move_done_action)
         QtWidgets.QApplication.processEvents()
 
-    def move_Rel(self, position):
+    def move_rel(self, position):
         """
             | Make the hardware relative move from the given position of the Kinesis instrument after thread command signal was received in DAQ_Move_main.
             |
             | The final target position is given by **current_position+position**.
 
             =============== ========= =======================
             **Parameters**  **Type**   **Description**
@@ -252,18 +208,16 @@
         position = self.check_bound(self.current_position + position) - self.current_position
         self.target_position = position + self.current_position
         logger.debug(f'Should move to {Decimal.ToDouble(Decimal(self.target_position))}')
         position = self.set_position_relative_with_scaling(position)
 
         self.controller.MoveRelative(Generic.MotorDirection.Forward, Decimal(position), self.move_done_action)
 
-
-
-    def move_Home(self):
+    def move_home(self):
         """
             Make the absolute move to original position (0).
         """
         self.controller.Home(self.move_done_action)
 
 
 if __name__ == '__main__':
-    main(__file__)
+    main(__file__, init=False)
```

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis_Flipper.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,74 @@
 from pymodaq.control_modules.move_utility_classes import DAQ_Move_base
 from pymodaq.control_modules.move_utility_classes import comon_parameters
-from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
 from easydict import EasyDict as edict
-import clr
-import sys
 
+import pylablib.devices.Thorlabs as Thorlabs
 
-class DAQ_Move_Kinesis_Flipper(DAQ_Move_base):
-    """
-        Wrapper object to access the conex fonctionnalities, similar wrapper for all controllers.
+is_multiaxes = False
+stage_names = []
 
-        ================ =================
+class DAQ_Move_MFF101_pylablib(DAQ_Move_base):
+    """
+        Wrapper object to access the Flipper functionalities, similar wrapper for all controllers.
+        =============== ==============
         **Attributes**    **Type**
-        *Kinesis_path*    string
-        *serialnumbers*   int list
-        *params*          dictionnary list
-        ================ =================
-
-        See Also
-        --------
-        daq_utils.ThreadCommand
+        *params*          dictionnary
+        =============== ==============
     """
     _controller_units = 'binary position'
 
-    #Kinesis_path=os.environ['Kinesis'] #environement variable pointing to 'C:\\Program Files\\Thorlabs\\Kinesis'
-    #to be adjusted on the different computers
-    Kinesis_path='C:\\Program Files\\Thorlabs\\Kinesis'
-    try:
-        from System import Decimal
-        from System import Action
-        from System import UInt32
-        from System import UInt64
-
-        sys.path.append(Kinesis_path)
-
-        clr.AddReference("Thorlabs.MotionControl.IntegratedStepperMotorsCLI")
-        clr.AddReference("Thorlabs.MotionControl.DeviceManagerCLI")
-        clr.AddReference("Thorlabs.MotionControl.GenericMotorCLI")
-        clr.AddReference("Thorlabs.MotionControl.FilterFlipperCLI")
-
-        import Thorlabs.MotionControl.FilterFlipperCLI as Flipper
-        import Thorlabs.MotionControl.DeviceManagerCLI as Device
-        import Thorlabs.MotionControl.GenericMotorCLI as Generic
-
-
-        Device.DeviceManagerCLI.BuildDeviceList()
-        serialnumbers=[str(ser) for ser in Device.DeviceManagerCLI.GetDeviceList(Flipper.FilterFlipper.DevicePrefix)]
-    except Exception as e:
-        serialnumbers=[]
-    is_multiaxes=False
-    stage_names=[]
-
-
-    params= [{'title': 'Kinesis library:', 'name': 'kinesis_lib', 'type': 'browsepath', 'value': Kinesis_path},
-             {'title': 'Controller ID:', 'name': 'controller_id', 'type': 'str', 'value': '', 'readonly': True},
-             {'title': 'Serial number:', 'name': 'serial_number', 'type': 'list', 'limits':serialnumbers},
-              {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group','visible':is_multiaxes, 'children':[
+    _dvc = Thorlabs.list_kinesis_devices()
+    serialnumbers = [d[0] for d in _dvc if d[1] == 'APT Filter Flipper']
+
+    params= [{'title': 'Controller ID:', 'name': 'controller_id', 'type': 'str', 'value': '', 'readonly': True},
+             {'title': 'Serial number:', 'name': 'serial_number', 'type': 'list', 'limits': serialnumbers},
+             {'title': 'Home Position:', 'name': 'home_position', 'type': 'list' , 'value': 0, 'limits' : [0,1]},
+             {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group', 'visible': is_multiaxes, 'children':[
                         {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes, 'default': False},
-                        {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master', 'limits': ['Master','Slave']},
-                        {'title': 'Axis:', 'name': 'axis', 'type': 'list',  'limits':stage_names},
-                        
-                        ]}]+comon_parameters
+                        {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master', 'limits': ['Master', 'Slave']},
+                        {'title': 'Axis:', 'name': 'axis', 'type': 'list', 'limits': stage_names},
+                        ]
+              }
+             ]+comon_parameters
+
 
     def __init__(self, parent=None, params_state=None):
         super().__init__(parent, params_state)
-        self.settings.child(('epsilon')).setValue(1)
+        self.settings.child('epsilon').setValue(0.1)
+        self.settings.child('epsilon').setReadonly()
+
         self.settings.child('bounds', 'is_bounds').setValue(True)
+        self.settings.child('bounds', 'is_bounds').setReadonly()
+
         self.settings.child('bounds', 'max_bound').setValue(1)
+        self.settings.child('bounds', 'max_bound').setReadonly()
+
         self.settings.child('bounds', 'min_bound').setValue(0)
+        self.settings.child('bounds', 'min_bound').setReadonly()
 
-        try:
-            #Kinesis_path=os.environ['Kinesis'] #environement variable pointing to 'C:\\Program Files\\Thorlabs\\Kinesis'
-            #to be adjusted on the different computers
-            self.move_done_action=self.Action[self.UInt64](self.move_done)
-
-        except Exception as e:
-            self.emit_status(ThreadCommand("Update_Status",[getLineInfo()+ str(e),'log']))
-            raise Exception(getLineInfo()+ str(e))
+        self.settings.child('scaling','use_scaling').setValue(False)
+        self.settings.child('scaling','use_scaling').setReadonly()
+        self.settings.child('scaling','scaling').setValue(1)
+        self.settings.child('scaling','scaling').setReadonly()
+        self.settings.child('scaling','offset').setValue(0)
+        self.settings.child('scaling','offset').setReadonly()
 
     def commit_settings(self,param):
         """
             | Activate any parameter changes on the hardware.
             | Called after a param_tree_changed signal received from DAQ_Move_main.
 
             =============== ================================ ========================
             **Parameters**  **Type**                          **Description**
             *param*         instance of pyqtgraph Parameter  The parameter to update
             =============== ================================ ========================
         """
-        if param.name()==kinesis_lib:
-            self.Kinesis_path=param.value()
-            try:
-                sys.path.append(self.Kinesis_path)
-                clr.AddReference("Thorlabs.MotionControl.IntegratedStepperMotorsCLI")
-                clr.AddReference("Thorlabs.MotionControl.DeviceManagerCLI")
-                clr.AddReference("Thorlabs.MotionControl.GenericMotorCLI")
-                clr.AddReference("Thorlabs.MotionControl.FilterFlipperCLI")
-
-                import Thorlabs.MotionControl.FilterFlipperCLI as Flipper
-                import Thorlabs.MotionControl.DeviceManagerCLI as Device
-                import Thorlabs.MotionControl.GenericMotorCLI as Generic
-                Device.DeviceManagerCLI.BuildDeviceList()
-                serialnumbers=[str(ser) for ser in Device.DeviceManagerCLI.GetDeviceList(Flipper.FilterFlipper.DevicePrefix)]
-
-            except:
-                serialnumbers=[]
-            self.settings.child(('serial_number')).setOpts(limits=serialnumbers)
-
-
+        pass
 
     def ini_stage(self,controller=None):
         """Initialize the controller and stages (axes) with given parameters.
 
             ============== =========================================== ===========================================================================================
             **Parameters**  **Type**                                     **Description**
 
@@ -127,86 +84,90 @@
                  * *stage*: instance of the stage (axis or whatever) object
                  * *initialized*: boolean indicating if initialization has been done corretly
 
             See Also
             --------
             daq_utils.ThreadCommand
         """
-            
         try:
             self.status.update(edict(info="",controller=None,initialized=False))
 
-
             #check whether this stage is controlled by a multiaxe controller (to be defined for each plugin)
 
-            # if mutliaxes then init the controller here if Master state otherwise use external controller
+            # if multiaxes then init the controller here if Master state otherwise use external controller
             if self.settings.child('multiaxes','ismultiaxes').value() and self.settings.child('multiaxes','multi_status').value()=="Slave":
                 if controller is None: 
                     raise Exception('no controller has been defined externally while this axe is a slave one')
                 else:
-                    self.controller=controller
+                    self.controller = controller
             else: #Master stage
-               
-                self.Device.DeviceManagerCLI.BuildDeviceList()
-                serialnumbers = self.Device.DeviceManagerCLI.GetDeviceList(self.Flipper.FilterFlipper.DevicePrefix)
-                #Check if the serial number in the parameters exists in the available devices
-                ser_bool = self.settings.child(('serial_number')).value() in serialnumbers
-                if ser_bool:
-                    self.controller=self.Flipper.FilterFlipper.CreateFilterFlipper(self.settings.child(('serial_number')).value())
-                    self.controller.Connect(self.settings.child(('serial_number')).value())
-                    self.controller.WaitForSettingsInitialized(5000)
-                    self.controller.StartPolling(250)
+                try:
+                    controller = Thorlabs.kinesis.MFF(self.settings.child('serial_number').value())
+                except:
+                    raise Exception(f'No controller found with serial number {self.settings.child("serial_number").value()}')
                 else:
-                    raise Exception("Not valid serial number")
+                    self.controller = controller
 
+            if not self.controller.is_opened():
+                self.controller.open()
 
-            info=self.controller.GetDeviceInfo().Name
-            self.settings.child(('controller_id')).setValue(info)
-            if not(self.controller.IsSettingsInitialized()):
-                raise(Exception("no Stage Connected"))
+            #Getting the information from the device
+            info = self.controller.get_device_info()
 
-            self.status.info = info
+            #Setting the name of the controller == Type of controller
+            self.settings.child('controller_id').setValue(info.notes)
+
+            #Setting the transit time
+            ttime_s = self.controller.get_flipper_parameters().transit_time
+            self.settings.child('timeout').setValue(ttime_s*1e3) #Transit time ms
+
+            #IDK what that does but ok
+            self.status.info = info.notes
             self.status.controller = self.controller
             self.status.initialized = True
             return self.status
-
+        #This is in case something fails
         except Exception as e:
             self.emit_status(ThreadCommand('Update_Status',[getLineInfo()+ str(e),'log']))
             self.status.info=getLineInfo()+ str(e)
             self.status.initialized=False
             return self.status
 
     def close(self):
         """
             close the current instance of Kinesis Flipper instrument.
         """
-        self.controller.StopPolling()
-        self.controller.Disconnect()
-        self.controller.Dispose()
+        self.controller.close()
         self.controller=None
 
     def stop_motion(self):
         """
             See Also
             --------
             DAQ_Move_base.move_done
         """
-        self.controller.stop(0)
+        # self.controller.stop(0)
         self.move_done()
 
     def check_position(self):
         """
-            Get the current hardware position with scaling conversion of the Kinsesis insrument provided by get_position_with_scaling
+            Get the current hardware position with scaling conversion of the Kinesis insrument provided by get_position_with_scaling
 
             See Also
             --------
             DAQ_Move_base.get_position_with_scaling, daq_utils.ThreadCommand
         """
-        pos = self.controller.Position
-        pos = self.get_position_with_scaling(pos)
+        #Get position = 0 or 1, possibly None if unknown
+        pos = self.controller.get_state()
+        #Repollif pos returns none
+        while pos == None:
+            pos = self.controller.get_state()
+
+        #This is superfluous as there is not scaling
+        # pos = self.get_position_with_scaling(pos)
         self.emit_status(ThreadCommand('check_position', [pos]))
         return pos
 
     def move_Abs(self,position):
         """
             Make the hardware absolute move from the given position after thread command signal was received in DAQ_Move_main.
 
@@ -217,52 +178,56 @@
             =============== ========= =======================
 
             See Also
             --------
             DAQ_Move_base.set_position_with_scaling
 
         """
-        pos = self.check_position()
-        if int(pos) == 1:
-            position = 2
-        else:
-            position = 1
+        position = self.check_bound(position)
+        # superfluous because there is no scaling for a flipper
+        # position = self.set_position_with_scaling(position)  # apply scaling if the user specified one
+
+        # pos = self.check_position()
+        # if pos == 0:
+        #     position = 1
+        # else:
+        #     position = 0
 
+        self.controller.move_to_state(position)
+        self.emit_status(ThreadCommand('Update_Status', [f'Moving to position: {position}']))
 
-        self.target_position=position
-        self.controller.SetPosition(self.UInt32(position),self.move_done_action)
+        self.target_position = position
+        self.poll_moving()
 
 
     def move_Rel(self,position):
-        """
-            | Make the hardware relative move from the given position of the Kinesis instrument after thread command signal was received in DAQ_Move_main.
-            |
-            | The final target position is given by (current_position+position).
-
-            =============== ========= =======================
-            **Parameters**  **Type**   **Description**
-
-            *position*       float     The absolute position
-            =============== ========= =======================
-
-            See Also
-            --------
-            hardware.set_position_with_scaling
-
-        """
-        pos = self.check_position()
-        if int(pos) == 1:
-            position = 2
-        else:
-            position = 1
-
-
-        self.target_position = position
-        self.controller.SetPosition(self.UInt32(position), self.move_done_action)
+        """ Move the actuator to the relative target actuator value defined by position
+        Parameters
+        ----------
+        position: (float) value of the relative target positioning
+        """
+        self.current_position = self.check_position()
+        # rel_move  = self.check_bound(self.current_position+position)-self.current_position
+        new_pos = self.check_bound(self.current_position + position)
+        self.target_position = new_pos
+
+        # pos = self.check_position()
+        # if pos == 0:
+        #     position = 1
+        # else:
+        #     position = 0
+
+        # self.target_position = position
+        self.controller.move_to_state(new_pos)
+        self.emit_status(ThreadCommand('Update_Status', [f'Moving to position: {position}']))
+        self.poll_moving()
 
 
     def move_Home(self):
         """
             Make the absolute move to original position (0).
         """
-        self.controller.Home(self.move_done_action)
-
+        home = self.settings.child('home_position').value()
+        self.target_position = home
+        self.controller.move_to_state(home)
+        self.emit_status(ThreadCommand('Update_Status', [f'Moving home: {home}']))
+        self.poll_moving()
```

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,74 +1,81 @@
-from pymodaq.control_modules.move_utility_classes import DAQ_Move_base
-from pymodaq.control_modules.move_utility_classes import comon_parameters
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main
+from pymodaq.control_modules.move_utility_classes import comon_parameters_fun
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
 from easydict import EasyDict as edict
 
 import pylablib.devices.Thorlabs as Thorlabs
 
-is_multiaxes = False
-stage_names = []
 
-class DAQ_Move_MFF101_pylablib(DAQ_Move_base):
+
+class DAQ_Move_PRM1Z8_pylablib(DAQ_Move_base):
     """
         Wrapper object to access the Flipper functionalities, similar wrapper for all controllers.
         =============== ==============
         **Attributes**    **Type**
         *params*          dictionnary
         =============== ==============
     """
-    _controller_units = 'binary position'
-
+    _controller_units = 'deg'
+    is_multiaxes = False
+    stage_names = []
+    _epsilon = 0.1
     _dvc = Thorlabs.list_kinesis_devices()
-    serialnumbers = [d[0] for d in _dvc if d[1] == 'APT Filter Flipper']
+    #serialnumbers = [d[0] for d in _dvc if d[1] == 'APT DC Motor Controller']
+    serialnumbers = [d[0] for d in _dvc]
 
     params= [{'title': 'Controller ID:', 'name': 'controller_id', 'type': 'str', 'value': '', 'readonly': True},
              {'title': 'Serial number:', 'name': 'serial_number', 'type': 'list', 'limits': serialnumbers},
-             {'title': 'Home Position:', 'name': 'home_position', 'type': 'list' , 'value': 0, 'limits' : [0,1]},
-             {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group', 'visible': is_multiaxes, 'children':[
-                        {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes, 'default': False},
-                        {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master', 'limits': ['Master', 'Slave']},
-                        {'title': 'Axis:', 'name': 'axis', 'type': 'list', 'limits': stage_names},
-                        ]
-              }
-             ]+comon_parameters
+             {'title': 'Home Position:', 'name': 'home_position', 'type': 'float', 'value': 0.0},
+             {'title': 'Set Zero', 'name': 'set_zero', 'type': 'bool_push', 'value': False},
+             {'title': 'Reset Home', 'name': 'reset_home', 'type': 'bool_push', 'value': False},
 
+             ] + comon_parameters_fun(is_multiaxes, stage_names, epsilon=_epsilon)
 
     def __init__(self, parent=None, params_state=None):
         super().__init__(parent, params_state)
-        self.settings.child('epsilon').setValue(0.1)
+        self.settings.child('epsilon').setValue(0.005)
         self.settings.child('epsilon').setReadonly()
 
-        self.settings.child('bounds', 'is_bounds').setValue(True)
-        self.settings.child('bounds', 'is_bounds').setReadonly()
+        self.settings.child('timeout').setValue(100)
 
-        self.settings.child('bounds', 'max_bound').setValue(1)
-        self.settings.child('bounds', 'max_bound').setReadonly()
+        #Scaling and bounds can be set to False because they are just not needed
+        self.settings.child('bounds', 'is_bounds').setValue(False)
+        self.settings.child('bounds', 'is_bounds').setReadonly()
+        self.settings.child('bounds').hide()
+        self.settings.child('scaling', 'use_scaling').setValue(False)
+        self.settings.child('scaling', 'use_scaling').setReadonly()
+        self.settings.child('scaling').hide()
 
-        self.settings.child('bounds', 'min_bound').setValue(0)
-        self.settings.child('bounds', 'min_bound').setReadonly()
+        #Home is fixed (for now)
+        # self.settings.child('home_position').setReadonly()
 
-        self.settings.child('scaling','use_scaling').setValue(False)
-        self.settings.child('scaling','use_scaling').setReadonly()
-        self.settings.child('scaling','scaling').setValue(1)
-        self.settings.child('scaling','scaling').setReadonly()
-        self.settings.child('scaling','offset').setValue(0)
-        self.settings.child('scaling','offset').setReadonly()
+        # self.settings.child('scaling','scaling').setReadonly()
+        # self.settings.child('scaling','offset').setReadonly()
 
     def commit_settings(self,param):
         """
             | Activate any parameter changes on the hardware.
             | Called after a param_tree_changed signal received from DAQ_Move_main.
 
             =============== ================================ ========================
             **Parameters**  **Type**                          **Description**
             *param*         instance of pyqtgraph Parameter  The parameter to update
             =============== ================================ ========================
         """
-        pass
+        if param.name() == 'set_zero':
+            if param.value() == True:
+                self.controller.set_position_reference(scale=True)
+                self.check_position()
+                self.settings.child('set_zero').setValue(False)
+        elif param.name() == 'reset_home':
+            if param.value() == True:
+                self.controller.home(force=True, timeout=self.settings.child('timeout').value())
+                self.check_position()
+                self.settings.child('reset_home').setValue(False)
 
     def ini_stage(self,controller=None):
         """Initialize the controller and stages (axes) with given parameters.
 
             ============== =========================================== ===========================================================================================
             **Parameters**  **Type**                                     **Description**
 
@@ -97,32 +104,34 @@
             if self.settings.child('multiaxes','ismultiaxes').value() and self.settings.child('multiaxes','multi_status').value()=="Slave":
                 if controller is None: 
                     raise Exception('no controller has been defined externally while this axe is a slave one')
                 else:
                     self.controller = controller
             else: #Master stage
                 try:
-                    controller = Thorlabs.kinesis.MFF(self.settings.child('serial_number').value())
+                    controller = Thorlabs.kinesis.KinesisMotor(self.settings.child('serial_number').value(),scale='stage')
                 except:
                     raise Exception(f'No controller found with serial number {self.settings.child("serial_number").value()}')
                 else:
                     self.controller = controller
 
             if not self.controller.is_opened():
                 self.controller.open()
 
             #Getting the information from the device
             info = self.controller.get_device_info()
 
-            #Setting the name of the controller == Type of controller
-            self.settings.child('controller_id').setValue(info.notes)
+            #Setting the name of the controller
+            #asserting that the controller is scale_aware and
+            stage_name = self.controller.get_stage()
+            assert stage_name == 'PRM1-Z8'
+            self.settings.child('controller_id').setValue(stage_name)
 
-            #Setting the transit time
-            ttime_s = self.controller.get_flipper_parameters().transit_time
-            self.settings.child('timeout').setValue(ttime_s*1e3) #Transit time ms
+            unit = self.controller.get_scale_units()
+            assert unit == 'deg'
 
             #IDK what that does but ok
             self.status.info = info.notes
             self.status.controller = self.controller
             self.status.initialized = True
             return self.status
         #This is in case something fails
@@ -133,45 +142,46 @@
             return self.status
 
     def close(self):
         """
             close the current instance of Kinesis Flipper instrument.
         """
         self.controller.close()
-        self.controller=None
+        self.controller = None
 
     def stop_motion(self):
         """
             See Also
             --------
             DAQ_Move_base.move_done
         """
         # self.controller.stop(0)
         self.move_done()
 
     def check_position(self):
         """
-            Get the current hardware position with scaling conversion of the Kinesis insrument provided by get_position_with_scaling
+            Get the current hardware position with scaling conversion of the Kinesis
+            instrument provided by get_position_with_scaling
 
             See Also
             --------
             DAQ_Move_base.get_position_with_scaling, daq_utils.ThreadCommand
         """
         #Get position = 0 or 1, possibly None if unknown
-        pos = self.controller.get_state()
-        #Repollif pos returns none
+        pos = self.controller.get_position()
+        #Repoll if pos returns none
         while pos == None:
-            pos = self.controller.get_state()
+            pos = self.controller.get_position()
 
         #This is superfluous as there is not scaling
         # pos = self.get_position_with_scaling(pos)
         self.emit_status(ThreadCommand('check_position', [pos]))
         return pos
 
-    def move_Abs(self,position):
+    def move_abs(self,position):
         """
             Make the hardware absolute move from the given position after thread command signal was received in DAQ_Move_main.
 
             =============== ========= =======================
             **Parameters**  **Type**   **Description**
 
             *position*       int       either 1 or 2 for the flipper
@@ -179,55 +189,43 @@
 
             See Also
             --------
             DAQ_Move_base.set_position_with_scaling
 
         """
         position = self.check_bound(position)
-        # superfluous because there is no scaling for a flipper
-        # position = self.set_position_with_scaling(position)  # apply scaling if the user specified one
-
-        # pos = self.check_position()
-        # if pos == 0:
-        #     position = 1
-        # else:
-        #     position = 0
 
-        self.controller.move_to_state(position)
+        self.controller.move_to(position)
         self.emit_status(ThreadCommand('Update_Status', [f'Moving to position: {position}']))
 
         self.target_position = position
         self.poll_moving()
 
-
-    def move_Rel(self,position):
+    def move_rel(self,position):
         """ Move the actuator to the relative target actuator value defined by position
         Parameters
         ----------
         position: (float) value of the relative target positioning
         """
         self.current_position = self.check_position()
         # rel_move  = self.check_bound(self.current_position+position)-self.current_position
         new_pos = self.check_bound(self.current_position + position)
         self.target_position = new_pos
 
-        # pos = self.check_position()
-        # if pos == 0:
-        #     position = 1
-        # else:
-        #     position = 0
-
         # self.target_position = position
-        self.controller.move_to_state(new_pos)
+        self.controller.move_to(new_pos)
         self.emit_status(ThreadCommand('Update_Status', [f'Moving to position: {position}']))
         self.poll_moving()
 
-
-    def move_Home(self):
+    def move_home(self):
         """
             Make the absolute move to original position (0).
         """
         home = self.settings.child('home_position').value()
         self.target_position = home
-        self.controller.move_to_state(home)
+        self.controller.move_to(home)
         self.emit_status(ThreadCommand('Update_Status', [f'Moving home: {home}']))
-        self.poll_moving()
+        self.poll_moving()
+
+
+if __name__ == '__main__':
+    main(__file__, init=False)
```

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,230 +1,184 @@
-from pymodaq.control_modules.move_utility_classes import DAQ_Move_base
-from pymodaq.control_modules.move_utility_classes import comon_parameters
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
+import sys
+from qtpy.QtCore import QThread
 from easydict import EasyDict as edict
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
+from collections import OrderedDict
+import numpy as np
+import clr
+from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 
-import pylablib.devices.Thorlabs as Thorlabs
 
-is_multiaxes = False
-stage_names = []
-
-class DAQ_Move_PRM1Z8_pylablib(DAQ_Move_base):
+class DAQ_0DViewer_Kinesis_KPA101(DAQ_Viewer_base):
     """
-        Wrapper object to access the Flipper functionalities, similar wrapper for all controllers.
-        =============== ==============
-        **Attributes**    **Type**
-        *params*          dictionnary
-        =============== ==============
+        ==================== ========================
+        **Attributes**        **Type**
+        *data_grabed_signal*  instance of Signal
+        *VISA_rm*             ResourceManager
+        *com_ports*           
+        *params*              dictionnary list
+        *keithley*
+        *settings*
+        ==================== ========================
     """
-    _controller_units = 'deg'
+    ##checking VISA ressources
 
-    _dvc = Thorlabs.list_kinesis_devices()
-    serialnumbers = [d[0] for d in _dvc if d[1] == 'APT DC Motor Controller']
+    _controller_units = 'V'
+    kinesis_path = 'C:\\Program Files\\Thorlabs\\Kinesis'
 
-    params= [{'title': 'Controller ID:', 'name': 'controller_id', 'type': 'str', 'value': '', 'readonly': True},
-             {'title': 'Serial number:', 'name': 'serial_number', 'type': 'list', 'limits': serialnumbers},
-             {'title': 'Home Position:', 'name': 'home_position', 'type': 'float', 'value': 0.0},
-             {'title': 'Set Zero', 'name': 'set_zero', 'type': 'bool_push', 'value': False},
-             {'title': 'Reset Home', 'name': 'reset_home', 'type': 'bool_push', 'value': False},
-             {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group', 'visible': is_multiaxes, 'children':[
-                        {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes, 'default': False},
-                        {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master', 'limits': ['Master', 'Slave']},
-                        {'title': 'Axis:', 'name': 'axis', 'type': 'list', 'limits': stage_names},
-                        ]
-              }
-             ]+comon_parameters
+    try:
+        sys.path.append(kinesis_path)
+        clr.AddReference("Thorlabs.MotionControl.DeviceManagerCLI")
+        clr.AddReference("Thorlabs.MotionControl.KCube.PositionAlignerCLI")
+        import Thorlabs.MotionControl.DeviceManagerCLI as Device
+        import Thorlabs.MotionControl.KCube.PositionAlignerCLI as PosAligner
+        Device.DeviceManagerCLI.BuildDeviceList()
+        # %%
+        serialnumbers = [str(ser) for ser in
+                         Device.DeviceManagerCLI.GetDeviceList(PosAligner.KCubePositionAligner.DevicePrefix)]
+        # %%
+
+    except:
+        serialnumbers=[]
+
+    params = comon_parameters+[
+            {'title': 'Kinesis library:', 'name': 'kinesis_lib', 'type': 'browsepath', 'value': kinesis_path},
+            {'title': 'Serial number:', 'name': 'serial_number', 'type': 'list', 'limits': serialnumbers},
+            {'title': 'Device:', 'name': 'device_name', 'type': 'str', 'value': ''},
+            {'title': 'Polling time (ms):', 'name': 'polling_time', 'type': 'int', 'value': 250},
+            ]
 
     def __init__(self, parent=None, params_state=None):
         super().__init__(parent, params_state)
-        self.settings.child('epsilon').setValue(0.005)
-        self.settings.child('epsilon').setReadonly()
-
-        self.settings.child('timeout').setValue(100)
-
-        #Scaling and bounds can be set to False because they are just not needed
-        self.settings.child('bounds', 'is_bounds').setValue(False)
-        self.settings.child('bounds', 'is_bounds').setReadonly()
-        self.settings.child('bounds').hide()
-        self.settings.child('scaling', 'use_scaling').setValue(False)
-        self.settings.child('scaling', 'use_scaling').setReadonly()
-        self.settings.child('scaling').hide()
-
-        #Home is fixed (for now)
-        # self.settings.child('home_position').setReadonly()
-
-        # self.settings.child('scaling','scaling').setReadonly()
-        # self.settings.child('scaling','offset').setReadonly()
-
-    def commit_settings(self,param):
-        """
-            | Activate any parameter changes on the hardware.
-            | Called after a param_tree_changed signal received from DAQ_Move_main.
-
-            =============== ================================ ========================
-            **Parameters**  **Type**                          **Description**
-            *param*         instance of pyqtgraph Parameter  The parameter to update
-            =============== ================================ ========================
-        """
-        if param.name() == 'set_zero':
-            if param.value() == True:
-                self.controller.set_position_reference(scale=True)
-                self.check_position()
-                self.settings.child('set_zero').setValue(False)
-        elif param.name() == 'reset_home':
-            if param.value() == True:
-                self.controller.home(force=True, timeout=self.settings.child('timeout').value())
-                self.check_position()
-                self.settings.child('reset_home').setValue(False)
-
-    def ini_stage(self,controller=None):
-        """Initialize the controller and stages (axes) with given parameters.
-
-            ============== =========================================== ===========================================================================================
-            **Parameters**  **Type**                                     **Description**
+        self.controller = None
 
-            *controller*    instance of the specific controller object  If defined this hardware will use it and will not initialize its own controller instance
-            ============== =========================================== ===========================================================================================
+    def ini_detector(self, controller=None):
+        """
+            Initialisation procedure of the detector.
 
             Returns
             -------
-            Easydict
-                dictionnary containing keys:
-                 * *info* : string displaying various info
-                 * *controller*: instance of the controller object in order to control other axes without the need to init the same controller twice
-                 * *stage*: instance of the stage (axis or whatever) object
-                 * *initialized*: boolean indicating if initialization has been done corretly
+
+                The initialized status.
 
             See Also
             --------
             daq_utils.ThreadCommand
         """
+        self.status.update(edict(initialized=False, info="", x_axis=None, y_axis=None, controller=None))
         try:
-            self.status.update(edict(info="",controller=None,initialized=False))
-
-            #check whether this stage is controlled by a multiaxe controller (to be defined for each plugin)
 
-            # if multiaxes then init the controller here if Master state otherwise use external controller
-            if self.settings.child('multiaxes','ismultiaxes').value() and self.settings.child('multiaxes','multi_status').value()=="Slave":
+            if self.settings.child(('controller_status')).value() == "Slave":
                 if controller is None: 
-                    raise Exception('no controller has been defined externally while this axe is a slave one')
+                    raise Exception('no controller has been defined externally while this detector is a slave one')
                 else:
                     self.controller = controller
-            else: #Master stage
-                try:
-                    controller = Thorlabs.kinesis.KinesisMotor(self.settings.child('serial_number').value(),scale='stage')
-                except:
-                    raise Exception(f'No controller found with serial number {self.settings.child("serial_number").value()}')
-                else:
-                    self.controller = controller
-
-            if not self.controller.is_opened():
-                self.controller.open()
-
-            #Getting the information from the device
-            info = self.controller.get_device_info()
-
-            #Setting the name of the controller
-            #asserting that the controller is scale_aware and
-            stage_name = self.controller.get_stage()
-            assert stage_name == 'PRM1-Z8'
-            self.settings.child('controller_id').setValue(stage_name)
+            else:
+                self.Device.DeviceManagerCLI.BuildDeviceList()
+                serialnumbers = self.Device.DeviceManagerCLI.GetDeviceList(self.PosAligner.KCubePositionAligner.DevicePrefix)
+                ser_bool = self.settings.child(('serial_number')).value() in serialnumbers
+                if ser_bool:
+                    self.controller = self.PosAligner.KCubePositionAligner.CreateKCubePositionAligner(
+                        self.settings.child(('serial_number')).value())
+                    self.controller.Connect(self.settings.child(('serial_number')).value())
+                    if not self.controller.IsSettingsInitialized():
+                        self.controller.WaitForSettingsInitialized(5000)
+                    self.controller.StartPolling(self.settings.child(('polling_time')).value())
+                    self.emit_status(ThreadCommand('update_main_settings', [['wait_time'],
+                                                            self.settings.child(('polling_time')).value(), 'value']))
+                    QThread.msleep(500)
+                    self.controller.EnableDevice()
+                    QThread.msleep(500)
+                    deviceInfo = self.controller.GetDeviceInfo()
+                    self.settings.child(('device_name')).setValue(deviceInfo.Name)
 
-            unit = self.controller.get_scale_units()
-            assert unit == 'deg'
+                else:
+                    raise Exception("Not valid serial number")
 
-            #IDK what that does but ok
-            self.status.info = info.notes
-            self.status.controller = self.controller
             self.status.initialized = True
+            self.status.controller = self.controller
             return self.status
-        #This is in case something fails
+
         except Exception as e:
-            self.emit_status(ThreadCommand('Update_Status',[getLineInfo()+ str(e),'log']))
-            self.status.info=getLineInfo()+ str(e)
-            self.status.initialized=False
+            self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
+            self.status.info = getLineInfo() + str(e)
+            self.status.initialized = False
             return self.status
 
-    def close(self):
-        """
-            close the current instance of Kinesis Flipper instrument.
-        """
-        self.controller.close()
-        self.controller = None
 
-    def stop_motion(self):
-        """
-            See Also
-            --------
-            DAQ_Move_base.move_done
+    def commit_settings(self, param):
         """
-        # self.controller.stop(0)
-        self.move_done()
+            Activate the parameters changes in the hardware.
 
-    def check_position(self):
-        """
-            Get the current hardware position with scaling conversion of the Kinesis
-            instrument provided by get_position_with_scaling
+            =============== ================================= ============================
+            **Parameters**   **Type**                         **Description**
+            *param*         instance of pyqtgraph.parameter   The parameter to be checked.
+            =============== ================================= ============================
 
             See Also
             --------
-            DAQ_Move_base.get_position_with_scaling, daq_utils.ThreadCommand
+            daq_utils.ThreadCommand
         """
-        #Get position = 0 or 1, possibly None if unknown
-        pos = self.controller.get_position()
-        #Repoll if pos returns none
-        while pos == None:
-            pos = self.controller.get_position()
-
-        #This is superfluous as there is not scaling
-        # pos = self.get_position_with_scaling(pos)
-        self.emit_status(ThreadCommand('check_position', [pos]))
-        return pos
+        try:
+            if param.name() == 'kinesis_lib':
+                try:
+                    sys.path.append(param.value())
+                    clr.AddReference("Thorlabs.MotionControl.DeviceManagerCLI")
+                    clr.AddReference("Thorlabs.MotionControl.IntegratedStepperMotorsCLI")
+                    clr.AddReference("Thorlabs.MotionControl.GenericMotorCLI")
+                    import Thorlabs.MotionControl.IntegratedStepperMotorsCLI as Integrated
+                    import Thorlabs.MotionControl.DeviceManagerCLI as Device
+                    import Thorlabs.MotionControl.GenericMotorCLI as Generic
+                    Device.DeviceManagerCLI.BuildDeviceList()
+                    serialnumbers = [str(ser) for ser in
+                                     Device.DeviceManagerCLI.GetDeviceList(Integrated.CageRotator.DevicePrefix)]
 
-    def move_Abs(self,position):
-        """
-            Make the hardware absolute move from the given position after thread command signal was received in DAQ_Move_main.
+                except:
+                    serialnumbers = []
+                self.settings.child(('serial_number')).setOpts(limits=serialnumbers)
 
-            =============== ========= =======================
-            **Parameters**  **Type**   **Description**
+            elif param.name() == 'polling_time':
+                self.controller.StopPolling()
+                QThread.msleep(500)
+                self.controller.StartPolling(self.settings.child(('polling_time')).value())
+                QThread.msleep(500)
+                self.emit_status(ThreadCommand('update_main_settings', [['wait_time'], param.value(), 'value']))
 
-            *position*       int       either 1 or 2 for the flipper
-            =============== ========= =======================
 
-            See Also
-            --------
-            DAQ_Move_base.set_position_with_scaling
+        except Exception as e:
+            self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
 
+    def close(self):
         """
-        position = self.check_bound(position)
-
-        self.controller.move_to(position)
-        self.emit_status(ThreadCommand('Update_Status', [f'Moving to position: {position}']))
+            close the current instance of Keithley viewer.
+        """
+        self.controller.DisableDevice()
+        self.controller.StopPolling()
+        self.controller.Disconnect(False)
 
-        self.target_position = position
-        self.poll_moving()
+    def grab_data(self, Naverage=1, **kwargs):
+        """
+            | Start new acquisition.
+            | grab the current values with keithley profile procedure.
+            | Send the data_grabed_signal once done.
 
-    def move_Rel(self,position):
-        """ Move the actuator to the relative target actuator value defined by position
-        Parameters
-        ----------
-        position: (float) value of the relative target positioning
+            =============== ======== ===============================================
+            **Parameters**  **Type**  **Description**
+            *Naverage*      int       Number of values to average
+            =============== ======== ===============================================
         """
-        self.current_position = self.check_position()
-        # rel_move  = self.check_bound(self.current_position+position)-self.current_position
-        new_pos = self.check_bound(self.current_position + position)
-        self.target_position = new_pos
+        status = self.controller.Status
+        data = [np.array([status.PositionDifference.X]), np.array([status.PositionDifference.Y])]
+        data_intens = [np.array([status.Sum])]
+        self.data_grabed_signal.emit([DataFromPlugins(name='KPA101 Positions', data=data, dim='Data0D',
+                                                      labels=['X (V)', 'Y (V)'],),
+                                      DataFromPlugins(name='KPA101 Intensity', data=data_intens, dim='Data0D',
+                                                      labels=['Intensity'],)])
 
-        # self.target_position = position
-        self.controller.move_to(new_pos)
-        self.emit_status(ThreadCommand('Update_Status', [f'Moving to position: {position}']))
-        self.poll_moving()
 
-    def move_Home(self):
+    def stop(self):
         """
-            Make the absolute move to original position (0).
+            not implemented?
         """
-        home = self.settings.child('home_position').value()
-        self.target_position = home
-        self.controller.move_to(home)
-        self.emit_status(ThreadCommand('Update_Status', [f'Moving home: {home}']))
-        self.poll_moving()
+        return ""
```

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,21 +143,27 @@
         kwargs: (dict) of others optionals arguments
         """
         #The instrumental library seems really broken AF unfortunately so I have to use this to acquire a frame otherwise
         #it just uses the default values...
         kwds = {'exposure_time': Q_(self.settings.child('exposure').value(), 'ms'),
                 'gain': self.settings.child('master_gain').value()}
 
-        data =self.controller.grab_image(**kwds)
+        data = self.controller.grab_image(**kwds)
+
+        if len(data.shape) > 2:
+            data_list = [data[..., ind] for ind in range(data.shape[2])]
+        else:
+            data_list = [data]
+
         # data = self.controller.grab_image(exposure_time=Q_(self.settings.child('exposure').value(), 'ms'))
-        self.data_grabed_signal.emit([DataFromPlugins(name='Thorcam', data=[data],
+        self.data_grabed_signal.emit([DataFromPlugins(name='Thorcam', data=data_list,
                                                       dim='Data2D')])
 
     def stop(self):
 
         self.controller.stop_live_video()
         # self.emit_status(ThreadCommand('Update_Status', ['Some info you want to log']))
         return ''
 
 
 if __name__ == '__main__':
-    main(__file__)
+    main(__file__, init=False)
```

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs/hardware/powermeter.py` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/powermeter.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-thorlabs
-Version: 1.0.0
+Version: 1.0.1
 Summary: Set of PyMoDAQ plugins for instruments from Thorlabs (Kinesis K10CR1 (stepper rotation actuator), Kinesis Flipper, Kinesis KSP100, DCx camera...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_thorlabs
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_thorlabs-1.0.0/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt` & `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 src/pymodaq_plugins_thorlabs.egg-info/dependency_links.txt
 src/pymodaq_plugins_thorlabs.egg-info/entry_points.txt
 src/pymodaq_plugins_thorlabs.egg-info/requires.txt
 src/pymodaq_plugins_thorlabs.egg-info/top_level.txt
 src/pymodaq_plugins_thorlabs/daq_move_plugins/__init__.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py
-src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis_Flipper.py
+src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisFlipper.py
+src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisIntegratedStepper.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/__init__.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/__init__.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/__init__.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/__init__.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/__init__.py
 src/pymodaq_plugins_thorlabs/hardware/__init__.py
+src/pymodaq_plugins_thorlabs/hardware/kinesis.py
 src/pymodaq_plugins_thorlabs/hardware/powermeter.py
```

