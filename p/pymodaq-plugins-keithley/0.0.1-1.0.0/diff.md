# Comparing `tmp/pymodaq_plugins_keithley-0.0.1.tar.gz` & `tmp/pymodaq_plugins_keithley-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_keithley-0.0.1.tar", last modified: Thu Jan 12 13:50:08 2023, max compression
+gzip compressed data, was "pymodaq_plugins_keithley-1.0.0.tar", last modified: Mon Jun 12 15:26:53 2023, max compression
```

## Comparing `pymodaq_plugins_keithley-0.0.1.tar` & `pymodaq_plugins_keithley-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.010091 pymodaq_plugins_keithley-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-01-12 13:50:08.010091 pymodaq_plugins_keithley-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 13:50:08.010091 pymodaq_plugins_keithley-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:07.998091 pymodaq_plugins_keithley-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.002091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.006091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_move_plugins/daq_move_Keithley2400.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.006091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.006091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Keithley2110.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Keithley_Pico.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.006091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.006091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.010091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.010091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.010091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/hardware/keithley2110/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/hardware/keithley2110/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-01-12 13:49:51.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/hardware/keithley2110/keithley2110_VISADriver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:50:08.006091 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-01-12 13:50:07.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-12 13:50:07.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 13:50:07.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-12 13:50:07.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-12 13:50:07.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-12 13:50:07.000000 pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.262825 pymodaq_plugins_keithley-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.262825 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_move_plugins/daq_move_Keithley2400.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Keithley2110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Keithley_Pico.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.266826 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/hardware/keithley2110/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/hardware/keithley2110/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-12 15:26:39.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/hardware/keithley2110/keithley2110_VISADriver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:26:53.262825 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-12 15:26:53.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-12 15:26:53.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:26:53.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 15:26:53.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 15:26:53.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 15:26:53.000000 pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_keithley-0.0.1/LICENSE` & `pymodaq_plugins_keithley-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_keithley-0.0.1/PKG-INFO` & `pymodaq_plugins_keithley-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_keithley
-Version: 0.0.1
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for various physical measurements from keithley
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_keithley
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_keithley-0.0.1/README.rst` & `pymodaq_plugins_keithley-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_keithley-0.0.1/setup.py` & `pymodaq_plugins_keithley-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_move_plugins/daq_move_Keithley2400.py` & `pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_move_plugins/daq_move_Keithley2400.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from easydict import EasyDict as edict
 from pymeasure.instruments.keithley import Keithley2400
 from pymeasure.adapters import VISAAdapter, PrologixAdapter
 
 from pymodaq.control_modules.move_utility_classes import DAQ_Move_base  # base class
 from pymodaq.control_modules.move_utility_classes import comon_parameters, main  # common set of parameters for all actuators
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, set_logger, get_module_name  # object used to send info back to the main thread
-from pymodaq.daq_utils.parameter.utils import iter_children
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.logger import set_logger, get_module_name  # object used to send info back to the main thread
+from pymodaq.utils.parameter.utils import iter_children
 from pyvisa import ResourceManager
 
 
 logger = set_logger(get_module_name(__file__))
 
 rm = ResourceManager()
```

### Comparing `pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Keithley2110.py` & `pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Keithley2110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, comon_parameters
-from pymodaq.daq_utils.daq_utils import DataFromPlugins
+from pymodaq.utils.data import DataFromPlugins
 from easydict import EasyDict as edict
 from collections import OrderedDict
 from ...hardware.keithley2110.keithley2110_VISADriver import Keithley2110VISADriver as Keithley2110
 
+
 class DAQ_0DViewer_Keithley2110(DAQ_Viewer_base):
     """
         Naive implementation of a DAQ 0D Viewer using the Keithley 2110 as data source
         This DAQ0D Viewer plugin only supports measurement mode selection and a simple data read acquisition mechanism
         with no averaging supported
         =============== =================
         **Attributes**  **Type**
```

### Comparing `pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Keithley_Pico.py` & `pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Keithley_Pico.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from qtpy.QtCore import Signal
 from easydict import EasyDict as edict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins
-from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import  DataFromPlugins
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main
 from collections import OrderedDict
 import numpy as np
 from enum import IntEnum
 from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 
+
 class DAQ_0DViewer_Keithley_Pico_type(IntEnum):
     """
         Enum class of Keithley_Pico_type
 
         =============== =========
         **Attributes**  **Type**
         *Pico_648X*     int
         *Pico_6430*     int
         *Pico_6514*     int
         =============== =========
     """
-    Pico_648X=0
-    Pico_6430=1
-    Pico_6514=2
+    Pico_648X = 0
+    Pico_6430 = 1
+    Pico_6514 = 2
+
     @classmethod
     def names(cls):
         return [name for name, member in cls.__members__.items()]
 
 
 class DAQ_0DViewer_Keithley_Pico(DAQ_Viewer_base):
     """
@@ -167,7 +170,11 @@
 
 
     def stop(self):
         """
             not implemented?
         """
         return ""
+
+
+if __name__ == '__main__':
+    main(__file__, init=False)
```

### Comparing `pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley/hardware/keithley2110/keithley2110_VISADriver.py` & `pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley/hardware/keithley2110/keithley2110_VISADriver.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley.egg-info/PKG-INFO` & `pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-keithley
-Version: 0.0.1
+Version: 1.0.0
 Summary: Set of PyMoDAQ plugins for various physical measurements from keithley
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_keithley
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_keithley-0.0.1/src/pymodaq_plugins_keithley.egg-info/SOURCES.txt` & `pymodaq_plugins_keithley-1.0.0/src/pymodaq_plugins_keithley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

