# Comparing `tmp/nidmm-1.4.4.tar.gz` & `tmp/nidmm-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nidmm-1.4.4.tar", last modified: Fri Apr 14 16:08:19 2023, max compression
+gzip compressed data, was "nidmm-1.4.5.tar", last modified: Mon Jun 12 00:40:21 2023, max compression
```

## Comparing `nidmm-1.4.4.tar` & `nidmm-1.4.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:29.933237 nidmm-1.4.4/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8758 2023-04-14 16:08:29.931235 nidmm-1.4.4/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7774 2023-04-14 16:05:28.000000 nidmm-1.4.4/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:29.852233 nidmm-1.4.4/nidmm/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:05:18.000000 nidmm-1.4.4/nidmm/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3023 2023-04-14 16:05:16.000000 nidmm-1.4.4/nidmm/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5432 2023-04-14 16:05:09.000000 nidmm-1.4.4/nidmm/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13869 2023-04-14 16:05:17.000000 nidmm-1.4.4/nidmm/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    16344 2023-04-14 16:05:19.000000 nidmm-1.4.4/nidmm/_grpc_stub_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    31587 2023-04-14 16:05:10.000000 nidmm-1.4.4/nidmm/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    33945 2023-04-14 16:05:11.000000 nidmm-1.4.4/nidmm/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1605 2023-04-14 16:05:12.000000 nidmm-1.4.4/nidmm/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:05:22.000000 nidmm-1.4.4/nidmm/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8301 2023-04-14 16:05:10.000000 nidmm-1.4.4/nidmm/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4348 2023-04-14 16:05:14.000000 nidmm-1.4.4/nidmm/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3450 2023-04-14 16:05:19.000000 nidmm-1.4.4/nidmm/grpc_session_options.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-04-14 16:05:21.000000 nidmm-1.4.4/nidmm/nidevice_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-04-14 16:05:21.000000 nidmm-1.4.4/nidmm/nidevice_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    81655 2023-04-14 16:05:20.000000 nidmm-1.4.4/nidmm/nidmm_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   141552 2023-04-14 16:05:20.000000 nidmm-1.4.4/nidmm/nidmm_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   126794 2023-04-14 16:05:13.000000 nidmm-1.4.4/nidmm/session.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-04-14 16:05:22.000000 nidmm-1.4.4/nidmm/session_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-04-14 16:05:22.000000 nidmm-1.4.4/nidmm/session_pb2_grpc.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:29.919235 nidmm-1.4.4/nidmm.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8758 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      605 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      154 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        6 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:08:29.934235 nidmm-1.4.4/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2188 2023-04-14 16:05:29.000000 nidmm-1.4.4/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:40:25.967060 nidmm-1.4.5/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8598 2023-06-12 00:40:25.966060 nidmm-1.4.5/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7523 2023-06-12 00:37:32.000000 nidmm-1.4.5/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:40:25.887059 nidmm-1.4.5/nidmm/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-06-12 00:37:21.000000 nidmm-1.4.5/nidmm/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3023 2023-06-12 00:37:19.000000 nidmm-1.4.5/nidmm/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5432 2023-06-12 00:37:13.000000 nidmm-1.4.5/nidmm/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13869 2023-06-12 00:37:20.000000 nidmm-1.4.5/nidmm/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    16542 2023-06-12 00:37:22.000000 nidmm-1.4.5/nidmm/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    32338 2023-06-12 00:37:14.000000 nidmm-1.4.5/nidmm/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    35327 2023-06-12 00:37:15.000000 nidmm-1.4.5/nidmm/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1605 2023-06-12 00:37:16.000000 nidmm-1.4.5/nidmm/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-06-12 00:37:24.000000 nidmm-1.4.5/nidmm/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8301 2023-06-12 00:37:14.000000 nidmm-1.4.5/nidmm/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4344 2023-06-12 00:37:17.000000 nidmm-1.4.5/nidmm/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3450 2023-06-12 00:37:22.000000 nidmm-1.4.5/nidmm/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-06-12 00:37:24.000000 nidmm-1.4.5/nidmm/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-06-12 00:37:24.000000 nidmm-1.4.5/nidmm/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    81655 2023-06-12 00:37:23.000000 nidmm-1.4.5/nidmm/nidmm_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   141552 2023-06-12 00:37:23.000000 nidmm-1.4.5/nidmm/nidmm_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   126794 2023-06-12 00:37:17.000000 nidmm-1.4.5/nidmm/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-06-12 00:37:24.000000 nidmm-1.4.5/nidmm/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-06-12 00:37:24.000000 nidmm-1.4.5/nidmm/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:40:25.953060 nidmm-1.4.5/nidmm.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8598 2023-06-12 00:40:25.000000 nidmm-1.4.5/nidmm.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      605 2023-06-12 00:40:25.000000 nidmm-1.4.5/nidmm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:40:25.000000 nidmm-1.4.5/nidmm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      148 2023-06-12 00:40:25.000000 nidmm-1.4.5/nidmm.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        6 2023-06-12 00:40:25.000000 nidmm-1.4.5/nidmm.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:40:25.000000 nidmm-1.4.5/nidmm.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-06-12 00:40:25.968060 nidmm-1.4.5/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2242 2023-06-12 00:37:32.000000 nidmm-1.4.5/setup.py
```

### Comparing `nidmm-1.4.4/PKG-INFO` & `nidmm-1.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidmm
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-DMM Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -17,14 +17,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Description-Content-Type: text/x-rst
 Provides-Extra: grpc
 
 Overall Status
 --------------
