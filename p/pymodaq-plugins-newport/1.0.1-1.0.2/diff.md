# Comparing `tmp/pymodaq_plugins_newport-1.0.1.tar.gz` & `tmp/pymodaq_plugins_newport-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_newport-1.0.1.tar", last modified: Tue Apr 25 16:27:43 2023, max compression
+gzip compressed data, was "pymodaq_plugins_newport-1.0.2.tar", last modified: Mon Jun 12 15:30:55 2023, max compression
```

## Comparing `pymodaq_plugins_newport-1.0.1.tar` & `pymodaq_plugins_newport-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.491520 pymodaq_plugins_newport-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-25 16:27:43.491520 pymodaq_plugins_newport-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:27:43.491520 pymodaq_plugins_newport-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.479519 pymodaq_plugins_newport-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.483519 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Conex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_AgilisSerial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_ESP100.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_SMC100.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_0D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.487520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.491520 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/agilis_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/esp100.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/serial_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-25 16:27:28.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/smc100.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:27:43.483519 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 16:27:43.000000 pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.760016 pymodaq_plugins_newport-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.760016 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Conex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_AgilisSerial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_ESP100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_SMC100.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_0D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/agilis_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/esp100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/serial_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-12 15:30:40.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/smc100.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:30:55.764016 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-12 15:30:55.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-12 15:30:55.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:30:55.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 15:30:55.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 15:30:55.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 15:30:55.000000 pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_newport-1.0.1/LICENSE` & `pymodaq_plugins_newport-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.1/PKG-INFO` & `pymodaq_plugins_newport-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_newport
-Version: 1.0.1
+Version: 1.0.2
 Summary: Set of PyMoDAQ plugins for instruments from Newport (Conex, ESP100,...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_newport
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_newport-1.0.1/README.rst` & `pymodaq_plugins_newport-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.1/setup.py` & `pymodaq_plugins_newport-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Conex.py` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Conex.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
         """
 
         """
         self.controller = self.ini_stage_init(controller, Conexcmd.ConexAGAPCmds())
 
         if self.settings['multiaxes', 'multi_status'] == "Master":
             out = self.controller.OpenInstrument(self.settings['com_port'][0:4])
+        else:
+            out = 0
 
         controller_name = self.controller.VE(self.settings['controller_address'], "", "")[1]
         motor_id = self.controller.ID_Get(self.settings['controller_address'], "", "")[1]
         self.settings.child('controller_name').setValue(controller_name)
         self.settings.child('motor_id').setValue(motor_id)
         info = controller_name + " / " + motor_id
         initialized = out == 0
```

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_AgilisSerial.py` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_AgilisSerial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, comon_parameters, main
-from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo, set_logger, get_module_name
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.logger import set_logger, get_module_name
 from easydict import EasyDict as edict
 
 from pymodaq_plugins_newport.hardware.agilis_serial import AgilisSerial, COMPORTS
 logger = set_logger(get_module_name(__file__))
 
 
 class DAQ_Move_Newport_AgilisSerial(DAQ_Move_base):
@@ -81,38 +82,38 @@
         except Exception as e:
             self.emit_status(
                 ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
             self.status.info = getLineInfo() + str(e)
             self.status.initialized = False
             return self.status
 
-    def check_position(self):
+    def get_actuator_value(self):
         """
         Get the current position from the hardware with scaling conversion.
 
         Returns
         -------
         float: The position obtained after scaling conversion.
         """
 
         #return self.controller.get_step_counter(self.settings.child('axis').value(), read_controller=False)
         return self.target_position
 
-    def move_Abs(self, position):
+    def move_abs(self, position):
         """
         Move the actuator to the absolute target defined by position.
         Parameters
         ----------
         position: (flaot) value of the absolute target positioning
         """
         position = self.check_bound(position)
         rel_position = position - self.current_position
-        self.move_Rel(rel_position)
+        self.move_rel(rel_position)
 
-    def move_Rel(self, relative_move):
+    def move_rel(self, relative_move):
         """
         Move the actuator to the relative target actuator value defined by
             relative_move
 
         Parameters
         ----------
         relative_move: (float) value of the relative distance to travel in
@@ -121,15 +122,15 @@
         """
         relative_move = self.check_bound(self.current_position + relative_move) - self.current_position
         relative_move = self.set_position_relative_with_scaling(relative_move)
         self.target_position = relative_move + self.current_position
 
         self.controller.move_rel(self.settings.child('axis').value(), int(relative_move))
 
-    def move_Home(self):
+    def move_home(self):
         """
 
         """
         self.controller.counter_to_zero(self.settings.child('axis').value())
         self.current_position = 0.
         self.target_position = 0.
```

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_ESP100.py` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_ESP100.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
-from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main
-from pymodaq.daq_move.utility_classes import comon_parameters
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main, comon_parameters_fun
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
 from pymodaq_plugins_newport.hardware.esp100 import ESP100
 from easydict import EasyDict as edict
 import pyvisa
 
 
 class DAQ_Move_Newport_ESP100(DAQ_Move_base):
     """
@@ -23,47 +22,41 @@
         ports.append(infos[k].alias)
     port = 'COM6' if 'COM6' in ports else ports[0] if len(ports) > 0 else ''
     #if ports==[]:
     #    ports.append('')
 
 
     is_multiaxes = False
-    stage_names = []
+    axes_names = []
+    _epsilon = 0.01
+
+    params = [{'title': 'Time interval (ms):', 'name': 'time_interval', 'type': 'int', 'value': 200},
+              {'title': 'Controller Info:', 'name': 'controller_id', 'type': 'text', 'value': '', 'readonly': True},
+              {'title': 'COM Port:', 'name': 'com_port', 'type': 'list', 'limits': ports, 'value': port},
+              {'title': 'Velocity:', 'name': 'velocity', 'type': 'float', 'value': 1.0},
+
+              ] + comon_parameters_fun(is_multiaxes, axes_names, epsilon=_epsilon)
 
-    params= [{'title': 'Time interval (ms):', 'name': 'time_interval', 'type': 'int', 'value': 200},
-             {'title': 'Controller Info:', 'name': 'controller_id', 'type': 'text', 'value': '', 'readonly': True},
-             {'title': 'COM Port:', 'name': 'com_port', 'type': 'list', 'limits': ports, 'value': port},
-             {'title': 'Velocity:', 'name': 'velocity', 'type': 'float', 'value': 1.0},
-
-            {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group','visible':is_multiaxes, 'children':[
-                        {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes, 'default': False},
-                        {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master', 'limits': ['Master', 'Slave']},
-                        {'title': 'Axis:', 'name': 'axis', 'type': 'list',  'limits': stage_names},
-                        
-                        ]}]+comon_parameters
 
-        
     def ini_attributes(self):
         self.settings.child('epsilon').setValue(0.01)
         self.controller: ESP100 = None
-        
 
     def ini_stage(self, controller=None):
             
         self.ini_stage_init(old_controller=controller,
                             new_controller=ESP100())
         
         if self.settings.child('multiaxes','multi_status').value() == "Master":
             self.controller.init_communication(self.settings.child('com_port').value(), self._axis)
             
         controller_id = self.controller.get_controller_infos()
         self.settings.child('controller_id').setValue(controller_id)
         self.settings.child('velocity').setValue(self.controller.get_velocity(self._axis))
         self.settings.child('velocity').setOpts(max=self.controller.get_velocity_max(self._axis))
-        self.settings.child('epsilon').setValue(0.1)
 
         info = f'Initialized with controller ID: {controller_id}'
         initialized = True
         return info, initialized
 
     def commit_settings(self,param):
         """
```

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_SMC100.py` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/daq_move_plugins/daq_move_Newport_SMC100.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 """
 Created on Mon Jan  9 15:57:26 2023
 
 @author: lb19g16
 """
 from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main  # base class
 from pymodaq.control_modules.move_utility_classes import comon_parameters_fun  # common set of parameters for all actuators
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo  # object used to send info back to the main thread
-from easydict import EasyDict as edict  # type of dict
+
 
 from pymodaq_plugins_newport.hardware.smc100 import SMC100
 import pyvisa
 
 VISA_rm = pyvisa.ResourceManager()
 infos = VISA_rm.list_resources_info()
 com_ports = [infos[key].alias for key in infos.keys() if infos[key].alias is not None]
@@ -25,33 +24,26 @@
     It then implements the particular communication with the instrument
 
     Attributes:
     -----------
     controller: object
         The particular object that allow the communication with the hardware, in general a python wrapper around the
          hardware library
-    # TODO add your particular attributes here if any
 
     """
-    _controller_units = 'mm'  # TODO for your plugin: put the correct unit here
-    is_multiaxes = True  # TODO for your plugin set to True if this plugin is controlled for a multiaxis controller
+    _controller_units = 'mm'
+    is_multiaxes = True
     axes_names = ['1']  # The axis list represents the number of smc controllers, indexed: first=1, second=2 etc.
     _epsilon = 0.0001
-    params = [  {'title': 'COM Port:', 'name': 'com_port', 'type': 'list', 'limits': com_ports, 'value': 'COM17'},
-              # TODO for your custom plugin: elements to be added here as dicts in order to control your custom stage
-                ] + comon_parameters_fun(is_multiaxes, axes_names)
+    params = [{'title': 'COM Port:', 'name': 'com_port', 'type': 'list', 'limits': com_ports, 'value': 'COM17'},
+                ] + comon_parameters_fun(is_multiaxes, axes_names, epsilon=_epsilon)
 
     def ini_attributes(self):
-        #  TODO declare the type of the wrapper (and assign it to self.controller) you're going to use for easy
-        #  autocompletion
         self.controller: SMC100 = None
 
-        #TODO declare here attributes you want/need to init with a default value
-        pass
-
     def get_actuator_value(self):
         """Get the current value from the hardware with scaling conversion.
 
         Returns
         -------
         float: The position obtained after scaling conversion.
         """
@@ -71,19 +63,15 @@
         """Apply the consequences of a change of value in the detector settings
 
         Parameters
         ----------
         param: Parameter
             A given parameter (within detector_settings) whose value has been changed by the user
         """
-        ## TODO for your custom plugin
-        if param.name() == "a_parameter_you've_added_in_self.params":
-           self.controller.your_method_to_apply_this_param_change()
-        else:
-            pass
+        pass
 
     def ini_stage(self, controller=None):
         """Actuator communication initialization
 
         Parameters
         ----------
         controller: (object)
@@ -99,57 +87,52 @@
         self.ini_stage_init(old_controller=controller,
                             new_controller=SMC100())
         if self.settings['multiaxes', 'multi_status'] == "Master":
             self.controller.init_communication(
                 self.settings['com_port'])
         axis = int(self.settings.child('multiaxes', 'axis').value())
         info = self.controller.get_controller_infos(axis)
-        initialized = True  # todo
+        initialized = True
         return info, initialized
 
     def move_abs(self, value):
         """ Move the actuator to the absolute target defined by value
 
         Parameters
         ----------
         value: (float) value of the absolute target positioning
         """
 
         value = self.check_bound(value)  #if user checked bounds, the defined bounds are applied here
         self.target_value = value
         value = self.set_position_with_scaling(value)  # apply scaling if the user specified one
-        ## TODO for your custom plugin
-        axis = int(self.settings.child('multiaxes', 'axis').value())
-        self.controller.move_axis(axis=axis,pos=value)  # when writing your own plugin replace this line
+
+        axis = int(self.settings['multiaxes', 'axis'])
+        self.controller.move_axis(axis=axis, pos=value)  # when writing your own plugin replace this line
 
     def move_rel(self, value):
         """ Move the actuator to the relative target actuator value defined by value
 
         Parameters
         ----------
         value: (float) value of the relative target positioning
         """
         value = self.check_bound(self.current_position + value) - self.current_position
         self.target_value = value + self.current_position
         value = self.set_position_relative_with_scaling(value)
 
-        axis = int(self.settings.child('multiaxes', 'axis').value())
-        self.controller.move_axis('REL',axis=axis,pos=value)  # when writing your own plugin replace this line
-
+        axis = int(self.settings['multiaxes', 'axis'])
+        self.controller.move_axis('REL', axis=axis, pos=value)  # when writing your own plugin replace this line
 
     def move_home(self):
         """Call the reference method of the controller"""
-
-        ## TODO for your custom plugin
-        axis = int(self.settings.child('multiaxes', 'axis').value())
+        axis = int(self.settings['multiaxes', 'axis'])
         self.controller.move_home(axis)  # when writing your own plugin replace this line
 
-
     def stop_motion(self):
-      """Stop the actuator and emits move_done signal"""
-
-      axis = int(self.settings.child('multiaxes', 'axis').value())
-      self.controller.stop_motion(axis)  # when writing your own plugin replace this line
+        """Stop the actuator and emits move_done signal"""
+        axis = int(self.settings['multiaxes', 'axis'])
+        self.controller.stop_motion(axis)  # when writing your own plugin replace this line
 
 
 if __name__ == '__main__':
-    main(__file__)
+    main(__file__)
```

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/agilis_serial.py` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/agilis_serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 import pyvisa
 from threading import Lock
 from pyvisa.errors import VisaIOError
-import pymodaq.daq_utils.daq_utils as utils
+import pymodaq.utils.daq_utils as utils
 from pymodaq.utils.logger import set_logger, get_module_name
 
 logger = set_logger(get_module_name(__file__), add_to_console=False)
 visa_rm = pyvisa.ResourceManager()
 
 _infos = visa_rm.list_resources_info()
 COMPORTS = []
```

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/esp100.py` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/esp100.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/serial_base.py` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/serial_base.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport/hardware/smc100.py` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport/hardware/smc100.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/PKG-INFO` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-newport
-Version: 1.0.1
+Version: 1.0.2
 Summary: Set of PyMoDAQ plugins for instruments from Newport (Conex, ESP100,...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_newport
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_newport-1.0.1/src/pymodaq_plugins_newport.egg-info/SOURCES.txt` & `pymodaq_plugins_newport-1.0.2/src/pymodaq_plugins_newport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

