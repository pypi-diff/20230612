# Comparing `tmp/coreali-0.0.2.tar.gz` & `tmp/coreali-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coreali-0.0.2.tar", last modified: Tue Aug 16 17:22:16 2022, max compression
+gzip compressed data, was "coreali-0.0.3.tar", last modified: Mon Jun 12 19:44:59 2023, max compression
```

## Comparing `coreali-0.0.2.tar` & `coreali-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 17:22:16.890219 coreali-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-08-16 17:22:07.000000 coreali-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-16 17:22:07.000000 coreali-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3225 2022-08-16 17:22:16.890219 coreali-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-08-16 17:22:07.000000 coreali-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-08-16 17:22:16.894219 coreali-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-16 17:22:07.000000 coreali-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 17:22:16.890219 coreali-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 17:22:16.890219 coreali-0.0.2/src/coreali/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 17:22:16.890219 coreali-0.0.2/src/coreali/registerio/
--rw-r--r--   0 runner    (1001) docker     (121)     2642 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/registerio/RegIo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/registerio/RegIoNoHW.py
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/registerio/Tester.py
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/registerio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 17:22:16.890219 coreali-0.0.2/src/coreali/regmodel/
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/regmodel/Component.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/regmodel/Field.py
--rw-r--r--   0 runner    (1001) docker     (121)     4051 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/regmodel/Memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/regmodel/Register.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/regmodel/RegisterFile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/regmodel/RegisterModel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4163 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/regmodel/SelectableComponent.py
--rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/regmodel/Selector.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-08-16 17:22:07.000000 coreali-0.0.2/src/coreali/regmodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 17:22:16.890219 coreali-0.0.2/src/coreali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3225 2022-08-16 17:22:16.000000 coreali-0.0.2/src/coreali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-08-16 17:22:16.000000 coreali-0.0.2/src/coreali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 17:22:16.000000 coreali-0.0.2/src/coreali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-16 17:22:16.000000 coreali-0.0.2/src/coreali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-16 17:22:16.000000 coreali-0.0.2/src/coreali.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.918453 coreali-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.910452 coreali-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.910452 coreali-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-12 19:44:43.000000 coreali-0.0.3/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-12 19:44:43.000000 coreali-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-12 19:44:43.000000 coreali-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 19:44:43.000000 coreali-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-12 19:44:43.000000 coreali-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-12 19:44:59.918453 coreali-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-12 19:44:43.000000 coreali-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.910452 coreali-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 19:44:43.000000 coreali-0.0.3/docs/coreali_reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 19:44:43.000000 coreali-0.0.3/docs/development_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-12 19:44:43.000000 coreali-0.0.3/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-12 19:44:43.000000 coreali-0.0.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.910452 coreali-0.0.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.910452 coreali-0.0.3/examples/jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.910452 coreali-0.0.3/examples/jupyterlab/.ipynb_checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-12 19:44:43.000000 coreali-0.0.3/examples/jupyterlab/.ipynb_checkpoints/run_example-checkpoint.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-12 19:44:43.000000 coreali-0.0.3/examples/jupyterlab/run_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.910452 coreali-0.0.3/examples/quickstart/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-12 19:44:43.000000 coreali-0.0.3/examples/quickstart/run_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.914452 coreali-0.0.3/examples/systemrdl/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 19:44:43.000000 coreali-0.0.3/examples/systemrdl/i2c_master_core.rdl
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 19:44:43.000000 coreali-0.0.3/examples/systemrdl/logger.rdl
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-12 19:44:43.000000 coreali-0.0.3/examples/systemrdl/top_sys.rdl
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-12 19:44:43.000000 coreali-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-12 19:44:43.000000 coreali-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 19:44:43.000000 coreali-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:44:59.918453 coreali-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 19:44:43.000000 coreali-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.910452 coreali-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.914452 coreali-0.0.3/src/coreali/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.914452 coreali-0.0.3/src/coreali/registerio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/registerio/RegIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/registerio/RegIoNoHW.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/registerio/Tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/registerio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.914452 coreali-0.0.3/src/coreali/regmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/regmodel/Component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/regmodel/Field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/regmodel/Memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/regmodel/Register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/regmodel/RegisterFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/regmodel/RegisterModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/regmodel/SelectableComponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/regmodel/Selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-12 19:44:43.000000 coreali-0.0.3/src/coreali/regmodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.914452 coreali-0.0.3/src/coreali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-12 19:44:59.000000 coreali-0.0.3/src/coreali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-12 19:44:59.000000 coreali-0.0.3/src/coreali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:44:59.000000 coreali-0.0.3/src/coreali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 19:44:59.000000 coreali-0.0.3/src/coreali.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 19:44:59.000000 coreali-0.0.3/src/coreali.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-12 19:44:43.000000 coreali-0.0.3/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:44:59.918453 coreali-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/regmodel_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/test_mem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/test_register_description.rdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/test_registerio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/test_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-06-12 19:44:43.000000 coreali-0.0.3/tests/test_use_cases.py
```

### Comparing `coreali-0.0.2/LICENSE` & `coreali-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coreali-0.0.2/PKG-INFO` & `coreali-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: coreali
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convenient Register Access Library
-Home-page: https://github.com/siforrer/coreali
 Author: Silvan Forrer