@@ -136,20 +137,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nidmm module, you must install the NI-DMM runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-DMM**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidmm~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidmm
+  $ python -m pip install nidmm~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -168,30 +164,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidmm/examples>`_
 
 .. _support-section:
 
 Support / Feedback
 ==================
 
-The packages included in **nimi-python** package are supported by NI. For support, open
-a request through the NI support portal at `ni.com <http://www.ni.com>`_.
+For support specific to the Python API, follow the processs in `Bugs / Feature Requests`_.
+For support with hardware, the driver runtime or any other questions not specific to the Python API, please visit `NI Community Forums <https://forums.ni.com/>`_.
 
 .. _bugs-section:
 
 Bugs / Feature Requests
 =======================
 
-To report a bug or submit a feature request specific to NI Modular Instruments Python bindings (nimi-python), please use the
+To report a bug or submit a feature request specific to Python API, please use the
 `GitHub issues page <https://github.com/ni/nimi-python/issues>`_.
 
 Fill in the issue template as completely as possible and we will respond as soon
 as we can.
 
-For hardware support or any other questions not specific to this GitHub project, please visit `NI Community Forums <https://forums.ni.com/>`_.
-
 
 .. _documentation-section:
 
 Documentation
 =============
 
 Documentation is available `here <http://nimi-python.readthedocs.io>`_.
```

### Comparing `nidmm-1.4.4/README.rst` & `nidmm-1.4.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -98,32 +98,27 @@
 
 
 .. |nidmmOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nidmm.svg
     :alt: Pull Requests for NI-DMM
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anidmm
 
 
-
-.. _nidmm_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nidmm module, you must install the NI-DMM runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-DMM**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nidmm~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidmm
-
-
+
+.. _nidmm_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nidmm module, you must install the NI-DMM runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-DMM**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nidmm~=1.4.5
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -135,36 +130,34 @@
     import nidmm
     with nidmm.Session("Dev1") as session:
         session.configureMeasurementDigits(nidmm.Function.DC_VOLTS, 10, 5.5)
         print("Measurement: " + str(session.read()))
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidmm/examples>`_
 
-.. _support-section:
-
-Support / Feedback
-==================
-
-The packages included in **nimi-python** package are supported by NI. For support, open
-a request through the NI support portal at `ni.com <http://www.ni.com>`_.
-
-.. _bugs-section:
-
-Bugs / Feature Requests
-=======================
-
-To report a bug or submit a feature request specific to NI Modular Instruments Python bindings (nimi-python), please use the
-`GitHub issues page <https://github.com/ni/nimi-python/issues>`_.
-
-Fill in the issue template as completely as possible and we will respond as soon
-as we can.
-
-For hardware support or any other questions not specific to this GitHub project, please visit `NI Community Forums <https://forums.ni.com/>`_.
-
-
+.. _support-section:
+
+Support / Feedback
+==================
+
+For support specific to the Python API, follow the processs in `Bugs / Feature Requests`_.
+For support with hardware, the driver runtime or any other questions not specific to the Python API, please visit `NI Community Forums <https://forums.ni.com/>`_.
+
+.. _bugs-section:
+
+Bugs / Feature Requests
+=======================
+
+To report a bug or submit a feature request specific to Python API, please use the
+`GitHub issues page <https://github.com/ni/nimi-python/issues>`_.
+
+Fill in the issue template as completely as possible and we will respond as soon
+as we can.
+
+
 .. _documentation-section:
 
 Documentation
 =============
 
 Documentation is available `here <http://nimi-python.readthedocs.io>`_.
```

### Comparing `nidmm-1.4.4/nidmm/__init__.py` & `nidmm-1.4.5/nidmm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.4'
+__version__ = '1.4.5'
 
 from nidmm.enums import *  # noqa: F403,F401,H303
 from nidmm.errors import DriverWarning  # noqa: F401
 from nidmm.errors import Error  # noqa: F401
 from nidmm.grpc_session_options import *  # noqa: F403,F401,H303
 from nidmm.session import Session  # noqa: F401
 
@@ -61,15 +61,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-DMM"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nidmm'
-    info['module']['version'] = "1.4.4"
+    info['module']['version'] = "1.4.5"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nidmm-1.4.4/nidmm/_attributes.py` & `nidmm-1.4.5/nidmm/_attributes.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/_converters.py` & `nidmm-1.4.5/nidmm/_converters.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/_grpc_stub_interpreter.py` & `nidmm-1.4.5/nidmm/_grpc_stub_interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,14 +356,17 @@
 
     def set_attribute_vi_string(self, channel_name, attribute_id, attribute_value):  # noqa: N802
         self._invoke(
             self._client.SetAttributeViString,
             grpc_types.SetAttributeViStringRequest(vi=self._vi, channel_name=channel_name, attribute_id=attribute_id, attribute_value_raw=attribute_value),
         )
 