-License: MIT
-Project-URL: Bug Tracker, https://github.com/siforrer/coreali/issues
+Project-URL: Homepage, https://github.com/siforrer/coreali
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # coreali - Convenient Register Access Library
 Generates Python code from a register model. This python code can the be used to access the registers of an FPGA, a MCU or another device which has a register map.
 ## Installation
 Coreali can be installed with pip by executing the following command
```

### Comparing `coreali-0.0.2/README.md` & `coreali-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `coreali-0.0.2/src/coreali/registerio/RegIo.py` & `coreali-0.0.3/src/coreali/registerio/RegIo.py`

 * *Files identical despite different names*

### Comparing `coreali-0.0.2/src/coreali/registerio/RegIoNoHW.py` & `coreali-0.0.3/src/coreali/registerio/RegIoNoHW.py`

 * *Files identical despite different names*

### Comparing `coreali-0.0.2/src/coreali/registerio/Tester.py` & `coreali-0.0.3/src/coreali/registerio/Tester.py`

 * *Files identical despite different names*

### Comparing `coreali-0.0.2/src/coreali/regmodel/Component.py` & `coreali-0.0.3/src/coreali/regmodel/Component.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import numpy as np
 
+
 class Component:
     def __init__(self, root, node, parent):
         self._root = root
         self.node = node
         self._parent = parent
+        self._update_attr()
+
+    def _update_attr(self):
+        pass
 
     def _format_string(self, indent, value=None):
         formstr = " "*indent + "{:" + str(22-indent) + "}:"
         if value is None:
             ret = formstr.format(self.node.inst_name)
         elif isinstance(value, (str)):
             formstr += " {:s}"