+    def set_runtime_environment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        raise NotImplementedError('set_runtime_environment is not supported over gRPC')
+
     def unlock(self):  # noqa: N802
         self._lock.release()
 
     def close(self):  # noqa: N802
         self._invoke(
             self._client.Close,
             grpc_types.CloseRequest(vi=self._vi),
```

### Comparing `nidmm-1.4.4/nidmm/_library.py` & `nidmm-1.4.5/nidmm/_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         self.niDMM_ResetWithDefaults_cfunc = None
         self.niDMM_SelfCal_cfunc = None
         self.niDMM_SendSoftwareTrigger_cfunc = None
         self.niDMM_SetAttributeViBoolean_cfunc = None
         self.niDMM_SetAttributeViInt32_cfunc = None
         self.niDMM_SetAttributeViReal64_cfunc = None
         self.niDMM_SetAttributeViString_cfunc = None
+        self.niDMM_SetRuntimeEnvironment_cfunc = None
         self.niDMM_UnlockSession_cfunc = None
         self.niDMM_close_cfunc = None
         self.niDMM_error_message_cfunc = None
         self.niDMM_reset_cfunc = None
         self.niDMM_self_test_cfunc = None
 
     def _get_library_function(self, name):
@@ -424,14 +425,22 @@
         with self._func_lock:
             if self.niDMM_SetAttributeViString_cfunc is None:
                 self.niDMM_SetAttributeViString_cfunc = self._get_library_function('niDMM_SetAttributeViString')
                 self.niDMM_SetAttributeViString_cfunc.argtypes = [ViSession, ctypes.POINTER(ViChar), ViAttr, ctypes.POINTER(ViChar)]  # noqa: F405
                 self.niDMM_SetAttributeViString_cfunc.restype = ViStatus  # noqa: F405
         return self.niDMM_SetAttributeViString_cfunc(vi, channel_name, attribute_id, attribute_value)
 
+    def niDMM_SetRuntimeEnvironment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        with self._func_lock:
+            if self.niDMM_SetRuntimeEnvironment_cfunc is None:
+                self.niDMM_SetRuntimeEnvironment_cfunc = self._get_library_function('niDMM_SetRuntimeEnvironment')
+                self.niDMM_SetRuntimeEnvironment_cfunc.argtypes = [ctypes.POINTER(ViChar), ctypes.POINTER(ViChar), ctypes.POINTER(ViChar), ctypes.POINTER(ViChar)]  # noqa: F405
+                self.niDMM_SetRuntimeEnvironment_cfunc.restype = ViStatus  # noqa: F405
+        return self.niDMM_SetRuntimeEnvironment_cfunc(environment, environment_version, reserved1, reserved2)
+
     def niDMM_UnlockSession(self, vi, caller_has_lock):  # noqa: N802
         with self._func_lock:
             if self.niDMM_UnlockSession_cfunc is None:
                 self.niDMM_UnlockSession_cfunc = self._get_library_function('niDMM_UnlockSession')
                 self.niDMM_UnlockSession_cfunc.argtypes = [ViSession, ctypes.POINTER(ViBoolean)]  # noqa: F405
                 self.niDMM_UnlockSession_cfunc.restype = ViStatus  # noqa: F405
         return self.niDMM_UnlockSession_cfunc(vi, caller_has_lock)
```

### Comparing `nidmm-1.4.4/nidmm/_library_interpreter.py` & `nidmm-1.4.5/nidmm/_library_interpreter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 import array
 import ctypes
 import hightime  # noqa: F401
+import platform
+
 import nidmm._library_singleton as _library_singleton
 import nidmm._visatype as _visatype
 import nidmm.enums as enums  # noqa: F401
 import nidmm.errors as errors
 
 
+_was_runtime_environment_set = None
+
+
 # Helper functions for creating ctypes needed for calling into the driver DLL
 def _get_ctypes_pointer_for_buffer(value=None, library_type=None, size=None):
     if isinstance(value, array.array):
         assert library_type is not None, 'library_type is required for array.array'
         addr, _ = value.buffer_info()
         return ctypes.cast(addr, ctypes.POINTER(library_type))
     elif str(type(value)).find("'numpy.ndarray'") != -1:
@@ -52,14 +57,29 @@
     * Allocating memory.
     * Converting errors returned by Library into Python exceptions.
     '''
 
     def __init__(self, encoding):
         self._encoding = encoding
         self._library = _library_singleton.get()
+        global _was_runtime_environment_set
+        if _was_runtime_environment_set is None:
+            try:
+                runtime_env = platform.python_implementation()
+                version = platform.python_version()
+                self.set_runtime_environment(
+                    runtime_env,
+                    version,
+                    '',
+                    ''
+                )
+            except errors.DriverTooOldError:
+                pass
+            finally:
+                _was_runtime_environment_set = True
         # Initialize _vi to 0 for now.
         # Session will directly update it once the driver runtime init function has been called and
         # we have a valid session handle.
         self.set_session_handle()
 
     def set_session_handle(self, value=0):
         self._vi = value
@@ -487,14 +507,23 @@
         channel_name_ctype = ctypes.create_string_buffer(channel_name.encode(self._encoding))  # case C010
         attribute_id_ctype = _visatype.ViAttr(attribute_id)  # case S150
         attribute_value_ctype = ctypes.create_string_buffer(attribute_value.encode(self._encoding))  # case C020
         error_code = self._library.niDMM_SetAttributeViString(vi_ctype, channel_name_ctype, attribute_id_ctype, attribute_value_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
+    def set_runtime_environment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        environment_ctype = ctypes.create_string_buffer(environment.encode(self._encoding))  # case C020
+        environment_version_ctype = ctypes.create_string_buffer(environment_version.encode(self._encoding))  # case C020
+        reserved1_ctype = ctypes.create_string_buffer(reserved1.encode(self._encoding))  # case C020
+        reserved2_ctype = ctypes.create_string_buffer(reserved2.encode(self._encoding))  # case C020
+        error_code = self._library.niDMM_SetRuntimeEnvironment(environment_ctype, environment_version_ctype, reserved1_ctype, reserved2_ctype)
+        errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
+        return
+
     def unlock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         error_code = self._library.niDMM_UnlockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def close(self):  # noqa: N802
```

### Comparing `nidmm-1.4.4/nidmm/_library_singleton.py` & `nidmm-1.4.5/nidmm/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/_visatype.py` & `nidmm-1.4.5/nidmm/_visatype.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/enums.py` & `nidmm-1.4.5/nidmm/enums.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/errors.py` & `nidmm-1.4.5/nidmm/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         super(Error, self).__init__(message)
 
 
 class DriverError(Error):
     '''An error originating from the NI-DMM driver'''
 
     def __init__(self, code, description):
-        assert (_is_error(code)), "Should not raise Error if code is not fatal."
+        assert _is_error(code), "Should not raise Error if code is not fatal."
         self.code = code
         self.description = description
         super(DriverError, self).__init__(str(self.code) + ": " + self.description)
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-DMM driver'''
 
     def __init__(self, code, description):
-        assert (_is_warning(code)), "Should not create Warning if code is not positive."
+        assert _is_warning(code), "Should not create Warning if code is not positive."
         super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
 
 
 class RpcError(Error):
     '''An error specific to sessions to the NI gRPC Device Server'''
 
     def __init__(self, rpc_code, description):
```

### Comparing `nidmm-1.4.4/nidmm/grpc_session_options.py` & `nidmm-1.4.5/nidmm/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/nidevice_pb2.py` & `nidmm-1.4.5/nidmm/nidevice_pb2.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/nidmm_pb2.py` & `nidmm-1.4.5/nidmm/nidmm_pb2.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/nidmm_pb2_grpc.py` & `nidmm-1.4.5/nidmm/nidmm_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/session.py` & `nidmm-1.4.5/nidmm/session.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/session_pb2.py` & `nidmm-1.4.5/nidmm/session_pb2.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm/session_pb2_grpc.py` & `nidmm-1.4.5/nidmm/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/nidmm.egg-info/PKG-INFO` & `nidmm-1.4.5/nidmm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidmm
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-DMM Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -17,14 +17,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Description-Content-Type: text/x-rst
 Provides-Extra: grpc
 
 Overall Status
 --------------
@@ -136,20 +137,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nidmm module, you must install the NI-DMM runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-DMM**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidmm~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidmm
+  $ python -m pip install nidmm~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -168,30 +164,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidmm/examples>`_
 
 .. _support-section:
 
 Support / Feedback
 ==================
 
-The packages included in **nimi-python** package are supported by NI. For support, open
-a request through the NI support portal at `ni.com <http://www.ni.com>`_.
+For support specific to the Python API, follow the processs in `Bugs / Feature Requests`_.
+For support with hardware, the driver runtime or any other questions not specific to the Python API, please visit `NI Community Forums <https://forums.ni.com/>`_.
 
 .. _bugs-section:
 
 Bugs / Feature Requests
 =======================
 
-To report a bug or submit a feature request specific to NI Modular Instruments Python bindings (nimi-python), please use the
+To report a bug or submit a feature request specific to Python API, please use the
 `GitHub issues page <https://github.com/ni/nimi-python/issues>`_.
 
 Fill in the issue template as completely as possible and we will respond as soon
 as we can.
 
-For hardware support or any other questions not specific to this GitHub project, please visit `NI Community Forums <https://forums.ni.com/>`_.
-
 
 .. _documentation-section:
 
 Documentation
 =============
 
 Documentation is available `here <http://nimi-python.readthedocs.io>`_.
```

### Comparing `nidmm-1.4.4/nidmm.egg-info/SOURCES.txt` & `nidmm-1.4.5/nidmm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.4/setup.py` & `nidmm-1.4.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.4',
+    version='1.4.5',
     description='NI-DMM Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -43,15 +43,15 @@
     include_package_data=True,
     packages=['nidmm'],
     install_requires=[
         'hightime>=0.2.0',
     ],
     extras_require={
         'grpc': [
-            'grpcio>=1.49.1,<2.0,!=1.53;python_version=="3.7"',  # no 32-bit wheel for 1.53.0
+            'grpcio>=1.49.1,<1.53;python_version=="3.7"',  # no 32-bit wheel for 1.53.0 and later
             'grpcio>=1.49.1,<2.0;python_version>"3.7"',
             'protobuf>=4.21,<5.0'
         ],
     },
     setup_requires=['pytest-runner', ],
     tests_require=['pytest'],
     test_suite='tests',
@@ -64,13 +64,14 @@
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: System :: Hardware :: Hardware Drivers"
     ],
     cmdclass={'test': PyTest},
     package_data={pypi_name: ['VERSION']},
 )
```