```

### Comparing `coreali-0.0.2/src/coreali/regmodel/Field.py` & `coreali-0.0.3/src/coreali/regmodel/Field.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,40 +7,49 @@
 
     This class allows the read and write access to fields in a register.
     """
 
     def __init__(self, root, node, parent, rio):
         Component.__init__(self, root, node, parent)
 
+    def _update_attr(self):
+        """
+            Update attributes that object has a read/write function only
+            if the field itself is read/writeable
+        """
+        if self.node.is_sw_writable:
+            setattr(self, "write", self._write)
+        if self.node.is_sw_readable:
+            setattr(self, "read", self._read)
+
     def _register_to_field_value(self, register_value):
         field_value = np.uint64(register_value*2**(-self.node.lsb))
         field_value = np.mod(field_value, np.uint64(
             2**(self.node.msb-self.node.lsb+1)))
         return field_value
 
-    def read(self):
+    def _read(self):
         """Read field value
 
         Returns:
             np.uint64: Field value
         """
         return self._register_to_field_value(self._parent.read())
 
-    def write(self, field_value):
+    def _write(self, field_value):
         """Write field value
 
         """
         self._parent.modify(self.node.lsb, self.node.msb, field_value)
 
     def _tostr(self, indent, value):
         field_value = self._register_to_field_value(value)
         return self._format_string(indent, field_value)
 
     def _format_string(self, indent, value=None):
         formstr = " "*indent + "{:" + str(22-indent) + "}:"
         if value is None or isinstance(value, (list, np.ndarray)):
-            ret = Component._format_string(self,indent, value)
+            ret = Component._format_string(self, indent, value)
         else:
             formstr += " {:10d} = 0x{:0" + str(self.node.parent.size*2) + "x}"
             ret = formstr.format(self.node.inst_name, value, value)
         return ret
-
```

### Comparing `coreali-0.0.2/src/coreali/regmodel/Memory.py` & `coreali-0.0.3/src/coreali/regmodel/Memory.py`

 * *Files identical despite different names*

### Comparing `coreali-0.0.2/src/coreali/regmodel/Register.py` & `coreali-0.0.3/src/coreali/regmodel/Register.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 from .SelectableComponent import SelectableComponent
 from .Field import Field
 
+
 class Register(SelectableComponent):
     def __init__(self, root, path, parent, rio):
         SelectableComponent.__init__(self, root, path, parent, rio)
-        
+
+    def _update_attr(self):
+        if self.node.has_sw_writable:
+            setattr(self, "write", self._write)
+        if self.node.has_sw_readable:
+            setattr(self, "read", self._read)
+
     def _read_has_side_effect(self):
         for child in self.node.children():
             if "onread" in child.list_properties():
                 return True
         return False
-    
+
     def _tostr(self, indent=0):
         if not self._do_print:
             return ""
         if self._read_has_side_effect():
             return self._format_string(indent, "(SIDE EFFECTS - NOT READ)")
+        if not self.node.has_sw_readable:
+            return self._format_string(indent, "(NOT READABLE)")
         if self.node.is_array and self.node.array_dimensions[0] > 50:
             value = self[:50].read()
         else:
             value = self.read()
         s = self._format_string(indent, value)
-        
+
         for child in self.__dict__.keys():
             if not child == "_parent":
                 if isinstance(self.__dict__[child], Field):
-                    s += "\n" + self.__dict__[child]._tostr(indent+2,value)   
+                    s += "\n" + self.__dict__[child]._tostr(indent+2, value)
 
-        return s
+        return s
```

### Comparing `coreali-0.0.2/src/coreali/regmodel/RegisterFile.py` & `coreali-0.0.3/src/coreali/regmodel/RegisterFile.py`

 * *Files identical despite different names*

### Comparing `coreali-0.0.2/src/coreali/regmodel/RegisterModel.py` & `coreali-0.0.3/src/coreali/regmodel/RegisterModel.py`

 * *Files identical despite different names*

### Comparing `coreali-0.0.2/src/coreali/regmodel/SelectableComponent.py` & `coreali-0.0.3/src/coreali/regmodel/SelectableComponent.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,23 +28,22 @@
 
     def _default_selection(self):
         if self.node.is_array:
             return self._default_slice()
         return 0
 
     def modify(self, lsb, msb, value):
-
         selector = Selector()
         self._construct_selector(selector.selected)
         if not selector.data_shape():
             self._set_current_idx(selector.selected)
             self._rio.modify_words(
                 self.node.absolute_address, self.node.size, self.node.size, lsb, msb, [value])
 
-    def read(self):
+    def _read(self):
         selector = Selector()
         self._construct_selector(selector.selected)
         if not selector.data_shape():
             self._set_current_idx(selector.selected)
             return self._rio.read_words(self.node.absolute_address, self.node.size, self.node.size, 1)[0]
 
         flat_data = np.empty([selector.numel()], dtype=np.uint64)
@@ -56,15 +55,15 @@
             else:
                 array_stride = self.node.size
             flat_data[flat_idx:flat_idx+selector.flat_len()] = self._rio.read_words(
                 self.node.absolute_address, self.node.size, array_stride, selector.flat_len())
         data = flat_data.reshape(selector.data_shape())
         return data
 
-    def write(self, value):
+    def _write(self, value):
         """Write to register
 
             Use case examples based on the example register description
             Use case 1: Write 1 to 1
                 Write single value to a single register
                 test_reg_desc.AnAddrmap.ARegWithFields.write(100)
```

### Comparing `coreali-0.0.2/src/coreali/regmodel/Selector.py` & `coreali-0.0.3/src/coreali/regmodel/Selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 
 
 class Selectable():
     def __init__(self, parent):
         self._parent = parent
         self._select = None
 
+    def _update_attr(self):
+        pass
+
     def __getitem__(self, key):
         c = self._get_copy()
         c._select = key
         return c
 
     def _get_copy(self):
         c = copy.copy(self)
+        c._update_attr()
         for child in self.__dict__.keys():
             if isinstance(self.__dict__[child], Selectable):
                 if not child == "_parent":
                     c.__dict__[child] = self.__dict__[child]._get_copy()
                     c.__dict__[child]._parent = c
             elif isinstance(self.__dict__[child], Component):
                 if not child == "_parent":
                     c.__dict__[child] = copy.copy(self.__dict__[child])
+                    c.__dict__[child]._update_attr()
                     c.__dict__[child]._parent = c
         return c
 
     def _default_start(self):
         return 0
 
     def _default_stop(self):
```

### Comparing `coreali-0.0.2/src/coreali.egg-info/PKG-INFO` & `coreali-0.0.3/src/coreali.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: coreali
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convenient Register Access Library
-Home-page: https://github.com/siforrer/coreali
 Author: Silvan Forrer
-License: MIT
-Project-URL: Bug Tracker, https://github.com/siforrer/coreali/issues
+Project-URL: Homepage, https://github.com/siforrer/coreali
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # coreali - Convenient Register Access Library
 Generates Python code from a register model. This python code can the be used to access the registers of an FPGA, a MCU or another device which has a register map.
 ## Installation
 Coreali can be installed with pip by executing the following command
```

