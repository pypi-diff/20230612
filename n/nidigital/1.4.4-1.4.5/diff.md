# Comparing `tmp/nidigital-1.4.4.tar.gz` & `tmp/nidigital-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nidigital-1.4.4.tar", last modified: Fri Apr 14 16:08:03 2023, max compression
+gzip compressed data, was "nidigital-1.4.5.tar", last modified: Mon Jun 12 00:40:07 2023, max compression
```

## Comparing `nidigital-1.4.4.tar` & `nidigital-1.4.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:14.106667 nidigital-1.4.4/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10556 2023-04-14 16:08:14.104666 nidigital-1.4.4/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9545 2023-04-14 16:05:06.000000 nidigital-1.4.4/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:14.025665 nidigital-1.4.4/nidigital/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:04:52.000000 nidigital-1.4.4/nidigital/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3179 2023-04-14 16:04:50.000000 nidigital-1.4.4/nidigital/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5448 2023-04-14 16:04:42.000000 nidigital-1.4.4/nidigital/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13877 2023-04-14 16:04:51.000000 nidigital-1.4.4/nidigital/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    29543 2023-04-14 16:04:53.000000 nidigital-1.4.4/nidigital/_grpc_stub_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    65575 2023-04-14 16:04:43.000000 nidigital-1.4.4/nidigital/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    73551 2023-04-14 16:04:44.000000 nidigital-1.4.4/nidigital/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1629 2023-04-14 16:04:45.000000 nidigital-1.4.4/nidigital/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:04:57.000000 nidigital-1.4.4/nidigital/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7810 2023-04-14 16:04:42.000000 nidigital-1.4.4/nidigital/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4512 2023-04-14 16:04:47.000000 nidigital-1.4.4/nidigital/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3465 2023-04-14 16:04:54.000000 nidigital-1.4.4/nidigital/grpc_session_options.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2890 2023-04-14 16:04:57.000000 nidigital-1.4.4/nidigital/history_ram_cycle_information.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-04-14 16:04:56.000000 nidigital-1.4.4/nidigital/nidevice_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-04-14 16:04:56.000000 nidigital-1.4.4/nidigital/nidevice_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   105590 2023-04-14 16:04:55.000000 nidigital-1.4.4/nidigital/nidigitalpattern_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   226597 2023-04-14 16:04:55.000000 nidigital-1.4.4/nidigital/nidigitalpattern_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   234062 2023-04-14 16:04:47.000000 nidigital-1.4.4/nidigital/session.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-04-14 16:04:57.000000 nidigital-1.4.4/nidigital/session_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-04-14 16:04:57.000000 nidigital-1.4.4/nidigital/session_pb2_grpc.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:14.092666 nidigital-1.4.4/nidigital.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10556 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      770 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      161 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:08:14.107666 nidigital-1.4.4/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2237 2023-04-14 16:05:07.000000 nidigital-1.4.4/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:40:11.927433 nidigital-1.4.5/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10392 2023-06-12 00:40:11.925433 nidigital-1.4.5/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9290 2023-06-12 00:37:08.000000 nidigital-1.4.5/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:40:11.743473 nidigital-1.4.5/nidigital/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-06-12 00:36:55.000000 nidigital-1.4.5/nidigital/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3179 2023-06-12 00:36:53.000000 nidigital-1.4.5/nidigital/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5448 2023-06-12 00:36:46.000000 nidigital-1.4.5/nidigital/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13877 2023-06-12 00:36:54.000000 nidigital-1.4.5/nidigital/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    29741 2023-06-12 00:36:56.000000 nidigital-1.4.5/nidigital/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    66358 2023-06-12 00:36:47.000000 nidigital-1.4.5/nidigital/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    74937 2023-06-12 00:36:48.000000 nidigital-1.4.5/nidigital/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1629 2023-06-12 00:36:49.000000 nidigital-1.4.5/nidigital/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-06-12 00:36:59.000000 nidigital-1.4.5/nidigital/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7810 2023-06-12 00:36:47.000000 nidigital-1.4.5/nidigital/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4508 2023-06-12 00:36:51.000000 nidigital-1.4.5/nidigital/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3465 2023-06-12 00:36:57.000000 nidigital-1.4.5/nidigital/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2890 2023-06-12 00:36:59.000000 nidigital-1.4.5/nidigital/history_ram_cycle_information.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-06-12 00:36:58.000000 nidigital-1.4.5/nidigital/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-06-12 00:36:58.000000 nidigital-1.4.5/nidigital/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   105590 2023-06-12 00:36:57.000000 nidigital-1.4.5/nidigital/nidigitalpattern_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   226597 2023-06-12 00:36:57.000000 nidigital-1.4.5/nidigital/nidigitalpattern_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   234061 2023-06-12 00:36:50.000000 nidigital-1.4.5/nidigital/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-06-12 00:36:59.000000 nidigital-1.4.5/nidigital/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-06-12 00:36:59.000000 nidigital-1.4.5/nidigital/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:40:11.912422 nidigital-1.4.5/nidigital.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10392 2023-06-12 00:40:11.000000 nidigital-1.4.5/nidigital.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      770 2023-06-12 00:40:11.000000 nidigital-1.4.5/nidigital.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:40:11.000000 nidigital-1.4.5/nidigital.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      155 2023-06-12 00:40:11.000000 nidigital-1.4.5/nidigital.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2023-06-12 00:40:11.000000 nidigital-1.4.5/nidigital.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:40:11.000000 nidigital-1.4.5/nidigital.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-06-12 00:40:11.927433 nidigital-1.4.5/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2291 2023-06-12 00:37:09.000000 nidigital-1.4.5/setup.py
```

### Comparing `nidigital-1.4.4/PKG-INFO` & `nidigital-1.4.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidigital
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-Digital Pattern Driver Python API
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
 
 As a prerequisite to using the nidigital module, you must install the NI-Digital Pattern Driver runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-Digital Pattern Driver**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidigital~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidigital
+  $ python -m pip install nidigital~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -199,30 +195,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidigital/examples>`_
 
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

### Comparing `nidigital-1.4.4/README.rst` & `nidigital-1.4.5/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -98,32 +98,27 @@
 
 
 .. |nidigitalOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nidigital.svg
     :alt: Pull Requests for NI-Digital Pattern Driver
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anidigital
 
 
-
-.. _nidigital_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nidigital module, you must install the NI-Digital Pattern Driver runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-Digital Pattern Driver**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nidigital~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidigital
-
-
+
+.. _nidigital_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nidigital module, you must install the NI-Digital Pattern Driver runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-Digital Pattern Driver**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nidigital~=1.4.5
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -166,36 +161,34 @@
             print('{:<20} {:<10f} {:<10f}'.format(channel, current, voltage))
 
         # Disconnect all channels using programmable onboard switching
         session.channels[channels].selected_function = nidigital.SelectedFunction.DISCONNECT
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidigital/examples>`_
 
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

### Comparing `nidigital-1.4.4/nidigital/__init__.py` & `nidigital-1.4.5/nidigital/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.4'
+__version__ = '1.4.5'
 
 from nidigital.enums import *  # noqa: F403,F401,H303
 from nidigital.errors import DriverWarning  # noqa: F401
 from nidigital.errors import Error  # noqa: F401
 from nidigital.grpc_session_options import *  # noqa: F403,F401,H303
 from nidigital.session import Session  # noqa: F401
 
@@ -63,15 +63,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-Digital Pattern Driver"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nidigital'
-    info['module']['version'] = "1.4.4"
+    info['module']['version'] = "1.4.5"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nidigital-1.4.4/nidigital/_attributes.py` & `nidigital-1.4.5/nidigital/_attributes.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/_converters.py` & `nidigital-1.4.5/nidigital/_converters.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/_grpc_stub_interpreter.py` & `nidigital-1.4.5/nidigital/_grpc_stub_interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,14 +564,17 @@
 
     def set_attribute_vi_string(self, channel_name, attribute, value):  # noqa: N802
         self._invoke(
             self._client.SetAttributeViString,
             grpc_types.SetAttributeViStringRequest(vi=self._vi, channel_name=channel_name, attribute=attribute, value_raw=value),
         )
 
+    def set_runtime_environment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        raise NotImplementedError('set_runtime_environment is not supported over gRPC')
+
     def tdr(self, channel_list, apply_offsets):  # noqa: N802
         response = self._invoke(
             self._client.TDR,
             grpc_types.TDRRequest(vi=self._vi, channel_list=channel_list, apply_offsets=apply_offsets),
         )
         return response.offsets
```

### Comparing `nidigital-1.4.4/nidigital/_library.py` & `nidigital-1.4.5/nidigital/_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         self.niDigital_SelfCalibrate_cfunc = None
         self.niDigital_SendSoftwareEdgeTrigger_cfunc = None
         self.niDigital_SetAttributeViBoolean_cfunc = None
         self.niDigital_SetAttributeViInt32_cfunc = None
         self.niDigital_SetAttributeViInt64_cfunc = None
         self.niDigital_SetAttributeViReal64_cfunc = None
         self.niDigital_SetAttributeViString_cfunc = None
+        self.niDigital_SetRuntimeEnvironment_cfunc = None
         self.niDigital_TDR_cfunc = None
         self.niDigital_UnloadAllPatterns_cfunc = None
         self.niDigital_UnloadSpecifications_cfunc = None
         self.niDigital_UnlockSession_cfunc = None
         self.niDigital_WaitUntilDone_cfunc = None
         self.niDigital_WriteSequencerFlag_cfunc = None
         self.niDigital_WriteSequencerRegister_cfunc = None
@@ -733,14 +734,22 @@
         with self._func_lock:
             if self.niDigital_SetAttributeViString_cfunc is None:
                 self.niDigital_SetAttributeViString_cfunc = self._get_library_function('niDigital_SetAttributeViString')
                 self.niDigital_SetAttributeViString_cfunc.argtypes = [ViSession, ctypes.POINTER(ViChar), ViAttr, ctypes.POINTER(ViChar)]  # noqa: F405
                 self.niDigital_SetAttributeViString_cfunc.restype = ViStatus  # noqa: F405
         return self.niDigital_SetAttributeViString_cfunc(vi, channel_name, attribute, value)
 
+    def niDigital_SetRuntimeEnvironment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        with self._func_lock:
+            if self.niDigital_SetRuntimeEnvironment_cfunc is None:
+                self.niDigital_SetRuntimeEnvironment_cfunc = self._get_library_function('niDigital_SetRuntimeEnvironment')
+                self.niDigital_SetRuntimeEnvironment_cfunc.argtypes = [ctypes.POINTER(ViChar), ctypes.POINTER(ViChar), ctypes.POINTER(ViChar), ctypes.POINTER(ViChar)]  # noqa: F405
+                self.niDigital_SetRuntimeEnvironment_cfunc.restype = ViStatus  # noqa: F405
+        return self.niDigital_SetRuntimeEnvironment_cfunc(environment, environment_version, reserved1, reserved2)
+
     def niDigital_TDR(self, vi, channel_list, apply_offsets, offsets_buffer_size, offsets, actual_num_offsets):  # noqa: N802
         with self._func_lock:
             if self.niDigital_TDR_cfunc is None:
                 self.niDigital_TDR_cfunc = self._get_library_function('niDigital_TDR')
                 self.niDigital_TDR_cfunc.argtypes = [ViSession, ctypes.POINTER(ViChar), ViBoolean, ViInt32, ctypes.POINTER(ViReal64), ctypes.POINTER(ViInt32)]  # noqa: F405
                 self.niDigital_TDR_cfunc.restype = ViStatus  # noqa: F405
         return self.niDigital_TDR_cfunc(vi, channel_list, apply_offsets, offsets_buffer_size, offsets, actual_num_offsets)
```

### Comparing `nidigital-1.4.4/nidigital/_library_interpreter.py` & `nidigital-1.4.5/nidigital/_library_interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 import array
 import ctypes
 import hightime  # noqa: F401
+import platform
+
 import nidigital._library_singleton as _library_singleton
 import nidigital._visatype as _visatype
 import nidigital.enums as enums  # noqa: F401
 import nidigital.errors as errors
 
 import nidigital.history_ram_cycle_information as history_ram_cycle_information  # noqa: F401
 
 
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
@@ -54,14 +59,29 @@
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
@@ -866,14 +886,23 @@
         channel_name_ctype = ctypes.create_string_buffer(channel_name.encode(self._encoding))  # case C010
         attribute_ctype = _visatype.ViAttr(attribute)  # case S150
         value_ctype = ctypes.create_string_buffer(value.encode(self._encoding))  # case C020
         error_code = self._library.niDigital_SetAttributeViString(vi_ctype, channel_name_ctype, attribute_ctype, value_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
+    def set_runtime_environment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        environment_ctype = ctypes.create_string_buffer(environment.encode(self._encoding))  # case C020
+        environment_version_ctype = ctypes.create_string_buffer(environment_version.encode(self._encoding))  # case C020
+        reserved1_ctype = ctypes.create_string_buffer(reserved1.encode(self._encoding))  # case C020
+        reserved2_ctype = ctypes.create_string_buffer(reserved2.encode(self._encoding))  # case C020
+        error_code = self._library.niDigital_SetRuntimeEnvironment(environment_ctype, environment_version_ctype, reserved1_ctype, reserved2_ctype)
+        errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
+        return
+
     def tdr(self, channel_list, apply_offsets):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         channel_list_ctype = ctypes.create_string_buffer(channel_list.encode(self._encoding))  # case C010
         apply_offsets_ctype = _visatype.ViBoolean(apply_offsets)  # case S150
         offsets_buffer_size_ctype = _visatype.ViInt32(0)  # case S190
         offsets_ctype = None  # case B610
         actual_num_offsets_ctype = _visatype.ViInt32()  # case S220
```

### Comparing `nidigital-1.4.4/nidigital/_library_singleton.py` & `nidigital-1.4.5/nidigital/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/_visatype.py` & `nidigital-1.4.5/nidigital/_visatype.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/enums.py` & `nidigital-1.4.5/nidigital/enums.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/errors.py` & `nidigital-1.4.5/nidigital/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         super(Error, self).__init__(message)
 
 
 class DriverError(Error):
     '''An error originating from the NI-Digital Pattern Driver driver'''
 
     def __init__(self, code, description):
-        assert (_is_error(code)), "Should not raise Error if code is not fatal."
+        assert _is_error(code), "Should not raise Error if code is not fatal."
         self.code = code
         self.description = description
         super(DriverError, self).__init__(str(self.code) + ": " + self.description)
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-Digital Pattern Driver driver'''
 
     def __init__(self, code, description):
-        assert (_is_warning(code)), "Should not create Warning if code is not positive."
+        assert _is_warning(code), "Should not create Warning if code is not positive."
         super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
 
 
 class RpcError(Error):
     '''An error specific to sessions to the NI gRPC Device Server'''
 
     def __init__(self, rpc_code, description):
```

### Comparing `nidigital-1.4.4/nidigital/grpc_session_options.py` & `nidigital-1.4.5/nidigital/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/history_ram_cycle_information.py` & `nidigital-1.4.5/nidigital/history_ram_cycle_information.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/nidevice_pb2.py` & `nidigital-1.4.5/nidigital/nidevice_pb2.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/nidigitalpattern_pb2.py` & `nidigital-1.4.5/nidigital/nidigitalpattern_pb2.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/nidigitalpattern_pb2_grpc.py` & `nidigital-1.4.5/nidigital/nidigitalpattern_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/session.py` & `nidigital-1.4.5/nidigital/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -10032,4598 +10032,4598 @@
 000272f0: 7572 6e73 2061 206c 6973 7420 6f66 2063  urns a list of c
 00027300: 6861 6e6e 656c 206e 616d 6573 2066 6f72  hannel names for
 00027310: 2067 6976 656e 2063 6861 6e6e 656c 2069   given channel i
 00027320: 6e64 6963 6573 2e0a 0a20 2020 2020 2020  ndices...       
 00027330: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
 00027340: 2020 2069 6e64 6963 6573 2028 6261 7369     indices (basi
 00027350: 6320 7365 7175 656e 6365 2074 7970 6573  c sequence types
-00027360: 206f 7220 7374 7220 6f72 2069 6e74 293a   or str or int):
-00027370: 2049 6e64 6578 206c 6973 7420 666f 7220   Index list for 
-00027380: 7468 6520 6368 616e 6e65 6c73 2069 6e20  the channels in 
-00027390: 7468 6520 7365 7373 696f 6e2e 2056 616c  the session. Val
-000273a0: 6964 2076 616c 7565 7320 6172 6520 6672  id values are fr
-000273b0: 6f6d 207a 6572 6f20 746f 2074 6865 2074  om zero to the t
-000273c0: 6f74 616c 206e 756d 6265 7220 6f66 2063  otal number of c
-000273d0: 6861 6e6e 656c 7320 696e 2074 6865 2073  hannels in the s
-000273e0: 6573 7369 6f6e 206d 696e 7573 206f 6e65  ession minus one
-000273f0: 2e20 5468 6520 696e 6465 7820 7374 7269  . The index stri
-00027400: 6e67 2063 616e 2062 6520 6f6e 6520 6f66  ng can be one of
-00027410: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
-00027420: 6f72 6d61 7473 3a0a 0a20 2020 2020 2020  ormats:..       
-00027430: 2020 2020 2020 2020 202d 2020 2041 2063           -   A c
-00027440: 6f6d 6d61 2d73 6570 6172 6174 6564 206c  omma-separated l
-00027450: 6973 74e2 8094 666f 7220 6578 616d 706c  ist...for exampl
-00027460: 652c 2022 302c 322c 332c 3122 0a20 2020  e, "0,2,3,1".   
-00027470: 2020 2020 2020 2020 2020 2020 202d 2020               -  
-00027480: 2041 2072 616e 6765 2075 7369 6e67 2061   A range using a
-00027490: 2068 7970 6865 6ee2 8094 666f 7220 6578   hyphen...for ex
-000274a0: 616d 706c 652c 2022 302d 3322 0a20 2020  ample, "0-3".   
-000274b0: 2020 2020 2020 2020 2020 2020 202d 2020               -  
-000274c0: 2041 2072 616e 6765 2075 7369 6e67 2061   A range using a
-000274d0: 2063 6f6c 6f6e e280 9466 6f72 2065 7861   colon...for exa
-000274e0: 6d70 6c65 2c20 2230 3a33 2022 0a0a 2020  mple, "0:3 "..  
-000274f0: 2020 2020 2020 2020 2020 2020 2020 596f                Yo
-00027500: 7520 6361 6e20 636f 6d62 696e 6520 636f  u can combine co
-00027510: 6d6d 612d 7365 7061 7261 7465 6420 6c69  mma-separated li
-00027520: 7374 7320 616e 6420 7261 6e67 6573 2074  sts and ranges t
-00027530: 6861 7420 7573 6520 6120 6879 7068 656e  hat use a hyphen
-00027540: 206f 7220 636f 6c6f 6e2e 2042 6f74 6820   or colon. Both 
-00027550: 6f75 742d 6f66 2d6f 7264 6572 2061 6e64  out-of-order and
-00027560: 2072 6570 6561 7465 6420 696e 6469 6365   repeated indice
-00027570: 7320 6172 6520 7375 7070 6f72 7465 6420  s are supported 
-00027580: 2822 322c 332c 302c 2220 2231 2c32 2c32  ("2,3,0," "1,2,2
-00027590: 2c33 2229 2e20 5768 6974 6520 7370 6163  ,3"). White spac
-000275a0: 6520 6368 6172 6163 7465 7273 2c20 696e  e characters, in
-000275b0: 636c 7564 696e 6720 7370 6163 6573 2c20  cluding spaces, 
-000275c0: 7461 6273 2c20 6665 6564 732c 2061 6e64  tabs, feeds, and
-000275d0: 2063 6172 7269 6167 6520 7265 7475 726e   carriage return
-000275e0: 732c 2061 7265 2061 6c6c 6f77 6564 2062  s, are allowed b
-000275f0: 6574 7765 656e 2063 6861 7261 6374 6572  etween character
-00027600: 732e 2052 616e 6765 7320 6361 6e20 6265  s. Ranges can be
-00027610: 2069 6e63 7265 6d65 6e74 696e 6720 6f72   incrementing or
-00027620: 2064 6563 7265 6d65 6e74 696e 672e 0a0a   decrementing...
-00027630: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00027640: 3a0a 2020 2020 2020 2020 2020 2020 6e61  :.            na
-00027650: 6d65 7320 286c 6973 7420 6f66 2073 7472  mes (list of str
-00027660: 293a 2054 6865 2063 6861 6e6e 656c 206e  ): The channel n
-00027670: 616d 6528 7329 2061 7420 7468 6520 7370  ame(s) at the sp
-00027680: 6563 6966 6965 6420 696e 6469 6365 732e  ecified indices.
-00027690: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-000276a0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-000276b0: 5f63 6f6e 7665 7274 6572 732e 636f 6e76  _converters.conv
-000276c0: 6572 745f 7265 7065 6174 6564 5f63 6170  ert_repeated_cap
-000276d0: 6162 696c 6974 6965 735f 7769 7468 6f75  abilities_withou
-000276e0: 745f 7072 6566 6978 2869 6e64 6963 6573  t_prefix(indices
-000276f0: 290a 2020 2020 2020 2020 6e61 6d65 7320  ).        names 
-00027700: 3d20 7365 6c66 2e5f 696e 7465 7270 7265  = self._interpre
-00027710: 7465 722e 6765 745f 6368 616e 6e65 6c5f  ter.get_channel_
-00027720: 6e61 6d65 7328 696e 6469 6365 7329 0a20  names(indices). 
-00027730: 2020 2020 2020 2072 6574 7572 6e20 5f63         return _c
-00027740: 6f6e 7665 7274 6572 732e 636f 6e76 6572  onverters.conver
-00027750: 745f 636f 6d6d 615f 7365 7061 7261 7465  t_comma_separate
-00027760: 645f 7374 7269 6e67 5f74 6f5f 6c69 7374  d_string_to_list
-00027770: 286e 616d 6573 290a 0a20 2020 2040 6976  (names)..    @iv
-00027780: 695f 7379 6e63 6872 6f6e 697a 6564 0a20  i_synchronized. 
-00027790: 2020 2064 6566 2067 6574 5f66 6169 6c5f     def get_fail_
-000277a0: 636f 756e 7428 7365 6c66 293a 0a20 2020  count(self):.   
-000277b0: 2020 2020 2072 2727 2767 6574 5f66 6169       r'''get_fai
-000277c0: 6c5f 636f 756e 740a 0a20 2020 2020 2020  l_count..       
-000277d0: 2052 6574 7572 6e73 2074 6865 2063 6f6d   Returns the com
-000277e0: 7061 7269 736f 6e20 6661 696c 2063 6f75  parison fail cou
-000277f0: 6e74 2066 6f72 2070 696e 7320 696e 2074  nt for pins in t
-00027800: 6865 2072 6570 6561 7465 6420 6361 7061  he repeated capa
-00027810: 6269 6c69 7469 6573 2e0a 0a20 2020 2020  bilities...     
-00027820: 2020 2054 6970 3a0a 2020 2020 2020 2020     Tip:.        
-00027830: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
-00027840: 6265 2063 616c 6c65 6420 6f6e 2073 7065  be called on spe
-00027850: 6369 6669 6320 6368 616e 6e65 6c73 2077  cific channels w
-00027860: 6974 6869 6e20 796f 7572 203a 7079 3a63  ithin your :py:c
-00027870: 6c61 7373 3a60 6e69 6469 6769 7461 6c2e  lass:`nidigital.
-00027880: 5365 7373 696f 6e60 2069 6e73 7461 6e63  Session` instanc
-00027890: 652e 0a20 2020 2020 2020 2055 7365 2050  e..        Use P
-000278a0: 7974 686f 6e20 696e 6465 7820 6e6f 7461  ython index nota
-000278b0: 7469 6f6e 206f 6e20 7468 6520 7265 7065  tion on the repe
-000278c0: 6174 6564 2063 6170 6162 696c 6974 6965  ated capabilitie
-000278d0: 7320 636f 6e74 6169 6e65 7220 6368 616e  s container chan
-000278e0: 6e65 6c73 2074 6f20 7370 6563 6966 7920  nels to specify 
-000278f0: 6120 7375 6273 6574 2c0a 2020 2020 2020  a subset,.      
-00027900: 2020 616e 6420 7468 656e 2063 616c 6c20    and then call 
-00027910: 7468 6973 206d 6574 686f 6420 6f6e 2074  this method on t
-00027920: 6865 2072 6573 756c 742e 0a0a 2020 2020  he result...    
-00027930: 2020 2020 4578 616d 706c 653a 203a 7079      Example: :py
-00027940: 3a6d 6574 683a 606d 795f 7365 7373 696f  :meth:`my_sessio
-00027950: 6e2e 6368 616e 6e65 6c73 5b20 2e2e 2e20  n.channels[ ... 
-00027960: 5d2e 6765 745f 6661 696c 5f63 6f75 6e74  ].get_fail_count
-00027970: 600a 0a20 2020 2020 2020 2054 6f20 6361  `..        To ca
-00027980: 6c6c 2074 6865 206d 6574 686f 6420 6f6e  ll the method on
-00027990: 2061 6c6c 2063 6861 6e6e 656c 732c 2079   all channels, y
-000279a0: 6f75 2063 616e 2063 616c 6c20 6974 2064  ou can call it d
-000279b0: 6972 6563 746c 7920 6f6e 2074 6865 203a  irectly on the :
-000279c0: 7079 3a63 6c61 7373 3a60 6e69 6469 6769  py:class:`nidigi
-000279d0: 7461 6c2e 5365 7373 696f 6e60 2e0a 0a20  tal.Session`... 
-000279e0: 2020 2020 2020 2045 7861 6d70 6c65 3a20         Example: 
-000279f0: 3a70 793a 6d65 7468 3a60 6d79 5f73 6573  :py:meth:`my_ses
-00027a00: 7369 6f6e 2e67 6574 5f66 6169 6c5f 636f  sion.get_fail_co
-00027a10: 756e 7460 0a0a 2020 2020 2020 2020 5265  unt`..        Re
-00027a20: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00027a30: 2020 2066 6169 6c75 7265 5f63 6f75 6e74     failure_count
-00027a40: 2028 6c69 7374 206f 6620 696e 7429 3a20   (list of int): 
-00027a50: 4e75 6d62 6572 206f 6620 6661 696c 7572  Number of failur
-00027a60: 6573 2069 6e20 616e 2061 7272 6179 2e20  es in an array. 
-00027a70: 4966 2061 2073 6974 6520 6973 2064 6973  If a site is dis
-00027a80: 6162 6c65 6420 6f72 206e 6f74 2065 6e61  abled or not ena
-00027a90: 626c 6564 2066 6f72 2062 7572 7374 2c20  bled for burst, 
-00027aa0: 7468 6520 6d65 7468 6f64 2064 6f65 7320  the method does 
-00027ab0: 6e6f 7420 7265 7475 726e 2064 6174 6120  not return data 
-00027ac0: 666f 7220 7468 6174 2073 6974 652e 2059  for that site. Y
-00027ad0: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
-00027ae0: 7468 6520 6765 745f 7069 6e5f 7265 7375  the get_pin_resu
-00027af0: 6c74 735f 7069 6e5f 696e 666f 726d 6174  lts_pin_informat
-00027b00: 696f 6e20 6d65 7468 6f64 2074 6f20 6f62  ion method to ob
-00027b10: 7461 696e 2061 2073 6f72 7465 6420 6c69  tain a sorted li
-00027b20: 7374 206f 6620 7265 7475 726e 6564 2073  st of returned s
-00027b30: 6974 6573 2061 6e64 2063 6861 6e6e 656c  ites and channel
-00027b40: 732e 0a0a 2020 2020 2020 2020 2727 270a  s...        '''.
-00027b50: 2020 2020 2020 2020 6661 696c 7572 655f          failure_
-00027b60: 636f 756e 7420 3d20 7365 6c66 2e5f 696e  count = self._in
-00027b70: 7465 7270 7265 7465 722e 6765 745f 6661  terpreter.get_fa
-00027b80: 696c 5f63 6f75 6e74 2873 656c 662e 5f72  il_count(self._r
-00027b90: 6570 6561 7465 645f 6361 7061 6269 6c69  epeated_capabili
-00027ba0: 7479 290a 2020 2020 2020 2020 7265 7475  ty).        retu
-00027bb0: 726e 2066 6169 6c75 7265 5f63 6f75 6e74  rn failure_count
-00027bc0: 0a0a 2020 2020 4069 7669 5f73 796e 6368  ..    @ivi_synch
-00027bd0: 726f 6e69 7a65 640a 2020 2020 6465 6620  ronized.    def 
-00027be0: 6765 745f 6869 7374 6f72 795f 7261 6d5f  get_history_ram_
-00027bf0: 7361 6d70 6c65 5f63 6f75 6e74 2873 656c  sample_count(sel
-00027c00: 6629 3a0a 2020 2020 2020 2020 7227 2727  f):.        r'''
-00027c10: 6765 745f 6869 7374 6f72 795f 7261 6d5f  get_history_ram_
-00027c20: 7361 6d70 6c65 5f63 6f75 6e74 0a0a 2020  sample_count..  
-00027c30: 2020 2020 2020 5265 7475 726e 7320 7468        Returns th
-00027c40: 6520 6e75 6d62 6572 206f 6620 7361 6d70  e number of samp
-00027c50: 6c65 7320 4869 7374 6f72 7920 5241 4d20  les History RAM 
-00027c60: 6163 7175 6972 6564 206f 6e20 7468 6520  acquired on the 
-00027c70: 6c61 7374 2070 6174 7465 726e 2062 7572  last pattern bur
-00027c80: 7374 2e0a 0a20 2020 2020 2020 204e 6f74  st...        Not
-00027c90: 653a 0a20 2020 2020 2020 2042 6566 6f72  e:.        Befor
-00027ca0: 6520 6275 7273 7469 6e67 2061 2070 6174  e bursting a pat
-00027cb0: 7465 726e 2c20 796f 7520 6d75 7374 2063  tern, you must c
-00027cc0: 6f6e 6669 6775 7265 2074 6865 2048 6973  onfigure the His
-00027cd0: 746f 7279 2052 414d 2074 7269 6767 6572  tory RAM trigger
-00027ce0: 2061 6e64 2073 7065 6369 6679 2077 6869   and specify whi
-00027cf0: 6368 2063 7963 6c65 7320 746f 2061 6371  ch cycles to acq
-00027d00: 7569 7265 2e0a 0a20 2020 2020 2020 2068  uire...        h
-00027d10: 6973 746f 7279 5f72 616d 5f74 7269 6767  istory_ram_trigg
-00027d20: 6572 5f74 7970 6520 7368 6f75 6c64 2062  er_type should b
-00027d30: 6520 7573 6564 2074 6f20 7370 6563 6966  e used to specif
-00027d40: 7920 7468 6520 7472 6967 6765 7220 636f  y the trigger co
-00027d50: 6e64 6974 696f 6e20 6f6e 2077 6869 6368  ndition on which
-00027d60: 2048 6973 746f 7279 2052 414d 0a20 2020   History RAM.   
-00027d70: 2020 2020 2073 7461 7274 7320 6163 7175       starts acqu
-00027d80: 6972 696e 6720 7061 7474 6572 6e20 696e  iring pattern in
-00027d90: 666f 726d 6174 696f 6e2e 0a0a 2020 2020  formation...    
-00027da0: 2020 2020 4966 2048 6973 746f 7279 2052      If History R
-00027db0: 414d 2074 7269 6767 6572 2069 7320 636f  AM trigger is co
-00027dc0: 6e66 6967 7572 6564 2061 7320 4869 7374  nfigured as Hist
-00027dd0: 6f72 7952 414d 5472 6967 6765 7254 7970  oryRAMTriggerTyp
-00027de0: 652e 4359 434c 455f 4e55 4d42 4552 2c0a  e.CYCLE_NUMBER,.
-00027df0: 2020 2020 2020 2020 6379 636c 655f 6e75          cycle_nu
-00027e00: 6d62 6572 5f68 6973 746f 7279 5f72 616d  mber_history_ram
-00027e10: 5f74 7269 6767 6572 5f63 7963 6c65 5f6e  _trigger_cycle_n
-00027e20: 756d 6265 7220 7368 6f75 6c64 2062 6520  umber should be 
-00027e30: 7573 6564 2074 6f20 7370 6563 6966 7920  used to specify 
-00027e40: 7468 6520 6379 636c 6520 6e75 6d62 6572  the cycle number
-00027e50: 206f 6e20 7768 6963 680a 2020 2020 2020   on which.      
-00027e60: 2020 4869 7374 6f72 7920 5241 4d20 7374    History RAM st
-00027e70: 6172 7473 2061 6371 7569 7269 6e67 2070  arts acquiring p
-00027e80: 6174 7465 726e 2069 6e66 6f72 6d61 7469  attern informati
-00027e90: 6f6e 2e0a 0a20 2020 2020 2020 2049 6620  on...        If 
-00027ea0: 4869 7374 6f72 7920 5241 4d20 7472 6967  History RAM trig
-00027eb0: 6765 7220 6973 2063 6f6e 6669 6775 7265  ger is configure
-00027ec0: 6420 6173 2048 6973 746f 7279 5241 4d54  d as HistoryRAMT
-00027ed0: 7269 6767 6572 5479 7065 2e50 4154 5445  riggerType.PATTE
-00027ee0: 524e 5f4c 4142 454c 2c0a 2020 2020 2020  RN_LABEL,.      
-00027ef0: 2020 7061 7474 6572 6e5f 6c61 6265 6c5f    pattern_label_
-00027f00: 6869 7374 6f72 795f 7261 6d5f 7472 6967  history_ram_trig
-00027f10: 6765 725f 6c61 6265 6c20 7368 6f75 6c64  ger_label should
-00027f20: 2062 6520 7573 6564 2074 6f20 7370 6563   be used to spec
-00027f30: 6966 7920 7468 6520 7061 7474 6572 6e20  ify the pattern 
-00027f40: 6c61 6265 6c20 6672 6f6d 2077 6869 6368  label from which
-00027f50: 2074 6f0a 2020 2020 2020 2020 7374 6172   to.        star
-00027f60: 7420 6163 7175 6972 696e 6720 7061 7474  t acquiring patt
-00027f70: 6572 6e20 696e 666f 726d 6174 696f 6e2e  ern information.
-00027f80: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00027f90: 5f6c 6162 656c 5f68 6973 746f 7279 5f72  _label_history_r
-00027fa0: 616d 5f74 7269 6767 6572 5f76 6563 746f  am_trigger_vecto
-00027fb0: 725f 6f66 6673 6574 2073 686f 756c 6420  r_offset should 
-00027fc0: 6265 2075 7365 6420 746f 2073 7065 6369  be used to speci
-00027fd0: 6679 2074 6865 206e 756d 6265 7220 6f66  fy the number of
-00027fe0: 2076 6563 746f 7273 0a20 2020 2020 2020   vectors.       
-00027ff0: 2066 6f6c 6c6f 7769 6e67 2074 6865 2073   following the s
-00028000: 7065 6369 6669 6564 2070 6174 7465 726e  pecified pattern
-00028010: 206c 6162 656c 2066 726f 6d20 7768 6963   label from whic
-00028020: 6820 746f 2073 7461 7274 2061 6371 7569  h to start acqui
-00028030: 7269 6e67 2070 6174 7465 726e 2069 6e66  ring pattern inf
-00028040: 6f72 6d61 7469 6f6e 2e0a 2020 2020 2020  ormation..      
-00028050: 2020 7061 7474 6572 6e5f 6c61 6265 6c5f    pattern_label_
-00028060: 6869 7374 6f72 795f 7261 6d5f 7472 6967  history_ram_trig
-00028070: 6765 725f 6379 636c 655f 6f66 6673 6574  ger_cycle_offset
-00028080: 2073 686f 756c 6420 6265 2075 7365 6420   should be used 
-00028090: 746f 2073 7065 6369 6679 2074 6865 206e  to specify the n
-000280a0: 756d 6265 7220 6f66 2063 7963 6c65 730a  umber of cycles.
-000280b0: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
-000280c0: 6720 7468 6520 7370 6563 6966 6965 6420  g the specified 
-000280d0: 7061 7474 6572 6e20 6c61 6265 6c20 616e  pattern label an
-000280e0: 6420 7665 6374 6f72 206f 6666 7365 7420  d vector offset 
-000280f0: 6672 6f6d 2077 6869 6368 2074 6f20 7374  from which to st
-00028100: 6172 7420 6163 7175 6972 696e 6720 7061  art acquiring pa
-00028110: 7474 6572 6e20 696e 666f 726d 6174 696f  ttern informatio
-00028120: 6e2e 0a0a 2020 2020 2020 2020 466f 7220  n...        For 
-00028130: 616c 6c20 4869 7374 6f72 7920 5241 4d20  all History RAM 
-00028140: 7472 6967 6765 7220 636f 6e64 6974 696f  trigger conditio
-00028150: 6e73 2c20 6869 7374 6f72 795f 7261 6d5f  ns, history_ram_
-00028160: 7072 6574 7269 6767 6572 5f73 616d 706c  pretrigger_sampl
-00028170: 6573 2073 686f 756c 6420 6265 2075 7365  es should be use
-00028180: 6420 746f 2073 7065 6369 6679 0a20 2020  d to specify.   
-00028190: 2020 2020 2074 6865 206e 756d 6265 7220       the number 
-000281a0: 6f66 2073 616d 706c 6573 2074 6f20 6163  of samples to ac
-000281b0: 7175 6972 6520 6265 666f 7265 2074 6865  quire before the
-000281c0: 2074 7269 6767 6572 2063 6f6e 6469 7469   trigger conditi
-000281d0: 6f6e 7320 6172 6520 6d65 742e 2049 6620  ons are met. If 
-000281e0: 796f 7520 636f 6e66 6967 7572 6520 4869  you configure Hi
-000281f0: 7374 6f72 7920 5241 4d20 746f 206f 6e6c  story RAM to onl
-00028200: 790a 2020 2020 2020 2020 6163 7175 6972  y.        acquir
-00028210: 6520 6661 696c 6564 2063 7963 6c65 732c  e failed cycles,
-00028220: 2079 6f75 206d 7573 7420 7365 7420 6869   you must set hi
-00028230: 7374 6f72 795f 7261 6d5f 7072 6574 7269  story_ram_pretri
-00028240: 6767 6572 5f73 616d 706c 6573 2074 6f20  gger_samples to 
-00028250: 302e 0a0a 2020 2020 2020 2020 6869 7374  0...        hist
-00028260: 6f72 795f 7261 6d5f 6379 636c 6573 5f74  ory_ram_cycles_t
-00028270: 6f5f 6163 7175 6972 6520 7368 6f75 6c64  o_acquire should
-00028280: 2062 6520 7573 6564 2074 6f20 7370 6563   be used to spec
-00028290: 6966 7920 7768 6963 6820 6379 636c 6573  ify which cycles
-000282a0: 2048 6973 746f 7279 2052 414d 2061 6371   History RAM acq
-000282b0: 7569 7265 7320 6166 7465 720a 2020 2020  uires after.    
-000282c0: 2020 2020 7468 6520 7472 6967 6765 7220      the trigger 
-000282d0: 636f 6e64 6974 696f 6e73 2061 7265 206d  conditions are m
-000282e0: 6574 2e0a 0a20 2020 2020 2020 2054 6970  et...        Tip
-000282f0: 3a0a 2020 2020 2020 2020 5468 6973 206d  :.        This m
-00028300: 6574 686f 6420 6361 6e20 6265 2063 616c  ethod can be cal
-00028310: 6c65 6420 6f6e 2073 7065 6369 6669 6320  led on specific 
-00028320: 7369 7465 7320 7769 7468 696e 2079 6f75  sites within you
-00028330: 7220 3a70 793a 636c 6173 733a 606e 6964  r :py:class:`nid
-00028340: 6967 6974 616c 2e53 6573 7369 6f6e 6020  igital.Session` 
-00028350: 696e 7374 616e 6365 2e0a 2020 2020 2020  instance..      
-00028360: 2020 5573 6520 5079 7468 6f6e 2069 6e64    Use Python ind
-00028370: 6578 206e 6f74 6174 696f 6e20 6f6e 2074  ex notation on t
-00028380: 6865 2072 6570 6561 7465 6420 6361 7061  he repeated capa
-00028390: 6269 6c69 7469 6573 2063 6f6e 7461 696e  bilities contain
-000283a0: 6572 2073 6974 6573 2074 6f20 7370 6563  er sites to spec
-000283b0: 6966 7920 6120 7375 6273 6574 2c0a 2020  ify a subset,.  
-000283c0: 2020 2020 2020 616e 6420 7468 656e 2063        and then c
-000283d0: 616c 6c20 7468 6973 206d 6574 686f 6420  all this method 
-000283e0: 6f6e 2074 6865 2072 6573 756c 742e 0a0a  on the result...
-000283f0: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
-00028400: 203a 7079 3a6d 6574 683a 606d 795f 7365   :py:meth:`my_se
-00028410: 7373 696f 6e2e 7369 7465 735b 202e 2e2e  ssion.sites[ ...
-00028420: 205d 2e67 6574 5f68 6973 746f 7279 5f72   ].get_history_r
-00028430: 616d 5f73 616d 706c 655f 636f 756e 7460  am_sample_count`
-00028440: 0a0a 2020 2020 2020 2020 546f 2063 616c  ..        To cal
-00028450: 6c20 7468 6520 6d65 7468 6f64 206f 6e20  l the method on 
-00028460: 616c 6c20 7369 7465 732c 2079 6f75 2063  all sites, you c
-00028470: 616e 2063 616c 6c20 6974 2064 6972 6563  an call it direc
-00028480: 746c 7920 6f6e 2074 6865 203a 7079 3a63  tly on the :py:c
-00028490: 6c61 7373 3a60 6e69 6469 6769 7461 6c2e  lass:`nidigital.
-000284a0: 5365 7373 696f 6e60 2e0a 0a20 2020 2020  Session`...     
-000284b0: 2020 2045 7861 6d70 6c65 3a20 3a70 793a     Example: :py:
-000284c0: 6d65 7468 3a60 6d79 5f73 6573 7369 6f6e  meth:`my_session
-000284d0: 2e67 6574 5f68 6973 746f 7279 5f72 616d  .get_history_ram
-000284e0: 5f73 616d 706c 655f 636f 756e 7460 0a0a  _sample_count`..
-000284f0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00028500: 0a20 2020 2020 2020 2020 2020 2073 616d  .            sam
-00028510: 706c 655f 636f 756e 7420 2869 6e74 293a  ple_count (int):
-00028520: 2054 6865 2072 6574 7572 6e65 6420 6e75   The returned nu
-00028530: 6d62 6572 206f 6620 7361 6d70 6c65 7320  mber of samples 
-00028540: 7468 6174 2048 6973 746f 7279 2052 414d  that History RAM
-00028550: 2061 6371 7569 7265 642e 0a0a 2020 2020   acquired...    
-00028560: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00028570: 7361 6d70 6c65 5f63 6f75 6e74 203d 2073  sample_count = s
-00028580: 656c 662e 5f69 6e74 6572 7072 6574 6572  elf._interpreter
-00028590: 2e67 6574 5f68 6973 746f 7279 5f72 616d  .get_history_ram
-000285a0: 5f73 616d 706c 655f 636f 756e 7428 7365  _sample_count(se
-000285b0: 6c66 2e5f 7265 7065 6174 6564 5f63 6170  lf._repeated_cap
-000285c0: 6162 696c 6974 7929 0a20 2020 2020 2020  ability).       
-000285d0: 2072 6574 7572 6e20 7361 6d70 6c65 5f63   return sample_c
-000285e0: 6f75 6e74 0a0a 2020 2020 4069 7669 5f73  ount..    @ivi_s
-000285f0: 796e 6368 726f 6e69 7a65 640a 2020 2020  ynchronized.    
-00028600: 6465 6620 5f67 6574 5f70 6174 7465 726e  def _get_pattern
-00028610: 5f6e 616d 6528 7365 6c66 2c20 7061 7474  _name(self, patt
-00028620: 6572 6e5f 696e 6465 7829 3a0a 2020 2020  ern_index):.    
-00028630: 2020 2020 7227 2727 5f67 6574 5f70 6174      r'''_get_pat
-00028640: 7465 726e 5f6e 616d 650a 0a20 2020 2020  tern_name..     
-00028650: 2020 2054 4244 0a0a 2020 2020 2020 2020     TBD..        
-00028660: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00028670: 2020 7061 7474 6572 6e5f 696e 6465 7820    pattern_index 
-00028680: 2869 6e74 293a 0a0a 0a20 2020 2020 2020  (int):...       
-00028690: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-000286a0: 2020 2020 2020 6e61 6d65 2028 7374 7229        name (str)
-000286b0: 3a0a 0a20 2020 2020 2020 2027 2727 0a20  :..        '''. 
-000286c0: 2020 2020 2020 206e 616d 6520 3d20 7365         name = se
-000286d0: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
-000286e0: 6765 745f 7061 7474 6572 6e5f 6e61 6d65  get_pattern_name
-000286f0: 2870 6174 7465 726e 5f69 6e64 6578 290a  (pattern_index).
-00028700: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-00028710: 616d 650a 0a20 2020 2040 6976 695f 7379  ame..    @ivi_sy
-00028720: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
-00028730: 6566 205f 6765 745f 7069 6e5f 6e61 6d65  ef _get_pin_name
-00028740: 2873 656c 662c 2070 696e 5f69 6e64 6578  (self, pin_index
-00028750: 293a 0a20 2020 2020 2020 2072 2727 275f  ):.        r'''_
-00028760: 6765 745f 7069 6e5f 6e61 6d65 0a0a 2020  get_pin_name..  
-00028770: 2020 2020 2020 5265 7475 726e 7320 7468        Returns th
-00028780: 6520 6e61 6d65 206f 6620 7468 6520 7069  e name of the pi
-00028790: 6e20 6174 2074 6865 2069 6e64 6578 2079  n at the index y
-000287a0: 6f75 2073 7065 6369 6679 2e20 596f 7520  ou specify. You 
-000287b0: 6d75 7374 2070 726f 7669 6465 2061 2056  must provide a V
-000287c0: 6943 6861 7220 6172 7261 7920 746f 2073  iChar array to s
-000287d0: 6572 7665 2061 7320 6120 6275 6666 6572  erve as a buffer
-000287e0: 2066 6f72 2074 6865 2076 616c 7565 2e20   for the value. 
-000287f0: 596f 7520 7061 7373 2074 6865 206e 756d  You pass the num
-00028800: 6265 7220 6f66 2062 7974 6573 2069 6e20  ber of bytes in 
-00028810: 7468 6520 6275 6666 6572 2061 7320 7468  the buffer as th
-00028820: 6520 2a2a 6e61 6d65 4275 6666 6572 5369  e **nameBufferSi
-00028830: 7a65 2a2a 2e20 4966 2074 6865 2063 7572  ze**. If the cur
-00028840: 7265 6e74 2076 616c 7565 206f 6620 7468  rent value of th
-00028850: 6520 7072 6f70 6572 7479 2c20 696e 636c  e property, incl
-00028860: 7564 696e 6720 7468 6520 7465 726d 696e  uding the termin
-00028870: 6174 696e 6720 4e55 4c4c 2062 7974 652c  ating NULL byte,
-00028880: 2069 7320 6c61 7267 6572 2074 6861 6e20   is larger than 
-00028890: 7468 6520 7369 7a65 2079 6f75 2069 6e64  the size you ind
-000288a0: 6963 6174 6520 696e 2074 6865 2062 7566  icate in the buf
-000288b0: 6665 7220 7369 7a65 2c20 7468 6520 6d65  fer size, the me
-000288c0: 7468 6f64 2063 6f70 6965 7320 2862 7566  thod copies (buf
-000288d0: 6665 7220 7369 7a65 202d 2031 2920 6279  fer size - 1) by
-000288e0: 7465 7320 696e 746f 2074 6865 2062 7566  tes into the buf
-000288f0: 6665 722c 2070 6c61 6365 7320 616e 2041  fer, places an A
-00028900: 5343 4949 204e 554c 4c20 6279 7465 2061  SCII NULL byte a
-00028910: 7420 7468 6520 656e 6420 6f66 2074 6865  t the end of the
-00028920: 2062 7566 6665 722c 2061 6e64 2072 6574   buffer, and ret
-00028930: 7572 6e73 2074 6865 2062 7566 6665 7220  urns the buffer 
-00028940: 7369 7a65 2079 6f75 206d 7573 7420 7061  size you must pa
-00028950: 7373 2074 6f20 6765 7420 7468 6520 656e  ss to get the en
-00028960: 7469 7265 2076 616c 7565 2e20 466f 7220  tire value. For 
-00028970: 6578 616d 706c 652c 2069 6620 7468 6520  example, if the 
-00028980: 7661 6c75 6520 6973 2022 3132 3334 3536  value is "123456
-00028990: 2220 616e 6420 7468 6520 6275 6666 6572  " and the buffer
-000289a0: 2073 697a 6520 6973 2034 2c20 7468 6520   size is 4, the 
-000289b0: 6d65 7468 6f64 2070 6c61 6365 7320 2231  method places "1
-000289c0: 3233 2220 696e 746f 2074 6865 2062 7566  23" into the buf
-000289d0: 6665 7220 616e 6420 7265 7475 726e 7320  fer and returns 
-000289e0: 372e 2049 6620 796f 7520 7761 6e74 2074  7. If you want t
-000289f0: 6f20 6361 6c6c 2074 6869 7320 6d65 7468  o call this meth
-00028a00: 6f64 206a 7573 7420 746f 2067 6574 2074  od just to get t
-00028a10: 6865 2072 6571 7569 7265 6420 6275 6666  he required buff
-00028a20: 6572 2073 697a 652c 2079 6f75 2063 616e  er size, you can
-00028a30: 2070 6173 7320 3020 666f 7220 2a2a 6e61   pass 0 for **na
-00028a40: 6d65 4275 6666 6572 5369 7a65 2a2a 2061  meBufferSize** a
-00028a50: 6e64 2056 495f 4e55 4c4c 2066 6f72 2074  nd VI_NULL for t
-00028a60: 6865 206e 616d 652e 0a0a 2020 2020 2020  he name...      
-00028a70: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00028a80: 2020 2020 7069 6e5f 696e 6465 7820 2869      pin_index (i
-00028a90: 6e74 293a 2049 6e64 6578 206f 6620 7069  nt): Index of pi
-00028aa0: 6e20 746f 2071 7565 7279 2e20 5069 6e20  n to query. Pin 
-00028ab0: 696e 6465 7865 7320 6265 6769 6e20 6174  indexes begin at
-00028ac0: 2030 2e0a 0a0a 2020 2020 2020 2020 5265   0....        Re
-00028ad0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00028ae0: 2020 206e 616d 6520 2873 7472 293a 2052     name (str): R
-00028af0: 6574 7572 6e73 2074 6865 2070 696e 206e  eturns the pin n
-00028b00: 616d 6520 6174 2074 6865 2073 7065 6369  ame at the speci
-00028b10: 6669 6564 202a 2a70 696e 496e 6465 782a  fied **pinIndex*
-00028b20: 2a2e 0a0a 2020 2020 2020 2020 2727 270a  *...        '''.
-00028b30: 2020 2020 2020 2020 6e61 6d65 203d 2073          name = s
-00028b40: 656c 662e 5f69 6e74 6572 7072 6574 6572  elf._interpreter
-00028b50: 2e67 6574 5f70 696e 5f6e 616d 6528 7069  .get_pin_name(pi
-00028b60: 6e5f 696e 6465 7829 0a20 2020 2020 2020  n_index).       
-00028b70: 2072 6574 7572 6e20 6e61 6d65 0a0a 2020   return name..  
-00028b80: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
-00028b90: 7a65 640a 2020 2020 6465 6620 5f67 6574  zed.    def _get
-00028ba0: 5f70 696e 5f72 6573 756c 7473 5f70 696e  _pin_results_pin
-00028bb0: 5f69 6e66 6f72 6d61 7469 6f6e 2873 656c  _information(sel
-00028bc0: 6629 3a0a 2020 2020 2020 2020 7227 2727  f):.        r'''
-00028bd0: 5f67 6574 5f70 696e 5f72 6573 756c 7473  _get_pin_results
-00028be0: 5f70 696e 5f69 6e66 6f72 6d61 7469 6f6e  _pin_information
-00028bf0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00028c00: 7320 7468 6520 7069 6e20 6e61 6d65 732c  s the pin names,
-00028c10: 2073 6974 6520 6e75 6d62 6572 732c 2061   site numbers, a
-00028c20: 6e64 2063 6861 6e6e 656c 206e 616d 6573  nd channel names
-00028c30: 2074 6861 7420 636f 7272 6573 706f 6e64   that correspond
-00028c40: 2074 6f20 7065 722d 7069 6e20 6461 7461   to per-pin data
-00028c50: 2072 6561 6420 6672 6f6d 2074 6865 2064   read from the d
-00028c60: 6967 6974 616c 2070 6174 7465 726e 2069  igital pattern i
-00028c70: 6e73 7472 756d 656e 742e 2054 6865 206d  nstrument. The m
-00028c80: 6574 686f 6420 7265 7475 726e 7320 7069  ethod returns pi
-00028c90: 6e20 696e 666f 726d 6174 696f 6e20 696e  n information in
-00028ca0: 2074 6865 2073 616d 6520 6f72 6465 7220   the same order 
-00028cb0: 6173 2076 616c 7565 7320 7265 6164 2075  as values read u
-00028cc0: 7369 6e67 2074 6865 2072 6561 645f 7374  sing the read_st
-00028cd0: 6174 6963 206d 6574 686f 642c 2070 706d  atic method, ppm
-00028ce0: 755f 6d65 6173 7572 6520 6d65 7468 6f64  u_measure method
-00028cf0: 2c20 616e 6420 6765 745f 6661 696c 5f63  , and get_fail_c
-00028d00: 6f75 6e74 206d 6574 686f 642e 2055 7365  ount method. Use
-00028d10: 2074 6869 7320 6d65 7468 6f64 2074 6f20   this method to 
-00028d20: 6d61 7463 6820 7661 6c75 6573 2074 6865  match values the
-00028d30: 2070 7265 7669 6f75 736c 7920 6c69 7374   previously list
-00028d40: 6564 206d 6574 686f 6473 2072 6574 7572  ed methods retur
-00028d50: 6e20 7769 7468 2070 696e 732c 2073 6974  n with pins, sit
-00028d60: 6573 2c20 616e 6420 696e 7374 7275 6d65  es, and instrume
-00028d70: 6e74 2063 6861 6e6e 656c 732e 0a0a 2020  nt channels...  
-00028d80: 2020 2020 2020 5469 703a 0a20 2020 2020        Tip:.     
-00028d90: 2020 2054 6869 7320 6d65 7468 6f64 2063     This method c
-00028da0: 616e 2062 6520 6361 6c6c 6564 206f 6e20  an be called on 
-00028db0: 7370 6563 6966 6963 2063 6861 6e6e 656c  specific channel
-00028dc0: 7320 7769 7468 696e 2079 6f75 7220 3a70  s within your :p
-00028dd0: 793a 636c 6173 733a 606e 6964 6967 6974  y:class:`nidigit
-00028de0: 616c 2e53 6573 7369 6f6e 6020 696e 7374  al.Session` inst
-00028df0: 616e 6365 2e0a 2020 2020 2020 2020 5573  ance..        Us
-00028e00: 6520 5079 7468 6f6e 2069 6e64 6578 206e  e Python index n
-00028e10: 6f74 6174 696f 6e20 6f6e 2074 6865 2072  otation on the r
-00028e20: 6570 6561 7465 6420 6361 7061 6269 6c69  epeated capabili
-00028e30: 7469 6573 2063 6f6e 7461 696e 6572 2063  ties container c
-00028e40: 6861 6e6e 656c 7320 746f 2073 7065 6369  hannels to speci
-00028e50: 6679 2061 2073 7562 7365 742c 0a20 2020  fy a subset,.   
-00028e60: 2020 2020 2061 6e64 2074 6865 6e20 6361       and then ca
-00028e70: 6c6c 2074 6869 7320 6d65 7468 6f64 206f  ll this method o
-00028e80: 6e20 7468 6520 7265 7375 6c74 2e0a 0a20  n the result... 
-00028e90: 2020 2020 2020 2045 7861 6d70 6c65 3a20         Example: 
-00028ea0: 3a70 793a 6d65 7468 3a60 6d79 5f73 6573  :py:meth:`my_ses
-00028eb0: 7369 6f6e 2e63 6861 6e6e 656c 735b 202e  sion.channels[ .
-00028ec0: 2e2e 205d 2e5f 6765 745f 7069 6e5f 7265  .. ]._get_pin_re
-00028ed0: 7375 6c74 735f 7069 6e5f 696e 666f 726d  sults_pin_inform
-00028ee0: 6174 696f 6e60 0a0a 2020 2020 2020 2020  ation`..        
-00028ef0: 546f 2063 616c 6c20 7468 6520 6d65 7468  To call the meth
-00028f00: 6f64 206f 6e20 616c 6c20 6368 616e 6e65  od on all channe
-00028f10: 6c73 2c20 796f 7520 6361 6e20 6361 6c6c  ls, you can call
-00028f20: 2069 7420 6469 7265 6374 6c79 206f 6e20   it directly on 
-00028f30: 7468 6520 3a70 793a 636c 6173 733a 606e  the :py:class:`n
-00028f40: 6964 6967 6974 616c 2e53 6573 7369 6f6e  idigital.Session
-00028f50: 602e 0a0a 2020 2020 2020 2020 4578 616d  `...        Exam
-00028f60: 706c 653a 203a 7079 3a6d 6574 683a 606d  ple: :py:meth:`m
-00028f70: 795f 7365 7373 696f 6e2e 5f67 6574 5f70  y_session._get_p
-00028f80: 696e 5f72 6573 756c 7473 5f70 696e 5f69  in_results_pin_i
-00028f90: 6e66 6f72 6d61 7469 6f6e 600a 0a20 2020  nformation`..   
-00028fa0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00028fb0: 2020 2020 2020 2020 2020 7069 6e5f 696e            pin_in
-00028fc0: 6465 7865 7320 286c 6973 7420 6f66 2069  dexes (list of i
-00028fd0: 6e74 293a 2054 6865 2072 6574 7572 6e65  nt): The returne
-00028fe0: 6420 696e 6465 7820 6f66 2074 6865 2070  d index of the p
-00028ff0: 696e 7320 636f 7272 6573 706f 6e64 696e  ins correspondin
-00029000: 6720 746f 2064 6174 6120 7265 6164 2066  g to data read f
-00029010: 726f 6d20 7468 6520 6469 6769 7461 6c20  rom the digital 
-00029020: 7061 7474 6572 6e20 696e 7374 7275 6d65  pattern instrume
-00029030: 6e74 2075 7369 6e67 2074 6865 2073 7065  nt using the spe
-00029040: 6369 6669 6564 2072 6570 6561 7465 6420  cified repeated 
-00029050: 6361 7061 6269 6c69 7469 6573 2e20 4966  capabilities. If
-00029060: 2079 6f75 2064 6f20 6e6f 7420 7761 6e74   you do not want
-00029070: 2074 6f20 7573 6520 7468 6973 2070 6172   to use this par
-00029080: 616d 6574 6572 2c20 7061 7373 2056 495f  ameter, pass VI_
-00029090: 4e55 4c4c 2e0a 2020 2020 2020 2020 2020  NULL..          
-000290a0: 2020 2020 2020 4361 6c6c 205f 6765 745f        Call _get_
-000290b0: 7069 6e5f 6e61 6d65 2074 6f20 6765 7420  pin_name to get 
-000290c0: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-000290d0: 7069 6e20 6173 736f 6369 6174 6564 2077  pin associated w
-000290e0: 6974 6820 616e 2069 6e64 6578 2e0a 0a20  ith an index... 
-000290f0: 2020 2020 2020 2020 2020 2073 6974 655f             site_
-00029100: 6e75 6d62 6572 7320 286c 6973 7420 6f66  numbers (list of
-00029110: 2069 6e74 293a 2054 6865 2072 6574 7572   int): The retur
-00029120: 6e65 6420 7369 7465 206e 756d 6265 7273  ned site numbers
-00029130: 2074 6861 7420 636f 7272 6573 706f 6e64   that correspond
-00029140: 2074 6f20 6461 7461 2072 6561 6420 6672   to data read fr
-00029150: 6f6d 2074 6865 2064 6967 6974 616c 2070  om the digital p
-00029160: 6174 7465 726e 2069 6e73 7472 756d 656e  attern instrumen
-00029170: 7420 7573 696e 6720 7468 6520 7370 6563  t using the spec
-00029180: 6966 6965 6420 7265 7065 6174 6564 2063  ified repeated c
-00029190: 6170 6162 696c 6974 6965 732e 2049 6620  apabilities. If 
-000291a0: 796f 7520 646f 206e 6f74 2077 616e 7420  you do not want 
-000291b0: 746f 2075 7365 2074 6869 7320 7061 7261  to use this para
-000291c0: 6d65 7465 722c 2070 6173 7320 5649 5f4e  meter, pass VI_N
-000291d0: 554c 4c2e 0a0a 2020 2020 2020 2020 2020  ULL...          
-000291e0: 2020 6368 616e 6e65 6c5f 696e 6465 7865    channel_indexe
-000291f0: 7320 286c 6973 7420 6f66 2069 6e74 293a  s (list of int):
-00029200: 2054 6865 2072 6574 7572 6e65 6420 696e   The returned in
-00029210: 6465 7820 6f66 2063 6861 6e6e 656c 7320  dex of channels 
-00029220: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
-00029230: 2064 6174 6120 7265 6164 2066 726f 6d20   data read from 
-00029240: 7468 6520 6469 6769 7461 6c20 7061 7474  the digital patt
-00029250: 6572 6e20 696e 7374 7275 6d65 6e74 2075  ern instrument u
-00029260: 7369 6e67 2074 6865 2073 7065 6369 6669  sing the specifi
-00029270: 6564 2072 6570 6561 7465 6420 6361 7061  ed repeated capa
-00029280: 6269 6c69 7469 6573 2e20 4966 2079 6f75  bilities. If you
-00029290: 2064 6f20 6e6f 7420 7761 6e74 2074 6f20   do not want to 
-000292a0: 7573 6520 7468 6973 2070 6172 616d 6574  use this paramet
-000292b0: 6572 2c20 7061 7373 2056 495f 4e55 4c4c  er, pass VI_NULL
-000292c0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000292d0: 2020 4361 6c6c 2047 6574 4368 616e 6e65    Call GetChanne
-000292e0: 6c4e 616d 6520 746f 2067 6574 2074 6865  lName to get the
-000292f0: 206e 616d 6520 6f66 2074 6865 2063 6861   name of the cha
-00029300: 6e6e 656c 2061 7373 6f63 6961 7465 6420  nnel associated 
-00029310: 7769 7468 2061 6e20 696e 6465 782e 2043  with an index. C
-00029320: 6861 6e6e 656c 2069 6e64 6578 6573 2061  hannel indexes a
-00029330: 7265 206f 6e65 2d62 6173 6564 2e0a 0a20  re one-based... 
-00029340: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-00029350: 6f74 653a 0a20 2020 2020 2020 2020 2020  ote:.           
-00029360: 2020 2020 204f 6e65 206f 7220 6d6f 7265       One or more
-00029370: 206f 6620 7468 6520 7265 6665 7265 6e63   of the referenc
-00029380: 6564 206d 6574 686f 6473 2061 7265 206e  ed methods are n
-00029390: 6f74 2069 6e20 7468 6520 5079 7468 6f6e  ot in the Python
-000293a0: 2041 5049 2066 6f72 2074 6869 7320 6472   API for this dr
-000293b0: 6976 6572 2e0a 0a20 2020 2020 2020 2027  iver...        '
-000293c0: 2727 0a20 2020 2020 2020 2070 696e 5f69  ''.        pin_i
-000293d0: 6e64 6578 6573 2c20 7369 7465 5f6e 756d  ndexes, site_num
-000293e0: 6265 7273 2c20 6368 616e 6e65 6c5f 696e  bers, channel_in
-000293f0: 6465 7865 7320 3d20 7365 6c66 2e5f 696e  dexes = self._in
-00029400: 7465 7270 7265 7465 722e 6765 745f 7069  terpreter.get_pi
-00029410: 6e5f 7265 7375 6c74 735f 7069 6e5f 696e  n_results_pin_in
-00029420: 666f 726d 6174 696f 6e28 7365 6c66 2e5f  formation(self._
-00029430: 7265 7065 6174 6564 5f63 6170 6162 696c  repeated_capabil
-00029440: 6974 7929 0a20 2020 2020 2020 2072 6574  ity).        ret
-00029450: 7572 6e20 7069 6e5f 696e 6465 7865 732c  urn pin_indexes,
-00029460: 2073 6974 655f 6e75 6d62 6572 732c 2063   site_numbers, c
-00029470: 6861 6e6e 656c 5f69 6e64 6578 6573 0a0a  hannel_indexes..
-00029480: 2020 2020 4069 7669 5f73 796e 6368 726f      @ivi_synchro
-00029490: 6e69 7a65 640a 2020 2020 6465 6620 5f67  nized.    def _g
-000294a0: 6574 5f73 6974 655f 7061 7373 5f66 6169  et_site_pass_fai
-000294b0: 6c28 7365 6c66 293a 0a20 2020 2020 2020  l(self):.       
-000294c0: 2072 2727 275f 6765 745f 7369 7465 5f70   r'''_get_site_p
-000294d0: 6173 735f 6661 696c 0a0a 2020 2020 2020  ass_fail..      
-000294e0: 2020 5265 7475 726e 7320 7468 6520 7061    Returns the pa
-000294f0: 7373 206f 7220 6661 696c 2072 6573 756c  ss or fail resul
-00029500: 7473 2066 6f72 2065 6163 6820 7369 7465  ts for each site
-00029510: 2e0a 0a20 2020 2020 2020 2054 6970 3a0a  ...        Tip:.
-00029520: 2020 2020 2020 2020 5468 6973 206d 6574          This met
-00029530: 686f 6420 6361 6e20 6265 2063 616c 6c65  hod can be calle
-00029540: 6420 6f6e 2073 7065 6369 6669 6320 7369  d on specific si
-00029550: 7465 7320 7769 7468 696e 2079 6f75 7220  tes within your 
-00029560: 3a70 793a 636c 6173 733a 606e 6964 6967  :py:class:`nidig
-00029570: 6974 616c 2e53 6573 7369 6f6e 6020 696e  ital.Session` in
-00029580: 7374 616e 6365 2e0a 2020 2020 2020 2020  stance..        
-00029590: 5573 6520 5079 7468 6f6e 2069 6e64 6578  Use Python index
-000295a0: 206e 6f74 6174 696f 6e20 6f6e 2074 6865   notation on the
-000295b0: 2072 6570 6561 7465 6420 6361 7061 6269   repeated capabi
-000295c0: 6c69 7469 6573 2063 6f6e 7461 696e 6572  lities container
-000295d0: 2073 6974 6573 2074 6f20 7370 6563 6966   sites to specif
-000295e0: 7920 6120 7375 6273 6574 2c0a 2020 2020  y a subset,.    
-000295f0: 2020 2020 616e 6420 7468 656e 2063 616c      and then cal
-00029600: 6c20 7468 6973 206d 6574 686f 6420 6f6e  l this method on
-00029610: 2074 6865 2072 6573 756c 742e 0a0a 2020   the result...  
-00029620: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
-00029630: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
-00029640: 696f 6e2e 7369 7465 735b 202e 2e2e 205d  ion.sites[ ... ]
-00029650: 2e5f 6765 745f 7369 7465 5f70 6173 735f  ._get_site_pass_
-00029660: 6661 696c 600a 0a20 2020 2020 2020 2054  fail`..        T
-00029670: 6f20 6361 6c6c 2074 6865 206d 6574 686f  o call the metho
-00029680: 6420 6f6e 2061 6c6c 2073 6974 6573 2c20  d on all sites, 
-00029690: 796f 7520 6361 6e20 6361 6c6c 2069 7420  you can call it 
-000296a0: 6469 7265 6374 6c79 206f 6e20 7468 6520  directly on the 
-000296b0: 3a70 793a 636c 6173 733a 606e 6964 6967  :py:class:`nidig
-000296c0: 6974 616c 2e53 6573 7369 6f6e 602e 0a0a  ital.Session`...
-000296d0: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
-000296e0: 203a 7079 3a6d 6574 683a 606d 795f 7365   :py:meth:`my_se
-000296f0: 7373 696f 6e2e 5f67 6574 5f73 6974 655f  ssion._get_site_
-00029700: 7061 7373 5f66 6169 6c60 0a0a 2020 2020  pass_fail`..    
-00029710: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00029720: 2020 2020 2020 2020 2070 6173 735f 6661           pass_fa
-00029730: 696c 2028 6c69 7374 206f 6620 626f 6f6c  il (list of bool
-00029740: 293a 2054 6865 2072 6574 7572 6e65 6420  ): The returned 
-00029750: 6172 7261 7920 6f66 2070 6173 7320 2854  array of pass (T
-00029760: 7275 6529 2061 6e64 2066 6169 6c20 7265  rue) and fail re
-00029770: 7375 6c74 7320 666f 7220 7468 6520 7369  sults for the si
-00029780: 7465 7320 796f 7520 7370 6563 6966 7920  tes you specify 
-00029790: 696e 2074 6865 2072 6570 6561 7465 6420  in the repeated 
-000297a0: 6361 7061 6269 6c69 7469 6573 2e20 4966  capabilities. If
-000297b0: 2073 6974 6573 2073 7061 6e20 6d75 6c74   sites span mult
-000297c0: 6970 6c65 2064 6967 6974 616c 2070 6174  iple digital pat
-000297d0: 7465 726e 2069 6e73 7472 756d 656e 7473  tern instruments
-000297e0: 2c20 796f 7520 6d75 7374 2075 7365 2061  , you must use a
-000297f0: 6e20 414e 4420 6f70 6572 6174 6f72 2066  n AND operator f
-00029800: 6f72 2074 6865 2070 6172 7469 616c 2072  or the partial r
-00029810: 6573 756c 7473 2066 6f72 2074 686f 7365  esults for those
-00029820: 2073 6974 6573 2072 6574 7572 6e65 6420   sites returned 
-00029830: 6279 2065 6163 6820 696e 7374 7275 6d65  by each instrume
-00029840: 6e74 2e20 4966 2061 2073 6974 6520 6973  nt. If a site is
-00029850: 2064 6973 6162 6c65 6420 6f72 206e 6f74   disabled or not
-00029860: 2065 6e61 626c 6564 2066 6f72 2062 7572   enabled for bur
-00029870: 7374 2c20 7468 6520 6d65 7468 6f64 2064  st, the method d
-00029880: 6f65 7320 6e6f 7420 7265 7475 726e 2064  oes not return d
-00029890: 6174 6120 666f 7220 7468 6174 2073 6974  ata for that sit
-000298a0: 652e 2055 7365 2074 6865 2053 6f72 7453  e. Use the SortS
-000298b0: 6974 6552 6573 756c 7473 5669 426f 6f6c  iteResultsViBool
-000298c0: 6561 6e20 6d65 7468 6f64 2074 6f20 6f72  ean method to or
-000298d0: 6465 7220 616e 6420 636f 6d62 696e 6520  der and combine 
-000298e0: 7468 6520 6461 7461 2074 6f20 6d61 7463  the data to matc
-000298f0: 6820 7468 6520 7265 7065 6174 6564 2063  h the repeated c
-00029900: 6170 6162 696c 6974 6965 732e 2059 6f75  apabilities. You
-00029910: 2063 616e 2061 6c73 6f20 7573 6520 7468   can also use th
-00029920: 6520 5f67 6574 5f73 6974 655f 7265 7375  e _get_site_resu
-00029930: 6c74 735f 7369 7465 5f6e 756d 6265 7273  lts_site_numbers
-00029940: 206d 6574 686f 6420 746f 2064 6574 6572   method to deter
-00029950: 6d69 6e65 2074 6865 206f 7264 6572 206f  mine the order o
-00029960: 6620 7468 6520 7369 7465 7320 7265 7475  f the sites retu
-00029970: 726e 6564 2066 726f 6d20 7468 6973 206d  rned from this m
-00029980: 6574 686f 6420 6361 6c6c 2073 6f20 7468  ethod call so th
-00029990: 6174 2079 6f75 2063 616e 206d 6174 6368  at you can match
-000299a0: 2074 6865 2070 6173 7320 6172 7261 7920   the pass array 
-000299b0: 7769 7468 2073 6974 6520 6e75 6d62 6572  with site number
-000299c0: 732e 0a0a 2020 2020 2020 2020 2020 2020  s...            
-000299d0: 2020 2020 4e6f 7465 3a0a 2020 2020 2020      Note:.      
-000299e0: 2020 2020 2020 2020 2020 4f6e 6520 6f72            One or
-000299f0: 206d 6f72 6520 6f66 2074 6865 2072 6566   more of the ref
-00029a00: 6572 656e 6365 6420 6d65 7468 6f64 7320  erenced methods 
-00029a10: 6172 6520 6e6f 7420 696e 2074 6865 2050  are not in the P
-00029a20: 7974 686f 6e20 4150 4920 666f 7220 7468  ython API for th
-00029a30: 6973 2064 7269 7665 722e 0a0a 2020 2020  is driver...    
-00029a40: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00029a50: 7061 7373 5f66 6169 6c20 3d20 7365 6c66  pass_fail = self
-00029a60: 2e5f 696e 7465 7270 7265 7465 722e 6765  ._interpreter.ge
-00029a70: 745f 7369 7465 5f70 6173 735f 6661 696c  t_site_pass_fail
-00029a80: 2873 656c 662e 5f72 6570 6561 7465 645f  (self._repeated_
-00029a90: 6361 7061 6269 6c69 7479 290a 2020 2020  capability).    
-00029aa0: 2020 2020 7265 7475 726e 2070 6173 735f      return pass_
-00029ab0: 6661 696c 0a0a 2020 2020 4069 7669 5f73  fail..    @ivi_s
-00029ac0: 796e 6368 726f 6e69 7a65 640a 2020 2020  ynchronized.    
-00029ad0: 6465 6620 5f67 6574 5f73 6974 655f 7265  def _get_site_re
-00029ae0: 7375 6c74 735f 7369 7465 5f6e 756d 6265  sults_site_numbe
-00029af0: 7273 2873 656c 662c 2073 6974 655f 7265  rs(self, site_re
-00029b00: 7375 6c74 5f74 7970 6529 3a0a 2020 2020  sult_type):.    
-00029b10: 2020 2020 7227 2727 5f67 6574 5f73 6974      r'''_get_sit
-00029b20: 655f 7265 7375 6c74 735f 7369 7465 5f6e  e_results_site_n
-00029b30: 756d 6265 7273 0a0a 2020 2020 2020 2020  umbers..        
-00029b40: 5265 7475 726e 7320 7468 6520 7369 7465  Returns the site
-00029b50: 206e 756d 6265 7273 2074 6861 7420 636f   numbers that co
-00029b60: 7272 6573 706f 6e64 2074 6f20 7065 722d  rrespond to per-
-00029b70: 7369 7465 2064 6174 6120 7265 6164 2066  site data read f
-00029b80: 726f 6d20 7468 6520 6469 6769 7461 6c20  rom the digital 
-00029b90: 7061 7474 6572 6e20 696e 7374 7275 6d65  pattern instrume
-00029ba0: 6e74 2e20 5468 6520 6d65 7468 6f64 2072  nt. The method r
-00029bb0: 6574 7572 6e73 2073 6974 6520 6e75 6d62  eturns site numb
-00029bc0: 6572 7320 696e 2074 6865 2073 616d 6520  ers in the same 
-00029bd0: 6f72 6465 7220 6173 2076 616c 7565 7320  order as values 
-00029be0: 7265 6164 2075 7369 6e67 2074 6865 205f  read using the _
-00029bf0: 6765 745f 7369 7465 5f70 6173 735f 6661  get_site_pass_fa
-00029c00: 696c 2061 6e64 2066 6574 6368 5f63 6170  il and fetch_cap
-00029c10: 7475 7265 5f77 6176 6566 6f72 6d5f 7533  ture_waveform_u3
-00029c20: 3220 6d65 7468 6f64 732e 2055 7365 2074  2 methods. Use t
-00029c30: 6869 7320 6d65 7468 6f64 2074 6f20 6d61  his method to ma
-00029c40: 7463 6820 7661 6c75 6573 2074 6865 2070  tch values the p
-00029c50: 7265 7669 6f75 736c 7920 6c69 7374 6564  reviously listed
-00029c60: 206d 6574 686f 6473 2072 6574 7572 6e20   methods return 
-00029c70: 7769 7468 2073 6974 6520 6e75 6d62 6572  with site number
-00029c80: 732e 0a0a 2020 2020 2020 2020 5469 703a  s...        Tip:
-00029c90: 0a20 2020 2020 2020 2054 6869 7320 6d65  .        This me
-00029ca0: 7468 6f64 2063 616e 2062 6520 6361 6c6c  thod can be call
-00029cb0: 6564 206f 6e20 7370 6563 6966 6963 2073  ed on specific s
-00029cc0: 6974 6573 2077 6974 6869 6e20 796f 7572  ites within your
-00029cd0: 203a 7079 3a63 6c61 7373 3a60 6e69 6469   :py:class:`nidi
-00029ce0: 6769 7461 6c2e 5365 7373 696f 6e60 2069  gital.Session` i
-00029cf0: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
-00029d00: 2055 7365 2050 7974 686f 6e20 696e 6465   Use Python inde
-00029d10: 7820 6e6f 7461 7469 6f6e 206f 6e20 7468  x notation on th
-00029d20: 6520 7265 7065 6174 6564 2063 6170 6162  e repeated capab
-00029d30: 696c 6974 6965 7320 636f 6e74 6169 6e65  ilities containe
-00029d40: 7220 7369 7465 7320 746f 2073 7065 6369  r sites to speci
-00029d50: 6679 2061 2073 7562 7365 742c 0a20 2020  fy a subset,.   
-00029d60: 2020 2020 2061 6e64 2074 6865 6e20 6361       and then ca
-00029d70: 6c6c 2074 6869 7320 6d65 7468 6f64 206f  ll this method o
-00029d80: 6e20 7468 6520 7265 7375 6c74 2e0a 0a20  n the result... 
-00029d90: 2020 2020 2020 2045 7861 6d70 6c65 3a20         Example: 
-00029da0: 3a70 793a 6d65 7468 3a60 6d79 5f73 6573  :py:meth:`my_ses
-00029db0: 7369 6f6e 2e73 6974 6573 5b20 2e2e 2e20  sion.sites[ ... 
-00029dc0: 5d2e 5f67 6574 5f73 6974 655f 7265 7375  ]._get_site_resu
-00029dd0: 6c74 735f 7369 7465 5f6e 756d 6265 7273  lts_site_numbers
-00029de0: 600a 0a20 2020 2020 2020 2054 6f20 6361  `..        To ca
-00029df0: 6c6c 2074 6865 206d 6574 686f 6420 6f6e  ll the method on
-00029e00: 2061 6c6c 2073 6974 6573 2c20 796f 7520   all sites, you 
-00029e10: 6361 6e20 6361 6c6c 2069 7420 6469 7265  can call it dire
-00029e20: 6374 6c79 206f 6e20 7468 6520 3a70 793a  ctly on the :py:
-00029e30: 636c 6173 733a 606e 6964 6967 6974 616c  class:`nidigital
-00029e40: 2e53 6573 7369 6f6e 602e 0a0a 2020 2020  .Session`...    
-00029e50: 2020 2020 4578 616d 706c 653a 203a 7079      Example: :py
-00029e60: 3a6d 6574 683a 606d 795f 7365 7373 696f  :meth:`my_sessio
-00029e70: 6e2e 5f67 6574 5f73 6974 655f 7265 7375  n._get_site_resu
-00029e80: 6c74 735f 7369 7465 5f6e 756d 6265 7273  lts_site_numbers
-00029e90: 600a 0a20 2020 2020 2020 2041 7267 733a  `..        Args:
-00029ea0: 0a20 2020 2020 2020 2020 2020 2073 6974  .            sit
-00029eb0: 655f 7265 7375 6c74 5f74 7970 6520 2865  e_result_type (e
-00029ec0: 6e75 6d73 2e53 6974 6552 6573 756c 7454  nums.SiteResultT
-00029ed0: 7970 6529 3a20 5468 6520 7479 7065 206f  ype): The type o
-00029ee0: 6620 6461 7461 2073 7065 6369 6669 6564  f data specified
-00029ef0: 2069 6e20 7468 6520 7265 7375 6c74 7320   in the results 
-00029f00: 6172 7261 792e 0a0a 2020 2020 2020 2020  array...        
-00029f10: 2020 2020 2020 2020 2d20 2020 5f53 6974          -   _Sit
-00029f20: 6552 6573 756c 7454 7970 652e 5041 5353  eResultType.PASS
-00029f30: 5f46 4149 4c3a 2047 6574 2073 6974 6520  _FAIL: Get site 
-00029f40: 6e75 6d62 6572 7320 666f 7220 7061 7373  numbers for pass
-00029f50: 2f66 6169 6c20 6461 7461 2e0a 2020 2020  /fail data..    
-00029f60: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
-00029f70: 5f53 6974 6552 6573 756c 7454 7970 652e  _SiteResultType.
-00029f80: 4341 5054 5552 455f 5741 5645 464f 524d  CAPTURE_WAVEFORM
-00029f90: 3a20 4765 7420 7369 7465 206e 756d 6265  : Get site numbe
-00029fa0: 7273 2066 6f72 2063 6170 7475 7265 2077  rs for capture w
-00029fb0: 6176 6566 6f72 6d73 2e0a 0a0a 2020 2020  aveforms....    
-00029fc0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00029fd0: 2020 2020 2020 2020 2073 6974 655f 6e75           site_nu
-00029fe0: 6d62 6572 7320 286c 6973 7420 6f66 2069  mbers (list of i
-00029ff0: 6e74 293a 2054 6865 2072 6574 7572 6e65  nt): The returne
-0002a000: 6420 6172 7261 7920 6f66 2073 6974 6520  d array of site 
-0002a010: 6e75 6d62 6572 7320 7468 6174 2063 6f72  numbers that cor
-0002a020: 7265 7370 6f6e 6420 746f 2074 6865 2076  respond to the v
-0002a030: 616c 7565 7320 7370 6563 6966 6965 6420  alues specified 
-0002a040: 6279 202a 2a73 6974 6552 6573 756c 7454  by **siteResultT
-0002a050: 7970 652a 2a2e 0a0a 2020 2020 2020 2020  ype**...        
-0002a060: 2727 270a 2020 2020 2020 2020 6966 2074  '''.        if t
-0002a070: 7970 6528 7369 7465 5f72 6573 756c 745f  ype(site_result_
-0002a080: 7479 7065 2920 6973 206e 6f74 2065 6e75  type) is not enu
-0002a090: 6d73 2e5f 5369 7465 5265 7375 6c74 5479  ms._SiteResultTy
-0002a0a0: 7065 3a0a 2020 2020 2020 2020 2020 2020  pe:.            
-0002a0b0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-0002a0c0: 2750 6172 616d 6574 6572 2073 6974 655f  'Parameter site_
-0002a0d0: 7265 7375 6c74 5f74 7970 6520 6d75 7374  result_type must
-0002a0e0: 2062 6520 6f66 2074 7970 6520 2720 2b20   be of type ' + 
-0002a0f0: 7374 7228 656e 756d 732e 5f53 6974 6552  str(enums._SiteR
-0002a100: 6573 756c 7454 7970 6529 290a 2020 2020  esultType)).    
-0002a110: 2020 2020 7369 7465 5f6e 756d 6265 7273      site_numbers
-0002a120: 203d 2073 656c 662e 5f69 6e74 6572 7072   = self._interpr
-0002a130: 6574 6572 2e67 6574 5f73 6974 655f 7265  eter.get_site_re
-0002a140: 7375 6c74 735f 7369 7465 5f6e 756d 6265  sults_site_numbe
-0002a150: 7273 2873 656c 662e 5f72 6570 6561 7465  rs(self._repeate
-0002a160: 645f 6361 7061 6269 6c69 7479 2c20 7369  d_capability, si
-0002a170: 7465 5f72 6573 756c 745f 7479 7065 290a  te_result_type).
-0002a180: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0002a190: 6974 655f 6e75 6d62 6572 730a 0a20 2020  ite_numbers..   
-0002a1a0: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
-0002a1b0: 6564 0a20 2020 2064 6566 2067 6574 5f74  ed.    def get_t
-0002a1c0: 696d 655f 7365 745f 6472 6976 655f 666f  ime_set_drive_fo
-0002a1d0: 726d 6174 2873 656c 662c 2074 696d 655f  rmat(self, time_
-0002a1e0: 7365 745f 6e61 6d65 293a 0a20 2020 2020  set_name):.     
-0002a1f0: 2020 2072 2727 2767 6574 5f74 696d 655f     r'''get_time_
-0002a200: 7365 745f 6472 6976 655f 666f 726d 6174  set_drive_format
-0002a210: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0002a220: 7320 7468 6520 6472 6976 6520 666f 726d  s the drive form
-0002a230: 6174 206f 6620 6120 7069 6e20 696e 2074  at of a pin in t
-0002a240: 6865 2073 7065 6369 6669 6564 2074 696d  he specified tim
-0002a250: 6520 7365 742e 0a0a 2020 2020 2020 2020  e set...        
-0002a260: 5469 703a 0a20 2020 2020 2020 2054 6869  Tip:.        Thi
-0002a270: 7320 6d65 7468 6f64 2063 616e 2062 6520  s method can be 
-0002a280: 6361 6c6c 6564 206f 6e20 7370 6563 6966  called on specif
-0002a290: 6963 2070 696e 7320 7769 7468 696e 2079  ic pins within y
-0002a2a0: 6f75 7220 3a70 793a 636c 6173 733a 606e  our :py:class:`n
-0002a2b0: 6964 6967 6974 616c 2e53 6573 7369 6f6e  idigital.Session
-0002a2c0: 6020 696e 7374 616e 6365 2e0a 2020 2020  ` instance..    
-0002a2d0: 2020 2020 5573 6520 5079 7468 6f6e 2069      Use Python i
-0002a2e0: 6e64 6578 206e 6f74 6174 696f 6e20 6f6e  ndex notation on
-0002a2f0: 2074 6865 2072 6570 6561 7465 6420 6361   the repeated ca
-0002a300: 7061 6269 6c69 7469 6573 2063 6f6e 7461  pabilities conta
-0002a310: 696e 6572 2070 696e 7320 746f 2073 7065  iner pins to spe
-0002a320: 6369 6679 2061 2073 7562 7365 742c 0a20  cify a subset,. 
-0002a330: 2020 2020 2020 2061 6e64 2074 6865 6e20         and then 
-0002a340: 6361 6c6c 2074 6869 7320 6d65 7468 6f64  call this method
-0002a350: 206f 6e20 7468 6520 7265 7375 6c74 2e0a   on the result..
-0002a360: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0002a370: 3a20 3a70 793a 6d65 7468 3a60 6d79 5f73  : :py:meth:`my_s
-0002a380: 6573 7369 6f6e 2e70 696e 735b 202e 2e2e  ession.pins[ ...
-0002a390: 205d 2e67 6574 5f74 696d 655f 7365 745f   ].get_time_set_
-0002a3a0: 6472 6976 655f 666f 726d 6174 600a 0a20  drive_format`.. 
-0002a3b0: 2020 2020 2020 2054 6f20 6361 6c6c 2074         To call t
-0002a3c0: 6865 206d 6574 686f 6420 6f6e 2061 6c6c  he method on all
-0002a3d0: 2070 696e 732c 2079 6f75 2063 616e 2063   pins, you can c
-0002a3e0: 616c 6c20 6974 2064 6972 6563 746c 7920  all it directly 
-0002a3f0: 6f6e 2074 6865 203a 7079 3a63 6c61 7373  on the :py:class
-0002a400: 3a60 6e69 6469 6769 7461 6c2e 5365 7373  :`nidigital.Sess
-0002a410: 696f 6e60 2e0a 0a20 2020 2020 2020 2045  ion`...        E
-0002a420: 7861 6d70 6c65 3a20 3a70 793a 6d65 7468  xample: :py:meth
-0002a430: 3a60 6d79 5f73 6573 7369 6f6e 2e67 6574  :`my_session.get
-0002a440: 5f74 696d 655f 7365 745f 6472 6976 655f  _time_set_drive_
-0002a450: 666f 726d 6174 600a 0a20 2020 2020 2020  format`..       
-0002a460: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0002a470: 2020 2074 696d 655f 7365 745f 6e61 6d65     time_set_name
-0002a480: 2028 7374 7229 3a20 5468 6520 7370 6563   (str): The spec
-0002a490: 6966 6965 6420 7469 6d65 2073 6574 206e  ified time set n
-0002a4a0: 616d 652e 0a0a 0a20 2020 2020 2020 2052  ame....        R
-0002a4b0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0002a4c0: 2020 2020 666f 726d 6174 2028 656e 756d      format (enum
-0002a4d0: 732e 4472 6976 6546 6f72 6d61 7429 3a20  s.DriveFormat): 
-0002a4e0: 5265 7475 726e 6564 2064 7269 7665 2066  Returned drive f
-0002a4f0: 6f72 6d61 7420 6f66 2074 6865 2074 696d  ormat of the tim
-0002a500: 6520 7365 7420 666f 7220 7468 6520 7370  e set for the sp
-0002a510: 6563 6966 6965 6420 7069 6e2e 0a0a 2020  ecified pin...  
-0002a520: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0002a530: 2020 666f 726d 6174 203d 2073 656c 662e    format = self.
-0002a540: 5f69 6e74 6572 7072 6574 6572 2e67 6574  _interpreter.get
-0002a550: 5f74 696d 655f 7365 745f 6472 6976 655f  _time_set_drive_
-0002a560: 666f 726d 6174 2873 656c 662e 5f72 6570  format(self._rep
-0002a570: 6561 7465 645f 6361 7061 6269 6c69 7479  eated_capability
-0002a580: 2c20 7469 6d65 5f73 6574 5f6e 616d 6529  , time_set_name)
-0002a590: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002a5a0: 666f 726d 6174 0a0a 2020 2020 4069 7669  format..    @ivi
-0002a5b0: 5f73 796e 6368 726f 6e69 7a65 640a 2020  _synchronized.  
-0002a5c0: 2020 6465 6620 6765 745f 7469 6d65 5f73    def get_time_s
-0002a5d0: 6574 5f65 6467 6528 7365 6c66 2c20 7469  et_edge(self, ti
-0002a5e0: 6d65 5f73 6574 5f6e 616d 652c 2065 6467  me_set_name, edg
-0002a5f0: 6529 3a0a 2020 2020 2020 2020 7227 2727  e):.        r'''
-0002a600: 6765 745f 7469 6d65 5f73 6574 5f65 6467  get_time_set_edg
-0002a610: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
-0002a620: 6e73 2074 6865 2065 6467 6520 7469 6d65  ns the edge time
-0002a630: 206f 6620 6120 7069 6e20 696e 2074 6865   of a pin in the
-0002a640: 2073 7065 6369 6669 6564 2074 696d 6520   specified time 
-0002a650: 7365 742e 0a0a 2020 2020 2020 2020 5469  set...        Ti
-0002a660: 703a 0a20 2020 2020 2020 2054 6869 7320  p:.        This 
-0002a670: 6d65 7468 6f64 2063 616e 2062 6520 6361  method can be ca
-0002a680: 6c6c 6564 206f 6e20 7370 6563 6966 6963  lled on specific
-0002a690: 2070 696e 7320 7769 7468 696e 2079 6f75   pins within you
-0002a6a0: 7220 3a70 793a 636c 6173 733a 606e 6964  r :py:class:`nid
-0002a6b0: 6967 6974 616c 2e53 6573 7369 6f6e 6020  igital.Session` 
-0002a6c0: 696e 7374 616e 6365 2e0a 2020 2020 2020  instance..      
-0002a6d0: 2020 5573 6520 5079 7468 6f6e 2069 6e64    Use Python ind
-0002a6e0: 6578 206e 6f74 6174 696f 6e20 6f6e 2074  ex notation on t
-0002a6f0: 6865 2072 6570 6561 7465 6420 6361 7061  he repeated capa
-0002a700: 6269 6c69 7469 6573 2063 6f6e 7461 696e  bilities contain
-0002a710: 6572 2070 696e 7320 746f 2073 7065 6369  er pins to speci
-0002a720: 6679 2061 2073 7562 7365 742c 0a20 2020  fy a subset,.   
-0002a730: 2020 2020 2061 6e64 2074 6865 6e20 6361       and then ca
-0002a740: 6c6c 2074 6869 7320 6d65 7468 6f64 206f  ll this method o
-0002a750: 6e20 7468 6520 7265 7375 6c74 2e0a 0a20  n the result... 
-0002a760: 2020 2020 2020 2045 7861 6d70 6c65 3a20         Example: 
-0002a770: 3a70 793a 6d65 7468 3a60 6d79 5f73 6573  :py:meth:`my_ses
-0002a780: 7369 6f6e 2e70 696e 735b 202e 2e2e 205d  sion.pins[ ... ]
-0002a790: 2e67 6574 5f74 696d 655f 7365 745f 6564  .get_time_set_ed
-0002a7a0: 6765 600a 0a20 2020 2020 2020 2054 6f20  ge`..        To 
-0002a7b0: 6361 6c6c 2074 6865 206d 6574 686f 6420  call the method 
-0002a7c0: 6f6e 2061 6c6c 2070 696e 732c 2079 6f75  on all pins, you
-0002a7d0: 2063 616e 2063 616c 6c20 6974 2064 6972   can call it dir
-0002a7e0: 6563 746c 7920 6f6e 2074 6865 203a 7079  ectly on the :py
-0002a7f0: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
-0002a800: 6c2e 5365 7373 696f 6e60 2e0a 0a20 2020  l.Session`...   
-0002a810: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
-0002a820: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
-0002a830: 6f6e 2e67 6574 5f74 696d 655f 7365 745f  on.get_time_set_
-0002a840: 6564 6765 600a 0a20 2020 2020 2020 2041  edge`..        A
-0002a850: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0002a860: 2074 696d 655f 7365 745f 6e61 6d65 2028   time_set_name (
-0002a870: 7374 7229 3a20 5468 6520 7370 6563 6966  str): The specif
-0002a880: 6965 6420 7469 6d65 2073 6574 206e 616d  ied time set nam
-0002a890: 652e 0a0a 2020 2020 2020 2020 2020 2020  e...            
-0002a8a0: 6564 6765 2028 656e 756d 732e 5469 6d65  edge (enums.Time
-0002a8b0: 5365 7445 6467 6554 7970 6529 3a20 4e61  SetEdgeType): Na
-0002a8c0: 6d65 206f 6620 7468 6520 6564 6765 2e0a  me of the edge..
-0002a8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a8e0: 202d 2020 2054 696d 6553 6574 4564 6765   -   TimeSetEdge
-0002a8f0: 5479 7065 2e44 5249 5645 5f4f 4e0a 2020  Type.DRIVE_ON.  
-0002a900: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-0002a910: 2020 5469 6d65 5365 7445 6467 6554 7970    TimeSetEdgeTyp
-0002a920: 652e 4452 4956 455f 4441 5441 0a20 2020  e.DRIVE_DATA.   
-0002a930: 2020 2020 2020 2020 2020 2020 202d 2020               -  
-0002a940: 2054 696d 6553 6574 4564 6765 5479 7065   TimeSetEdgeType
-0002a950: 2e44 5249 5645 5f52 4554 5552 4e0a 2020  .DRIVE_RETURN.  
-0002a960: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-0002a970: 2020 5469 6d65 5365 7445 6467 6554 7970    TimeSetEdgeTyp
-0002a980: 652e 4452 4956 455f 4f46 460a 2020 2020  e.DRIVE_OFF.    
-0002a990: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
-0002a9a0: 5469 6d65 5365 7445 6467 6554 7970 652e  TimeSetEdgeType.
-0002a9b0: 434f 4d50 4152 455f 5354 524f 4245 0a20  COMPARE_STROBE. 
-0002a9c0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-0002a9d0: 2020 2054 696d 6553 6574 4564 6765 5479     TimeSetEdgeTy
-0002a9e0: 7065 2e44 5249 5645 5f44 4154 4132 0a20  pe.DRIVE_DATA2. 
-0002a9f0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-0002aa00: 2020 2054 696d 6553 6574 4564 6765 5479     TimeSetEdgeTy
-0002aa10: 7065 2e44 5249 5645 5f52 4554 5552 4e32  pe.DRIVE_RETURN2
-0002aa20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002aa30: 202d 2020 2054 696d 6553 6574 4564 6765   -   TimeSetEdge
-0002aa40: 5479 7065 2e43 4f4d 5041 5245 5f53 5452  Type.COMPARE_STR
-0002aa50: 4f42 4532 0a0a 0a20 2020 2020 2020 2052  OBE2...        R
-0002aa60: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0002aa70: 2020 2020 7469 6d65 2028 6869 6768 7469      time (highti
-0002aa80: 6d65 2e74 696d 6564 656c 7461 293a 2054  me.timedelta): T
-0002aa90: 696d 6520 6672 6f6d 2074 6865 2062 6567  ime from the beg
-0002aaa0: 696e 6e69 6e67 206f 6620 7468 6520 7665  inning of the ve
-0002aab0: 6374 6f72 2070 6572 696f 6420 696e 2077  ctor period in w
-0002aac0: 6869 6368 2074 6f20 706c 6163 6520 7468  hich to place th
-0002aad0: 6520 6564 6765 2e0a 0a20 2020 2020 2020  e edge...       
-0002aae0: 2027 2727 0a20 2020 2020 2020 2069 6620   '''.        if 
-0002aaf0: 7479 7065 2865 6467 6529 2069 7320 6e6f  type(edge) is no
-0002ab00: 7420 656e 756d 732e 5469 6d65 5365 7445  t enums.TimeSetE
-0002ab10: 6467 6554 7970 653a 0a20 2020 2020 2020  dgeType:.       
-0002ab20: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-0002ab30: 7272 6f72 2827 5061 7261 6d65 7465 7220  rror('Parameter 
-0002ab40: 6564 6765 206d 7573 7420 6265 206f 6620  edge must be of 
-0002ab50: 7479 7065 2027 202b 2073 7472 2865 6e75  type ' + str(enu
-0002ab60: 6d73 2e54 696d 6553 6574 4564 6765 5479  ms.TimeSetEdgeTy
-0002ab70: 7065 2929 0a20 2020 2020 2020 2074 696d  pe)).        tim
-0002ab80: 6520 3d20 7365 6c66 2e5f 696e 7465 7270  e = self._interp
-0002ab90: 7265 7465 722e 6765 745f 7469 6d65 5f73  reter.get_time_s
-0002aba0: 6574 5f65 6467 6528 7365 6c66 2e5f 7265  et_edge(self._re
-0002abb0: 7065 6174 6564 5f63 6170 6162 696c 6974  peated_capabilit
-0002abc0: 792c 2074 696d 655f 7365 745f 6e61 6d65  y, time_set_name
-0002abd0: 2c20 6564 6765 290a 2020 2020 2020 2020  , edge).        
-0002abe0: 7265 7475 726e 205f 636f 6e76 6572 7465  return _converte
-0002abf0: 7273 2e63 6f6e 7665 7274 5f73 6563 6f6e  rs.convert_secon
-0002ac00: 6473 5f72 6561 6c36 345f 746f 5f74 696d  ds_real64_to_tim
-0002ac10: 6564 656c 7461 2874 696d 6529 0a0a 2020  edelta(time)..  
-0002ac20: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
-0002ac30: 7a65 640a 2020 2020 6465 6620 6765 745f  zed.    def get_
-0002ac40: 7469 6d65 5f73 6574 5f65 6467 655f 6d75  time_set_edge_mu
-0002ac50: 6c74 6970 6c69 6572 2873 656c 662c 2074  ltiplier(self, t
-0002ac60: 696d 655f 7365 745f 6e61 6d65 293a 0a20  ime_set_name):. 
-0002ac70: 2020 2020 2020 2072 2727 2767 6574 5f74         r'''get_t
-0002ac80: 696d 655f 7365 745f 6564 6765 5f6d 756c  ime_set_edge_mul
-0002ac90: 7469 706c 6965 720a 0a20 2020 2020 2020  tiplier..       
-0002aca0: 2052 6574 7572 6e73 2074 6865 2065 6467   Returns the edg
-0002acb0: 6520 6d75 6c74 6970 6c69 6572 206f 6620  e multiplier of 
-0002acc0: 7468 6520 7370 6563 6966 6965 6420 7469  the specified ti
-0002acd0: 6d65 2073 6574 2e0a 0a20 2020 2020 2020  me set...       
-0002ace0: 2054 6970 3a0a 2020 2020 2020 2020 5468   Tip:.        Th
-0002acf0: 6973 206d 6574 686f 6420 6361 6e20 6265  is method can be
-0002ad00: 2063 616c 6c65 6420 6f6e 2073 7065 6369   called on speci
-0002ad10: 6669 6320 7069 6e73 2077 6974 6869 6e20  fic pins within 
-0002ad20: 796f 7572 203a 7079 3a63 6c61 7373 3a60  your :py:class:`
-0002ad30: 6e69 6469 6769 7461 6c2e 5365 7373 696f  nidigital.Sessio
-0002ad40: 6e60 2069 6e73 7461 6e63 652e 0a20 2020  n` instance..   
-0002ad50: 2020 2020 2055 7365 2050 7974 686f 6e20       Use Python 
-0002ad60: 696e 6465 7820 6e6f 7461 7469 6f6e 206f  index notation o
-0002ad70: 6e20 7468 6520 7265 7065 6174 6564 2063  n the repeated c
-0002ad80: 6170 6162 696c 6974 6965 7320 636f 6e74  apabilities cont
-0002ad90: 6169 6e65 7220 7069 6e73 2074 6f20 7370  ainer pins to sp
-0002ada0: 6563 6966 7920 6120 7375 6273 6574 2c0a  ecify a subset,.
-0002adb0: 2020 2020 2020 2020 616e 6420 7468 656e          and then
-0002adc0: 2063 616c 6c20 7468 6973 206d 6574 686f   call this metho
-0002add0: 6420 6f6e 2074 6865 2072 6573 756c 742e  d on the result.
-0002ade0: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-0002adf0: 653a 203a 7079 3a6d 6574 683a 606d 795f  e: :py:meth:`my_
-0002ae00: 7365 7373 696f 6e2e 7069 6e73 5b20 2e2e  session.pins[ ..
-0002ae10: 2e20 5d2e 6765 745f 7469 6d65 5f73 6574  . ].get_time_set
-0002ae20: 5f65 6467 655f 6d75 6c74 6970 6c69 6572  _edge_multiplier
-0002ae30: 600a 0a20 2020 2020 2020 2054 6f20 6361  `..        To ca
-0002ae40: 6c6c 2074 6865 206d 6574 686f 6420 6f6e  ll the method on
-0002ae50: 2061 6c6c 2070 696e 732c 2079 6f75 2063   all pins, you c
-0002ae60: 616e 2063 616c 6c20 6974 2064 6972 6563  an call it direc
-0002ae70: 746c 7920 6f6e 2074 6865 203a 7079 3a63  tly on the :py:c
-0002ae80: 6c61 7373 3a60 6e69 6469 6769 7461 6c2e  lass:`nidigital.
-0002ae90: 5365 7373 696f 6e60 2e0a 0a20 2020 2020  Session`...     
-0002aea0: 2020 2045 7861 6d70 6c65 3a20 3a70 793a     Example: :py:
-0002aeb0: 6d65 7468 3a60 6d79 5f73 6573 7369 6f6e  meth:`my_session
-0002aec0: 2e67 6574 5f74 696d 655f 7365 745f 6564  .get_time_set_ed
-0002aed0: 6765 5f6d 756c 7469 706c 6965 7260 0a0a  ge_multiplier`..
-0002aee0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0002aef0: 2020 2020 2020 2020 2020 7469 6d65 5f73            time_s
-0002af00: 6574 5f6e 616d 6520 2873 7472 293a 2054  et_name (str): T
-0002af10: 6865 2073 7065 6369 6669 6564 2074 696d  he specified tim
-0002af20: 6520 7365 7420 6e61 6d65 2e0a 0a0a 2020  e set name....  
-0002af30: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0002af40: 2020 2020 2020 2020 2020 2065 6467 655f             edge_
-0002af50: 6d75 6c74 6970 6c69 6572 2028 696e 7429  multiplier (int)
-0002af60: 3a20 5265 7475 726e 6564 2065 6467 6520  : Returned edge 
-0002af70: 6d75 6c74 6970 6c69 6572 206f 6620 7468  multiplier of th
-0002af80: 6520 7469 6d65 2073 6574 2066 6f72 2074  e time set for t
-0002af90: 6865 2073 7065 6369 6669 6564 2070 696e  he specified pin
-0002afa0: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
-0002afb0: 2020 2020 2020 2065 6467 655f 6d75 6c74         edge_mult
-0002afc0: 6970 6c69 6572 203d 2073 656c 662e 5f69  iplier = self._i
-0002afd0: 6e74 6572 7072 6574 6572 2e67 6574 5f74  nterpreter.get_t
-0002afe0: 696d 655f 7365 745f 6564 6765 5f6d 756c  ime_set_edge_mul
-0002aff0: 7469 706c 6965 7228 7365 6c66 2e5f 7265  tiplier(self._re
-0002b000: 7065 6174 6564 5f63 6170 6162 696c 6974  peated_capabilit
-0002b010: 792c 2074 696d 655f 7365 745f 6e61 6d65  y, time_set_name
-0002b020: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002b030: 2065 6467 655f 6d75 6c74 6970 6c69 6572   edge_multiplier
-0002b040: 0a0a 2020 2020 4069 7669 5f73 796e 6368  ..    @ivi_synch
-0002b050: 726f 6e69 7a65 640a 2020 2020 6465 6620  ronized.    def 
-0002b060: 5f67 6574 5f74 696d 655f 7365 745f 6e61  _get_time_set_na
-0002b070: 6d65 2873 656c 662c 2074 696d 655f 7365  me(self, time_se
-0002b080: 745f 696e 6465 7829 3a0a 2020 2020 2020  t_index):.      
-0002b090: 2020 7227 2727 5f67 6574 5f74 696d 655f    r'''_get_time_
-0002b0a0: 7365 745f 6e61 6d65 0a0a 2020 2020 2020  set_name..      
-0002b0b0: 2020 5442 440a 0a20 2020 2020 2020 2041    TBD..        A
-0002b0c0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0002b0d0: 2074 696d 655f 7365 745f 696e 6465 7820   time_set_index 
-0002b0e0: 2869 6e74 293a 0a0a 0a20 2020 2020 2020  (int):...       
-0002b0f0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0002b100: 2020 2020 2020 6e61 6d65 2028 7374 7229        name (str)
-0002b110: 3a0a 0a20 2020 2020 2020 2027 2727 0a20  :..        '''. 
-0002b120: 2020 2020 2020 206e 616d 6520 3d20 7365         name = se
-0002b130: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
-0002b140: 6765 745f 7469 6d65 5f73 6574 5f6e 616d  get_time_set_nam
-0002b150: 6528 7469 6d65 5f73 6574 5f69 6e64 6578  e(time_set_index
-0002b160: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002b170: 206e 616d 650a 0a20 2020 2040 6976 695f   name..    @ivi_
-0002b180: 7379 6e63 6872 6f6e 697a 6564 0a20 2020  synchronized.   
-0002b190: 2064 6566 2069 735f 7369 7465 5f65 6e61   def is_site_ena
-0002b1a0: 626c 6564 2873 656c 6629 3a0a 2020 2020  bled(self):.    
-0002b1b0: 2020 2020 7227 2727 6973 5f73 6974 655f      r'''is_site_
-0002b1c0: 656e 6162 6c65 640a 0a20 2020 2020 2020  enabled..       
-0002b1d0: 2043 6865 636b 7320 6966 2061 2073 7065   Checks if a spe
-0002b1e0: 6369 6669 6564 2073 6974 6520 6973 2065  cified site is e
-0002b1f0: 6e61 626c 6564 2e0a 0a20 2020 2020 2020  nabled...       
-0002b200: 204e 6f74 653a 2054 6865 206d 6574 686f   Note: The metho
-0002b210: 6420 7265 7475 726e 7320 616e 2065 7272  d returns an err
-0002b220: 6f72 2069 6620 6d6f 7265 2074 6861 6e20  or if more than 
-0002b230: 6f6e 6520 7369 7465 2069 7320 7370 6563  one site is spec
-0002b240: 6966 6965 642e 0a0a 2020 2020 2020 2020  ified...        
-0002b250: 5469 703a 0a20 2020 2020 2020 2054 6869  Tip:.        Thi
-0002b260: 7320 6d65 7468 6f64 2063 616e 2062 6520  s method can be 
-0002b270: 6361 6c6c 6564 206f 6e20 7370 6563 6966  called on specif
-0002b280: 6963 2073 6974 6573 2077 6974 6869 6e20  ic sites within 
-0002b290: 796f 7572 203a 7079 3a63 6c61 7373 3a60  your :py:class:`
-0002b2a0: 6e69 6469 6769 7461 6c2e 5365 7373 696f  nidigital.Sessio
-0002b2b0: 6e60 2069 6e73 7461 6e63 652e 0a20 2020  n` instance..   
-0002b2c0: 2020 2020 2055 7365 2050 7974 686f 6e20       Use Python 
-0002b2d0: 696e 6465 7820 6e6f 7461 7469 6f6e 206f  index notation o
-0002b2e0: 6e20 7468 6520 7265 7065 6174 6564 2063  n the repeated c
-0002b2f0: 6170 6162 696c 6974 6965 7320 636f 6e74  apabilities cont
-0002b300: 6169 6e65 7220 7369 7465 7320 746f 2073  ainer sites to s
-0002b310: 7065 6369 6679 2061 2073 7562 7365 742c  pecify a subset,
-0002b320: 0a20 2020 2020 2020 2061 6e64 2074 6865  .        and the
-0002b330: 6e20 6361 6c6c 2074 6869 7320 6d65 7468  n call this meth
-0002b340: 6f64 206f 6e20 7468 6520 7265 7375 6c74  od on the result
-0002b350: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
-0002b360: 6c65 3a20 3a70 793a 6d65 7468 3a60 6d79  le: :py:meth:`my
-0002b370: 5f73 6573 7369 6f6e 2e73 6974 6573 5b20  _session.sites[ 
-0002b380: 2e2e 2e20 5d2e 6973 5f73 6974 655f 656e  ... ].is_site_en
-0002b390: 6162 6c65 6460 0a0a 2020 2020 2020 2020  abled`..        
-0002b3a0: 546f 2063 616c 6c20 7468 6520 6d65 7468  To call the meth
-0002b3b0: 6f64 206f 6e20 616c 6c20 7369 7465 732c  od on all sites,
-0002b3c0: 2079 6f75 2063 616e 2063 616c 6c20 6974   you can call it
-0002b3d0: 2064 6972 6563 746c 7920 6f6e 2074 6865   directly on the
-0002b3e0: 203a 7079 3a63 6c61 7373 3a60 6e69 6469   :py:class:`nidi
-0002b3f0: 6769 7461 6c2e 5365 7373 696f 6e60 2e0a  gital.Session`..
-0002b400: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0002b410: 3a20 3a70 793a 6d65 7468 3a60 6d79 5f73  : :py:meth:`my_s
-0002b420: 6573 7369 6f6e 2e69 735f 7369 7465 5f65  ession.is_site_e
-0002b430: 6e61 626c 6564 600a 0a20 2020 2020 2020  nabled`..       
-0002b440: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0002b450: 2020 2020 2020 656e 6162 6c65 2028 626f        enable (bo
-0002b460: 6f6c 293a 2042 6f6f 6c65 616e 2076 616c  ol): Boolean val
-0002b470: 7565 2074 6861 7420 7265 7475 726e 7320  ue that returns 
-0002b480: 7768 6574 6865 7220 7468 6520 7369 7465  whether the site
-0002b490: 2069 7320 656e 6162 6c65 6420 6f72 2064   is enabled or d
-0002b4a0: 6973 6162 6c65 642e 0a0a 2020 2020 2020  isabled...      
-0002b4b0: 2020 2727 270a 2020 2020 2020 2020 656e    '''.        en
-0002b4c0: 6162 6c65 203d 2073 656c 662e 5f69 6e74  able = self._int
-0002b4d0: 6572 7072 6574 6572 2e69 735f 7369 7465  erpreter.is_site
-0002b4e0: 5f65 6e61 626c 6564 2873 656c 662e 5f72  _enabled(self._r
-0002b4f0: 6570 6561 7465 645f 6361 7061 6269 6c69  epeated_capabili
-0002b500: 7479 290a 2020 2020 2020 2020 7265 7475  ty).        retu
-0002b510: 726e 2065 6e61 626c 650a 0a20 2020 2064  rn enable..    d
-0002b520: 6566 206c 6f63 6b28 7365 6c66 293a 0a20  ef lock(self):. 
-0002b530: 2020 2020 2020 2027 2727 6c6f 636b 0a0a         '''lock..
-0002b540: 2020 2020 2020 2020 4f62 7461 696e 7320          Obtains 
-0002b550: 6120 6d75 6c74 6974 6872 6561 6420 6c6f  a multithread lo
-0002b560: 636b 206f 6e20 7468 6520 6465 7669 6365  ck on the device
-0002b570: 2073 6573 7369 6f6e 2e20 4265 666f 7265   session. Before
-0002b580: 2064 6f69 6e67 2073 6f2c 2074 6865 0a20   doing so, the. 
-0002b590: 2020 2020 2020 2073 6f66 7477 6172 6520         software 
-0002b5a0: 7761 6974 7320 756e 7469 6c20 616c 6c20  waits until all 
-0002b5b0: 6f74 6865 7220 6578 6563 7574 696f 6e20  other execution 
-0002b5c0: 7468 7265 6164 7320 7265 6c65 6173 6520  threads release 
-0002b5d0: 7468 6569 7220 6c6f 636b 730a 2020 2020  their locks.    
-0002b5e0: 2020 2020 6f6e 2074 6865 2064 6576 6963      on the devic
-0002b5f0: 6520 7365 7373 696f 6e2e 0a0a 2020 2020  e session...    
-0002b600: 2020 2020 4f74 6865 7220 7468 7265 6164      Other thread
-0002b610: 7320 6d61 7920 6861 7665 206f 6274 6169  s may have obtai
-0002b620: 6e65 6420 6120 6c6f 636b 206f 6e20 7468  ned a lock on th
-0002b630: 6973 2073 6573 7369 6f6e 2066 6f72 2074  is session for t
-0002b640: 6865 0a20 2020 2020 2020 2066 6f6c 6c6f  he.        follo
-0002b650: 7769 6e67 2072 6561 736f 6e73 3a0a 0a20  wing reasons:.. 
-0002b660: 2020 2020 2020 2020 2020 202d 2020 5468             -  Th
-0002b670: 6520 6170 706c 6963 6174 696f 6e20 6361  e application ca
-0002b680: 6c6c 6564 2074 6865 206c 6f63 6b20 6d65  lled the lock me
-0002b690: 7468 6f64 2e0a 2020 2020 2020 2020 2020  thod..          
-0002b6a0: 2020 2d20 2041 2063 616c 6c20 746f 204e    -  A call to N
-0002b6b0: 492d 4469 6769 7461 6c20 5061 7474 6572  I-Digital Patter
-0002b6c0: 6e20 4472 6976 6572 206c 6f63 6b65 6420  n Driver locked 
-0002b6d0: 7468 6520 7365 7373 696f 6e2e 0a20 2020  the session..   
-0002b6e0: 2020 2020 2020 2020 202d 2020 4166 7465           -  Afte
-0002b6f0: 7220 6120 6361 6c6c 2074 6f20 7468 6520  r a call to the 
-0002b700: 6c6f 636b 206d 6574 686f 6420 7265 7475  lock method retu
-0002b710: 726e 730a 2020 2020 2020 2020 2020 2020  rns.            
-0002b720: 2020 2073 7563 6365 7373 6675 6c6c 792c     successfully,
-0002b730: 206e 6f20 6f74 6865 7220 7468 7265 6164   no other thread
-0002b740: 7320 6361 6e20 6163 6365 7373 2074 6865  s can access the
-0002b750: 2064 6576 6963 6520 7365 7373 696f 6e20   device session 
-0002b760: 756e 7469 6c0a 2020 2020 2020 2020 2020  until.          
-0002b770: 2020 2020 2079 6f75 2063 616c 6c20 7468       you call th
-0002b780: 6520 756e 6c6f 636b 206d 6574 686f 6420  e unlock method 
-0002b790: 6f72 2065 7869 7420 6f75 7420 6f66 2074  or exit out of t
-0002b7a0: 6865 2077 6974 6820 626c 6f63 6b20 7768  he with block wh
-0002b7b0: 656e 2075 7369 6e67 0a20 2020 2020 2020  en using.       
-0002b7c0: 2020 2020 2020 2020 6c6f 636b 2063 6f6e          lock con
-0002b7d0: 7465 7874 206d 616e 6167 6572 2e0a 2020  text manager..  
-0002b7e0: 2020 2020 2020 2020 2020 2d20 2055 7365            -  Use
-0002b7f0: 2074 6865 206c 6f63 6b20 6d65 7468 6f64   the lock method
-0002b800: 2061 6e64 2074 6865 0a20 2020 2020 2020   and the.       
-0002b810: 2020 2020 2020 2020 756e 6c6f 636b 206d          unlock m
-0002b820: 6574 686f 6420 6172 6f75 6e64 2061 2073  ethod around a s
-0002b830: 6571 7565 6e63 6520 6f66 2063 616c 6c73  equence of calls
-0002b840: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-0002b850: 2020 2069 6e73 7472 756d 656e 7420 6472     instrument dr
-0002b860: 6976 6572 206d 6574 686f 6473 2069 6620  iver methods if 
-0002b870: 796f 7520 7265 7175 6972 6520 7468 6174  you require that
-0002b880: 2074 6865 2064 6576 6963 6520 7265 7461   the device reta
-0002b890: 696e 2069 7473 0a20 2020 2020 2020 2020  in its.         
-0002b8a0: 2020 2020 2020 7365 7474 696e 6773 2074        settings t
-0002b8b0: 6872 6f75 6768 2074 6865 2065 6e64 206f  hrough the end o
-0002b8c0: 6620 7468 6520 7365 7175 656e 6365 2e0a  f the sequence..
-0002b8d0: 0a20 2020 2020 2020 2059 6f75 2063 616e  .        You can
-0002b8e0: 2073 6166 656c 7920 6d61 6b65 206e 6573   safely make nes
-0002b8f0: 7465 6420 6361 6c6c 7320 746f 2074 6865  ted calls to the
-0002b900: 206c 6f63 6b20 6d65 7468 6f64 0a20 2020   lock method.   
-0002b910: 2020 2020 2077 6974 6869 6e20 7468 6520       within the 
-0002b920: 7361 6d65 2074 6872 6561 642e 2054 6f20  same thread. To 
-0002b930: 636f 6d70 6c65 7465 6c79 2075 6e6c 6f63  completely unloc
-0002b940: 6b20 7468 6520 7365 7373 696f 6e2c 2079  k the session, y
-0002b950: 6f75 206d 7573 740a 2020 2020 2020 2020  ou must.        
-0002b960: 6261 6c61 6e63 6520 6561 6368 2063 616c  balance each cal
-0002b970: 6c20 746f 2074 6865 206c 6f63 6b20 6d65  l to the lock me
-0002b980: 7468 6f64 2077 6974 6820 6120 6361 6c6c  thod with a call
-0002b990: 2074 6f0a 2020 2020 2020 2020 7468 6520   to.        the 
-0002b9a0: 756e 6c6f 636b 206d 6574 686f 642e 0a0a  unlock method...
-0002b9b0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0002b9c0: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-0002b9d0: 6b20 2863 6f6e 7465 7874 206d 616e 6167  k (context manag
-0002b9e0: 6572 293a 2057 6865 6e20 7573 6564 2069  er): When used i
-0002b9f0: 6e20 6120 7769 7468 2073 7461 7465 6d65  n a with stateme
-0002ba00: 6e74 2c20 6e69 6469 6769 7461 6c2e 5365  nt, nidigital.Se
-0002ba10: 7373 696f 6e2e 6c6f 636b 2061 6374 7320  ssion.lock acts 
-0002ba20: 6173 0a20 2020 2020 2020 2020 2020 2061  as.            a
-0002ba30: 2063 6f6e 7465 7874 206d 616e 6167 6572   context manager
-0002ba40: 2061 6e64 2075 6e6c 6f63 6b20 7769 6c6c   and unlock will
-0002ba50: 2062 6520 6361 6c6c 6564 2077 6865 6e20   be called when 
-0002ba60: 7468 6520 7769 7468 2062 6c6f 636b 2069  the with block i
-0002ba70: 7320 6578 6974 6564 0a20 2020 2020 2020  s exited.       
-0002ba80: 2027 2727 0a20 2020 2020 2020 2073 656c   '''.        sel
-0002ba90: 662e 5f69 6e74 6572 7072 6574 6572 2e6c  f._interpreter.l
-0002baa0: 6f63 6b28 2920 2023 2057 6520 646f 206e  ock()  # We do n
-0002bab0: 6f74 2063 616c 6c20 7468 6973 2069 6e20  ot call this in 
-0002bac0: 7468 6520 636f 6e74 6578 7420 6d61 6e61  the context mana
-0002bad0: 6765 7220 736f 2074 6861 7420 7468 6973  ger so that this
-0002bae0: 2066 756e 6374 696f 6e20 6361 6e0a 2020   function can.  
-0002baf0: 2020 2020 2020 2320 6163 7420 7374 616e        # act stan
-0002bb00: 6461 6c6f 6e65 2061 7320 7765 6c6c 2061  dalone as well a
-0002bb10: 6e64 206c 6574 2074 6865 2063 6c69 656e  nd let the clien
-0002bb20: 7420 6361 6c6c 2075 6e6c 6f63 6b28 2920  t call unlock() 
-0002bb30: 6578 706c 6963 6974 6c79 2e20 4966 2074  explicitly. If t
-0002bb40: 6865 7920 646f 2075 7365 2074 6865 2063  hey do use the c
-0002bb50: 6f6e 7465 7874 206d 616e 6167 6572 2c0a  ontext manager,.
-0002bb60: 2020 2020 2020 2020 2320 7468 6174 2077          # that w
-0002bb70: 696c 6c20 6861 6e64 6c65 2074 6865 2075  ill handle the u
-0002bb80: 6e6c 6f63 6b20 666f 7220 7468 656d 0a20  nlock for them. 
-0002bb90: 2020 2020 2020 2072 6574 7572 6e20 5f4c         return _L
-0002bba0: 6f63 6b28 7365 6c66 290a 0a20 2020 2040  ock(self)..    @
-0002bbb0: 6976 695f 7379 6e63 6872 6f6e 697a 6564  ivi_synchronized
-0002bbc0: 0a20 2020 2064 6566 2070 706d 755f 6d65  .    def ppmu_me
-0002bbd0: 6173 7572 6528 7365 6c66 2c20 6d65 6173  asure(self, meas
-0002bbe0: 7572 656d 656e 745f 7479 7065 293a 0a20  urement_type):. 
-0002bbf0: 2020 2020 2020 2072 2727 2770 706d 755f         r'''ppmu_
-0002bc00: 6d65 6173 7572 650a 0a20 2020 2020 2020  measure..       
-0002bc10: 2049 6e73 7472 7563 7473 2074 6865 2050   Instructs the P
-0002bc20: 504d 5520 746f 206d 6561 7375 7265 2076  PMU to measure v
-0002bc30: 6f6c 7461 6765 206f 7220 6375 7272 656e  oltage or curren
-0002bc40: 742e 2054 6869 7320 6d65 7468 6f64 2063  t. This method c
-0002bc50: 616e 2062 6520 6361 6c6c 6564 2074 6f20  an be called to 
-0002bc60: 7461 6b65 2061 2076 6f6c 7461 6765 206d  take a voltage m
-0002bc70: 6561 7375 7265 6d65 6e74 2065 7665 6e20  easurement even 
-0002bc80: 6966 2074 6865 2070 696e 206d 6574 686f  if the pin metho
-0002bc90: 6420 6973 206e 6f74 2073 6574 2074 6f20  d is not set to 
-0002bca0: 5050 4d55 2e0a 0a20 2020 2020 2020 2054  PPMU...        T
-0002bcb0: 6970 3a0a 2020 2020 2020 2020 5468 6973  ip:.        This
-0002bcc0: 206d 6574 686f 6420 6361 6e20 6265 2063   method can be c
-0002bcd0: 616c 6c65 6420 6f6e 2073 7065 6369 6669  alled on specifi
-0002bce0: 6320 6368 616e 6e65 6c73 2077 6974 6869  c channels withi
-0002bcf0: 6e20 796f 7572 203a 7079 3a63 6c61 7373  n your :py:class
-0002bd00: 3a60 6e69 6469 6769 7461 6c2e 5365 7373  :`nidigital.Sess
-0002bd10: 696f 6e60 2069 6e73 7461 6e63 652e 0a20  ion` instance.. 
-0002bd20: 2020 2020 2020 2055 7365 2050 7974 686f         Use Pytho
-0002bd30: 6e20 696e 6465 7820 6e6f 7461 7469 6f6e  n index notation
-0002bd40: 206f 6e20 7468 6520 7265 7065 6174 6564   on the repeated
-0002bd50: 2063 6170 6162 696c 6974 6965 7320 636f   capabilities co
-0002bd60: 6e74 6169 6e65 7220 6368 616e 6e65 6c73  ntainer channels
-0002bd70: 2074 6f20 7370 6563 6966 7920 6120 7375   to specify a su
-0002bd80: 6273 6574 2c0a 2020 2020 2020 2020 616e  bset,.        an
-0002bd90: 6420 7468 656e 2063 616c 6c20 7468 6973  d then call this
-0002bda0: 206d 6574 686f 6420 6f6e 2074 6865 2072   method on the r
-0002bdb0: 6573 756c 742e 0a0a 2020 2020 2020 2020  esult...        
-0002bdc0: 4578 616d 706c 653a 203a 7079 3a6d 6574  Example: :py:met
-0002bdd0: 683a 606d 795f 7365 7373 696f 6e2e 6368  h:`my_session.ch
-0002bde0: 616e 6e65 6c73 5b20 2e2e 2e20 5d2e 7070  annels[ ... ].pp
-0002bdf0: 6d75 5f6d 6561 7375 7265 600a 0a20 2020  mu_measure`..   
-0002be00: 2020 2020 2054 6f20 6361 6c6c 2074 6865       To call the
-0002be10: 206d 6574 686f 6420 6f6e 2061 6c6c 2063   method on all c
-0002be20: 6861 6e6e 656c 732c 2079 6f75 2063 616e  hannels, you can
-0002be30: 2063 616c 6c20 6974 2064 6972 6563 746c   call it directl
-0002be40: 7920 6f6e 2074 6865 203a 7079 3a63 6c61  y on the :py:cla
-0002be50: 7373 3a60 6e69 6469 6769 7461 6c2e 5365  ss:`nidigital.Se
-0002be60: 7373 696f 6e60 2e0a 0a20 2020 2020 2020  ssion`...       
-0002be70: 2045 7861 6d70 6c65 3a20 3a70 793a 6d65   Example: :py:me
-0002be80: 7468 3a60 6d79 5f73 6573 7369 6f6e 2e70  th:`my_session.p
-0002be90: 706d 755f 6d65 6173 7572 6560 0a0a 2020  pmu_measure`..  
-0002bea0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0002beb0: 2020 2020 2020 2020 6d65 6173 7572 656d          measurem
-0002bec0: 656e 745f 7479 7065 2028 656e 756d 732e  ent_type (enums.
-0002bed0: 5050 4d55 4d65 6173 7572 656d 656e 7454  PPMUMeasurementT
-0002bee0: 7970 6529 3a20 5061 7261 6d65 7465 7220  ype): Parameter 
-0002bef0: 7468 6174 2073 7065 6369 6669 6573 2077  that specifies w
-0002bf00: 6865 7468 6572 2074 6865 2050 504d 5520  hether the PPMU 
-0002bf10: 6d65 6173 7572 6573 2076 6f6c 7461 6765  measures voltage
-0002bf20: 206f 7220 6375 7272 656e 7420 6672 6f6d   or current from
-0002bf30: 2074 6865 2044 5554 2e0a 0a20 2020 2020   the DUT...     
-0002bf40: 2020 2020 2020 2020 2020 202d 2020 2050             -   P
-0002bf50: 504d 554d 6561 7375 7265 6d65 6e74 5479  PMUMeasurementTy
-0002bf60: 7065 2e43 5552 5245 4e54 3a20 5468 6520  pe.CURRENT: The 
-0002bf70: 5050 4d55 206d 6561 7375 7265 7320 6375  PPMU measures cu
-0002bf80: 7272 656e 7420 6672 6f6d 2074 6865 2044  rrent from the D
-0002bf90: 5554 2e0a 2020 2020 2020 2020 2020 2020  UT..            
-0002bfa0: 2020 2020 2d20 2020 5050 4d55 4d65 6173      -   PPMUMeas
-0002bfb0: 7572 656d 656e 7454 7970 652e 564f 4c54  urementType.VOLT
-0002bfc0: 4147 453a 2054 6865 2050 504d 5520 6d65  AGE: The PPMU me
-0002bfd0: 6173 7572 6573 2076 6f6c 7461 6765 2066  asures voltage f
-0002bfe0: 726f 6d20 7468 6520 4455 542e 0a0a 0a20  rom the DUT.... 
-0002bff0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0002c000: 2020 2020 2020 2020 2020 2020 6d65 6173              meas
-0002c010: 7572 656d 656e 7473 2028 6c69 7374 206f  urements (list o
-0002c020: 6620 666c 6f61 7429 3a20 5468 6520 7265  f float): The re
-0002c030: 7475 726e 6564 2061 7272 6179 206f 6620  turned array of 
-0002c040: 6d65 6173 7572 656d 656e 7473 2069 6e20  measurements in 
-0002c050: 7468 6520 6f72 6465 7220 796f 7520 7370  the order you sp
-0002c060: 6563 6966 7920 696e 2074 6865 2072 6570  ecify in the rep
-0002c070: 6561 7465 6420 6361 7061 6269 6c69 7469  eated capabiliti
-0002c080: 6573 2e20 4966 2061 2073 6974 6520 6973  es. If a site is
-0002c090: 2064 6973 6162 6c65 642c 2074 6865 206d   disabled, the m
-0002c0a0: 6574 686f 6420 646f 6573 206e 6f74 2072  ethod does not r
-0002c0b0: 6574 7572 6e20 6461 7461 2066 6f72 2074  eturn data for t
-0002c0c0: 6861 7420 7369 7465 2e20 596f 7520 6361  hat site. You ca
-0002c0d0: 6e20 616c 736f 2075 7365 2074 6865 2067  n also use the g
-0002c0e0: 6574 5f70 696e 5f72 6573 756c 7473 5f70  et_pin_results_p
-0002c0f0: 696e 5f69 6e66 6f72 6d61 7469 6f6e 206d  in_information m
-0002c100: 6574 686f 6420 746f 206f 6274 6169 6e20  ethod to obtain 
-0002c110: 6120 736f 7274 6564 206c 6973 7420 6f66  a sorted list of
-0002c120: 2072 6574 7572 6e65 6420 7369 7465 7320   returned sites 
-0002c130: 616e 6420 6368 616e 6e65 6c73 2e0a 0a20  and channels... 
-0002c140: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-0002c150: 2020 2069 6620 7479 7065 286d 6561 7375     if type(measu
-0002c160: 7265 6d65 6e74 5f74 7970 6529 2069 7320  rement_type) is 
-0002c170: 6e6f 7420 656e 756d 732e 5050 4d55 4d65  not enums.PPMUMe
-0002c180: 6173 7572 656d 656e 7454 7970 653a 0a20  asurementType:. 
-0002c190: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0002c1a0: 2054 7970 6545 7272 6f72 2827 5061 7261   TypeError('Para
-0002c1b0: 6d65 7465 7220 6d65 6173 7572 656d 656e  meter measuremen
-0002c1c0: 745f 7479 7065 206d 7573 7420 6265 206f  t_type must be o
-0002c1d0: 6620 7479 7065 2027 202b 2073 7472 2865  f type ' + str(e
-0002c1e0: 6e75 6d73 2e50 504d 554d 6561 7375 7265  nums.PPMUMeasure
-0002c1f0: 6d65 6e74 5479 7065 2929 0a20 2020 2020  mentType)).     
-0002c200: 2020 206d 6561 7375 7265 6d65 6e74 7320     measurements 
-0002c210: 3d20 7365 6c66 2e5f 696e 7465 7270 7265  = self._interpre
-0002c220: 7465 722e 7070 6d75 5f6d 6561 7375 7265  ter.ppmu_measure
-0002c230: 2873 656c 662e 5f72 6570 6561 7465 645f  (self._repeated_
-0002c240: 6361 7061 6269 6c69 7479 2c20 6d65 6173  capability, meas
-0002c250: 7572 656d 656e 745f 7479 7065 290a 2020  urement_type).  
-0002c260: 2020 2020 2020 7265 7475 726e 206d 6561        return mea
-0002c270: 7375 7265 6d65 6e74 730a 0a20 2020 2040  surements..    @
-0002c280: 6976 695f 7379 6e63 6872 6f6e 697a 6564  ivi_synchronized
-0002c290: 0a20 2020 2064 6566 2070 706d 755f 736f  .    def ppmu_so
-0002c2a0: 7572 6365 2873 656c 6629 3a0a 2020 2020  urce(self):.    
-0002c2b0: 2020 2020 7227 2727 7070 6d75 5f73 6f75      r'''ppmu_sou
-0002c2c0: 7263 650a 0a20 2020 2020 2020 2053 7461  rce..        Sta
-0002c2d0: 7274 7320 736f 7572 6369 6e67 2076 6f6c  rts sourcing vol
-0002c2e0: 7461 6765 206f 7220 6375 7272 656e 7420  tage or current 
-0002c2f0: 6672 6f6d 2074 6865 2050 504d 552e 2054  from the PPMU. T
-0002c300: 6869 7320 6d65 7468 6f64 2061 7574 6f6d  his method autom
-0002c310: 6174 6963 616c 6c79 2073 656c 6563 7473  atically selects
-0002c320: 2074 6865 2050 504d 5520 6d65 7468 6f64   the PPMU method
-0002c330: 2e20 4368 616e 6765 7320 746f 2050 504d  . Changes to PPM
-0002c340: 5520 736f 7572 6365 2073 6574 7469 6e67  U source setting
-0002c350: 7320 646f 206e 6f74 2074 616b 6520 6566  s do not take ef
-0002c360: 6665 6374 2075 6e74 696c 2079 6f75 2063  fect until you c
-0002c370: 616c 6c20 7468 6973 206d 6574 686f 642e  all this method.
-0002c380: 2049 6620 796f 7520 6d6f 6469 6679 2073   If you modify s
-0002c390: 6f75 7263 6520 7365 7474 696e 6773 2061  ource settings a
-0002c3a0: 6674 6572 2079 6f75 2063 616c 6c20 7468  fter you call th
-0002c3b0: 6973 206d 6574 686f 642c 2079 6f75 206d  is method, you m
-0002c3c0: 7573 7420 6361 6c6c 2074 6869 7320 6d65  ust call this me
-0002c3d0: 7468 6f64 2061 6761 696e 2066 6f72 2063  thod again for c
-0002c3e0: 6861 6e67 6573 2069 6e20 7468 6520 636f  hanges in the co
-0002c3f0: 6e66 6967 7572 6174 696f 6e20 746f 2074  nfiguration to t
-0002c400: 616b 6520 6566 6665 6374 2e0a 0a20 2020  ake effect...   
-0002c410: 2020 2020 2054 6970 3a0a 2020 2020 2020       Tip:.      
-0002c420: 2020 5468 6973 206d 6574 686f 6420 6361    This method ca
-0002c430: 6e20 6265 2063 616c 6c65 6420 6f6e 2073  n be called on s
-0002c440: 7065 6369 6669 6320 6368 616e 6e65 6c73  pecific channels
-0002c450: 2077 6974 6869 6e20 796f 7572 203a 7079   within your :py
-0002c460: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
-0002c470: 6c2e 5365 7373 696f 6e60 2069 6e73 7461  l.Session` insta
-0002c480: 6e63 652e 0a20 2020 2020 2020 2055 7365  nce..        Use
-0002c490: 2050 7974 686f 6e20 696e 6465 7820 6e6f   Python index no
-0002c4a0: 7461 7469 6f6e 206f 6e20 7468 6520 7265  tation on the re
-0002c4b0: 7065 6174 6564 2063 6170 6162 696c 6974  peated capabilit
-0002c4c0: 6965 7320 636f 6e74 6169 6e65 7220 6368  ies container ch
-0002c4d0: 616e 6e65 6c73 2074 6f20 7370 6563 6966  annels to specif
-0002c4e0: 7920 6120 7375 6273 6574 2c0a 2020 2020  y a subset,.    
-0002c4f0: 2020 2020 616e 6420 7468 656e 2063 616c      and then cal
-0002c500: 6c20 7468 6973 206d 6574 686f 6420 6f6e  l this method on
-0002c510: 2074 6865 2072 6573 756c 742e 0a0a 2020   the result...  
-0002c520: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
-0002c530: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
-0002c540: 696f 6e2e 6368 616e 6e65 6c73 5b20 2e2e  ion.channels[ ..
-0002c550: 2e20 5d2e 7070 6d75 5f73 6f75 7263 6560  . ].ppmu_source`
-0002c560: 0a0a 2020 2020 2020 2020 546f 2063 616c  ..        To cal
-0002c570: 6c20 7468 6520 6d65 7468 6f64 206f 6e20  l the method on 
-0002c580: 616c 6c20 6368 616e 6e65 6c73 2c20 796f  all channels, yo
-0002c590: 7520 6361 6e20 6361 6c6c 2069 7420 6469  u can call it di
-0002c5a0: 7265 6374 6c79 206f 6e20 7468 6520 3a70  rectly on the :p
-0002c5b0: 793a 636c 6173 733a 606e 6964 6967 6974  y:class:`nidigit
-0002c5c0: 616c 2e53 6573 7369 6f6e 602e 0a0a 2020  al.Session`...  
-0002c5d0: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
-0002c5e0: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
-0002c5f0: 696f 6e2e 7070 6d75 5f73 6f75 7263 6560  ion.ppmu_source`
-0002c600: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0002c610: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
-0002c620: 7072 6574 6572 2e70 706d 755f 736f 7572  preter.ppmu_sour
-0002c630: 6365 2873 656c 662e 5f72 6570 6561 7465  ce(self._repeate
-0002c640: 645f 6361 7061 6269 6c69 7479 290a 0a20  d_capability).. 
-0002c650: 2020 2040 6976 695f 7379 6e63 6872 6f6e     @ivi_synchron
-0002c660: 697a 6564 0a20 2020 2064 6566 2072 6561  ized.    def rea
-0002c670: 645f 7374 6174 6963 2873 656c 6629 3a0a  d_static(self):.
-0002c680: 2020 2020 2020 2020 7227 2727 7265 6164          r'''read
-0002c690: 5f73 7461 7469 630a 0a20 2020 2020 2020  _static..       
-0002c6a0: 2052 6561 6473 2074 6865 2063 7572 7265   Reads the curre
-0002c6b0: 6e74 2073 7461 7465 206f 6620 636f 6d70  nt state of comp
-0002c6c0: 6172 6174 6f72 7320 666f 7220 7069 6e73  arators for pins
-0002c6d0: 2079 6f75 2073 7065 6369 6679 2069 6e20   you specify in 
-0002c6e0: 7468 6520 7265 7065 6174 6564 2063 6170  the repeated cap
-0002c6f0: 6162 696c 6974 6965 732e 2049 6620 7468  abilities. If th
-0002c700: 6572 6520 6172 6520 756e 636f 6d6d 6974  ere are uncommit
-0002c710: 7465 6420 6368 616e 6765 7320 746f 206c  ted changes to l
-0002c720: 6576 656c 7320 6f72 2074 6865 2074 6572  evels or the ter
-0002c730: 6d69 6e61 7469 6f6e 206d 6f64 652c 2074  mination mode, t
-0002c740: 6869 7320 6d65 7468 6f64 2063 6f6d 6d69  his method commi
-0002c750: 7473 2074 6865 2063 6861 6e67 6573 2074  ts the changes t
-0002c760: 6f20 7468 6520 7069 6e73 2e0a 0a20 2020  o the pins...   
-0002c770: 2020 2020 2054 6970 3a0a 2020 2020 2020       Tip:.      
-0002c780: 2020 5468 6973 206d 6574 686f 6420 6361    This method ca
-0002c790: 6e20 6265 2063 616c 6c65 6420 6f6e 2073  n be called on s
-0002c7a0: 7065 6369 6669 6320 6368 616e 6e65 6c73  pecific channels
-0002c7b0: 2077 6974 6869 6e20 796f 7572 203a 7079   within your :py
-0002c7c0: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
-0002c7d0: 6c2e 5365 7373 696f 6e60 2069 6e73 7461  l.Session` insta
-0002c7e0: 6e63 652e 0a20 2020 2020 2020 2055 7365  nce..        Use
-0002c7f0: 2050 7974 686f 6e20 696e 6465 7820 6e6f   Python index no
-0002c800: 7461 7469 6f6e 206f 6e20 7468 6520 7265  tation on the re
-0002c810: 7065 6174 6564 2063 6170 6162 696c 6974  peated capabilit
-0002c820: 6965 7320 636f 6e74 6169 6e65 7220 6368  ies container ch
-0002c830: 616e 6e65 6c73 2074 6f20 7370 6563 6966  annels to specif
-0002c840: 7920 6120 7375 6273 6574 2c0a 2020 2020  y a subset,.    
-0002c850: 2020 2020 616e 6420 7468 656e 2063 616c      and then cal
-0002c860: 6c20 7468 6973 206d 6574 686f 6420 6f6e  l this method on
-0002c870: 2074 6865 2072 6573 756c 742e 0a0a 2020   the result...  
-0002c880: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
-0002c890: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
-0002c8a0: 696f 6e2e 6368 616e 6e65 6c73 5b20 2e2e  ion.channels[ ..
-0002c8b0: 2e20 5d2e 7265 6164 5f73 7461 7469 6360  . ].read_static`
-0002c8c0: 0a0a 2020 2020 2020 2020 546f 2063 616c  ..        To cal
-0002c8d0: 6c20 7468 6520 6d65 7468 6f64 206f 6e20  l the method on 
-0002c8e0: 616c 6c20 6368 616e 6e65 6c73 2c20 796f  all channels, yo
-0002c8f0: 7520 6361 6e20 6361 6c6c 2069 7420 6469  u can call it di
-0002c900: 7265 6374 6c79 206f 6e20 7468 6520 3a70  rectly on the :p
-0002c910: 793a 636c 6173 733a 606e 6964 6967 6974  y:class:`nidigit
-0002c920: 616c 2e53 6573 7369 6f6e 602e 0a0a 2020  al.Session`...  
-0002c930: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
-0002c940: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
-0002c950: 696f 6e2e 7265 6164 5f73 7461 7469 6360  ion.read_static`
-0002c960: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0002c970: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
-0002c980: 6174 6120 286c 6973 7420 6f66 2065 6e75  ata (list of enu
-0002c990: 6d73 2e50 696e 5374 6174 6529 3a20 5468  ms.PinState): Th
-0002c9a0: 6520 7265 7475 726e 6564 2061 7272 6179  e returned array
-0002c9b0: 206f 6620 7069 6e20 7374 6174 6573 2072   of pin states r
-0002c9c0: 6561 6420 6672 6f6d 2074 6865 2063 6861  ead from the cha
-0002c9d0: 6e6e 656c 7320 696e 2074 6865 2072 6570  nnels in the rep
-0002c9e0: 6561 7465 6420 6361 7061 6269 6c69 7469  eated capabiliti
-0002c9f0: 6573 2e20 4461 7461 2069 7320 7265 7475  es. Data is retu
-0002ca00: 726e 6564 2069 6e20 7468 6520 6f72 6465  rned in the orde
-0002ca10: 7220 796f 7520 7370 6563 6966 7920 696e  r you specify in
-0002ca20: 2074 6865 2072 6570 6561 7465 6420 6361   the repeated ca
-0002ca30: 7061 6269 6c69 7469 6573 2e20 4966 2061  pabilities. If a
-0002ca40: 2073 6974 6520 6973 2064 6973 6162 6c65   site is disable
-0002ca50: 642c 2074 6865 206d 6574 686f 6420 646f  d, the method do
-0002ca60: 6573 206e 6f74 2072 6574 7572 6e20 6461  es not return da
-0002ca70: 7461 2066 6f72 2074 6861 7420 7369 7465  ta for that site
-0002ca80: 2e20 596f 7520 6361 6e20 616c 736f 2075  . You can also u
-0002ca90: 7365 2074 6865 2067 6574 5f70 696e 5f72  se the get_pin_r
-0002caa0: 6573 756c 7473 5f70 696e 5f69 6e66 6f72  esults_pin_infor
-0002cab0: 6d61 7469 6f6e 206d 6574 686f 6420 746f  mation method to
-0002cac0: 206f 6274 6169 6e20 6120 736f 7274 6564   obtain a sorted
-0002cad0: 206c 6973 7420 6f66 2072 6574 7572 6e65   list of returne
-0002cae0: 6420 7369 7465 7320 616e 6420 6368 616e  d sites and chan
-0002caf0: 6e65 6c73 2e0a 0a20 2020 2020 2020 2020  nels...         
-0002cb00: 2020 2020 2020 202d 2020 2050 696e 5374         -   PinSt
-0002cb10: 6174 652e 4c3a 2054 6865 2063 6f6d 7061  ate.L: The compa
-0002cb20: 7261 746f 7273 2072 6561 6420 6120 6c6f  rators read a lo
-0002cb30: 6769 6320 6c6f 7720 7069 6e20 7374 6174  gic low pin stat
-0002cb40: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
-0002cb50: 2020 202d 2020 2050 696e 5374 6174 652e     -   PinState.
-0002cb60: 483a 2054 6865 2063 6f6d 7061 7261 746f  H: The comparato
-0002cb70: 7273 2072 6561 6420 6120 6c6f 6769 6320  rs read a logic 
-0002cb80: 6869 6768 2070 696e 2073 7461 7465 2e0a  high pin state..
-0002cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002cba0: 2d20 2020 5069 6e53 7461 7465 2e4d 3a20  -   PinState.M: 
-0002cbb0: 5468 6520 636f 6d70 6172 6174 6f72 7320  The comparators 
-0002cbc0: 7265 6164 2061 206d 6964 6261 6e64 2070  read a midband p
-0002cbd0: 696e 2073 7461 7465 2e0a 2020 2020 2020  in state..      
-0002cbe0: 2020 2020 2020 2020 2020 2d20 2020 5069            -   Pi
-0002cbf0: 6e53 7461 7465 2e56 3a20 5468 6520 636f  nState.V: The co
-0002cc00: 6d70 6172 6174 6f72 7320 7265 6164 2061  mparators read a
-0002cc10: 2076 616c 7565 2074 6861 7420 6973 2061   value that is a
-0002cc20: 626f 7665 2056 4f48 2061 6e64 2062 656c  bove VOH and bel
-0002cc30: 6f77 2056 4f4c 2c20 7768 6963 6820 6361  ow VOL, which ca
-0002cc40: 6e20 6f63 6375 7220 7768 656e 2079 6f75  n occur when you
-0002cc50: 2073 6574 2056 4f4c 2068 6967 6865 7220   set VOL higher 
-0002cc60: 7468 616e 2056 4f48 2e0a 0a20 2020 2020  than VOH...     
-0002cc70: 2020 2027 2727 0a20 2020 2020 2020 2064     '''.        d
-0002cc80: 6174 6120 3d20 7365 6c66 2e5f 696e 7465  ata = self._inte
-0002cc90: 7270 7265 7465 722e 7265 6164 5f73 7461  rpreter.read_sta
-0002cca0: 7469 6328 7365 6c66 2e5f 7265 7065 6174  tic(self._repeat
-0002ccb0: 6564 5f63 6170 6162 696c 6974 7929 0a20  ed_capability). 
-0002ccc0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-0002ccd0: 7461 0a0a 2020 2020 4069 7669 5f73 796e  ta..    @ivi_syn
-0002cce0: 6368 726f 6e69 7a65 640a 2020 2020 6465  chronized.    de
-0002ccf0: 6620 5f73 6574 5f61 7474 7269 6275 7465  f _set_attribute
-0002cd00: 5f76 695f 626f 6f6c 6561 6e28 7365 6c66  _vi_boolean(self
-0002cd10: 2c20 6174 7472 6962 7574 652c 2076 616c  , attribute, val
-0002cd20: 7565 293a 0a20 2020 2020 2020 2072 2727  ue):.        r''
-0002cd30: 275f 7365 745f 6174 7472 6962 7574 655f  '_set_attribute_
-0002cd40: 7669 5f62 6f6f 6c65 616e 0a0a 2020 2020  vi_boolean..    
-0002cd50: 2020 2020 5365 7473 2074 6865 2076 616c      Sets the val
-0002cd60: 7565 206f 6620 6120 5669 426f 6f6c 6561  ue of a ViBoolea
-0002cd70: 6e20 7072 6f70 6572 7479 2e20 5573 6520  n property. Use 
-0002cd80: 7468 6973 206d 6574 686f 6420 746f 2073  this method to s
-0002cd90: 6574 2074 6865 2076 616c 7565 7320 6f66  et the values of
-0002cda0: 2064 6967 6974 616c 2070 6174 7465 726e   digital pattern
-0002cdb0: 2069 6e73 7472 756d 656e 742d 7370 6563   instrument-spec
-0002cdc0: 6966 6963 2070 726f 7065 7274 6965 7320  ific properties 
-0002cdd0: 616e 6420 696e 6865 7265 6e74 2049 5649  and inherent IVI
-0002cde0: 2070 726f 7065 7274 6965 732e 0a0a 2020   properties...  
-0002cdf0: 2020 2020 2020 5469 703a 0a20 2020 2020        Tip:.     
-0002ce00: 2020 2054 6869 7320 6d65 7468 6f64 2063     This method c
-0002ce10: 616e 2062 6520 6361 6c6c 6564 206f 6e20  an be called on 
-0002ce20: 7370 6563 6966 6963 2063 6861 6e6e 656c  specific channel
-0002ce30: 7320 7769 7468 696e 2079 6f75 7220 3a70  s within your :p
-0002ce40: 793a 636c 6173 733a 606e 6964 6967 6974  y:class:`nidigit
-0002ce50: 616c 2e53 6573 7369 6f6e 6020 696e 7374  al.Session` inst
-0002ce60: 616e 6365 2e0a 2020 2020 2020 2020 5573  ance..        Us
-0002ce70: 6520 5079 7468 6f6e 2069 6e64 6578 206e  e Python index n
-0002ce80: 6f74 6174 696f 6e20 6f6e 2074 6865 2072  otation on the r
-0002ce90: 6570 6561 7465 6420 6361 7061 6269 6c69  epeated capabili
-0002cea0: 7469 6573 2063 6f6e 7461 696e 6572 2063  ties container c
-0002ceb0: 6861 6e6e 656c 7320 746f 2073 7065 6369  hannels to speci
-0002cec0: 6679 2061 2073 7562 7365 742c 0a20 2020  fy a subset,.   
-0002ced0: 2020 2020 2061 6e64 2074 6865 6e20 6361       and then ca
-0002cee0: 6c6c 2074 6869 7320 6d65 7468 6f64 206f  ll this method o
-0002cef0: 6e20 7468 6520 7265 7375 6c74 2e0a 0a20  n the result... 
-0002cf00: 2020 2020 2020 2045 7861 6d70 6c65 3a20         Example: 
-0002cf10: 3a70 793a 6d65 7468 3a60 6d79 5f73 6573  :py:meth:`my_ses
-0002cf20: 7369 6f6e 2e63 6861 6e6e 656c 735b 202e  sion.channels[ .
-0002cf30: 2e2e 205d 2e5f 7365 745f 6174 7472 6962  .. ]._set_attrib
-0002cf40: 7574 655f 7669 5f62 6f6f 6c65 616e 600a  ute_vi_boolean`.
-0002cf50: 0a20 2020 2020 2020 2054 6f20 6361 6c6c  .        To call
-0002cf60: 2074 6865 206d 6574 686f 6420 6f6e 2061   the method on a
-0002cf70: 6c6c 2063 6861 6e6e 656c 732c 2079 6f75  ll channels, you
-0002cf80: 2063 616e 2063 616c 6c20 6974 2064 6972   can call it dir
-0002cf90: 6563 746c 7920 6f6e 2074 6865 203a 7079  ectly on the :py
-0002cfa0: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
-0002cfb0: 6c2e 5365 7373 696f 6e60 2e0a 0a20 2020  l.Session`...   
-0002cfc0: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
-0002cfd0: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
-0002cfe0: 6f6e 2e5f 7365 745f 6174 7472 6962 7574  on._set_attribut
-0002cff0: 655f 7669 5f62 6f6f 6c65 616e 600a 0a20  e_vi_boolean`.. 
-0002d000: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0002d010: 2020 2020 2020 2020 2061 7474 7269 6275           attribu
-0002d020: 7465 2028 696e 7429 3a20 5468 6520 4944  te (int): The ID
-0002d030: 206f 6620 6120 7072 6f70 6572 7479 2e0a   of a property..
-0002d040: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-0002d050: 7565 2028 626f 6f6c 293a 2054 6865 2076  ue (bool): The v
-0002d060: 616c 7565 2074 6f20 7768 6963 6820 796f  alue to which yo
-0002d070: 7520 7761 6e74 2074 6f20 7365 7420 7468  u want to set th
-0002d080: 6520 7072 6f70 6572 7479 3b20 736f 6d65  e property; some
-0002d090: 206f 6620 7468 6520 7661 6c75 6573 206d   of the values m
-0002d0a0: 6967 6874 206e 6f74 2062 6520 7661 6c69  ight not be vali
-0002d0b0: 6420 6465 7065 6e64 696e 6720 6f6e 2074  d depending on t
-0002d0c0: 6865 2063 7572 7265 6e74 2073 6574 7469  he current setti
-0002d0d0: 6e67 7320 6f66 2074 6865 2069 6e73 7472  ngs of the instr
-0002d0e0: 756d 656e 7420 7365 7373 696f 6e2e 0a0a  ument session...
-0002d0f0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0002d100: 2020 2020 7365 6c66 2e5f 696e 7465 7270      self._interp
-0002d110: 7265 7465 722e 7365 745f 6174 7472 6962  reter.set_attrib
-0002d120: 7574 655f 7669 5f62 6f6f 6c65 616e 2873  ute_vi_boolean(s
-0002d130: 656c 662e 5f72 6570 6561 7465 645f 6361  elf._repeated_ca
-0002d140: 7061 6269 6c69 7479 2c20 6174 7472 6962  pability, attrib
-0002d150: 7574 652c 2076 616c 7565 290a 0a20 2020  ute, value)..   
-0002d160: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
-0002d170: 6564 0a20 2020 2064 6566 205f 7365 745f  ed.    def _set_
-0002d180: 6174 7472 6962 7574 655f 7669 5f69 6e74  attribute_vi_int
-0002d190: 3332 2873 656c 662c 2061 7474 7269 6275  32(self, attribu
-0002d1a0: 7465 2c20 7661 6c75 6529 3a0a 2020 2020  te, value):.    
-0002d1b0: 2020 2020 7227 2727 5f73 6574 5f61 7474      r'''_set_att
-0002d1c0: 7269 6275 7465 5f76 695f 696e 7433 320a  ribute_vi_int32.
-0002d1d0: 0a20 2020 2020 2020 2053 6574 7320 7468  .        Sets th
-0002d1e0: 6520 7661 6c75 6520 6f66 2061 2056 6949  e value of a ViI
-0002d1f0: 6e74 3332 2070 726f 7065 7274 792e 2055  nt32 property. U
-0002d200: 7365 2074 6869 7320 6d65 7468 6f64 2074  se this method t
-0002d210: 6f20 7365 7420 7468 6520 7661 6c75 6573  o set the values
-0002d220: 206f 6620 6469 6769 7461 6c20 7061 7474   of digital patt
-0002d230: 6572 6e20 696e 7374 7275 6d65 6e74 2d73  ern instrument-s
-0002d240: 7065 6369 6669 6320 7072 6f70 6572 7469  pecific properti
-0002d250: 6573 2061 6e64 2069 6e68 6572 656e 7420  es and inherent 
-0002d260: 4956 4920 7072 6f70 6572 7469 6573 2e0a  IVI properties..
-0002d270: 0a20 2020 2020 2020 2054 6970 3a0a 2020  .        Tip:.  
-0002d280: 2020 2020 2020 5468 6973 206d 6574 686f        This metho
-0002d290: 6420 6361 6e20 6265 2063 616c 6c65 6420  d can be called 
-0002d2a0: 6f6e 2073 7065 6369 6669 6320 6368 616e  on specific chan
-0002d2b0: 6e65 6c73 2077 6974 6869 6e20 796f 7572  nels within your
-0002d2c0: 203a 7079 3a63 6c61 7373 3a60 6e69 6469   :py:class:`nidi
-0002d2d0: 6769 7461 6c2e 5365 7373 696f 6e60 2069  gital.Session` i
-0002d2e0: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
-0002d2f0: 2055 7365 2050 7974 686f 6e20 696e 6465   Use Python inde
-0002d300: 7820 6e6f 7461 7469 6f6e 206f 6e20 7468  x notation on th
-0002d310: 6520 7265 7065 6174 6564 2063 6170 6162  e repeated capab
-0002d320: 696c 6974 6965 7320 636f 6e74 6169 6e65  ilities containe
-0002d330: 7220 6368 616e 6e65 6c73 2074 6f20 7370  r channels to sp
-0002d340: 6563 6966 7920 6120 7375 6273 6574 2c0a  ecify a subset,.
-0002d350: 2020 2020 2020 2020 616e 6420 7468 656e          and then
-0002d360: 2063 616c 6c20 7468 6973 206d 6574 686f   call this metho
-0002d370: 6420 6f6e 2074 6865 2072 6573 756c 742e  d on the result.
-0002d380: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-0002d390: 653a 203a 7079 3a6d 6574 683a 606d 795f  e: :py:meth:`my_
-0002d3a0: 7365 7373 696f 6e2e 6368 616e 6e65 6c73  session.channels
-0002d3b0: 5b20 2e2e 2e20 5d2e 5f73 6574 5f61 7474  [ ... ]._set_att
-0002d3c0: 7269 6275 7465 5f76 695f 696e 7433 3260  ribute_vi_int32`
-0002d3d0: 0a0a 2020 2020 2020 2020 546f 2063 616c  ..        To cal
-0002d3e0: 6c20 7468 6520 6d65 7468 6f64 206f 6e20  l the method on 
-0002d3f0: 616c 6c20 6368 616e 6e65 6c73 2c20 796f  all channels, yo
-0002d400: 7520 6361 6e20 6361 6c6c 2069 7420 6469  u can call it di
-0002d410: 7265 6374 6c79 206f 6e20 7468 6520 3a70  rectly on the :p
-0002d420: 793a 636c 6173 733a 606e 6964 6967 6974  y:class:`nidigit
-0002d430: 616c 2e53 6573 7369 6f6e 602e 0a0a 2020  al.Session`...  
-0002d440: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
-0002d450: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
-0002d460: 696f 6e2e 5f73 6574 5f61 7474 7269 6275  ion._set_attribu
-0002d470: 7465 5f76 695f 696e 7433 3260 0a0a 2020  te_vi_int32`..  
-0002d480: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0002d490: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
-0002d4a0: 6520 2869 6e74 293a 2054 6865 2049 4420  e (int): The ID 
-0002d4b0: 6f66 2061 2070 726f 7065 7274 792e 0a0a  of a property...
-0002d4c0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0002d4d0: 6520 2869 6e74 293a 2054 6865 2076 616c  e (int): The val
-0002d4e0: 7565 2074 6f20 7768 6963 6820 796f 7520  ue to which you 
-0002d4f0: 7761 6e74 2074 6f20 7365 7420 7468 6520  want to set the 
-0002d500: 7072 6f70 6572 7479 3b20 736f 6d65 206f  property; some o
-0002d510: 6620 7468 6520 7661 6c75 6573 206d 6967  f the values mig
-0002d520: 6874 206e 6f74 2062 6520 7661 6c69 6420  ht not be valid 
-0002d530: 6465 7065 6e64 696e 6720 6f6e 2074 6865  depending on the
-0002d540: 2063 7572 7265 6e74 2073 6574 7469 6e67   current setting
-0002d550: 7320 6f66 2074 6865 2069 6e73 7472 756d  s of the instrum
-0002d560: 656e 7420 7365 7373 696f 6e2e 0a0a 2020  ent session...  
-0002d570: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0002d580: 2020 7365 6c66 2e5f 696e 7465 7270 7265    self._interpre
-0002d590: 7465 722e 7365 745f 6174 7472 6962 7574  ter.set_attribut
-0002d5a0: 655f 7669 5f69 6e74 3332 2873 656c 662e  e_vi_int32(self.
-0002d5b0: 5f72 6570 6561 7465 645f 6361 7061 6269  _repeated_capabi
-0002d5c0: 6c69 7479 2c20 6174 7472 6962 7574 652c  lity, attribute,
-0002d5d0: 2076 616c 7565 290a 0a20 2020 2040 6976   value)..    @iv
-0002d5e0: 695f 7379 6e63 6872 6f6e 697a 6564 0a20  i_synchronized. 
-0002d5f0: 2020 2064 6566 205f 7365 745f 6174 7472     def _set_attr
-0002d600: 6962 7574 655f 7669 5f69 6e74 3634 2873  ibute_vi_int64(s
-0002d610: 656c 662c 2061 7474 7269 6275 7465 2c20  elf, attribute, 
-0002d620: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
-0002d630: 7227 2727 5f73 6574 5f61 7474 7269 6275  r'''_set_attribu
-0002d640: 7465 5f76 695f 696e 7436 340a 0a20 2020  te_vi_int64..   
-0002d650: 2020 2020 2053 6574 7320 7468 6520 7661       Sets the va
-0002d660: 6c75 6520 6f66 2061 2056 6949 6e74 3634  lue of a ViInt64
-0002d670: 2070 726f 7065 7274 792e 2055 7365 2074   property. Use t
-0002d680: 6869 7320 6d65 7468 6f64 2074 6f20 7365  his method to se
-0002d690: 7420 7468 6520 7661 6c75 6573 206f 6620  t the values of 
-0002d6a0: 6469 6769 7461 6c20 7061 7474 6572 6e20  digital pattern 
-0002d6b0: 696e 7374 7275 6d65 6e74 2d73 7065 6369  instrument-speci
-0002d6c0: 6669 6320 7072 6f70 6572 7469 6573 2061  fic properties a
-0002d6d0: 6e64 2069 6e68 6572 656e 7420 4956 4920  nd inherent IVI 
-0002d6e0: 7072 6f70 6572 7469 6573 2e0a 0a20 2020  properties...   
-0002d6f0: 2020 2020 2054 6970 3a0a 2020 2020 2020       Tip:.      
-0002d700: 2020 5468 6973 206d 6574 686f 6420 6361    This method ca
-0002d710: 6e20 6265 2063 616c 6c65 6420 6f6e 2073  n be called on s
-0002d720: 7065 6369 6669 6320 6368 616e 6e65 6c73  pecific channels
-0002d730: 2077 6974 6869 6e20 796f 7572 203a 7079   within your :py
-0002d740: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
-0002d750: 6c2e 5365 7373 696f 6e60 2069 6e73 7461  l.Session` insta
-0002d760: 6e63 652e 0a20 2020 2020 2020 2055 7365  nce..        Use
-0002d770: 2050 7974 686f 6e20 696e 6465 7820 6e6f   Python index no
-0002d780: 7461 7469 6f6e 206f 6e20 7468 6520 7265  tation on the re
-0002d790: 7065 6174 6564 2063 6170 6162 696c 6974  peated capabilit
-0002d7a0: 6965 7320 636f 6e74 6169 6e65 7220 6368  ies container ch
-0002d7b0: 616e 6e65 6c73 2074 6f20 7370 6563 6966  annels to specif
-0002d7c0: 7920 6120 7375 6273 6574 2c0a 2020 2020  y a subset,.    
-0002d7d0: 2020 2020 616e 6420 7468 656e 2063 616c      and then cal
-0002d7e0: 6c20 7468 6973 206d 6574 686f 6420 6f6e  l this method on
-0002d7f0: 2074 6865 2072 6573 756c 742e 0a0a 2020   the result...  
-0002d800: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
-0002d810: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
-0002d820: 696f 6e2e 6368 616e 6e65 6c73 5b20 2e2e  ion.channels[ ..
-0002d830: 2e20 5d2e 5f73 6574 5f61 7474 7269 6275  . ]._set_attribu
-0002d840: 7465 5f76 695f 696e 7436 3460 0a0a 2020  te_vi_int64`..  
-0002d850: 2020 2020 2020 546f 2063 616c 6c20 7468        To call th
-0002d860: 6520 6d65 7468 6f64 206f 6e20 616c 6c20  e method on all 
-0002d870: 6368 616e 6e65 6c73 2c20 796f 7520 6361  channels, you ca
-0002d880: 6e20 6361 6c6c 2069 7420 6469 7265 6374  n call it direct
-0002d890: 6c79 206f 6e20 7468 6520 3a70 793a 636c  ly on the :py:cl
-0002d8a0: 6173 733a 606e 6964 6967 6974 616c 2e53  ass:`nidigital.S
-0002d8b0: 6573 7369 6f6e 602e 0a0a 2020 2020 2020  ession`...      
-0002d8c0: 2020 4578 616d 706c 653a 203a 7079 3a6d    Example: :py:m
-0002d8d0: 6574 683a 606d 795f 7365 7373 696f 6e2e  eth:`my_session.
-0002d8e0: 5f73 6574 5f61 7474 7269 6275 7465 5f76  _set_attribute_v
-0002d8f0: 695f 696e 7436 3460 0a0a 2020 2020 2020  i_int64`..      
-0002d900: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0002d910: 2020 2020 6174 7472 6962 7574 6520 2869      attribute (i
-0002d920: 6e74 293a 2054 6865 2049 4420 6f66 2061  nt): The ID of a
-0002d930: 2070 726f 7065 7274 792e 0a0a 2020 2020   property...    
-0002d940: 2020 2020 2020 2020 7661 6c75 6520 2869          value (i
-0002d950: 6e74 293a 2054 6865 2076 616c 7565 2074  nt): The value t
-0002d960: 6f20 7768 6963 6820 796f 7520 7761 6e74  o which you want
-0002d970: 2074 6f20 7365 7420 7468 6520 7072 6f70   to set the prop
-0002d980: 6572 7479 3b20 736f 6d65 206f 6620 7468  erty; some of th
-0002d990: 6520 7661 6c75 6573 206d 6967 6874 206e  e values might n
-0002d9a0: 6f74 2062 6520 7661 6c69 6420 6465 7065  ot be valid depe
-0002d9b0: 6e64 696e 6720 6f6e 2074 6865 2063 7572  nding on the cur
-0002d9c0: 7265 6e74 2073 6574 7469 6e67 7320 6f66  rent settings of
-0002d9d0: 2074 6865 2069 6e73 7472 756d 656e 7420   the instrument 
-0002d9e0: 7365 7373 696f 6e2e 0a0a 2020 2020 2020  session...      
-0002d9f0: 2020 2727 270a 2020 2020 2020 2020 7365    '''.        se
-0002da00: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
-0002da10: 7365 745f 6174 7472 6962 7574 655f 7669  set_attribute_vi
-0002da20: 5f69 6e74 3634 2873 656c 662e 5f72 6570  _int64(self._rep
-0002da30: 6561 7465 645f 6361 7061 6269 6c69 7479  eated_capability
-0002da40: 2c20 6174 7472 6962 7574 652c 2076 616c  , attribute, val
-0002da50: 7565 290a 0a20 2020 2040 6976 695f 7379  ue)..    @ivi_sy
-0002da60: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
-0002da70: 6566 205f 7365 745f 6174 7472 6962 7574  ef _set_attribut
-0002da80: 655f 7669 5f72 6561 6c36 3428 7365 6c66  e_vi_real64(self
-0002da90: 2c20 6174 7472 6962 7574 652c 2076 616c  , attribute, val
-0002daa0: 7565 293a 0a20 2020 2020 2020 2072 2727  ue):.        r''
-0002dab0: 275f 7365 745f 6174 7472 6962 7574 655f  '_set_attribute_
-0002dac0: 7669 5f72 6561 6c36 340a 0a20 2020 2020  vi_real64..     
-0002dad0: 2020 2053 6574 7320 7468 6520 7661 6c75     Sets the valu
-0002dae0: 6520 6f66 2061 2056 6949 6e74 5265 616c  e of a ViIntReal
-0002daf0: 3634 2070 726f 7065 7274 792e 2055 7365  64 property. Use
-0002db00: 2074 6869 7320 6d65 7468 6f64 2074 6f20   this method to 
-0002db10: 7365 7420 7468 6520 7661 6c75 6573 206f  set the values o
-0002db20: 6620 6469 6769 7461 6c20 7061 7474 6572  f digital patter
-0002db30: 6e20 696e 7374 7275 6d65 6e74 2d73 7065  n instrument-spe
-0002db40: 6369 6669 6320 7072 6f70 6572 7469 6573  cific properties
-0002db50: 2061 6e64 2069 6e68 6572 656e 7420 4956   and inherent IV
-0002db60: 4920 7072 6f70 6572 7469 6573 2e0a 0a20  I properties... 
-0002db70: 2020 2020 2020 2054 6970 3a0a 2020 2020         Tip:.    
-0002db80: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
-0002db90: 6361 6e20 6265 2063 616c 6c65 6420 6f6e  can be called on
-0002dba0: 2073 7065 6369 6669 6320 6368 616e 6e65   specific channe
-0002dbb0: 6c73 2077 6974 6869 6e20 796f 7572 203a  ls within your :
-0002dbc0: 7079 3a63 6c61 7373 3a60 6e69 6469 6769  py:class:`nidigi
-0002dbd0: 7461 6c2e 5365 7373 696f 6e60 2069 6e73  tal.Session` ins
-0002dbe0: 7461 6e63 652e 0a20 2020 2020 2020 2055  tance..        U
-0002dbf0: 7365 2050 7974 686f 6e20 696e 6465 7820  se Python index 
-0002dc00: 6e6f 7461 7469 6f6e 206f 6e20 7468 6520  notation on the 
-0002dc10: 7265 7065 6174 6564 2063 6170 6162 696c  repeated capabil
-0002dc20: 6974 6965 7320 636f 6e74 6169 6e65 7220  ities container 
-0002dc30: 6368 616e 6e65 6c73 2074 6f20 7370 6563  channels to spec
-0002dc40: 6966 7920 6120 7375 6273 6574 2c0a 2020  ify a subset,.  
-0002dc50: 2020 2020 2020 616e 6420 7468 656e 2063        and then c
-0002dc60: 616c 6c20 7468 6973 206d 6574 686f 6420  all this method 
-0002dc70: 6f6e 2074 6865 2072 6573 756c 742e 0a0a  on the result...
-0002dc80: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
-0002dc90: 203a 7079 3a6d 6574 683a 606d 795f 7365   :py:meth:`my_se
-0002dca0: 7373 696f 6e2e 6368 616e 6e65 6c73 5b20  ssion.channels[ 
-0002dcb0: 2e2e 2e20 5d2e 5f73 6574 5f61 7474 7269  ... ]._set_attri
-0002dcc0: 6275 7465 5f76 695f 7265 616c 3634 600a  bute_vi_real64`.
-0002dcd0: 0a20 2020 2020 2020 2054 6f20 6361 6c6c  .        To call
-0002dce0: 2074 6865 206d 6574 686f 6420 6f6e 2061   the method on a
-0002dcf0: 6c6c 2063 6861 6e6e 656c 732c 2079 6f75  ll channels, you
-0002dd00: 2063 616e 2063 616c 6c20 6974 2064 6972   can call it dir
-0002dd10: 6563 746c 7920 6f6e 2074 6865 203a 7079  ectly on the :py
-0002dd20: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
-0002dd30: 6c2e 5365 7373 696f 6e60 2e0a 0a20 2020  l.Session`...   
-0002dd40: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
-0002dd50: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
-0002dd60: 6f6e 2e5f 7365 745f 6174 7472 6962 7574  on._set_attribut
-0002dd70: 655f 7669 5f72 6561 6c36 3460 0a0a 2020  e_vi_real64`..  
-0002dd80: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0002dd90: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
-0002dda0: 6520 2869 6e74 293a 2054 6865 2049 4420  e (int): The ID 
-0002ddb0: 6f66 2061 2070 726f 7065 7274 792e 0a0a  of a property...
-0002ddc0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0002ddd0: 6520 2866 6c6f 6174 293a 2054 6865 2076  e (float): The v
-0002dde0: 616c 7565 2074 6f20 7768 6963 6820 796f  alue to which yo
-0002ddf0: 7520 7761 6e74 2074 6f20 7365 7420 7468  u want to set th
-0002de00: 6520 7072 6f70 6572 7479 3b20 736f 6d65  e property; some
-0002de10: 206f 6620 7468 6520 7661 6c75 6573 206d   of the values m
-0002de20: 6967 6874 206e 6f74 2062 6520 7661 6c69  ight not be vali
-0002de30: 6420 6465 7065 6e64 696e 6720 6f6e 2074  d depending on t
-0002de40: 6865 2063 7572 7265 6e74 2073 6574 7469  he current setti
-0002de50: 6e67 7320 6f66 2074 6865 2069 6e73 7472  ngs of the instr
-0002de60: 756d 656e 7420 7365 7373 696f 6e2e 0a0a  ument session...
-0002de70: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-0002de80: 2020 2020 7365 6c66 2e5f 696e 7465 7270      self._interp
-0002de90: 7265 7465 722e 7365 745f 6174 7472 6962  reter.set_attrib
-0002dea0: 7574 655f 7669 5f72 6561 6c36 3428 7365  ute_vi_real64(se
-0002deb0: 6c66 2e5f 7265 7065 6174 6564 5f63 6170  lf._repeated_cap
-0002dec0: 6162 696c 6974 792c 2061 7474 7269 6275  ability, attribu
-0002ded0: 7465 2c20 7661 6c75 6529 0a0a 2020 2020  te, value)..    
-0002dee0: 4069 7669 5f73 796e 6368 726f 6e69 7a65  @ivi_synchronize
-0002def0: 640a 2020 2020 6465 6620 5f73 6574 5f61  d.    def _set_a
-0002df00: 7474 7269 6275 7465 5f76 695f 7374 7269  ttribute_vi_stri
-0002df10: 6e67 2873 656c 662c 2061 7474 7269 6275  ng(self, attribu
-0002df20: 7465 2c20 7661 6c75 6529 3a0a 2020 2020  te, value):.    
-0002df30: 2020 2020 7227 2727 5f73 6574 5f61 7474      r'''_set_att
-0002df40: 7269 6275 7465 5f76 695f 7374 7269 6e67  ribute_vi_string
-0002df50: 0a0a 2020 2020 2020 2020 5365 7473 2074  ..        Sets t
-0002df60: 6865 2076 616c 7565 206f 6620 6120 5669  he value of a Vi
-0002df70: 5374 7269 6e67 2070 726f 7065 7274 792e  String property.
-0002df80: 2055 7365 2074 6869 7320 6d65 7468 6f64   Use this method
-0002df90: 2074 6f20 7365 7420 7468 6520 7661 6c75   to set the valu
-0002dfa0: 6573 206f 6620 6469 6769 7461 6c20 7061  es of digital pa
-0002dfb0: 7474 6572 6e20 696e 7374 7275 6d65 6e74  ttern instrument
-0002dfc0: 2d73 7065 6369 6669 6320 7072 6f70 6572  -specific proper
-0002dfd0: 7469 6573 2061 6e64 2069 6e68 6572 656e  ties and inheren
-0002dfe0: 7420 4956 4920 7072 6f70 6572 7469 6573  t IVI properties
-0002dff0: 2e0a 0a20 2020 2020 2020 2054 6970 3a0a  ...        Tip:.
-0002e000: 2020 2020 2020 2020 5468 6973 206d 6574          This met
-0002e010: 686f 6420 6361 6e20 6265 2063 616c 6c65  hod can be calle
-0002e020: 6420 6f6e 2073 7065 6369 6669 6320 6368  d on specific ch
-0002e030: 616e 6e65 6c73 2077 6974 6869 6e20 796f  annels within yo
-0002e040: 7572 203a 7079 3a63 6c61 7373 3a60 6e69  ur :py:class:`ni
-0002e050: 6469 6769 7461 6c2e 5365 7373 696f 6e60  digital.Session`
-0002e060: 2069 6e73 7461 6e63 652e 0a20 2020 2020   instance..     
-0002e070: 2020 2055 7365 2050 7974 686f 6e20 696e     Use Python in
-0002e080: 6465 7820 6e6f 7461 7469 6f6e 206f 6e20  dex notation on 
-0002e090: 7468 6520 7265 7065 6174 6564 2063 6170  the repeated cap
-0002e0a0: 6162 696c 6974 6965 7320 636f 6e74 6169  abilities contai
-0002e0b0: 6e65 7220 6368 616e 6e65 6c73 2074 6f20  ner channels to 
-0002e0c0: 7370 6563 6966 7920 6120 7375 6273 6574  specify a subset
-0002e0d0: 2c0a 2020 2020 2020 2020 616e 6420 7468  ,.        and th
-0002e0e0: 656e 2063 616c 6c20 7468 6973 206d 6574  en call this met
-0002e0f0: 686f 6420 6f6e 2074 6865 2072 6573 756c  hod on the resul
-0002e100: 742e 0a0a 2020 2020 2020 2020 4578 616d  t...        Exam
-0002e110: 706c 653a 203a 7079 3a6d 6574 683a 606d  ple: :py:meth:`m
-0002e120: 795f 7365 7373 696f 6e2e 6368 616e 6e65  y_session.channe
-0002e130: 6c73 5b20 2e2e 2e20 5d2e 5f73 6574 5f61  ls[ ... ]._set_a
-0002e140: 7474 7269 6275 7465 5f76 695f 7374 7269  ttribute_vi_stri
-0002e150: 6e67 600a 0a20 2020 2020 2020 2054 6f20  ng`..        To 
-0002e160: 6361 6c6c 2074 6865 206d 6574 686f 6420  call the method 
-0002e170: 6f6e 2061 6c6c 2063 6861 6e6e 656c 732c  on all channels,
-0002e180: 2079 6f75 2063 616e 2063 616c 6c20 6974   you can call it
-0002e190: 2064 6972 6563 746c 7920 6f6e 2074 6865   directly on the
-0002e1a0: 203a 7079 3a63 6c61 7373 3a60 6e69 6469   :py:class:`nidi
-0002e1b0: 6769 7461 6c2e 5365 7373 696f 6e60 2e0a  gital.Session`..
-0002e1c0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-0002e1d0: 3a20 3a70 793a 6d65 7468 3a60 6d79 5f73  : :py:meth:`my_s
-0002e1e0: 6573 7369 6f6e 2e5f 7365 745f 6174 7472  ession._set_attr
-0002e1f0: 6962 7574 655f 7669 5f73 7472 696e 6760  ibute_vi_string`
-0002e200: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0002e210: 2020 2020 2020 2020 2020 2020 6174 7472              attr
-0002e220: 6962 7574 6520 2869 6e74 293a 2054 6865  ibute (int): The
-0002e230: 2049 4420 6f66 2061 2070 726f 7065 7274   ID of a propert
-0002e240: 792e 0a0a 2020 2020 2020 2020 2020 2020  y...            
-0002e250: 7661 6c75 6520 2873 7472 293a 2054 6865  value (str): The
-0002e260: 2076 616c 7565 2074 6f20 7768 6963 6820   value to which 
-0002e270: 796f 7520 7761 6e74 2074 6f20 7365 7420  you want to set 
-0002e280: 7468 6520 7072 6f70 6572 7479 3b20 736f  the property; so
-0002e290: 6d65 206f 6620 7468 6520 7661 6c75 6573  me of the values
-0002e2a0: 206d 6967 6874 206e 6f74 2062 6520 7661   might not be va
-0002e2b0: 6c69 6420 6465 7065 6e64 696e 6720 6f6e  lid depending on
-0002e2c0: 2074 6865 2063 7572 7265 6e74 2073 6574   the current set
-0002e2d0: 7469 6e67 7320 6f66 2074 6865 2069 6e73  tings of the ins
-0002e2e0: 7472 756d 656e 7420 7365 7373 696f 6e2e  trument session.
-0002e2f0: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-0002e300: 2020 2020 2020 7365 6c66 2e5f 696e 7465        self._inte
-0002e310: 7270 7265 7465 722e 7365 745f 6174 7472  rpreter.set_attr
-0002e320: 6962 7574 655f 7669 5f73 7472 696e 6728  ibute_vi_string(
-0002e330: 7365 6c66 2e5f 7265 7065 6174 6564 5f63  self._repeated_c
-0002e340: 6170 6162 696c 6974 792c 2061 7474 7269  apability, attri
-0002e350: 6275 7465 2c20 7661 6c75 6529 0a0a 2020  bute, value)..  
-0002e360: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
-0002e370: 7a65 640a 2020 2020 6465 6620 7464 7228  zed.    def tdr(
-0002e380: 7365 6c66 2c20 6170 706c 795f 6f66 6673  self, apply_offs
-0002e390: 6574 733d 5472 7565 293a 0a20 2020 2020  ets=True):.     
-0002e3a0: 2020 2072 2727 2774 6472 0a0a 2020 2020     r'''tdr..    
-0002e3b0: 2020 2020 4d65 6173 7572 6573 2070 726f      Measures pro
-0002e3c0: 7061 6761 7469 6f6e 2064 656c 6179 7320  pagation delays 
-0002e3d0: 7468 726f 7567 6820 6361 626c 6573 2c20  through cables, 
-0002e3e0: 636f 6e6e 6563 746f 7273 2c20 616e 6420  connectors, and 
-0002e3f0: 6c6f 6164 2062 6f61 7264 7320 7573 696e  load boards usin
-0002e400: 6720 5469 6d65 2d44 6f6d 6169 6e20 5265  g Time-Domain Re
-0002e410: 666c 6563 746f 6d65 7472 7920 2854 4452  flectometry (TDR
-0002e420: 292e 2045 6e73 7572 6520 7468 6174 2074  ). Ensure that t
-0002e430: 6865 2063 6861 6e6e 656c 7320 616e 6420  he channels and 
-0002e440: 7069 6e73 2079 6f75 2073 656c 6563 7420  pins you select 
-0002e450: 6172 6520 636f 6e6e 6563 7465 6420 746f  are connected to
-0002e460: 2061 6e20 6f70 656e 2063 6972 6375 6974   an open circuit
-0002e470: 2e0a 0a20 2020 2020 2020 2054 6970 3a0a  ...        Tip:.
-0002e480: 2020 2020 2020 2020 5468 6973 206d 6574          This met
-0002e490: 686f 6420 6361 6e20 6265 2063 616c 6c65  hod can be calle
-0002e4a0: 6420 6f6e 2073 7065 6369 6669 6320 6368  d on specific ch
-0002e4b0: 616e 6e65 6c73 2077 6974 6869 6e20 796f  annels within yo
-0002e4c0: 7572 203a 7079 3a63 6c61 7373 3a60 6e69  ur :py:class:`ni
-0002e4d0: 6469 6769 7461 6c2e 5365 7373 696f 6e60  digital.Session`
-0002e4e0: 2069 6e73 7461 6e63 652e 0a20 2020 2020   instance..     
-0002e4f0: 2020 2055 7365 2050 7974 686f 6e20 696e     Use Python in
-0002e500: 6465 7820 6e6f 7461 7469 6f6e 206f 6e20  dex notation on 
-0002e510: 7468 6520 7265 7065 6174 6564 2063 6170  the repeated cap
-0002e520: 6162 696c 6974 6965 7320 636f 6e74 6169  abilities contai
-0002e530: 6e65 7220 6368 616e 6e65 6c73 2074 6f20  ner channels to 
-0002e540: 7370 6563 6966 7920 6120 7375 6273 6574  specify a subset
-0002e550: 2c0a 2020 2020 2020 2020 616e 6420 7468  ,.        and th
-0002e560: 656e 2063 616c 6c20 7468 6973 206d 6574  en call this met
-0002e570: 686f 6420 6f6e 2074 6865 2072 6573 756c  hod on the resul
-0002e580: 742e 0a0a 2020 2020 2020 2020 4578 616d  t...        Exam
-0002e590: 706c 653a 203a 7079 3a6d 6574 683a 606d  ple: :py:meth:`m
-0002e5a0: 795f 7365 7373 696f 6e2e 6368 616e 6e65  y_session.channe
-0002e5b0: 6c73 5b20 2e2e 2e20 5d2e 7464 7260 0a0a  ls[ ... ].tdr`..
-0002e5c0: 2020 2020 2020 2020 546f 2063 616c 6c20          To call 
-0002e5d0: 7468 6520 6d65 7468 6f64 206f 6e20 616c  the method on al
-0002e5e0: 6c20 6368 616e 6e65 6c73 2c20 796f 7520  l channels, you 
-0002e5f0: 6361 6e20 6361 6c6c 2069 7420 6469 7265  can call it dire
-0002e600: 6374 6c79 206f 6e20 7468 6520 3a70 793a  ctly on the :py:
-0002e610: 636c 6173 733a 606e 6964 6967 6974 616c  class:`nidigital
-0002e620: 2e53 6573 7369 6f6e 602e 0a0a 2020 2020  .Session`...    
-0002e630: 2020 2020 4578 616d 706c 653a 203a 7079      Example: :py
-0002e640: 3a6d 6574 683a 606d 795f 7365 7373 696f  :meth:`my_sessio
-0002e650: 6e2e 7464 7260 0a0a 2020 2020 2020 2020  n.tdr`..        
-0002e660: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0002e670: 2020 6170 706c 795f 6f66 6673 6574 7320    apply_offsets 
-0002e680: 2862 6f6f 6c29 3a20 4120 426f 6f6c 6561  (bool): A Boolea
-0002e690: 6e20 7468 6174 2073 7065 6369 6669 6573  n that specifies
-0002e6a0: 2077 6865 7468 6572 2074 6f20 6170 706c   whether to appl
-0002e6b0: 7920 7468 6520 6d65 6173 7572 6564 2054  y the measured T
-0002e6c0: 4452 206f 6666 7365 7473 2e20 4966 2079  DR offsets. If y
-0002e6d0: 6f75 206e 6565 6420 746f 2061 646a 7573  ou need to adjus
-0002e6e0: 7420 7468 6520 6d65 6173 7572 6564 206f  t the measured o
-0002e6f0: 6666 7365 7473 2070 7269 6f72 2074 6f20  ffsets prior to 
-0002e700: 6170 706c 7969 6e67 2c20 7365 7420 7468  applying, set th
-0002e710: 6973 2069 6e70 7574 2074 6f20 4661 6c73  is input to Fals
-0002e720: 652c 2061 6e64 2063 616c 6c20 7468 6520  e, and call the 
-0002e730: 6170 706c 795f 7464 725f 6f66 6673 6574  apply_tdr_offset
-0002e740: 7320 6d65 7468 6f64 2074 6f20 7370 6563  s method to spec
-0002e750: 6966 7920 7468 6520 6164 6a75 7374 6564  ify the adjusted
-0002e760: 2054 4452 206f 6666 7365 7473 2076 616c   TDR offsets val
-0002e770: 7565 732e 0a0a 0a20 2020 2020 2020 2052  ues....        R
-0002e780: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0002e790: 2020 2020 6f66 6673 6574 7320 286c 6973      offsets (lis
-0002e7a0: 7420 6f66 2068 6967 6874 696d 652e 7469  t of hightime.ti
-0002e7b0: 6d65 6465 6c74 6129 3a20 4d65 6173 7572  medelta): Measur
-0002e7c0: 6564 2054 4452 206f 6666 7365 7473 2073  ed TDR offsets s
-0002e7d0: 7065 6369 6669 6564 2069 6e20 7365 636f  pecified in seco
-0002e7e0: 6e64 732e 0a0a 2020 2020 2020 2020 2727  nds...        ''
-0002e7f0: 270a 2020 2020 2020 2020 6f66 6673 6574  '.        offset
-0002e800: 7320 3d20 7365 6c66 2e5f 696e 7465 7270  s = self._interp
-0002e810: 7265 7465 722e 7464 7228 7365 6c66 2e5f  reter.tdr(self._
-0002e820: 7265 7065 6174 6564 5f63 6170 6162 696c  repeated_capabil
-0002e830: 6974 792c 2061 7070 6c79 5f6f 6666 7365  ity, apply_offse
-0002e840: 7473 290a 2020 2020 2020 2020 7265 7475  ts).        retu
-0002e850: 726e 205f 636f 6e76 6572 7465 7273 2e63  rn _converters.c
-0002e860: 6f6e 7665 7274 5f73 6563 6f6e 6473 5f72  onvert_seconds_r
-0002e870: 6561 6c36 345f 746f 5f74 696d 6564 656c  eal64_to_timedel
-0002e880: 7461 7328 6f66 6673 6574 7329 0a0a 2020  tas(offsets)..  
-0002e890: 2020 6465 6620 756e 6c6f 636b 2873 656c    def unlock(sel
-0002e8a0: 6629 3a0a 2020 2020 2020 2020 2727 2775  f):.        '''u
-0002e8b0: 6e6c 6f63 6b0a 0a20 2020 2020 2020 2052  nlock..        R
-0002e8c0: 656c 6561 7365 7320 6120 6c6f 636b 2074  eleases a lock t
-0002e8d0: 6861 7420 796f 7520 6163 7175 6972 6564  hat you acquired
-0002e8e0: 206f 6e20 616e 2064 6576 6963 6520 7365   on an device se
-0002e8f0: 7373 696f 6e20 7573 696e 670a 2020 2020  ssion using.    
-0002e900: 2020 2020 6c6f 636b 2e20 5265 6665 7220      lock. Refer 
-0002e910: 746f 206c 6f63 6b20 666f 7220 6164 6469  to lock for addi
-0002e920: 7469 6f6e 616c 0a20 2020 2020 2020 2069  tional.        i
-0002e930: 6e66 6f72 6d61 7469 6f6e 206f 6e20 7365  nformation on se
-0002e940: 7373 696f 6e20 6c6f 636b 732e 0a20 2020  ssion locks..   
-0002e950: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-0002e960: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
-0002e970: 6572 2e75 6e6c 6f63 6b28 290a 0a20 2020  er.unlock()..   
-0002e980: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
-0002e990: 6564 0a20 2020 2064 6566 205f 7772 6974  ed.    def _writ
-0002e9a0: 655f 736f 7572 6365 5f77 6176 6566 6f72  e_source_wavefor
-0002e9b0: 6d5f 7369 7465 5f75 6e69 7175 655f 7533  m_site_unique_u3
-0002e9c0: 3228 7365 6c66 2c20 7761 7665 666f 726d  2(self, waveform
-0002e9d0: 5f6e 616d 652c 206e 756d 5f77 6176 6566  _name, num_wavef
-0002e9e0: 6f72 6d73 2c20 7361 6d70 6c65 735f 7065  orms, samples_pe
-0002e9f0: 725f 7761 7665 666f 726d 2c20 7761 7665  r_waveform, wave
-0002ea00: 666f 726d 5f64 6174 6129 3a0a 2020 2020  form_data):.    
-0002ea10: 2020 2020 7227 2727 5f77 7269 7465 5f73      r'''_write_s
-0002ea20: 6f75 7263 655f 7761 7665 666f 726d 5f73  ource_waveform_s
-0002ea30: 6974 655f 756e 6971 7565 5f75 3332 0a0a  ite_unique_u32..
-0002ea40: 2020 2020 2020 2020 5772 6974 6573 206f          Writes o
-0002ea50: 6e65 2077 6176 6566 6f72 6d20 7065 7220  ne waveform per 
-0002ea60: 7369 7465 2e20 5573 6520 7468 6973 2077  site. Use this w
-0002ea70: 7269 7465 206d 6574 686f 6420 6966 2079  rite method if y
-0002ea80: 6f75 2073 6574 2074 6865 2070 6172 616d  ou set the param
-0002ea90: 6574 6572 206f 6620 7468 6520 6372 6561  eter of the crea
-0002eaa0: 7465 2073 6f75 7263 6520 7761 7665 666f  te source wavefo
-0002eab0: 726d 206d 6574 686f 6420 746f 2053 6974  rm method to Sit
-0002eac0: 6520 556e 6971 7565 2e0a 0a20 2020 2020  e Unique...     
-0002ead0: 2020 2054 6970 3a0a 2020 2020 2020 2020     Tip:.        
-0002eae0: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
-0002eaf0: 6265 2063 616c 6c65 6420 6f6e 2073 7065  be called on spe
-0002eb00: 6369 6669 6320 7369 7465 7320 7769 7468  cific sites with
-0002eb10: 696e 2079 6f75 7220 3a70 793a 636c 6173  in your :py:clas
-0002eb20: 733a 606e 6964 6967 6974 616c 2e53 6573  s:`nidigital.Ses
-0002eb30: 7369 6f6e 6020 696e 7374 616e 6365 2e0a  sion` instance..
-0002eb40: 2020 2020 2020 2020 5573 6520 5079 7468          Use Pyth
-0002eb50: 6f6e 2069 6e64 6578 206e 6f74 6174 696f  on index notatio
-0002eb60: 6e20 6f6e 2074 6865 2072 6570 6561 7465  n on the repeate
-0002eb70: 6420 6361 7061 6269 6c69 7469 6573 2063  d capabilities c
-0002eb80: 6f6e 7461 696e 6572 2073 6974 6573 2074  ontainer sites t
-0002eb90: 6f20 7370 6563 6966 7920 6120 7375 6273  o specify a subs
-0002eba0: 6574 2c0a 2020 2020 2020 2020 616e 6420  et,.        and 
-0002ebb0: 7468 656e 2063 616c 6c20 7468 6973 206d  then call this m
-0002ebc0: 6574 686f 6420 6f6e 2074 6865 2072 6573  ethod on the res
-0002ebd0: 756c 742e 0a0a 2020 2020 2020 2020 4578  ult...        Ex
-0002ebe0: 616d 706c 653a 203a 7079 3a6d 6574 683a  ample: :py:meth:
-0002ebf0: 606d 795f 7365 7373 696f 6e2e 7369 7465  `my_session.site
-0002ec00: 735b 202e 2e2e 205d 2e5f 7772 6974 655f  s[ ... ]._write_
-0002ec10: 736f 7572 6365 5f77 6176 6566 6f72 6d5f  source_waveform_
-0002ec20: 7369 7465 5f75 6e69 7175 655f 7533 3260  site_unique_u32`
-0002ec30: 0a0a 2020 2020 2020 2020 546f 2063 616c  ..        To cal
-0002ec40: 6c20 7468 6520 6d65 7468 6f64 206f 6e20  l the method on 
-0002ec50: 616c 6c20 7369 7465 732c 2079 6f75 2063  all sites, you c
-0002ec60: 616e 2063 616c 6c20 6974 2064 6972 6563  an call it direc
-0002ec70: 746c 7920 6f6e 2074 6865 203a 7079 3a63  tly on the :py:c
-0002ec80: 6c61 7373 3a60 6e69 6469 6769 7461 6c2e  lass:`nidigital.
-0002ec90: 5365 7373 696f 6e60 2e0a 0a20 2020 2020  Session`...     
-0002eca0: 2020 2045 7861 6d70 6c65 3a20 3a70 793a     Example: :py:
-0002ecb0: 6d65 7468 3a60 6d79 5f73 6573 7369 6f6e  meth:`my_session
-0002ecc0: 2e5f 7772 6974 655f 736f 7572 6365 5f77  ._write_source_w
-0002ecd0: 6176 6566 6f72 6d5f 7369 7465 5f75 6e69  aveform_site_uni
-0002ece0: 7175 655f 7533 3260 0a0a 2020 2020 2020  que_u32`..      
-0002ecf0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0002ed00: 2020 2020 7761 7665 666f 726d 5f6e 616d      waveform_nam
-0002ed10: 6520 2873 7472 293a 2054 6865 206e 616d  e (str): The nam
-0002ed20: 6520 746f 2061 7373 6967 6e20 746f 2074  e to assign to t
-0002ed30: 6865 2077 6176 6566 6f72 6d2e 2055 7365  he waveform. Use
-0002ed40: 2074 6865 2077 6176 6566 6f72 6d5f 6e61   the waveform_na
-0002ed50: 6d65 2020 7769 7468 2073 6f75 7263 655f  me  with source_
-0002ed60: 7374 6172 7420 6f70 636f 6465 2069 6e20  start opcode in 
-0002ed70: 796f 7572 2070 6174 7465 726e 2e0a 0a20  your pattern... 
-0002ed80: 2020 2020 2020 2020 2020 206e 756d 5f77             num_w
-0002ed90: 6176 6566 6f72 6d73 2028 696e 7429 3a20  aveforms (int): 
-0002eda0: 4e75 6d62 6572 206f 6620 7761 7665 666f  Number of wavefo
-0002edb0: 726d 732e 0a0a 2020 2020 2020 2020 2020  rms...          
-0002edc0: 2020 7361 6d70 6c65 735f 7065 725f 7761    samples_per_wa
-0002edd0: 7665 666f 726d 2028 696e 7429 3a20 4e75  veform (int): Nu
-0002ede0: 6d62 6572 206f 6620 7361 6d70 6c65 7320  mber of samples 
-0002edf0: 7065 7220 7761 7665 666f 726d 2e0a 0a20  per waveform... 
-0002ee00: 2020 2020 2020 2020 2020 2077 6176 6566             wavef
-0002ee10: 6f72 6d5f 6461 7461 2028 6172 7261 792e  orm_data (array.
-0002ee20: 6172 7261 7928 224c 2229 293a 2041 6e20  array("L")): An 
-0002ee30: 6172 7261 7920 6f66 2073 616d 706c 6573  array of samples
-0002ee40: 2074 6f20 7573 6520 6173 2073 6f75 7263   to use as sourc
-0002ee50: 6520 6461 7461 2e20 4461 7461 2066 6f72  e data. Data for
-0002ee60: 2065 6163 6820 7369 7465 206d 7573 7420   each site must 
-0002ee70: 6265 2061 7070 656e 6465 6420 7365 7175  be appended sequ
-0002ee80: 656e 7469 616c 6c79 2069 6e20 7468 6520  entially in the 
-0002ee90: 6172 7261 7920 286e 6f6e 2d69 6e74 6572  array (non-inter
-0002eea0: 6c65 6176 6564 292e 0a0a 2020 2020 2020  leaved)...      
-0002eeb0: 2020 2727 270a 2020 2020 2020 2020 7365    '''.        se
-0002eec0: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
-0002eed0: 7772 6974 655f 736f 7572 6365 5f77 6176  write_source_wav
-0002eee0: 6566 6f72 6d5f 7369 7465 5f75 6e69 7175  eform_site_uniqu
-0002eef0: 655f 7533 3228 7365 6c66 2e5f 7265 7065  e_u32(self._repe
-0002ef00: 6174 6564 5f63 6170 6162 696c 6974 792c  ated_capability,
-0002ef10: 2077 6176 6566 6f72 6d5f 6e61 6d65 2c20   waveform_name, 
-0002ef20: 6e75 6d5f 7761 7665 666f 726d 732c 2073  num_waveforms, s
-0002ef30: 616d 706c 6573 5f70 6572 5f77 6176 6566  amples_per_wavef
-0002ef40: 6f72 6d2c 2077 6176 6566 6f72 6d5f 6461  orm, waveform_da
-0002ef50: 7461 290a 0a20 2020 2040 6976 695f 7379  ta)..    @ivi_sy
-0002ef60: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
-0002ef70: 6566 2077 7269 7465 5f73 7461 7469 6328  ef write_static(
-0002ef80: 7365 6c66 2c20 7374 6174 6529 3a0a 2020  self, state):.  
-0002ef90: 2020 2020 2020 7227 2727 7772 6974 655f        r'''write_
-0002efa0: 7374 6174 6963 0a0a 2020 2020 2020 2020  static..        
-0002efb0: 5772 6974 6573 2061 2073 7461 7469 6320  Writes a static 
-0002efc0: 7374 6174 6520 746f 2074 6865 2073 7065  state to the spe
-0002efd0: 6369 6669 6564 2070 696e 732e 2054 6865  cified pins. The
-0002efe0: 2073 656c 6563 7465 6420 7069 6e73 2072   selected pins r
-0002eff0: 656d 6169 6e20 696e 2074 6865 2073 7065  emain in the spe
-0002f000: 6369 6669 6564 2073 7461 7465 2075 6e74  cified state unt
-0002f010: 696c 2074 6865 206e 6578 7420 7061 7474  il the next patt
-0002f020: 6572 6e20 6275 7273 7420 6f72 2063 616c  ern burst or cal
-0002f030: 6c20 746f 2074 6869 7320 6d65 7468 6f64  l to this method
-0002f040: 2e20 4966 2074 6865 7265 2061 7265 2075  . If there are u
-0002f050: 6e63 6f6d 6d69 7474 6564 2063 6861 6e67  ncommitted chang
-0002f060: 6573 2074 6f20 6c65 7665 6c73 206f 7220  es to levels or 
-0002f070: 7468 6520 7465 726d 696e 6174 696f 6e20  the termination 
-0002f080: 6d6f 6465 2c20 7468 6973 206d 6574 686f  mode, this metho
-0002f090: 6420 636f 6d6d 6974 7320 7468 6520 6368  d commits the ch
-0002f0a0: 616e 6765 7320 746f 2074 6865 2070 696e  anges to the pin
-0002f0b0: 732e 2054 6869 7320 6d65 7468 6f64 2064  s. This method d
-0002f0c0: 6f65 7320 6e6f 7420 6368 616e 6765 2074  oes not change t
-0002f0d0: 6865 2073 656c 6563 7465 6420 7069 6e20  he selected pin 
-0002f0e0: 6d65 7468 6f64 2e20 4966 2079 6f75 2077  method. If you w
-0002f0f0: 7269 7465 2061 2073 7461 7469 6320 7374  rite a static st
-0002f100: 6174 6520 746f 2061 2070 696e 2074 6861  ate to a pin tha
-0002f110: 7420 646f 6573 206e 6f74 2068 6176 6520  t does not have 
-0002f120: 7468 6520 4469 6769 7461 6c20 6d65 7468  the Digital meth
-0002f130: 6f64 2073 656c 6563 7465 642c 2074 6865  od selected, the
-0002f140: 206e 6577 2073 7461 7469 6320 7374 6174   new static stat
-0002f150: 6520 6973 2073 746f 7265 6420 6279 2074  e is stored by t
-0002f160: 6865 2069 6e73 7472 756d 656e 742c 2061  he instrument, a
-0002f170: 6e64 2061 6666 6563 7473 2074 6865 2073  nd affects the s
-0002f180: 7461 7465 206f 6620 7468 6520 7069 6e20  tate of the pin 
-0002f190: 7468 6520 6e65 7874 2074 696d 6520 796f  the next time yo
-0002f1a0: 7520 6368 616e 6765 2074 6865 2073 656c  u change the sel
-0002f1b0: 6563 7465 6420 6d65 7468 6f64 2074 6f20  ected method to 
-0002f1c0: 4469 6769 7461 6c2e 0a0a 2020 2020 2020  Digital...      
-0002f1d0: 2020 5469 703a 0a20 2020 2020 2020 2054    Tip:.        T
-0002f1e0: 6869 7320 6d65 7468 6f64 2063 616e 2062  his method can b
-0002f1f0: 6520 6361 6c6c 6564 206f 6e20 7370 6563  e called on spec
-0002f200: 6966 6963 2063 6861 6e6e 656c 7320 7769  ific channels wi
-0002f210: 7468 696e 2079 6f75 7220 3a70 793a 636c  thin your :py:cl
-0002f220: 6173 733a 606e 6964 6967 6974 616c 2e53  ass:`nidigital.S
-0002f230: 6573 7369 6f6e 6020 696e 7374 616e 6365  ession` instance
-0002f240: 2e0a 2020 2020 2020 2020 5573 6520 5079  ..        Use Py
-0002f250: 7468 6f6e 2069 6e64 6578 206e 6f74 6174  thon index notat
-0002f260: 696f 6e20 6f6e 2074 6865 2072 6570 6561  ion on the repea
-0002f270: 7465 6420 6361 7061 6269 6c69 7469 6573  ted capabilities
-0002f280: 2063 6f6e 7461 696e 6572 2063 6861 6e6e   container chann
-0002f290: 656c 7320 746f 2073 7065 6369 6679 2061  els to specify a
-0002f2a0: 2073 7562 7365 742c 0a20 2020 2020 2020   subset,.       
-0002f2b0: 2061 6e64 2074 6865 6e20 6361 6c6c 2074   and then call t
-0002f2c0: 6869 7320 6d65 7468 6f64 206f 6e20 7468  his method on th
-0002f2d0: 6520 7265 7375 6c74 2e0a 0a20 2020 2020  e result...     
-0002f2e0: 2020 2045 7861 6d70 6c65 3a20 3a70 793a     Example: :py:
-0002f2f0: 6d65 7468 3a60 6d79 5f73 6573 7369 6f6e  meth:`my_session
-0002f300: 2e63 6861 6e6e 656c 735b 202e 2e2e 205d  .channels[ ... ]
-0002f310: 2e77 7269 7465 5f73 7461 7469 6360 0a0a  .write_static`..
-0002f320: 2020 2020 2020 2020 546f 2063 616c 6c20          To call 
-0002f330: 7468 6520 6d65 7468 6f64 206f 6e20 616c  the method on al
-0002f340: 6c20 6368 616e 6e65 6c73 2c20 796f 7520  l channels, you 
-0002f350: 6361 6e20 6361 6c6c 2069 7420 6469 7265  can call it dire
-0002f360: 6374 6c79 206f 6e20 7468 6520 3a70 793a  ctly on the :py:
-0002f370: 636c 6173 733a 606e 6964 6967 6974 616c  class:`nidigital
-0002f380: 2e53 6573 7369 6f6e 602e 0a0a 2020 2020  .Session`...    
-0002f390: 2020 2020 4578 616d 706c 653a 203a 7079      Example: :py
-0002f3a0: 3a6d 6574 683a 606d 795f 7365 7373 696f  :meth:`my_sessio
-0002f3b0: 6e2e 7772 6974 655f 7374 6174 6963 600a  n.write_static`.
-0002f3c0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0002f3d0: 2020 2020 2020 2020 2020 2073 7461 7465             state
-0002f3e0: 2028 656e 756d 732e 5772 6974 6553 7461   (enums.WriteSta
-0002f3f0: 7469 6350 696e 5374 6174 6529 3a20 5061  ticPinState): Pa
-0002f400: 7261 6d65 7465 7220 7468 6174 2073 7065  rameter that spe
-0002f410: 6369 6669 6573 206f 6e65 206f 6620 7468  cifies one of th
-0002f420: 6520 666f 6c6c 6f77 696e 6720 6469 6769  e following digi
-0002f430: 7461 6c20 7374 6174 6573 2074 6f20 6173  tal states to as
-0002f440: 7369 676e 2074 6f20 7468 6520 7069 6e2e  sign to the pin.
-0002f450: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0002f460: 2020 2d20 2020 5772 6974 6553 7461 7469    -   WriteStati
-0002f470: 6350 696e 5374 6174 652e 5a45 524f 3a20  cPinState.ZERO: 
-0002f480: 5370 6563 6966 6965 7320 746f 2064 7269  Specifies to dri
-0002f490: 7665 206c 6f77 2e0a 2020 2020 2020 2020  ve low..        
-0002f4a0: 2020 2020 2020 2020 2d20 2020 5772 6974          -   Writ
-0002f4b0: 6553 7461 7469 6350 696e 5374 6174 652e  eStaticPinState.
-0002f4c0: 4f4e 453a 2053 7065 6369 6669 6573 2074  ONE: Specifies t
-0002f4d0: 6f20 6472 6976 6520 6869 6768 2e0a 2020  o drive high..  
-0002f4e0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-0002f4f0: 2020 5772 6974 6553 7461 7469 6350 696e    WriteStaticPin
-0002f500: 5374 6174 652e 583a 2053 7065 6369 6669  State.X: Specifi
-0002f510: 6573 2074 6f20 6e6f 7420 6472 6976 652e  es to not drive.
-0002f520: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0002f530: 2020 4e6f 7465 3a0a 2020 2020 2020 2020    Note:.        
-0002f540: 2020 2020 2020 2020 4f6e 6520 6f72 206d          One or m
-0002f550: 6f72 6520 6f66 2074 6865 2072 6566 6572  ore of the refer
-0002f560: 656e 6365 6420 7661 6c75 6573 2061 7265  enced values are
-0002f570: 206e 6f74 2069 6e20 7468 6520 5079 7468   not in the Pyth
-0002f580: 6f6e 2041 5049 2066 6f72 2074 6869 7320  on API for this 
-0002f590: 6472 6976 6572 2e20 456e 756d 7320 7468  driver. Enums th
-0002f5a0: 6174 206f 6e6c 7920 6465 6669 6e65 2076  at only define v
-0002f5b0: 616c 7565 732c 206f 7220 7265 7072 6573  alues, or repres
-0002f5c0: 656e 7420 5472 7565 2f46 616c 7365 2c20  ent True/False, 
-0002f5d0: 6861 7665 2062 6565 6e20 7265 6d6f 7665  have been remove
-0002f5e0: 642e 0a0a 2020 2020 2020 2020 2727 270a  d...        '''.
-0002f5f0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-0002f600: 7374 6174 6529 2069 7320 6e6f 7420 656e  state) is not en
-0002f610: 756d 732e 5772 6974 6553 7461 7469 6350  ums.WriteStaticP
-0002f620: 696e 5374 6174 653a 0a20 2020 2020 2020  inState:.       
-0002f630: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-0002f640: 7272 6f72 2827 5061 7261 6d65 7465 7220  rror('Parameter 
-0002f650: 7374 6174 6520 6d75 7374 2062 6520 6f66  state must be of
-0002f660: 2074 7970 6520 2720 2b20 7374 7228 656e   type ' + str(en
-0002f670: 756d 732e 5772 6974 6553 7461 7469 6350  ums.WriteStaticP
-0002f680: 696e 5374 6174 6529 290a 2020 2020 2020  inState)).      
-0002f690: 2020 7365 6c66 2e5f 696e 7465 7270 7265    self._interpre
-0002f6a0: 7465 722e 7772 6974 655f 7374 6174 6963  ter.write_static
-0002f6b0: 2873 656c 662e 5f72 6570 6561 7465 645f  (self._repeated_
-0002f6c0: 6361 7061 6269 6c69 7479 2c20 7374 6174  capability, stat
-0002f6d0: 6529 0a0a 2020 2020 6465 6620 5f65 7272  e)..    def _err
-0002f6e0: 6f72 5f6d 6573 7361 6765 2873 656c 662c  or_message(self,
-0002f6f0: 2065 7272 6f72 5f63 6f64 6529 3a0a 2020   error_code):.  
-0002f700: 2020 2020 2020 7227 2727 5f65 7272 6f72        r'''_error
-0002f710: 5f6d 6573 7361 6765 0a0a 2020 2020 2020  _message..      
-0002f720: 2020 5461 6b65 7320 7468 6520 6572 726f    Takes the erro
-0002f730: 7220 636f 6465 2072 6574 7572 6e65 6420  r code returned 
-0002f740: 6279 2074 6865 2064 6967 6974 616c 2070  by the digital p
-0002f750: 6174 7465 726e 2069 6e73 7472 756d 656e  attern instrumen
-0002f760: 7420 6472 6976 6572 206d 6574 686f 6473  t driver methods
-0002f770: 2c20 696e 7465 7270 7265 7473 2069 742c  , interprets it,
-0002f780: 2061 6e64 2072 6574 7572 6e73 2069 7420   and returns it 
-0002f790: 6173 2061 2075 7365 7220 7265 6164 6162  as a user readab
-0002f7a0: 6c65 2073 7472 696e 672e 0a0a 2020 2020  le string...    
-0002f7b0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0002f7c0: 2020 2020 2020 6572 726f 725f 636f 6465        error_code
-0002f7d0: 2028 696e 7429 3a20 5468 6520 7370 6563   (int): The spec
-0002f7e0: 6966 6965 6420 6572 726f 7220 636f 6465  ified error code
-0002f7f0: 2e0a 0a0a 2020 2020 2020 2020 5265 7475  ....        Retu
-0002f800: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0002f810: 2065 7272 6f72 5f6d 6573 7361 6765 2028   error_message (
-0002f820: 7374 7229 3a20 5468 6520 6572 726f 7220  str): The error 
-0002f830: 696e 666f 726d 6174 696f 6e20 666f 726d  information form
-0002f840: 6174 7465 6420 6173 2061 2073 7472 696e  atted as a strin
-0002f850: 672e 2054 6865 2061 7272 6179 206d 7573  g. The array mus
-0002f860: 7420 636f 6e74 6169 6e20 6174 206c 6561  t contain at lea
-0002f870: 7374 2032 3536 2063 6861 7261 6374 6572  st 256 character
-0002f880: 732e 0a0a 2020 2020 2020 2020 2727 270a  s...        '''.
-0002f890: 2020 2020 2020 2020 6572 726f 725f 6d65          error_me
-0002f8a0: 7373 6167 6520 3d20 7365 6c66 2e5f 696e  ssage = self._in
-0002f8b0: 7465 7270 7265 7465 722e 6572 726f 725f  terpreter.error_
-0002f8c0: 6d65 7373 6167 6528 6572 726f 725f 636f  message(error_co
-0002f8d0: 6465 290a 2020 2020 2020 2020 7265 7475  de).        retu
-0002f8e0: 726e 2065 7272 6f72 5f6d 6573 7361 6765  rn error_message
-0002f8f0: 0a0a 0a63 6c61 7373 2053 6573 7369 6f6e  ...class Session
-0002f900: 285f 5365 7373 696f 6e42 6173 6529 3a0a  (_SessionBase):.
-0002f910: 2020 2020 2727 2741 6e20 4e49 2d44 6967      '''An NI-Dig
-0002f920: 6974 616c 2050 6174 7465 726e 2044 7269  ital Pattern Dri
-0002f930: 7665 7220 7365 7373 696f 6e27 2727 0a0a  ver session'''..
-0002f940: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0002f950: 2873 656c 662c 2072 6573 6f75 7263 655f  (self, resource_
-0002f960: 6e61 6d65 2c20 6964 5f71 7565 7279 3d46  name, id_query=F
-0002f970: 616c 7365 2c20 7265 7365 745f 6465 7669  alse, reset_devi
-0002f980: 6365 3d46 616c 7365 2c20 6f70 7469 6f6e  ce=False, option
-0002f990: 733d 7b7d 2c20 2a2c 2067 7270 635f 6f70  s={}, *, grpc_op
-0002f9a0: 7469 6f6e 733d 4e6f 6e65 293a 0a20 2020  tions=None):.   
-0002f9b0: 2020 2020 2072 2727 2741 6e20 4e49 2d44       r'''An NI-D
-0002f9c0: 6967 6974 616c 2050 6174 7465 726e 2044  igital Pattern D
-0002f9d0: 7269 7665 7220 7365 7373 696f 6e0a 0a20  river session.. 
-0002f9e0: 2020 2020 2020 2043 7265 6174 6573 2061         Creates a
-0002f9f0: 6e64 2072 6574 7572 6e73 2061 206e 6577  nd returns a new
-0002fa00: 2073 6573 7369 6f6e 2074 6f20 7468 6520   session to the 
-0002fa10: 7370 6563 6966 6965 6420 6469 6769 7461  specified digita
-0002fa20: 6c20 7061 7474 6572 6e20 696e 7374 7275  l pattern instru
-0002fa30: 6d65 6e74 2074 6f20 7573 6520 696e 2061  ment to use in a
-0002fa40: 6c6c 2073 7562 7365 7175 656e 7420 6d65  ll subsequent me
-0002fa50: 7468 6f64 2063 616c 6c73 2e20 546f 2070  thod calls. To p
-0002fa60: 6c61 6365 2074 6865 2069 6e73 7472 756d  lace the instrum
-0002fa70: 656e 7420 696e 2061 206b 6e6f 776e 2073  ent in a known s
-0002fa80: 7461 7274 7570 2073 7461 7465 2077 6865  tartup state whe
-0002fa90: 6e20 6372 6561 7469 6e67 2061 206e 6577  n creating a new
-0002faa0: 2073 6573 7369 6f6e 2c20 7365 7420 7468   session, set th
-0002fab0: 6520 7265 7365 7420 7061 7261 6d65 7465  e reset paramete
-0002fac0: 7220 746f 2054 7275 652c 2077 6869 6368  r to True, which
-0002fad0: 2069 7320 6571 7569 7661 6c65 6e74 2074   is equivalent t
-0002fae0: 6f20 6361 6c6c 696e 6720 7468 6520 7265  o calling the re
-0002faf0: 7365 7420 6d65 7468 6f64 2069 6d6d 6564  set method immed
-0002fb00: 6961 7465 6c79 2061 6674 6572 2069 6e69  iately after ini
-0002fb10: 7469 616c 697a 696e 6720 7468 6520 7365  tializing the se
-0002fb20: 7373 696f 6e2e 0a0a 2020 2020 2020 2020  ssion...        
-0002fb30: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0002fb40: 2020 7265 736f 7572 6365 5f6e 616d 6520    resource_name 
-0002fb50: 2873 7472 293a 2054 6865 2073 7065 6369  (str): The speci
-0002fb60: 6669 6564 2072 6573 6f75 7263 6520 6e61  fied resource na
-0002fb70: 6d65 2073 686f 776e 2069 6e20 4d65 6173  me shown in Meas
-0002fb80: 7572 656d 656e 7420 2620 4175 746f 6d61  urement & Automa
-0002fb90: 7469 6f6e 2045 7870 6c6f 7265 7220 284d  tion Explorer (M
-0002fba0: 4158 2920 666f 7220 6120 6469 6769 7461  AX) for a digita
-0002fbb0: 6c20 7061 7474 6572 6e20 696e 7374 7275  l pattern instru
-0002fbc0: 6d65 6e74 2c20 666f 7220 6578 616d 706c  ment, for exampl
-0002fbd0: 652c 2050 5849 3153 6c6f 7433 2c20 7768  e, PXI1Slot3, wh
-0002fbe0: 6572 6520 5058 4931 536c 6f74 3320 6973  ere PXI1Slot3 is
-0002fbf0: 2061 6e20 696e 7374 7275 6d65 6e74 2072   an instrument r
-0002fc00: 6573 6f75 7263 6520 6e61 6d65 2e20 2a2a  esource name. **
-0002fc10: 7265 736f 7572 6365 4e61 6d65 2a2a 2063  resourceName** c
-0002fc20: 616e 2061 6c73 6f20 6265 2061 206c 6f67  an also be a log
-0002fc30: 6963 616c 2049 5649 206e 616d 652e 2054  ical IVI name. T
-0002fc40: 6869 7320 7061 7261 6d65 7465 7220 6163  his parameter ac
-0002fc50: 6365 7074 7320 6120 636f 6d6d 612d 6465  cepts a comma-de
-0002fc60: 6c69 6d69 7465 6420 6c69 7374 206f 6620  limited list of 
-0002fc70: 7374 7269 6e67 7320 696e 2074 6865 2066  strings in the f
-0002fc80: 6f72 6d20 5058 4931 536c 6f74 322c 5058  orm PXI1Slot2,PX
-0002fc90: 4931 536c 6f74 332c 2077 6865 7265 2060  I1Slot3, where `
-0002fca0: 6050 5849 3153 6c6f 7432 6060 2069 7320  `PXI1Slot2`` is 
-0002fcb0: 6f6e 6520 696e 7374 7275 6d65 6e74 2072  one instrument r
-0002fcc0: 6573 6f75 7263 6520 6e61 6d65 2061 6e64  esource name and
-0002fcd0: 2060 6050 5849 3153 6c6f 7433 6060 2069   ``PXI1Slot3`` i
-0002fce0: 7320 616e 6f74 6865 722e 2057 6865 6e20  s another. When 
-0002fcf0: 696e 636c 7564 696e 6720 6d6f 7265 2074  including more t
-0002fd00: 6861 6e20 6f6e 6520 6469 6769 7461 6c20  han one digital 
-0002fd10: 7061 7474 6572 6e20 696e 7374 7275 6d65  pattern instrume
-0002fd20: 6e74 2069 6e20 7468 6520 636f 6d6d 612d  nt in the comma-
-0002fd30: 6465 6c69 6d69 7465 6420 6c69 7374 206f  delimited list o
-0002fd40: 6620 7374 7269 6e67 732c 206c 6973 7420  f strings, list 
-0002fd50: 7468 6520 696e 7374 7275 6d65 6e74 7320  the instruments 
-0002fd60: 696e 2074 6865 2073 616d 6520 6f72 6465  in the same orde
-0002fd70: 7220 7468 6579 2061 7070 6561 7220 696e  r they appear in
-0002fd80: 2074 6865 2070 696e 206d 6170 2e0a 0a20   the pin map... 
-0002fd90: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0002fda0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00027360: 2c20 7374 722c 206f 7220 696e 7429 3a20  , str, or int): 
+00027370: 496e 6465 7820 6c69 7374 2066 6f72 2074  Index list for t
+00027380: 6865 2063 6861 6e6e 656c 7320 696e 2074  he channels in t
+00027390: 6865 2073 6573 7369 6f6e 2e20 5661 6c69  he session. Vali
+000273a0: 6420 7661 6c75 6573 2061 7265 2066 726f  d values are fro
+000273b0: 6d20 7a65 726f 2074 6f20 7468 6520 746f  m zero to the to
+000273c0: 7461 6c20 6e75 6d62 6572 206f 6620 6368  tal number of ch
+000273d0: 616e 6e65 6c73 2069 6e20 7468 6520 7365  annels in the se
+000273e0: 7373 696f 6e20 6d69 6e75 7320 6f6e 652e  ssion minus one.
+000273f0: 2054 6865 2069 6e64 6578 2073 7472 696e   The index strin
+00027400: 6720 6361 6e20 6265 206f 6e65 206f 6620  g can be one of 
+00027410: 7468 6520 666f 6c6c 6f77 696e 6720 666f  the following fo
+00027420: 726d 6174 733a 0a0a 2020 2020 2020 2020  rmats:..        
+00027430: 2020 2020 2020 2020 2d20 2020 4120 636f          -   A co
+00027440: 6d6d 612d 7365 7061 7261 7465 6420 6c69  mma-separated li
+00027450: 7374 e280 9466 6f72 2065 7861 6d70 6c65  st...for example
+00027460: 2c20 2230 2c32 2c33 2c31 220a 2020 2020  , "0,2,3,1".    
+00027470: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
+00027480: 4120 7261 6e67 6520 7573 696e 6720 6120  A range using a 
+00027490: 6879 7068 656e e280 9466 6f72 2065 7861  hyphen...for exa
+000274a0: 6d70 6c65 2c20 2230 2d33 220a 2020 2020  mple, "0-3".    
+000274b0: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
+000274c0: 4120 7261 6e67 6520 7573 696e 6720 6120  A range using a 
+000274d0: 636f 6c6f 6ee2 8094 666f 7220 6578 616d  colon...for exam
+000274e0: 706c 652c 2022 303a 3320 220a 0a20 2020  ple, "0:3 "..   
+000274f0: 2020 2020 2020 2020 2020 2020 2059 6f75               You
+00027500: 2063 616e 2063 6f6d 6269 6e65 2063 6f6d   can combine com
+00027510: 6d61 2d73 6570 6172 6174 6564 206c 6973  ma-separated lis
+00027520: 7473 2061 6e64 2072 616e 6765 7320 7468  ts and ranges th
+00027530: 6174 2075 7365 2061 2068 7970 6865 6e20  at use a hyphen 
+00027540: 6f72 2063 6f6c 6f6e 2e20 426f 7468 206f  or colon. Both o
+00027550: 7574 2d6f 662d 6f72 6465 7220 616e 6420  ut-of-order and 
+00027560: 7265 7065 6174 6564 2069 6e64 6963 6573  repeated indices
+00027570: 2061 7265 2073 7570 706f 7274 6564 2028   are supported (
+00027580: 2232 2c33 2c30 222c 2022 312c 322c 322c  "2,3,0", "1,2,2,
+00027590: 3322 292e 2057 6869 7465 2073 7061 6365  3"). White space
+000275a0: 2063 6861 7261 6374 6572 732c 2069 6e63   characters, inc
+000275b0: 6c75 6469 6e67 2073 7061 6365 732c 2074  luding spaces, t
+000275c0: 6162 732c 2066 6565 6473 2c20 616e 6420  abs, feeds, and 
+000275d0: 6361 7272 6961 6765 2072 6574 7572 6e73  carriage returns
+000275e0: 2c20 6172 6520 616c 6c6f 7765 6420 6265  , are allowed be
+000275f0: 7477 6565 6e20 6368 6172 6163 7465 7273  tween characters
+00027600: 2e20 5261 6e67 6573 2063 616e 2062 6520  . Ranges can be 
+00027610: 696e 6372 656d 656e 7469 6e67 206f 7220  incrementing or 
+00027620: 6465 6372 656d 656e 7469 6e67 2e0a 0a0a  decrementing....
+00027630: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00027640: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+00027650: 6573 2028 6c69 7374 206f 6620 7374 7229  es (list of str)
+00027660: 3a20 5468 6520 6368 616e 6e65 6c20 6e61  : The channel na
+00027670: 6d65 2873 2920 6174 2074 6865 2073 7065  me(s) at the spe
+00027680: 6369 6669 6564 2069 6e64 6963 6573 2e0a  cified indices..
+00027690: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000276a0: 2020 2020 2069 6e64 6963 6573 203d 205f       indices = _
+000276b0: 636f 6e76 6572 7465 7273 2e63 6f6e 7665  converters.conve
+000276c0: 7274 5f72 6570 6561 7465 645f 6361 7061  rt_repeated_capa
+000276d0: 6269 6c69 7469 6573 5f77 6974 686f 7574  bilities_without
+000276e0: 5f70 7265 6669 7828 696e 6469 6365 7329  _prefix(indices)
+000276f0: 0a20 2020 2020 2020 206e 616d 6573 203d  .        names =
+00027700: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
+00027710: 6572 2e67 6574 5f63 6861 6e6e 656c 5f6e  er.get_channel_n
+00027720: 616d 6573 2869 6e64 6963 6573 290a 2020  ames(indices).  
+00027730: 2020 2020 2020 7265 7475 726e 205f 636f        return _co
+00027740: 6e76 6572 7465 7273 2e63 6f6e 7665 7274  nverters.convert
+00027750: 5f63 6f6d 6d61 5f73 6570 6172 6174 6564  _comma_separated
+00027760: 5f73 7472 696e 675f 746f 5f6c 6973 7428  _string_to_list(
+00027770: 6e61 6d65 7329 0a0a 2020 2020 4069 7669  names)..    @ivi
+00027780: 5f73 796e 6368 726f 6e69 7a65 640a 2020  _synchronized.  
+00027790: 2020 6465 6620 6765 745f 6661 696c 5f63    def get_fail_c
+000277a0: 6f75 6e74 2873 656c 6629 3a0a 2020 2020  ount(self):.    
+000277b0: 2020 2020 7227 2727 6765 745f 6661 696c      r'''get_fail
+000277c0: 5f63 6f75 6e74 0a0a 2020 2020 2020 2020  _count..        
+000277d0: 5265 7475 726e 7320 7468 6520 636f 6d70  Returns the comp
+000277e0: 6172 6973 6f6e 2066 6169 6c20 636f 756e  arison fail coun
+000277f0: 7420 666f 7220 7069 6e73 2069 6e20 7468  t for pins in th
+00027800: 6520 7265 7065 6174 6564 2063 6170 6162  e repeated capab
+00027810: 696c 6974 6965 732e 0a0a 2020 2020 2020  ilities...      
+00027820: 2020 5469 703a 0a20 2020 2020 2020 2054    Tip:.        T
+00027830: 6869 7320 6d65 7468 6f64 2063 616e 2062  his method can b
+00027840: 6520 6361 6c6c 6564 206f 6e20 7370 6563  e called on spec
+00027850: 6966 6963 2063 6861 6e6e 656c 7320 7769  ific channels wi
+00027860: 7468 696e 2079 6f75 7220 3a70 793a 636c  thin your :py:cl
+00027870: 6173 733a 606e 6964 6967 6974 616c 2e53  ass:`nidigital.S
+00027880: 6573 7369 6f6e 6020 696e 7374 616e 6365  ession` instance
+00027890: 2e0a 2020 2020 2020 2020 5573 6520 5079  ..        Use Py
+000278a0: 7468 6f6e 2069 6e64 6578 206e 6f74 6174  thon index notat
+000278b0: 696f 6e20 6f6e 2074 6865 2072 6570 6561  ion on the repea
+000278c0: 7465 6420 6361 7061 6269 6c69 7469 6573  ted capabilities
+000278d0: 2063 6f6e 7461 696e 6572 2063 6861 6e6e   container chann
+000278e0: 656c 7320 746f 2073 7065 6369 6679 2061  els to specify a
+000278f0: 2073 7562 7365 742c 0a20 2020 2020 2020   subset,.       
+00027900: 2061 6e64 2074 6865 6e20 6361 6c6c 2074   and then call t
+00027910: 6869 7320 6d65 7468 6f64 206f 6e20 7468  his method on th
+00027920: 6520 7265 7375 6c74 2e0a 0a20 2020 2020  e result...     
+00027930: 2020 2045 7861 6d70 6c65 3a20 3a70 793a     Example: :py:
+00027940: 6d65 7468 3a60 6d79 5f73 6573 7369 6f6e  meth:`my_session
+00027950: 2e63 6861 6e6e 656c 735b 202e 2e2e 205d  .channels[ ... ]
+00027960: 2e67 6574 5f66 6169 6c5f 636f 756e 7460  .get_fail_count`
+00027970: 0a0a 2020 2020 2020 2020 546f 2063 616c  ..        To cal
+00027980: 6c20 7468 6520 6d65 7468 6f64 206f 6e20  l the method on 
+00027990: 616c 6c20 6368 616e 6e65 6c73 2c20 796f  all channels, yo
+000279a0: 7520 6361 6e20 6361 6c6c 2069 7420 6469  u can call it di
+000279b0: 7265 6374 6c79 206f 6e20 7468 6520 3a70  rectly on the :p
+000279c0: 793a 636c 6173 733a 606e 6964 6967 6974  y:class:`nidigit
+000279d0: 616c 2e53 6573 7369 6f6e 602e 0a0a 2020  al.Session`...  
+000279e0: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
+000279f0: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
+00027a00: 696f 6e2e 6765 745f 6661 696c 5f63 6f75  ion.get_fail_cou
+00027a10: 6e74 600a 0a20 2020 2020 2020 2052 6574  nt`..        Ret
+00027a20: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00027a30: 2020 6661 696c 7572 655f 636f 756e 7420    failure_count 
+00027a40: 286c 6973 7420 6f66 2069 6e74 293a 204e  (list of int): N
+00027a50: 756d 6265 7220 6f66 2066 6169 6c75 7265  umber of failure
+00027a60: 7320 696e 2061 6e20 6172 7261 792e 2049  s in an array. I
+00027a70: 6620 6120 7369 7465 2069 7320 6469 7361  f a site is disa
+00027a80: 626c 6564 206f 7220 6e6f 7420 656e 6162  bled or not enab
+00027a90: 6c65 6420 666f 7220 6275 7273 742c 2074  led for burst, t
+00027aa0: 6865 206d 6574 686f 6420 646f 6573 206e  he method does n
+00027ab0: 6f74 2072 6574 7572 6e20 6461 7461 2066  ot return data f
+00027ac0: 6f72 2074 6861 7420 7369 7465 2e20 596f  or that site. Yo
+00027ad0: 7520 6361 6e20 616c 736f 2075 7365 2074  u can also use t
+00027ae0: 6865 2067 6574 5f70 696e 5f72 6573 756c  he get_pin_resul
+00027af0: 7473 5f70 696e 5f69 6e66 6f72 6d61 7469  ts_pin_informati
+00027b00: 6f6e 206d 6574 686f 6420 746f 206f 6274  on method to obt
+00027b10: 6169 6e20 6120 736f 7274 6564 206c 6973  ain a sorted lis
+00027b20: 7420 6f66 2072 6574 7572 6e65 6420 7369  t of returned si
+00027b30: 7465 7320 616e 6420 6368 616e 6e65 6c73  tes and channels
+00027b40: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
+00027b50: 2020 2020 2020 2066 6169 6c75 7265 5f63         failure_c
+00027b60: 6f75 6e74 203d 2073 656c 662e 5f69 6e74  ount = self._int
+00027b70: 6572 7072 6574 6572 2e67 6574 5f66 6169  erpreter.get_fai
+00027b80: 6c5f 636f 756e 7428 7365 6c66 2e5f 7265  l_count(self._re
+00027b90: 7065 6174 6564 5f63 6170 6162 696c 6974  peated_capabilit
+00027ba0: 7929 0a20 2020 2020 2020 2072 6574 7572  y).        retur
+00027bb0: 6e20 6661 696c 7572 655f 636f 756e 740a  n failure_count.
+00027bc0: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
+00027bd0: 6f6e 697a 6564 0a20 2020 2064 6566 2067  onized.    def g
+00027be0: 6574 5f68 6973 746f 7279 5f72 616d 5f73  et_history_ram_s
+00027bf0: 616d 706c 655f 636f 756e 7428 7365 6c66  ample_count(self
+00027c00: 293a 0a20 2020 2020 2020 2072 2727 2767  ):.        r'''g
+00027c10: 6574 5f68 6973 746f 7279 5f72 616d 5f73  et_history_ram_s
+00027c20: 616d 706c 655f 636f 756e 740a 0a20 2020  ample_count..   
+00027c30: 2020 2020 2052 6574 7572 6e73 2074 6865       Returns the
+00027c40: 206e 756d 6265 7220 6f66 2073 616d 706c   number of sampl
+00027c50: 6573 2048 6973 746f 7279 2052 414d 2061  es History RAM a
+00027c60: 6371 7569 7265 6420 6f6e 2074 6865 206c  cquired on the l
+00027c70: 6173 7420 7061 7474 6572 6e20 6275 7273  ast pattern burs
+00027c80: 742e 0a0a 2020 2020 2020 2020 4e6f 7465  t...        Note
+00027c90: 3a0a 2020 2020 2020 2020 4265 666f 7265  :.        Before
+00027ca0: 2062 7572 7374 696e 6720 6120 7061 7474   bursting a patt
+00027cb0: 6572 6e2c 2079 6f75 206d 7573 7420 636f  ern, you must co
+00027cc0: 6e66 6967 7572 6520 7468 6520 4869 7374  nfigure the Hist
+00027cd0: 6f72 7920 5241 4d20 7472 6967 6765 7220  ory RAM trigger 
+00027ce0: 616e 6420 7370 6563 6966 7920 7768 6963  and specify whic
+00027cf0: 6820 6379 636c 6573 2074 6f20 6163 7175  h cycles to acqu
+00027d00: 6972 652e 0a0a 2020 2020 2020 2020 6869  ire...        hi
+00027d10: 7374 6f72 795f 7261 6d5f 7472 6967 6765  story_ram_trigge
+00027d20: 725f 7479 7065 2073 686f 756c 6420 6265  r_type should be
+00027d30: 2075 7365 6420 746f 2073 7065 6369 6679   used to specify
+00027d40: 2074 6865 2074 7269 6767 6572 2063 6f6e   the trigger con
+00027d50: 6469 7469 6f6e 206f 6e20 7768 6963 6820  dition on which 
+00027d60: 4869 7374 6f72 7920 5241 4d0a 2020 2020  History RAM.    
+00027d70: 2020 2020 7374 6172 7473 2061 6371 7569      starts acqui
+00027d80: 7269 6e67 2070 6174 7465 726e 2069 6e66  ring pattern inf
+00027d90: 6f72 6d61 7469 6f6e 2e0a 0a20 2020 2020  ormation...     
+00027da0: 2020 2049 6620 4869 7374 6f72 7920 5241     If History RA
+00027db0: 4d20 7472 6967 6765 7220 6973 2063 6f6e  M trigger is con
+00027dc0: 6669 6775 7265 6420 6173 2048 6973 746f  figured as Histo
+00027dd0: 7279 5241 4d54 7269 6767 6572 5479 7065  ryRAMTriggerType
+00027de0: 2e43 5943 4c45 5f4e 554d 4245 522c 0a20  .CYCLE_NUMBER,. 
+00027df0: 2020 2020 2020 2063 7963 6c65 5f6e 756d         cycle_num
+00027e00: 6265 725f 6869 7374 6f72 795f 7261 6d5f  ber_history_ram_
+00027e10: 7472 6967 6765 725f 6379 636c 655f 6e75  trigger_cycle_nu
+00027e20: 6d62 6572 2073 686f 756c 6420 6265 2075  mber should be u
+00027e30: 7365 6420 746f 2073 7065 6369 6679 2074  sed to specify t
+00027e40: 6865 2063 7963 6c65 206e 756d 6265 7220  he cycle number 
+00027e50: 6f6e 2077 6869 6368 0a20 2020 2020 2020  on which.       
+00027e60: 2048 6973 746f 7279 2052 414d 2073 7461   History RAM sta
+00027e70: 7274 7320 6163 7175 6972 696e 6720 7061  rts acquiring pa
+00027e80: 7474 6572 6e20 696e 666f 726d 6174 696f  ttern informatio
+00027e90: 6e2e 0a0a 2020 2020 2020 2020 4966 2048  n...        If H
+00027ea0: 6973 746f 7279 2052 414d 2074 7269 6767  istory RAM trigg
+00027eb0: 6572 2069 7320 636f 6e66 6967 7572 6564  er is configured
+00027ec0: 2061 7320 4869 7374 6f72 7952 414d 5472   as HistoryRAMTr
+00027ed0: 6967 6765 7254 7970 652e 5041 5454 4552  iggerType.PATTER
+00027ee0: 4e5f 4c41 4245 4c2c 0a20 2020 2020 2020  N_LABEL,.       
+00027ef0: 2070 6174 7465 726e 5f6c 6162 656c 5f68   pattern_label_h
+00027f00: 6973 746f 7279 5f72 616d 5f74 7269 6767  istory_ram_trigg
+00027f10: 6572 5f6c 6162 656c 2073 686f 756c 6420  er_label should 
+00027f20: 6265 2075 7365 6420 746f 2073 7065 6369  be used to speci
+00027f30: 6679 2074 6865 2070 6174 7465 726e 206c  fy the pattern l
+00027f40: 6162 656c 2066 726f 6d20 7768 6963 6820  abel from which 
+00027f50: 746f 0a20 2020 2020 2020 2073 7461 7274  to.        start
+00027f60: 2061 6371 7569 7269 6e67 2070 6174 7465   acquiring patte
+00027f70: 726e 2069 6e66 6f72 6d61 7469 6f6e 2e0a  rn information..
+00027f80: 2020 2020 2020 2020 7061 7474 6572 6e5f          pattern_
+00027f90: 6c61 6265 6c5f 6869 7374 6f72 795f 7261  label_history_ra
+00027fa0: 6d5f 7472 6967 6765 725f 7665 6374 6f72  m_trigger_vector
+00027fb0: 5f6f 6666 7365 7420 7368 6f75 6c64 2062  _offset should b
+00027fc0: 6520 7573 6564 2074 6f20 7370 6563 6966  e used to specif
+00027fd0: 7920 7468 6520 6e75 6d62 6572 206f 6620  y the number of 
+00027fe0: 7665 6374 6f72 730a 2020 2020 2020 2020  vectors.        
+00027ff0: 666f 6c6c 6f77 696e 6720 7468 6520 7370  following the sp
+00028000: 6563 6966 6965 6420 7061 7474 6572 6e20  ecified pattern 
+00028010: 6c61 6265 6c20 6672 6f6d 2077 6869 6368  label from which
+00028020: 2074 6f20 7374 6172 7420 6163 7175 6972   to start acquir
+00028030: 696e 6720 7061 7474 6572 6e20 696e 666f  ing pattern info
+00028040: 726d 6174 696f 6e2e 0a20 2020 2020 2020  rmation..       
+00028050: 2070 6174 7465 726e 5f6c 6162 656c 5f68   pattern_label_h
+00028060: 6973 746f 7279 5f72 616d 5f74 7269 6767  istory_ram_trigg
+00028070: 6572 5f63 7963 6c65 5f6f 6666 7365 7420  er_cycle_offset 
+00028080: 7368 6f75 6c64 2062 6520 7573 6564 2074  should be used t
+00028090: 6f20 7370 6563 6966 7920 7468 6520 6e75  o specify the nu
+000280a0: 6d62 6572 206f 6620 6379 636c 6573 0a20  mber of cycles. 
+000280b0: 2020 2020 2020 2066 6f6c 6c6f 7769 6e67         following
+000280c0: 2074 6865 2073 7065 6369 6669 6564 2070   the specified p
+000280d0: 6174 7465 726e 206c 6162 656c 2061 6e64  attern label and
+000280e0: 2076 6563 746f 7220 6f66 6673 6574 2066   vector offset f
+000280f0: 726f 6d20 7768 6963 6820 746f 2073 7461  rom which to sta
+00028100: 7274 2061 6371 7569 7269 6e67 2070 6174  rt acquiring pat
+00028110: 7465 726e 2069 6e66 6f72 6d61 7469 6f6e  tern information
+00028120: 2e0a 0a20 2020 2020 2020 2046 6f72 2061  ...        For a
+00028130: 6c6c 2048 6973 746f 7279 2052 414d 2074  ll History RAM t
+00028140: 7269 6767 6572 2063 6f6e 6469 7469 6f6e  rigger condition
+00028150: 732c 2068 6973 746f 7279 5f72 616d 5f70  s, history_ram_p
+00028160: 7265 7472 6967 6765 725f 7361 6d70 6c65  retrigger_sample
+00028170: 7320 7368 6f75 6c64 2062 6520 7573 6564  s should be used
+00028180: 2074 6f20 7370 6563 6966 790a 2020 2020   to specify.    
+00028190: 2020 2020 7468 6520 6e75 6d62 6572 206f      the number o
+000281a0: 6620 7361 6d70 6c65 7320 746f 2061 6371  f samples to acq
+000281b0: 7569 7265 2062 6566 6f72 6520 7468 6520  uire before the 
+000281c0: 7472 6967 6765 7220 636f 6e64 6974 696f  trigger conditio
+000281d0: 6e73 2061 7265 206d 6574 2e20 4966 2079  ns are met. If y
+000281e0: 6f75 2063 6f6e 6669 6775 7265 2048 6973  ou configure His
+000281f0: 746f 7279 2052 414d 2074 6f20 6f6e 6c79  tory RAM to only
+00028200: 0a20 2020 2020 2020 2061 6371 7569 7265  .        acquire
+00028210: 2066 6169 6c65 6420 6379 636c 6573 2c20   failed cycles, 
+00028220: 796f 7520 6d75 7374 2073 6574 2068 6973  you must set his
+00028230: 746f 7279 5f72 616d 5f70 7265 7472 6967  tory_ram_pretrig
+00028240: 6765 725f 7361 6d70 6c65 7320 746f 2030  ger_samples to 0
+00028250: 2e0a 0a20 2020 2020 2020 2068 6973 746f  ...        histo
+00028260: 7279 5f72 616d 5f63 7963 6c65 735f 746f  ry_ram_cycles_to
+00028270: 5f61 6371 7569 7265 2073 686f 756c 6420  _acquire should 
+00028280: 6265 2075 7365 6420 746f 2073 7065 6369  be used to speci
+00028290: 6679 2077 6869 6368 2063 7963 6c65 7320  fy which cycles 
+000282a0: 4869 7374 6f72 7920 5241 4d20 6163 7175  History RAM acqu
+000282b0: 6972 6573 2061 6674 6572 0a20 2020 2020  ires after.     
+000282c0: 2020 2074 6865 2074 7269 6767 6572 2063     the trigger c
+000282d0: 6f6e 6469 7469 6f6e 7320 6172 6520 6d65  onditions are me
+000282e0: 742e 0a0a 2020 2020 2020 2020 5469 703a  t...        Tip:
+000282f0: 0a20 2020 2020 2020 2054 6869 7320 6d65  .        This me
+00028300: 7468 6f64 2063 616e 2062 6520 6361 6c6c  thod can be call
+00028310: 6564 206f 6e20 7370 6563 6966 6963 2073  ed on specific s
+00028320: 6974 6573 2077 6974 6869 6e20 796f 7572  ites within your
+00028330: 203a 7079 3a63 6c61 7373 3a60 6e69 6469   :py:class:`nidi
+00028340: 6769 7461 6c2e 5365 7373 696f 6e60 2069  gital.Session` i
+00028350: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
+00028360: 2055 7365 2050 7974 686f 6e20 696e 6465   Use Python inde
+00028370: 7820 6e6f 7461 7469 6f6e 206f 6e20 7468  x notation on th
+00028380: 6520 7265 7065 6174 6564 2063 6170 6162  e repeated capab
+00028390: 696c 6974 6965 7320 636f 6e74 6169 6e65  ilities containe
+000283a0: 7220 7369 7465 7320 746f 2073 7065 6369  r sites to speci
+000283b0: 6679 2061 2073 7562 7365 742c 0a20 2020  fy a subset,.   
+000283c0: 2020 2020 2061 6e64 2074 6865 6e20 6361       and then ca
+000283d0: 6c6c 2074 6869 7320 6d65 7468 6f64 206f  ll this method o
+000283e0: 6e20 7468 6520 7265 7375 6c74 2e0a 0a20  n the result... 
+000283f0: 2020 2020 2020 2045 7861 6d70 6c65 3a20         Example: 
+00028400: 3a70 793a 6d65 7468 3a60 6d79 5f73 6573  :py:meth:`my_ses
+00028410: 7369 6f6e 2e73 6974 6573 5b20 2e2e 2e20  sion.sites[ ... 
+00028420: 5d2e 6765 745f 6869 7374 6f72 795f 7261  ].get_history_ra
+00028430: 6d5f 7361 6d70 6c65 5f63 6f75 6e74 600a  m_sample_count`.
+00028440: 0a20 2020 2020 2020 2054 6f20 6361 6c6c  .        To call
+00028450: 2074 6865 206d 6574 686f 6420 6f6e 2061   the method on a
+00028460: 6c6c 2073 6974 6573 2c20 796f 7520 6361  ll sites, you ca
+00028470: 6e20 6361 6c6c 2069 7420 6469 7265 6374  n call it direct
+00028480: 6c79 206f 6e20 7468 6520 3a70 793a 636c  ly on the :py:cl
+00028490: 6173 733a 606e 6964 6967 6974 616c 2e53  ass:`nidigital.S
+000284a0: 6573 7369 6f6e 602e 0a0a 2020 2020 2020  ession`...      
+000284b0: 2020 4578 616d 706c 653a 203a 7079 3a6d    Example: :py:m
+000284c0: 6574 683a 606d 795f 7365 7373 696f 6e2e  eth:`my_session.
+000284d0: 6765 745f 6869 7374 6f72 795f 7261 6d5f  get_history_ram_
+000284e0: 7361 6d70 6c65 5f63 6f75 6e74 600a 0a20  sample_count`.. 
+000284f0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00028500: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
+00028510: 6c65 5f63 6f75 6e74 2028 696e 7429 3a20  le_count (int): 
+00028520: 5468 6520 7265 7475 726e 6564 206e 756d  The returned num
+00028530: 6265 7220 6f66 2073 616d 706c 6573 2074  ber of samples t
+00028540: 6861 7420 4869 7374 6f72 7920 5241 4d20  hat History RAM 
+00028550: 6163 7175 6972 6564 2e0a 0a20 2020 2020  acquired...     
+00028560: 2020 2027 2727 0a20 2020 2020 2020 2073     '''.        s
+00028570: 616d 706c 655f 636f 756e 7420 3d20 7365  ample_count = se
+00028580: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
+00028590: 6765 745f 6869 7374 6f72 795f 7261 6d5f  get_history_ram_
+000285a0: 7361 6d70 6c65 5f63 6f75 6e74 2873 656c  sample_count(sel
+000285b0: 662e 5f72 6570 6561 7465 645f 6361 7061  f._repeated_capa
+000285c0: 6269 6c69 7479 290a 2020 2020 2020 2020  bility).        
+000285d0: 7265 7475 726e 2073 616d 706c 655f 636f  return sample_co
+000285e0: 756e 740a 0a20 2020 2040 6976 695f 7379  unt..    @ivi_sy
+000285f0: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
+00028600: 6566 205f 6765 745f 7061 7474 6572 6e5f  ef _get_pattern_
+00028610: 6e61 6d65 2873 656c 662c 2070 6174 7465  name(self, patte
+00028620: 726e 5f69 6e64 6578 293a 0a20 2020 2020  rn_index):.     
+00028630: 2020 2072 2727 275f 6765 745f 7061 7474     r'''_get_patt
+00028640: 6572 6e5f 6e61 6d65 0a0a 2020 2020 2020  ern_name..      
+00028650: 2020 5442 440a 0a20 2020 2020 2020 2041    TBD..        A
+00028660: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00028670: 2070 6174 7465 726e 5f69 6e64 6578 2028   pattern_index (
+00028680: 696e 7429 3a0a 0a0a 2020 2020 2020 2020  int):...        
+00028690: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000286a0: 2020 2020 206e 616d 6520 2873 7472 293a       name (str):
+000286b0: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+000286c0: 2020 2020 2020 6e61 6d65 203d 2073 656c        name = sel
+000286d0: 662e 5f69 6e74 6572 7072 6574 6572 2e67  f._interpreter.g
+000286e0: 6574 5f70 6174 7465 726e 5f6e 616d 6528  et_pattern_name(
+000286f0: 7061 7474 6572 6e5f 696e 6465 7829 0a20  pattern_index). 
+00028700: 2020 2020 2020 2072 6574 7572 6e20 6e61         return na
+00028710: 6d65 0a0a 2020 2020 4069 7669 5f73 796e  me..    @ivi_syn
+00028720: 6368 726f 6e69 7a65 640a 2020 2020 6465  chronized.    de
+00028730: 6620 5f67 6574 5f70 696e 5f6e 616d 6528  f _get_pin_name(
+00028740: 7365 6c66 2c20 7069 6e5f 696e 6465 7829  self, pin_index)
+00028750: 3a0a 2020 2020 2020 2020 7227 2727 5f67  :.        r'''_g
+00028760: 6574 5f70 696e 5f6e 616d 650a 0a20 2020  et_pin_name..   
+00028770: 2020 2020 2052 6574 7572 6e73 2074 6865       Returns the
+00028780: 206e 616d 6520 6f66 2074 6865 2070 696e   name of the pin
+00028790: 2061 7420 7468 6520 696e 6465 7820 796f   at the index yo
+000287a0: 7520 7370 6563 6966 792e 2059 6f75 206d  u specify. You m
+000287b0: 7573 7420 7072 6f76 6964 6520 6120 5669  ust provide a Vi
+000287c0: 4368 6172 2061 7272 6179 2074 6f20 7365  Char array to se
+000287d0: 7276 6520 6173 2061 2062 7566 6665 7220  rve as a buffer 
+000287e0: 666f 7220 7468 6520 7661 6c75 652e 2059  for the value. Y
+000287f0: 6f75 2070 6173 7320 7468 6520 6e75 6d62  ou pass the numb
+00028800: 6572 206f 6620 6279 7465 7320 696e 2074  er of bytes in t
+00028810: 6865 2062 7566 6665 7220 6173 2074 6865  he buffer as the
+00028820: 202a 2a6e 616d 6542 7566 6665 7253 697a   **nameBufferSiz
+00028830: 652a 2a2e 2049 6620 7468 6520 6375 7272  e**. If the curr
+00028840: 656e 7420 7661 6c75 6520 6f66 2074 6865  ent value of the
+00028850: 2070 726f 7065 7274 792c 2069 6e63 6c75   property, inclu
+00028860: 6469 6e67 2074 6865 2074 6572 6d69 6e61  ding the termina
+00028870: 7469 6e67 204e 554c 4c20 6279 7465 2c20  ting NULL byte, 
+00028880: 6973 206c 6172 6765 7220 7468 616e 2074  is larger than t
+00028890: 6865 2073 697a 6520 796f 7520 696e 6469  he size you indi
+000288a0: 6361 7465 2069 6e20 7468 6520 6275 6666  cate in the buff
+000288b0: 6572 2073 697a 652c 2074 6865 206d 6574  er size, the met
+000288c0: 686f 6420 636f 7069 6573 2028 6275 6666  hod copies (buff
+000288d0: 6572 2073 697a 6520 2d20 3129 2062 7974  er size - 1) byt
+000288e0: 6573 2069 6e74 6f20 7468 6520 6275 6666  es into the buff
+000288f0: 6572 2c20 706c 6163 6573 2061 6e20 4153  er, places an AS
+00028900: 4349 4920 4e55 4c4c 2062 7974 6520 6174  CII NULL byte at
+00028910: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
+00028920: 6275 6666 6572 2c20 616e 6420 7265 7475  buffer, and retu
+00028930: 726e 7320 7468 6520 6275 6666 6572 2073  rns the buffer s
+00028940: 697a 6520 796f 7520 6d75 7374 2070 6173  ize you must pas
+00028950: 7320 746f 2067 6574 2074 6865 2065 6e74  s to get the ent
+00028960: 6972 6520 7661 6c75 652e 2046 6f72 2065  ire value. For e
+00028970: 7861 6d70 6c65 2c20 6966 2074 6865 2076  xample, if the v
+00028980: 616c 7565 2069 7320 2231 3233 3435 3622  alue is "123456"
+00028990: 2061 6e64 2074 6865 2062 7566 6665 7220   and the buffer 
+000289a0: 7369 7a65 2069 7320 342c 2074 6865 206d  size is 4, the m
+000289b0: 6574 686f 6420 706c 6163 6573 2022 3132  ethod places "12
+000289c0: 3322 2069 6e74 6f20 7468 6520 6275 6666  3" into the buff
+000289d0: 6572 2061 6e64 2072 6574 7572 6e73 2037  er and returns 7
+000289e0: 2e20 4966 2079 6f75 2077 616e 7420 746f  . If you want to
+000289f0: 2063 616c 6c20 7468 6973 206d 6574 686f   call this metho
+00028a00: 6420 6a75 7374 2074 6f20 6765 7420 7468  d just to get th
+00028a10: 6520 7265 7175 6972 6564 2062 7566 6665  e required buffe
+00028a20: 7220 7369 7a65 2c20 796f 7520 6361 6e20  r size, you can 
+00028a30: 7061 7373 2030 2066 6f72 202a 2a6e 616d  pass 0 for **nam
+00028a40: 6542 7566 6665 7253 697a 652a 2a20 616e  eBufferSize** an
+00028a50: 6420 5649 5f4e 554c 4c20 666f 7220 7468  d VI_NULL for th
+00028a60: 6520 6e61 6d65 2e0a 0a20 2020 2020 2020  e name...       
+00028a70: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00028a80: 2020 2070 696e 5f69 6e64 6578 2028 696e     pin_index (in
+00028a90: 7429 3a20 496e 6465 7820 6f66 2070 696e  t): Index of pin
+00028aa0: 2074 6f20 7175 6572 792e 2050 696e 2069   to query. Pin i
+00028ab0: 6e64 6578 6573 2062 6567 696e 2061 7420  ndexes begin at 
+00028ac0: 302e 0a0a 0a20 2020 2020 2020 2052 6574  0....        Ret
+00028ad0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00028ae0: 2020 6e61 6d65 2028 7374 7229 3a20 5265    name (str): Re
+00028af0: 7475 726e 7320 7468 6520 7069 6e20 6e61  turns the pin na
+00028b00: 6d65 2061 7420 7468 6520 7370 6563 6966  me at the specif
+00028b10: 6965 6420 2a2a 7069 6e49 6e64 6578 2a2a  ied **pinIndex**
+00028b20: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
+00028b30: 2020 2020 2020 206e 616d 6520 3d20 7365         name = se
+00028b40: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
+00028b50: 6765 745f 7069 6e5f 6e61 6d65 2870 696e  get_pin_name(pin
+00028b60: 5f69 6e64 6578 290a 2020 2020 2020 2020  _index).        
+00028b70: 7265 7475 726e 206e 616d 650a 0a20 2020  return name..   
+00028b80: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
+00028b90: 6564 0a20 2020 2064 6566 205f 6765 745f  ed.    def _get_
+00028ba0: 7069 6e5f 7265 7375 6c74 735f 7069 6e5f  pin_results_pin_
+00028bb0: 696e 666f 726d 6174 696f 6e28 7365 6c66  information(self
+00028bc0: 293a 0a20 2020 2020 2020 2072 2727 275f  ):.        r'''_
+00028bd0: 6765 745f 7069 6e5f 7265 7375 6c74 735f  get_pin_results_
+00028be0: 7069 6e5f 696e 666f 726d 6174 696f 6e0a  pin_information.
+00028bf0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00028c00: 2074 6865 2070 696e 206e 616d 6573 2c20   the pin names, 
+00028c10: 7369 7465 206e 756d 6265 7273 2c20 616e  site numbers, an
+00028c20: 6420 6368 616e 6e65 6c20 6e61 6d65 7320  d channel names 
+00028c30: 7468 6174 2063 6f72 7265 7370 6f6e 6420  that correspond 
+00028c40: 746f 2070 6572 2d70 696e 2064 6174 6120  to per-pin data 
+00028c50: 7265 6164 2066 726f 6d20 7468 6520 6469  read from the di
+00028c60: 6769 7461 6c20 7061 7474 6572 6e20 696e  gital pattern in
+00028c70: 7374 7275 6d65 6e74 2e20 5468 6520 6d65  strument. The me
+00028c80: 7468 6f64 2072 6574 7572 6e73 2070 696e  thod returns pin
+00028c90: 2069 6e66 6f72 6d61 7469 6f6e 2069 6e20   information in 
+00028ca0: 7468 6520 7361 6d65 206f 7264 6572 2061  the same order a
+00028cb0: 7320 7661 6c75 6573 2072 6561 6420 7573  s values read us
+00028cc0: 696e 6720 7468 6520 7265 6164 5f73 7461  ing the read_sta
+00028cd0: 7469 6320 6d65 7468 6f64 2c20 7070 6d75  tic method, ppmu
+00028ce0: 5f6d 6561 7375 7265 206d 6574 686f 642c  _measure method,
+00028cf0: 2061 6e64 2067 6574 5f66 6169 6c5f 636f   and get_fail_co
+00028d00: 756e 7420 6d65 7468 6f64 2e20 5573 6520  unt method. Use 
+00028d10: 7468 6973 206d 6574 686f 6420 746f 206d  this method to m
+00028d20: 6174 6368 2076 616c 7565 7320 7468 6520  atch values the 
+00028d30: 7072 6576 696f 7573 6c79 206c 6973 7465  previously liste
+00028d40: 6420 6d65 7468 6f64 7320 7265 7475 726e  d methods return
+00028d50: 2077 6974 6820 7069 6e73 2c20 7369 7465   with pins, site
+00028d60: 732c 2061 6e64 2069 6e73 7472 756d 656e  s, and instrumen
+00028d70: 7420 6368 616e 6e65 6c73 2e0a 0a20 2020  t channels...   
+00028d80: 2020 2020 2054 6970 3a0a 2020 2020 2020       Tip:.      
+00028d90: 2020 5468 6973 206d 6574 686f 6420 6361    This method ca
+00028da0: 6e20 6265 2063 616c 6c65 6420 6f6e 2073  n be called on s
+00028db0: 7065 6369 6669 6320 6368 616e 6e65 6c73  pecific channels
+00028dc0: 2077 6974 6869 6e20 796f 7572 203a 7079   within your :py
+00028dd0: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
+00028de0: 6c2e 5365 7373 696f 6e60 2069 6e73 7461  l.Session` insta
+00028df0: 6e63 652e 0a20 2020 2020 2020 2055 7365  nce..        Use
+00028e00: 2050 7974 686f 6e20 696e 6465 7820 6e6f   Python index no
+00028e10: 7461 7469 6f6e 206f 6e20 7468 6520 7265  tation on the re
+00028e20: 7065 6174 6564 2063 6170 6162 696c 6974  peated capabilit
+00028e30: 6965 7320 636f 6e74 6169 6e65 7220 6368  ies container ch
+00028e40: 616e 6e65 6c73 2074 6f20 7370 6563 6966  annels to specif
+00028e50: 7920 6120 7375 6273 6574 2c0a 2020 2020  y a subset,.    
+00028e60: 2020 2020 616e 6420 7468 656e 2063 616c      and then cal
+00028e70: 6c20 7468 6973 206d 6574 686f 6420 6f6e  l this method on
+00028e80: 2074 6865 2072 6573 756c 742e 0a0a 2020   the result...  
+00028e90: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
+00028ea0: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
+00028eb0: 696f 6e2e 6368 616e 6e65 6c73 5b20 2e2e  ion.channels[ ..
+00028ec0: 2e20 5d2e 5f67 6574 5f70 696e 5f72 6573  . ]._get_pin_res
+00028ed0: 756c 7473 5f70 696e 5f69 6e66 6f72 6d61  ults_pin_informa
+00028ee0: 7469 6f6e 600a 0a20 2020 2020 2020 2054  tion`..        T
+00028ef0: 6f20 6361 6c6c 2074 6865 206d 6574 686f  o call the metho
+00028f00: 6420 6f6e 2061 6c6c 2063 6861 6e6e 656c  d on all channel
+00028f10: 732c 2079 6f75 2063 616e 2063 616c 6c20  s, you can call 
+00028f20: 6974 2064 6972 6563 746c 7920 6f6e 2074  it directly on t
+00028f30: 6865 203a 7079 3a63 6c61 7373 3a60 6e69  he :py:class:`ni
+00028f40: 6469 6769 7461 6c2e 5365 7373 696f 6e60  digital.Session`
+00028f50: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+00028f60: 6c65 3a20 3a70 793a 6d65 7468 3a60 6d79  le: :py:meth:`my
+00028f70: 5f73 6573 7369 6f6e 2e5f 6765 745f 7069  _session._get_pi
+00028f80: 6e5f 7265 7375 6c74 735f 7069 6e5f 696e  n_results_pin_in
+00028f90: 666f 726d 6174 696f 6e60 0a0a 2020 2020  formation`..    
+00028fa0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00028fb0: 2020 2020 2020 2020 2070 696e 5f69 6e64           pin_ind
+00028fc0: 6578 6573 2028 6c69 7374 206f 6620 696e  exes (list of in
+00028fd0: 7429 3a20 5468 6520 7265 7475 726e 6564  t): The returned
+00028fe0: 2069 6e64 6578 206f 6620 7468 6520 7069   index of the pi
+00028ff0: 6e73 2063 6f72 7265 7370 6f6e 6469 6e67  ns corresponding
+00029000: 2074 6f20 6461 7461 2072 6561 6420 6672   to data read fr
+00029010: 6f6d 2074 6865 2064 6967 6974 616c 2070  om the digital p
+00029020: 6174 7465 726e 2069 6e73 7472 756d 656e  attern instrumen
+00029030: 7420 7573 696e 6720 7468 6520 7370 6563  t using the spec
+00029040: 6966 6965 6420 7265 7065 6174 6564 2063  ified repeated c
+00029050: 6170 6162 696c 6974 6965 732e 2049 6620  apabilities. If 
+00029060: 796f 7520 646f 206e 6f74 2077 616e 7420  you do not want 
+00029070: 746f 2075 7365 2074 6869 7320 7061 7261  to use this para
+00029080: 6d65 7465 722c 2070 6173 7320 5649 5f4e  meter, pass VI_N
+00029090: 554c 4c2e 0a20 2020 2020 2020 2020 2020  ULL..           
+000290a0: 2020 2020 2043 616c 6c20 5f67 6574 5f70       Call _get_p
+000290b0: 696e 5f6e 616d 6520 746f 2067 6574 2074  in_name to get t
+000290c0: 6865 206e 616d 6520 6f66 2074 6865 2070  he name of the p
+000290d0: 696e 2061 7373 6f63 6961 7465 6420 7769  in associated wi
+000290e0: 7468 2061 6e20 696e 6465 782e 0a0a 2020  th an index...  
+000290f0: 2020 2020 2020 2020 2020 7369 7465 5f6e            site_n
+00029100: 756d 6265 7273 2028 6c69 7374 206f 6620  umbers (list of 
+00029110: 696e 7429 3a20 5468 6520 7265 7475 726e  int): The return
+00029120: 6564 2073 6974 6520 6e75 6d62 6572 7320  ed site numbers 
+00029130: 7468 6174 2063 6f72 7265 7370 6f6e 6420  that correspond 
+00029140: 746f 2064 6174 6120 7265 6164 2066 726f  to data read fro
+00029150: 6d20 7468 6520 6469 6769 7461 6c20 7061  m the digital pa
+00029160: 7474 6572 6e20 696e 7374 7275 6d65 6e74  ttern instrument
+00029170: 2075 7369 6e67 2074 6865 2073 7065 6369   using the speci
+00029180: 6669 6564 2072 6570 6561 7465 6420 6361  fied repeated ca
+00029190: 7061 6269 6c69 7469 6573 2e20 4966 2079  pabilities. If y
+000291a0: 6f75 2064 6f20 6e6f 7420 7761 6e74 2074  ou do not want t
+000291b0: 6f20 7573 6520 7468 6973 2070 6172 616d  o use this param
+000291c0: 6574 6572 2c20 7061 7373 2056 495f 4e55  eter, pass VI_NU
+000291d0: 4c4c 2e0a 0a20 2020 2020 2020 2020 2020  LL...           
+000291e0: 2063 6861 6e6e 656c 5f69 6e64 6578 6573   channel_indexes
+000291f0: 2028 6c69 7374 206f 6620 696e 7429 3a20   (list of int): 
+00029200: 5468 6520 7265 7475 726e 6564 2069 6e64  The returned ind
+00029210: 6578 206f 6620 6368 616e 6e65 6c73 2063  ex of channels c
+00029220: 6f72 7265 7370 6f6e 6469 6e67 2074 6f20  orresponding to 
+00029230: 6461 7461 2072 6561 6420 6672 6f6d 2074  data read from t
+00029240: 6865 2064 6967 6974 616c 2070 6174 7465  he digital patte
+00029250: 726e 2069 6e73 7472 756d 656e 7420 7573  rn instrument us
+00029260: 696e 6720 7468 6520 7370 6563 6966 6965  ing the specifie
+00029270: 6420 7265 7065 6174 6564 2063 6170 6162  d repeated capab
+00029280: 696c 6974 6965 732e 2049 6620 796f 7520  ilities. If you 
+00029290: 646f 206e 6f74 2077 616e 7420 746f 2075  do not want to u
+000292a0: 7365 2074 6869 7320 7061 7261 6d65 7465  se this paramete
+000292b0: 722c 2070 6173 7320 5649 5f4e 554c 4c2e  r, pass VI_NULL.
+000292c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000292d0: 2043 616c 6c20 4765 7443 6861 6e6e 656c   Call GetChannel
+000292e0: 4e61 6d65 2074 6f20 6765 7420 7468 6520  Name to get the 
+000292f0: 6e61 6d65 206f 6620 7468 6520 6368 616e  name of the chan
+00029300: 6e65 6c20 6173 736f 6369 6174 6564 2077  nel associated w
+00029310: 6974 6820 616e 2069 6e64 6578 2e20 4368  ith an index. Ch
+00029320: 616e 6e65 6c20 696e 6465 7865 7320 6172  annel indexes ar
+00029330: 6520 6f6e 652d 6261 7365 642e 0a0a 2020  e one-based...  
+00029340: 2020 2020 2020 2020 2020 2020 2020 4e6f                No
+00029350: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
+00029360: 2020 2020 4f6e 6520 6f72 206d 6f72 6520      One or more 
+00029370: 6f66 2074 6865 2072 6566 6572 656e 6365  of the reference
+00029380: 6420 6d65 7468 6f64 7320 6172 6520 6e6f  d methods are no
+00029390: 7420 696e 2074 6865 2050 7974 686f 6e20  t in the Python 
+000293a0: 4150 4920 666f 7220 7468 6973 2064 7269  API for this dri
+000293b0: 7665 722e 0a0a 2020 2020 2020 2020 2727  ver...        ''
+000293c0: 270a 2020 2020 2020 2020 7069 6e5f 696e  '.        pin_in
+000293d0: 6465 7865 732c 2073 6974 655f 6e75 6d62  dexes, site_numb
+000293e0: 6572 732c 2063 6861 6e6e 656c 5f69 6e64  ers, channel_ind
+000293f0: 6578 6573 203d 2073 656c 662e 5f69 6e74  exes = self._int
+00029400: 6572 7072 6574 6572 2e67 6574 5f70 696e  erpreter.get_pin
+00029410: 5f72 6573 756c 7473 5f70 696e 5f69 6e66  _results_pin_inf
+00029420: 6f72 6d61 7469 6f6e 2873 656c 662e 5f72  ormation(self._r
+00029430: 6570 6561 7465 645f 6361 7061 6269 6c69  epeated_capabili
+00029440: 7479 290a 2020 2020 2020 2020 7265 7475  ty).        retu
+00029450: 726e 2070 696e 5f69 6e64 6578 6573 2c20  rn pin_indexes, 
+00029460: 7369 7465 5f6e 756d 6265 7273 2c20 6368  site_numbers, ch
+00029470: 616e 6e65 6c5f 696e 6465 7865 730a 0a20  annel_indexes.. 
+00029480: 2020 2040 6976 695f 7379 6e63 6872 6f6e     @ivi_synchron
+00029490: 697a 6564 0a20 2020 2064 6566 205f 6765  ized.    def _ge
+000294a0: 745f 7369 7465 5f70 6173 735f 6661 696c  t_site_pass_fail
+000294b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000294c0: 7227 2727 5f67 6574 5f73 6974 655f 7061  r'''_get_site_pa
+000294d0: 7373 5f66 6169 6c0a 0a20 2020 2020 2020  ss_fail..       
+000294e0: 2052 6574 7572 6e73 2074 6865 2070 6173   Returns the pas
+000294f0: 7320 6f72 2066 6169 6c20 7265 7375 6c74  s or fail result
+00029500: 7320 666f 7220 6561 6368 2073 6974 652e  s for each site.
+00029510: 0a0a 2020 2020 2020 2020 5469 703a 0a20  ..        Tip:. 
+00029520: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
+00029530: 6f64 2063 616e 2062 6520 6361 6c6c 6564  od can be called
+00029540: 206f 6e20 7370 6563 6966 6963 2073 6974   on specific sit
+00029550: 6573 2077 6974 6869 6e20 796f 7572 203a  es within your :
+00029560: 7079 3a63 6c61 7373 3a60 6e69 6469 6769  py:class:`nidigi
+00029570: 7461 6c2e 5365 7373 696f 6e60 2069 6e73  tal.Session` ins
+00029580: 7461 6e63 652e 0a20 2020 2020 2020 2055  tance..        U
+00029590: 7365 2050 7974 686f 6e20 696e 6465 7820  se Python index 
+000295a0: 6e6f 7461 7469 6f6e 206f 6e20 7468 6520  notation on the 
+000295b0: 7265 7065 6174 6564 2063 6170 6162 696c  repeated capabil
+000295c0: 6974 6965 7320 636f 6e74 6169 6e65 7220  ities container 
+000295d0: 7369 7465 7320 746f 2073 7065 6369 6679  sites to specify
+000295e0: 2061 2073 7562 7365 742c 0a20 2020 2020   a subset,.     
+000295f0: 2020 2061 6e64 2074 6865 6e20 6361 6c6c     and then call
+00029600: 2074 6869 7320 6d65 7468 6f64 206f 6e20   this method on 
+00029610: 7468 6520 7265 7375 6c74 2e0a 0a20 2020  the result...   
+00029620: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
+00029630: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
+00029640: 6f6e 2e73 6974 6573 5b20 2e2e 2e20 5d2e  on.sites[ ... ].
+00029650: 5f67 6574 5f73 6974 655f 7061 7373 5f66  _get_site_pass_f
+00029660: 6169 6c60 0a0a 2020 2020 2020 2020 546f  ail`..        To
+00029670: 2063 616c 6c20 7468 6520 6d65 7468 6f64   call the method
+00029680: 206f 6e20 616c 6c20 7369 7465 732c 2079   on all sites, y
+00029690: 6f75 2063 616e 2063 616c 6c20 6974 2064  ou can call it d
+000296a0: 6972 6563 746c 7920 6f6e 2074 6865 203a  irectly on the :
+000296b0: 7079 3a63 6c61 7373 3a60 6e69 6469 6769  py:class:`nidigi
+000296c0: 7461 6c2e 5365 7373 696f 6e60 2e0a 0a20  tal.Session`... 
+000296d0: 2020 2020 2020 2045 7861 6d70 6c65 3a20         Example: 
+000296e0: 3a70 793a 6d65 7468 3a60 6d79 5f73 6573  :py:meth:`my_ses
+000296f0: 7369 6f6e 2e5f 6765 745f 7369 7465 5f70  sion._get_site_p
+00029700: 6173 735f 6661 696c 600a 0a20 2020 2020  ass_fail`..     
+00029710: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00029720: 2020 2020 2020 2020 7061 7373 5f66 6169          pass_fai
+00029730: 6c20 286c 6973 7420 6f66 2062 6f6f 6c29  l (list of bool)
+00029740: 3a20 5468 6520 7265 7475 726e 6564 2061  : The returned a
+00029750: 7272 6179 206f 6620 7061 7373 2028 5472  rray of pass (Tr
+00029760: 7565 2920 616e 6420 6661 696c 2072 6573  ue) and fail res
+00029770: 756c 7473 2066 6f72 2074 6865 2073 6974  ults for the sit
+00029780: 6573 2079 6f75 2073 7065 6369 6679 2069  es you specify i
+00029790: 6e20 7468 6520 7265 7065 6174 6564 2063  n the repeated c
+000297a0: 6170 6162 696c 6974 6965 732e 2049 6620  apabilities. If 
+000297b0: 7369 7465 7320 7370 616e 206d 756c 7469  sites span multi
+000297c0: 706c 6520 6469 6769 7461 6c20 7061 7474  ple digital patt
+000297d0: 6572 6e20 696e 7374 7275 6d65 6e74 732c  ern instruments,
+000297e0: 2079 6f75 206d 7573 7420 7573 6520 616e   you must use an
+000297f0: 2041 4e44 206f 7065 7261 746f 7220 666f   AND operator fo
+00029800: 7220 7468 6520 7061 7274 6961 6c20 7265  r the partial re
+00029810: 7375 6c74 7320 666f 7220 7468 6f73 6520  sults for those 
+00029820: 7369 7465 7320 7265 7475 726e 6564 2062  sites returned b
+00029830: 7920 6561 6368 2069 6e73 7472 756d 656e  y each instrumen
+00029840: 742e 2049 6620 6120 7369 7465 2069 7320  t. If a site is 
+00029850: 6469 7361 626c 6564 206f 7220 6e6f 7420  disabled or not 
+00029860: 656e 6162 6c65 6420 666f 7220 6275 7273  enabled for burs
+00029870: 742c 2074 6865 206d 6574 686f 6420 646f  t, the method do
+00029880: 6573 206e 6f74 2072 6574 7572 6e20 6461  es not return da
+00029890: 7461 2066 6f72 2074 6861 7420 7369 7465  ta for that site
+000298a0: 2e20 5573 6520 7468 6520 536f 7274 5369  . Use the SortSi
+000298b0: 7465 5265 7375 6c74 7356 6942 6f6f 6c65  teResultsViBoole
+000298c0: 616e 206d 6574 686f 6420 746f 206f 7264  an method to ord
+000298d0: 6572 2061 6e64 2063 6f6d 6269 6e65 2074  er and combine t
+000298e0: 6865 2064 6174 6120 746f 206d 6174 6368  he data to match
+000298f0: 2074 6865 2072 6570 6561 7465 6420 6361   the repeated ca
+00029900: 7061 6269 6c69 7469 6573 2e20 596f 7520  pabilities. You 
+00029910: 6361 6e20 616c 736f 2075 7365 2074 6865  can also use the
+00029920: 205f 6765 745f 7369 7465 5f72 6573 756c   _get_site_resul
+00029930: 7473 5f73 6974 655f 6e75 6d62 6572 7320  ts_site_numbers 
+00029940: 6d65 7468 6f64 2074 6f20 6465 7465 726d  method to determ
+00029950: 696e 6520 7468 6520 6f72 6465 7220 6f66  ine the order of
+00029960: 2074 6865 2073 6974 6573 2072 6574 7572   the sites retur
+00029970: 6e65 6420 6672 6f6d 2074 6869 7320 6d65  ned from this me
+00029980: 7468 6f64 2063 616c 6c20 736f 2074 6861  thod call so tha
+00029990: 7420 796f 7520 6361 6e20 6d61 7463 6820  t you can match 
+000299a0: 7468 6520 7061 7373 2061 7272 6179 2077  the pass array w
+000299b0: 6974 6820 7369 7465 206e 756d 6265 7273  ith site numbers
+000299c0: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
+000299d0: 2020 204e 6f74 653a 0a20 2020 2020 2020     Note:.       
+000299e0: 2020 2020 2020 2020 204f 6e65 206f 7220           One or 
+000299f0: 6d6f 7265 206f 6620 7468 6520 7265 6665  more of the refe
+00029a00: 7265 6e63 6564 206d 6574 686f 6473 2061  renced methods a
+00029a10: 7265 206e 6f74 2069 6e20 7468 6520 5079  re not in the Py
+00029a20: 7468 6f6e 2041 5049 2066 6f72 2074 6869  thon API for thi
+00029a30: 7320 6472 6976 6572 2e0a 0a20 2020 2020  s driver...     
+00029a40: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
+00029a50: 6173 735f 6661 696c 203d 2073 656c 662e  ass_fail = self.
+00029a60: 5f69 6e74 6572 7072 6574 6572 2e67 6574  _interpreter.get
+00029a70: 5f73 6974 655f 7061 7373 5f66 6169 6c28  _site_pass_fail(
+00029a80: 7365 6c66 2e5f 7265 7065 6174 6564 5f63  self._repeated_c
+00029a90: 6170 6162 696c 6974 7929 0a20 2020 2020  apability).     
+00029aa0: 2020 2072 6574 7572 6e20 7061 7373 5f66     return pass_f
+00029ab0: 6169 6c0a 0a20 2020 2040 6976 695f 7379  ail..    @ivi_sy
+00029ac0: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
+00029ad0: 6566 205f 6765 745f 7369 7465 5f72 6573  ef _get_site_res
+00029ae0: 756c 7473 5f73 6974 655f 6e75 6d62 6572  ults_site_number
+00029af0: 7328 7365 6c66 2c20 7369 7465 5f72 6573  s(self, site_res
+00029b00: 756c 745f 7479 7065 293a 0a20 2020 2020  ult_type):.     
+00029b10: 2020 2072 2727 275f 6765 745f 7369 7465     r'''_get_site
+00029b20: 5f72 6573 756c 7473 5f73 6974 655f 6e75  _results_site_nu
+00029b30: 6d62 6572 730a 0a20 2020 2020 2020 2052  mbers..        R
+00029b40: 6574 7572 6e73 2074 6865 2073 6974 6520  eturns the site 
+00029b50: 6e75 6d62 6572 7320 7468 6174 2063 6f72  numbers that cor
+00029b60: 7265 7370 6f6e 6420 746f 2070 6572 2d73  respond to per-s
+00029b70: 6974 6520 6461 7461 2072 6561 6420 6672  ite data read fr
+00029b80: 6f6d 2074 6865 2064 6967 6974 616c 2070  om the digital p
+00029b90: 6174 7465 726e 2069 6e73 7472 756d 656e  attern instrumen
+00029ba0: 742e 2054 6865 206d 6574 686f 6420 7265  t. The method re
+00029bb0: 7475 726e 7320 7369 7465 206e 756d 6265  turns site numbe
+00029bc0: 7273 2069 6e20 7468 6520 7361 6d65 206f  rs in the same o
+00029bd0: 7264 6572 2061 7320 7661 6c75 6573 2072  rder as values r
+00029be0: 6561 6420 7573 696e 6720 7468 6520 5f67  ead using the _g
+00029bf0: 6574 5f73 6974 655f 7061 7373 5f66 6169  et_site_pass_fai
+00029c00: 6c20 616e 6420 6665 7463 685f 6361 7074  l and fetch_capt
+00029c10: 7572 655f 7761 7665 666f 726d 5f75 3332  ure_waveform_u32
+00029c20: 206d 6574 686f 6473 2e20 5573 6520 7468   methods. Use th
+00029c30: 6973 206d 6574 686f 6420 746f 206d 6174  is method to mat
+00029c40: 6368 2076 616c 7565 7320 7468 6520 7072  ch values the pr
+00029c50: 6576 696f 7573 6c79 206c 6973 7465 6420  eviously listed 
+00029c60: 6d65 7468 6f64 7320 7265 7475 726e 2077  methods return w
+00029c70: 6974 6820 7369 7465 206e 756d 6265 7273  ith site numbers
+00029c80: 2e0a 0a20 2020 2020 2020 2054 6970 3a0a  ...        Tip:.
+00029c90: 2020 2020 2020 2020 5468 6973 206d 6574          This met
+00029ca0: 686f 6420 6361 6e20 6265 2063 616c 6c65  hod can be calle
+00029cb0: 6420 6f6e 2073 7065 6369 6669 6320 7369  d on specific si
+00029cc0: 7465 7320 7769 7468 696e 2079 6f75 7220  tes within your 
+00029cd0: 3a70 793a 636c 6173 733a 606e 6964 6967  :py:class:`nidig
+00029ce0: 6974 616c 2e53 6573 7369 6f6e 6020 696e  ital.Session` in
+00029cf0: 7374 616e 6365 2e0a 2020 2020 2020 2020  stance..        
+00029d00: 5573 6520 5079 7468 6f6e 2069 6e64 6578  Use Python index
+00029d10: 206e 6f74 6174 696f 6e20 6f6e 2074 6865   notation on the
+00029d20: 2072 6570 6561 7465 6420 6361 7061 6269   repeated capabi
+00029d30: 6c69 7469 6573 2063 6f6e 7461 696e 6572  lities container
+00029d40: 2073 6974 6573 2074 6f20 7370 6563 6966   sites to specif
+00029d50: 7920 6120 7375 6273 6574 2c0a 2020 2020  y a subset,.    
+00029d60: 2020 2020 616e 6420 7468 656e 2063 616c      and then cal
+00029d70: 6c20 7468 6973 206d 6574 686f 6420 6f6e  l this method on
+00029d80: 2074 6865 2072 6573 756c 742e 0a0a 2020   the result...  
+00029d90: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
+00029da0: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
+00029db0: 696f 6e2e 7369 7465 735b 202e 2e2e 205d  ion.sites[ ... ]
+00029dc0: 2e5f 6765 745f 7369 7465 5f72 6573 756c  ._get_site_resul
+00029dd0: 7473 5f73 6974 655f 6e75 6d62 6572 7360  ts_site_numbers`
+00029de0: 0a0a 2020 2020 2020 2020 546f 2063 616c  ..        To cal
+00029df0: 6c20 7468 6520 6d65 7468 6f64 206f 6e20  l the method on 
+00029e00: 616c 6c20 7369 7465 732c 2079 6f75 2063  all sites, you c
+00029e10: 616e 2063 616c 6c20 6974 2064 6972 6563  an call it direc
+00029e20: 746c 7920 6f6e 2074 6865 203a 7079 3a63  tly on the :py:c
+00029e30: 6c61 7373 3a60 6e69 6469 6769 7461 6c2e  lass:`nidigital.
+00029e40: 5365 7373 696f 6e60 2e0a 0a20 2020 2020  Session`...     
+00029e50: 2020 2045 7861 6d70 6c65 3a20 3a70 793a     Example: :py:
+00029e60: 6d65 7468 3a60 6d79 5f73 6573 7369 6f6e  meth:`my_session
+00029e70: 2e5f 6765 745f 7369 7465 5f72 6573 756c  ._get_site_resul
+00029e80: 7473 5f73 6974 655f 6e75 6d62 6572 7360  ts_site_numbers`
+00029e90: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00029ea0: 2020 2020 2020 2020 2020 2020 7369 7465              site
+00029eb0: 5f72 6573 756c 745f 7479 7065 2028 656e  _result_type (en
+00029ec0: 756d 732e 5369 7465 5265 7375 6c74 5479  ums.SiteResultTy
+00029ed0: 7065 293a 2054 6865 2074 7970 6520 6f66  pe): The type of
+00029ee0: 2064 6174 6120 7370 6563 6966 6965 6420   data specified 
+00029ef0: 696e 2074 6865 2072 6573 756c 7473 2061  in the results a
+00029f00: 7272 6179 2e0a 0a20 2020 2020 2020 2020  rray...         
+00029f10: 2020 2020 2020 202d 2020 205f 5369 7465         -   _Site
+00029f20: 5265 7375 6c74 5479 7065 2e50 4153 535f  ResultType.PASS_
+00029f30: 4641 494c 3a20 4765 7420 7369 7465 206e  FAIL: Get site n
+00029f40: 756d 6265 7273 2066 6f72 2070 6173 732f  umbers for pass/
+00029f50: 6661 696c 2064 6174 612e 0a20 2020 2020  fail data..     
+00029f60: 2020 2020 2020 2020 2020 202d 2020 205f             -   _
+00029f70: 5369 7465 5265 7375 6c74 5479 7065 2e43  SiteResultType.C
+00029f80: 4150 5455 5245 5f57 4156 4546 4f52 4d3a  APTURE_WAVEFORM:
+00029f90: 2047 6574 2073 6974 6520 6e75 6d62 6572   Get site number
+00029fa0: 7320 666f 7220 6361 7074 7572 6520 7761  s for capture wa
+00029fb0: 7665 666f 726d 732e 0a0a 0a20 2020 2020  veforms....     
+00029fc0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00029fd0: 2020 2020 2020 2020 7369 7465 5f6e 756d          site_num
+00029fe0: 6265 7273 2028 6c69 7374 206f 6620 696e  bers (list of in
+00029ff0: 7429 3a20 5468 6520 7265 7475 726e 6564  t): The returned
+0002a000: 2061 7272 6179 206f 6620 7369 7465 206e   array of site n
+0002a010: 756d 6265 7273 2074 6861 7420 636f 7272  umbers that corr
+0002a020: 6573 706f 6e64 2074 6f20 7468 6520 7661  espond to the va
+0002a030: 6c75 6573 2073 7065 6369 6669 6564 2062  lues specified b
+0002a040: 7920 2a2a 7369 7465 5265 7375 6c74 5479  y **siteResultTy
+0002a050: 7065 2a2a 2e0a 0a20 2020 2020 2020 2027  pe**...        '
+0002a060: 2727 0a20 2020 2020 2020 2069 6620 7479  ''.        if ty
+0002a070: 7065 2873 6974 655f 7265 7375 6c74 5f74  pe(site_result_t
+0002a080: 7970 6529 2069 7320 6e6f 7420 656e 756d  ype) is not enum
+0002a090: 732e 5f53 6974 6552 6573 756c 7454 7970  s._SiteResultTyp
+0002a0a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002a0b0: 6169 7365 2054 7970 6545 7272 6f72 2827  aise TypeError('
+0002a0c0: 5061 7261 6d65 7465 7220 7369 7465 5f72  Parameter site_r
+0002a0d0: 6573 756c 745f 7479 7065 206d 7573 7420  esult_type must 
+0002a0e0: 6265 206f 6620 7479 7065 2027 202b 2073  be of type ' + s
+0002a0f0: 7472 2865 6e75 6d73 2e5f 5369 7465 5265  tr(enums._SiteRe
+0002a100: 7375 6c74 5479 7065 2929 0a20 2020 2020  sultType)).     
+0002a110: 2020 2073 6974 655f 6e75 6d62 6572 7320     site_numbers 
+0002a120: 3d20 7365 6c66 2e5f 696e 7465 7270 7265  = self._interpre
+0002a130: 7465 722e 6765 745f 7369 7465 5f72 6573  ter.get_site_res
+0002a140: 756c 7473 5f73 6974 655f 6e75 6d62 6572  ults_site_number
+0002a150: 7328 7365 6c66 2e5f 7265 7065 6174 6564  s(self._repeated
+0002a160: 5f63 6170 6162 696c 6974 792c 2073 6974  _capability, sit
+0002a170: 655f 7265 7375 6c74 5f74 7970 6529 0a20  e_result_type). 
+0002a180: 2020 2020 2020 2072 6574 7572 6e20 7369         return si
+0002a190: 7465 5f6e 756d 6265 7273 0a0a 2020 2020  te_numbers..    
+0002a1a0: 4069 7669 5f73 796e 6368 726f 6e69 7a65  @ivi_synchronize
+0002a1b0: 640a 2020 2020 6465 6620 6765 745f 7469  d.    def get_ti
+0002a1c0: 6d65 5f73 6574 5f64 7269 7665 5f66 6f72  me_set_drive_for
+0002a1d0: 6d61 7428 7365 6c66 2c20 7469 6d65 5f73  mat(self, time_s
+0002a1e0: 6574 5f6e 616d 6529 3a0a 2020 2020 2020  et_name):.      
+0002a1f0: 2020 7227 2727 6765 745f 7469 6d65 5f73    r'''get_time_s
+0002a200: 6574 5f64 7269 7665 5f66 6f72 6d61 740a  et_drive_format.
+0002a210: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0002a220: 2074 6865 2064 7269 7665 2066 6f72 6d61   the drive forma
+0002a230: 7420 6f66 2061 2070 696e 2069 6e20 7468  t of a pin in th
+0002a240: 6520 7370 6563 6966 6965 6420 7469 6d65  e specified time
+0002a250: 2073 6574 2e0a 0a20 2020 2020 2020 2054   set...        T
+0002a260: 6970 3a0a 2020 2020 2020 2020 5468 6973  ip:.        This
+0002a270: 206d 6574 686f 6420 6361 6e20 6265 2063   method can be c
+0002a280: 616c 6c65 6420 6f6e 2073 7065 6369 6669  alled on specifi
+0002a290: 6320 7069 6e73 2077 6974 6869 6e20 796f  c pins within yo
+0002a2a0: 7572 203a 7079 3a63 6c61 7373 3a60 6e69  ur :py:class:`ni
+0002a2b0: 6469 6769 7461 6c2e 5365 7373 696f 6e60  digital.Session`
+0002a2c0: 2069 6e73 7461 6e63 652e 0a20 2020 2020   instance..     
+0002a2d0: 2020 2055 7365 2050 7974 686f 6e20 696e     Use Python in
+0002a2e0: 6465 7820 6e6f 7461 7469 6f6e 206f 6e20  dex notation on 
+0002a2f0: 7468 6520 7265 7065 6174 6564 2063 6170  the repeated cap
+0002a300: 6162 696c 6974 6965 7320 636f 6e74 6169  abilities contai
+0002a310: 6e65 7220 7069 6e73 2074 6f20 7370 6563  ner pins to spec
+0002a320: 6966 7920 6120 7375 6273 6574 2c0a 2020  ify a subset,.  
+0002a330: 2020 2020 2020 616e 6420 7468 656e 2063        and then c
+0002a340: 616c 6c20 7468 6973 206d 6574 686f 6420  all this method 
+0002a350: 6f6e 2074 6865 2072 6573 756c 742e 0a0a  on the result...
+0002a360: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+0002a370: 203a 7079 3a6d 6574 683a 606d 795f 7365   :py:meth:`my_se
+0002a380: 7373 696f 6e2e 7069 6e73 5b20 2e2e 2e20  ssion.pins[ ... 
+0002a390: 5d2e 6765 745f 7469 6d65 5f73 6574 5f64  ].get_time_set_d
+0002a3a0: 7269 7665 5f66 6f72 6d61 7460 0a0a 2020  rive_format`..  
+0002a3b0: 2020 2020 2020 546f 2063 616c 6c20 7468        To call th
+0002a3c0: 6520 6d65 7468 6f64 206f 6e20 616c 6c20  e method on all 
+0002a3d0: 7069 6e73 2c20 796f 7520 6361 6e20 6361  pins, you can ca
+0002a3e0: 6c6c 2069 7420 6469 7265 6374 6c79 206f  ll it directly o
+0002a3f0: 6e20 7468 6520 3a70 793a 636c 6173 733a  n the :py:class:
+0002a400: 606e 6964 6967 6974 616c 2e53 6573 7369  `nidigital.Sessi
+0002a410: 6f6e 602e 0a0a 2020 2020 2020 2020 4578  on`...        Ex
+0002a420: 616d 706c 653a 203a 7079 3a6d 6574 683a  ample: :py:meth:
+0002a430: 606d 795f 7365 7373 696f 6e2e 6765 745f  `my_session.get_
+0002a440: 7469 6d65 5f73 6574 5f64 7269 7665 5f66  time_set_drive_f
+0002a450: 6f72 6d61 7460 0a0a 2020 2020 2020 2020  ormat`..        
+0002a460: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+0002a470: 2020 7469 6d65 5f73 6574 5f6e 616d 6520    time_set_name 
+0002a480: 2873 7472 293a 2054 6865 2073 7065 6369  (str): The speci
+0002a490: 6669 6564 2074 696d 6520 7365 7420 6e61  fied time set na
+0002a4a0: 6d65 2e0a 0a0a 2020 2020 2020 2020 5265  me....        Re
+0002a4b0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0002a4c0: 2020 2066 6f72 6d61 7420 2865 6e75 6d73     format (enums
+0002a4d0: 2e44 7269 7665 466f 726d 6174 293a 2052  .DriveFormat): R
+0002a4e0: 6574 7572 6e65 6420 6472 6976 6520 666f  eturned drive fo
+0002a4f0: 726d 6174 206f 6620 7468 6520 7469 6d65  rmat of the time
+0002a500: 2073 6574 2066 6f72 2074 6865 2073 7065   set for the spe
+0002a510: 6369 6669 6564 2070 696e 2e0a 0a20 2020  cified pin...   
+0002a520: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+0002a530: 2066 6f72 6d61 7420 3d20 7365 6c66 2e5f   format = self._
+0002a540: 696e 7465 7270 7265 7465 722e 6765 745f  interpreter.get_
+0002a550: 7469 6d65 5f73 6574 5f64 7269 7665 5f66  time_set_drive_f
+0002a560: 6f72 6d61 7428 7365 6c66 2e5f 7265 7065  ormat(self._repe
+0002a570: 6174 6564 5f63 6170 6162 696c 6974 792c  ated_capability,
+0002a580: 2074 696d 655f 7365 745f 6e61 6d65 290a   time_set_name).
+0002a590: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+0002a5a0: 6f72 6d61 740a 0a20 2020 2040 6976 695f  ormat..    @ivi_
+0002a5b0: 7379 6e63 6872 6f6e 697a 6564 0a20 2020  synchronized.   
+0002a5c0: 2064 6566 2067 6574 5f74 696d 655f 7365   def get_time_se
+0002a5d0: 745f 6564 6765 2873 656c 662c 2074 696d  t_edge(self, tim
+0002a5e0: 655f 7365 745f 6e61 6d65 2c20 6564 6765  e_set_name, edge
+0002a5f0: 293a 0a20 2020 2020 2020 2072 2727 2767  ):.        r'''g
+0002a600: 6574 5f74 696d 655f 7365 745f 6564 6765  et_time_set_edge
+0002a610: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0002a620: 7320 7468 6520 6564 6765 2074 696d 6520  s the edge time 
+0002a630: 6f66 2061 2070 696e 2069 6e20 7468 6520  of a pin in the 
+0002a640: 7370 6563 6966 6965 6420 7469 6d65 2073  specified time s
+0002a650: 6574 2e0a 0a20 2020 2020 2020 2054 6970  et...        Tip
+0002a660: 3a0a 2020 2020 2020 2020 5468 6973 206d  :.        This m
+0002a670: 6574 686f 6420 6361 6e20 6265 2063 616c  ethod can be cal
+0002a680: 6c65 6420 6f6e 2073 7065 6369 6669 6320  led on specific 
+0002a690: 7069 6e73 2077 6974 6869 6e20 796f 7572  pins within your
+0002a6a0: 203a 7079 3a63 6c61 7373 3a60 6e69 6469   :py:class:`nidi
+0002a6b0: 6769 7461 6c2e 5365 7373 696f 6e60 2069  gital.Session` i
+0002a6c0: 6e73 7461 6e63 652e 0a20 2020 2020 2020  nstance..       
+0002a6d0: 2055 7365 2050 7974 686f 6e20 696e 6465   Use Python inde
+0002a6e0: 7820 6e6f 7461 7469 6f6e 206f 6e20 7468  x notation on th
+0002a6f0: 6520 7265 7065 6174 6564 2063 6170 6162  e repeated capab
+0002a700: 696c 6974 6965 7320 636f 6e74 6169 6e65  ilities containe
+0002a710: 7220 7069 6e73 2074 6f20 7370 6563 6966  r pins to specif
+0002a720: 7920 6120 7375 6273 6574 2c0a 2020 2020  y a subset,.    
+0002a730: 2020 2020 616e 6420 7468 656e 2063 616c      and then cal
+0002a740: 6c20 7468 6973 206d 6574 686f 6420 6f6e  l this method on
+0002a750: 2074 6865 2072 6573 756c 742e 0a0a 2020   the result...  
+0002a760: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
+0002a770: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
+0002a780: 696f 6e2e 7069 6e73 5b20 2e2e 2e20 5d2e  ion.pins[ ... ].
+0002a790: 6765 745f 7469 6d65 5f73 6574 5f65 6467  get_time_set_edg
+0002a7a0: 6560 0a0a 2020 2020 2020 2020 546f 2063  e`..        To c
+0002a7b0: 616c 6c20 7468 6520 6d65 7468 6f64 206f  all the method o
+0002a7c0: 6e20 616c 6c20 7069 6e73 2c20 796f 7520  n all pins, you 
+0002a7d0: 6361 6e20 6361 6c6c 2069 7420 6469 7265  can call it dire
+0002a7e0: 6374 6c79 206f 6e20 7468 6520 3a70 793a  ctly on the :py:
+0002a7f0: 636c 6173 733a 606e 6964 6967 6974 616c  class:`nidigital
+0002a800: 2e53 6573 7369 6f6e 602e 0a0a 2020 2020  .Session`...    
+0002a810: 2020 2020 4578 616d 706c 653a 203a 7079      Example: :py
+0002a820: 3a6d 6574 683a 606d 795f 7365 7373 696f  :meth:`my_sessio
+0002a830: 6e2e 6765 745f 7469 6d65 5f73 6574 5f65  n.get_time_set_e
+0002a840: 6467 6560 0a0a 2020 2020 2020 2020 4172  dge`..        Ar
+0002a850: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0002a860: 7469 6d65 5f73 6574 5f6e 616d 6520 2873  time_set_name (s
+0002a870: 7472 293a 2054 6865 2073 7065 6369 6669  tr): The specifi
+0002a880: 6564 2074 696d 6520 7365 7420 6e61 6d65  ed time set name
+0002a890: 2e0a 0a20 2020 2020 2020 2020 2020 2065  ...            e
+0002a8a0: 6467 6520 2865 6e75 6d73 2e54 696d 6553  dge (enums.TimeS
+0002a8b0: 6574 4564 6765 5479 7065 293a 204e 616d  etEdgeType): Nam
+0002a8c0: 6520 6f66 2074 6865 2065 6467 652e 0a0a  e of the edge...
+0002a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a8e0: 2d20 2020 5469 6d65 5365 7445 6467 6554  -   TimeSetEdgeT
+0002a8f0: 7970 652e 4452 4956 455f 4f4e 0a20 2020  ype.DRIVE_ON.   
+0002a900: 2020 2020 2020 2020 2020 2020 202d 2020               -  
+0002a910: 2054 696d 6553 6574 4564 6765 5479 7065   TimeSetEdgeType
+0002a920: 2e44 5249 5645 5f44 4154 410a 2020 2020  .DRIVE_DATA.    
+0002a930: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
+0002a940: 5469 6d65 5365 7445 6467 6554 7970 652e  TimeSetEdgeType.
+0002a950: 4452 4956 455f 5245 5455 524e 0a20 2020  DRIVE_RETURN.   
+0002a960: 2020 2020 2020 2020 2020 2020 202d 2020               -  
+0002a970: 2054 696d 6553 6574 4564 6765 5479 7065   TimeSetEdgeType
+0002a980: 2e44 5249 5645 5f4f 4646 0a20 2020 2020  .DRIVE_OFF.     
+0002a990: 2020 2020 2020 2020 2020 202d 2020 2054             -   T
+0002a9a0: 696d 6553 6574 4564 6765 5479 7065 2e43  imeSetEdgeType.C
+0002a9b0: 4f4d 5041 5245 5f53 5452 4f42 450a 2020  OMPARE_STROBE.  
+0002a9c0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+0002a9d0: 2020 5469 6d65 5365 7445 6467 6554 7970    TimeSetEdgeTyp
+0002a9e0: 652e 4452 4956 455f 4441 5441 320a 2020  e.DRIVE_DATA2.  
+0002a9f0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+0002aa00: 2020 5469 6d65 5365 7445 6467 6554 7970    TimeSetEdgeTyp
+0002aa10: 652e 4452 4956 455f 5245 5455 524e 320a  e.DRIVE_RETURN2.
+0002aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002aa30: 2d20 2020 5469 6d65 5365 7445 6467 6554  -   TimeSetEdgeT
+0002aa40: 7970 652e 434f 4d50 4152 455f 5354 524f  ype.COMPARE_STRO
+0002aa50: 4245 320a 0a0a 2020 2020 2020 2020 5265  BE2...        Re
+0002aa60: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0002aa70: 2020 2074 696d 6520 2868 6967 6874 696d     time (hightim
+0002aa80: 652e 7469 6d65 6465 6c74 6129 3a20 5469  e.timedelta): Ti
+0002aa90: 6d65 2066 726f 6d20 7468 6520 6265 6769  me from the begi
+0002aaa0: 6e6e 696e 6720 6f66 2074 6865 2076 6563  nning of the vec
+0002aab0: 746f 7220 7065 7269 6f64 2069 6e20 7768  tor period in wh
+0002aac0: 6963 6820 746f 2070 6c61 6365 2074 6865  ich to place the
+0002aad0: 2065 6467 652e 0a0a 2020 2020 2020 2020   edge...        
+0002aae0: 2727 270a 2020 2020 2020 2020 6966 2074  '''.        if t
+0002aaf0: 7970 6528 6564 6765 2920 6973 206e 6f74  ype(edge) is not
+0002ab00: 2065 6e75 6d73 2e54 696d 6553 6574 4564   enums.TimeSetEd
+0002ab10: 6765 5479 7065 3a0a 2020 2020 2020 2020  geType:.        
+0002ab20: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+0002ab30: 726f 7228 2750 6172 616d 6574 6572 2065  ror('Parameter e
+0002ab40: 6467 6520 6d75 7374 2062 6520 6f66 2074  dge must be of t
+0002ab50: 7970 6520 2720 2b20 7374 7228 656e 756d  ype ' + str(enum
+0002ab60: 732e 5469 6d65 5365 7445 6467 6554 7970  s.TimeSetEdgeTyp
+0002ab70: 6529 290a 2020 2020 2020 2020 7469 6d65  e)).        time
+0002ab80: 203d 2073 656c 662e 5f69 6e74 6572 7072   = self._interpr
+0002ab90: 6574 6572 2e67 6574 5f74 696d 655f 7365  eter.get_time_se
+0002aba0: 745f 6564 6765 2873 656c 662e 5f72 6570  t_edge(self._rep
+0002abb0: 6561 7465 645f 6361 7061 6269 6c69 7479  eated_capability
+0002abc0: 2c20 7469 6d65 5f73 6574 5f6e 616d 652c  , time_set_name,
+0002abd0: 2065 6467 6529 0a20 2020 2020 2020 2072   edge).        r
+0002abe0: 6574 7572 6e20 5f63 6f6e 7665 7274 6572  eturn _converter
+0002abf0: 732e 636f 6e76 6572 745f 7365 636f 6e64  s.convert_second
+0002ac00: 735f 7265 616c 3634 5f74 6f5f 7469 6d65  s_real64_to_time
+0002ac10: 6465 6c74 6128 7469 6d65 290a 0a20 2020  delta(time)..   
+0002ac20: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
+0002ac30: 6564 0a20 2020 2064 6566 2067 6574 5f74  ed.    def get_t
+0002ac40: 696d 655f 7365 745f 6564 6765 5f6d 756c  ime_set_edge_mul
+0002ac50: 7469 706c 6965 7228 7365 6c66 2c20 7469  tiplier(self, ti
+0002ac60: 6d65 5f73 6574 5f6e 616d 6529 3a0a 2020  me_set_name):.  
+0002ac70: 2020 2020 2020 7227 2727 6765 745f 7469        r'''get_ti
+0002ac80: 6d65 5f73 6574 5f65 6467 655f 6d75 6c74  me_set_edge_mult
+0002ac90: 6970 6c69 6572 0a0a 2020 2020 2020 2020  iplier..        
+0002aca0: 5265 7475 726e 7320 7468 6520 6564 6765  Returns the edge
+0002acb0: 206d 756c 7469 706c 6965 7220 6f66 2074   multiplier of t
+0002acc0: 6865 2073 7065 6369 6669 6564 2074 696d  he specified tim
+0002acd0: 6520 7365 742e 0a0a 2020 2020 2020 2020  e set...        
+0002ace0: 5469 703a 0a20 2020 2020 2020 2054 6869  Tip:.        Thi
+0002acf0: 7320 6d65 7468 6f64 2063 616e 2062 6520  s method can be 
+0002ad00: 6361 6c6c 6564 206f 6e20 7370 6563 6966  called on specif
+0002ad10: 6963 2070 696e 7320 7769 7468 696e 2079  ic pins within y
+0002ad20: 6f75 7220 3a70 793a 636c 6173 733a 606e  our :py:class:`n
+0002ad30: 6964 6967 6974 616c 2e53 6573 7369 6f6e  idigital.Session
+0002ad40: 6020 696e 7374 616e 6365 2e0a 2020 2020  ` instance..    
+0002ad50: 2020 2020 5573 6520 5079 7468 6f6e 2069      Use Python i
+0002ad60: 6e64 6578 206e 6f74 6174 696f 6e20 6f6e  ndex notation on
+0002ad70: 2074 6865 2072 6570 6561 7465 6420 6361   the repeated ca
+0002ad80: 7061 6269 6c69 7469 6573 2063 6f6e 7461  pabilities conta
+0002ad90: 696e 6572 2070 696e 7320 746f 2073 7065  iner pins to spe
+0002ada0: 6369 6679 2061 2073 7562 7365 742c 0a20  cify a subset,. 
+0002adb0: 2020 2020 2020 2061 6e64 2074 6865 6e20         and then 
+0002adc0: 6361 6c6c 2074 6869 7320 6d65 7468 6f64  call this method
+0002add0: 206f 6e20 7468 6520 7265 7375 6c74 2e0a   on the result..
+0002ade0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+0002adf0: 3a20 3a70 793a 6d65 7468 3a60 6d79 5f73  : :py:meth:`my_s
+0002ae00: 6573 7369 6f6e 2e70 696e 735b 202e 2e2e  ession.pins[ ...
+0002ae10: 205d 2e67 6574 5f74 696d 655f 7365 745f   ].get_time_set_
+0002ae20: 6564 6765 5f6d 756c 7469 706c 6965 7260  edge_multiplier`
+0002ae30: 0a0a 2020 2020 2020 2020 546f 2063 616c  ..        To cal
+0002ae40: 6c20 7468 6520 6d65 7468 6f64 206f 6e20  l the method on 
+0002ae50: 616c 6c20 7069 6e73 2c20 796f 7520 6361  all pins, you ca
+0002ae60: 6e20 6361 6c6c 2069 7420 6469 7265 6374  n call it direct
+0002ae70: 6c79 206f 6e20 7468 6520 3a70 793a 636c  ly on the :py:cl
+0002ae80: 6173 733a 606e 6964 6967 6974 616c 2e53  ass:`nidigital.S
+0002ae90: 6573 7369 6f6e 602e 0a0a 2020 2020 2020  ession`...      
+0002aea0: 2020 4578 616d 706c 653a 203a 7079 3a6d    Example: :py:m
+0002aeb0: 6574 683a 606d 795f 7365 7373 696f 6e2e  eth:`my_session.
+0002aec0: 6765 745f 7469 6d65 5f73 6574 5f65 6467  get_time_set_edg
+0002aed0: 655f 6d75 6c74 6970 6c69 6572 600a 0a20  e_multiplier`.. 
+0002aee0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0002aef0: 2020 2020 2020 2020 2074 696d 655f 7365           time_se
+0002af00: 745f 6e61 6d65 2028 7374 7229 3a20 5468  t_name (str): Th
+0002af10: 6520 7370 6563 6966 6965 6420 7469 6d65  e specified time
+0002af20: 2073 6574 206e 616d 652e 0a0a 0a20 2020   set name....   
+0002af30: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0002af40: 2020 2020 2020 2020 2020 6564 6765 5f6d            edge_m
+0002af50: 756c 7469 706c 6965 7220 2869 6e74 293a  ultiplier (int):
+0002af60: 2052 6574 7572 6e65 6420 6564 6765 206d   Returned edge m
+0002af70: 756c 7469 706c 6965 7220 6f66 2074 6865  ultiplier of the
+0002af80: 2074 696d 6520 7365 7420 666f 7220 7468   time set for th
+0002af90: 6520 7370 6563 6966 6965 6420 7069 6e2e  e specified pin.
+0002afa0: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+0002afb0: 2020 2020 2020 6564 6765 5f6d 756c 7469        edge_multi
+0002afc0: 706c 6965 7220 3d20 7365 6c66 2e5f 696e  plier = self._in
+0002afd0: 7465 7270 7265 7465 722e 6765 745f 7469  terpreter.get_ti
+0002afe0: 6d65 5f73 6574 5f65 6467 655f 6d75 6c74  me_set_edge_mult
+0002aff0: 6970 6c69 6572 2873 656c 662e 5f72 6570  iplier(self._rep
+0002b000: 6561 7465 645f 6361 7061 6269 6c69 7479  eated_capability
+0002b010: 2c20 7469 6d65 5f73 6574 5f6e 616d 6529  , time_set_name)
+0002b020: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002b030: 6564 6765 5f6d 756c 7469 706c 6965 720a  edge_multiplier.
+0002b040: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
+0002b050: 6f6e 697a 6564 0a20 2020 2064 6566 205f  onized.    def _
+0002b060: 6765 745f 7469 6d65 5f73 6574 5f6e 616d  get_time_set_nam
+0002b070: 6528 7365 6c66 2c20 7469 6d65 5f73 6574  e(self, time_set
+0002b080: 5f69 6e64 6578 293a 0a20 2020 2020 2020  _index):.       
+0002b090: 2072 2727 275f 6765 745f 7469 6d65 5f73   r'''_get_time_s
+0002b0a0: 6574 5f6e 616d 650a 0a20 2020 2020 2020  et_name..       
+0002b0b0: 2054 4244 0a0a 2020 2020 2020 2020 4172   TBD..        Ar
+0002b0c0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0002b0d0: 7469 6d65 5f73 6574 5f69 6e64 6578 2028  time_set_index (
+0002b0e0: 696e 7429 3a0a 0a0a 2020 2020 2020 2020  int):...        
+0002b0f0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0002b100: 2020 2020 206e 616d 6520 2873 7472 293a       name (str):
+0002b110: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+0002b120: 2020 2020 2020 6e61 6d65 203d 2073 656c        name = sel
+0002b130: 662e 5f69 6e74 6572 7072 6574 6572 2e67  f._interpreter.g
+0002b140: 6574 5f74 696d 655f 7365 745f 6e61 6d65  et_time_set_name
+0002b150: 2874 696d 655f 7365 745f 696e 6465 7829  (time_set_index)
+0002b160: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002b170: 6e61 6d65 0a0a 2020 2020 4069 7669 5f73  name..    @ivi_s
+0002b180: 796e 6368 726f 6e69 7a65 640a 2020 2020  ynchronized.    
+0002b190: 6465 6620 6973 5f73 6974 655f 656e 6162  def is_site_enab
+0002b1a0: 6c65 6428 7365 6c66 293a 0a20 2020 2020  led(self):.     
+0002b1b0: 2020 2072 2727 2769 735f 7369 7465 5f65     r'''is_site_e
+0002b1c0: 6e61 626c 6564 0a0a 2020 2020 2020 2020  nabled..        
+0002b1d0: 4368 6563 6b73 2069 6620 6120 7370 6563  Checks if a spec
+0002b1e0: 6966 6965 6420 7369 7465 2069 7320 656e  ified site is en
+0002b1f0: 6162 6c65 642e 0a0a 2020 2020 2020 2020  abled...        
+0002b200: 4e6f 7465 3a20 5468 6520 6d65 7468 6f64  Note: The method
+0002b210: 2072 6574 7572 6e73 2061 6e20 6572 726f   returns an erro
+0002b220: 7220 6966 206d 6f72 6520 7468 616e 206f  r if more than o
+0002b230: 6e65 2073 6974 6520 6973 2073 7065 6369  ne site is speci
+0002b240: 6669 6564 2e0a 0a20 2020 2020 2020 2054  fied...        T
+0002b250: 6970 3a0a 2020 2020 2020 2020 5468 6973  ip:.        This
+0002b260: 206d 6574 686f 6420 6361 6e20 6265 2063   method can be c
+0002b270: 616c 6c65 6420 6f6e 2073 7065 6369 6669  alled on specifi
+0002b280: 6320 7369 7465 7320 7769 7468 696e 2079  c sites within y
+0002b290: 6f75 7220 3a70 793a 636c 6173 733a 606e  our :py:class:`n
+0002b2a0: 6964 6967 6974 616c 2e53 6573 7369 6f6e  idigital.Session
+0002b2b0: 6020 696e 7374 616e 6365 2e0a 2020 2020  ` instance..    
+0002b2c0: 2020 2020 5573 6520 5079 7468 6f6e 2069      Use Python i
+0002b2d0: 6e64 6578 206e 6f74 6174 696f 6e20 6f6e  ndex notation on
+0002b2e0: 2074 6865 2072 6570 6561 7465 6420 6361   the repeated ca
+0002b2f0: 7061 6269 6c69 7469 6573 2063 6f6e 7461  pabilities conta
+0002b300: 696e 6572 2073 6974 6573 2074 6f20 7370  iner sites to sp
+0002b310: 6563 6966 7920 6120 7375 6273 6574 2c0a  ecify a subset,.
+0002b320: 2020 2020 2020 2020 616e 6420 7468 656e          and then
+0002b330: 2063 616c 6c20 7468 6973 206d 6574 686f   call this metho
+0002b340: 6420 6f6e 2074 6865 2072 6573 756c 742e  d on the result.
+0002b350: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
+0002b360: 653a 203a 7079 3a6d 6574 683a 606d 795f  e: :py:meth:`my_
+0002b370: 7365 7373 696f 6e2e 7369 7465 735b 202e  session.sites[ .
+0002b380: 2e2e 205d 2e69 735f 7369 7465 5f65 6e61  .. ].is_site_ena
+0002b390: 626c 6564 600a 0a20 2020 2020 2020 2054  bled`..        T
+0002b3a0: 6f20 6361 6c6c 2074 6865 206d 6574 686f  o call the metho
+0002b3b0: 6420 6f6e 2061 6c6c 2073 6974 6573 2c20  d on all sites, 
+0002b3c0: 796f 7520 6361 6e20 6361 6c6c 2069 7420  you can call it 
+0002b3d0: 6469 7265 6374 6c79 206f 6e20 7468 6520  directly on the 
+0002b3e0: 3a70 793a 636c 6173 733a 606e 6964 6967  :py:class:`nidig
+0002b3f0: 6974 616c 2e53 6573 7369 6f6e 602e 0a0a  ital.Session`...
+0002b400: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+0002b410: 203a 7079 3a6d 6574 683a 606d 795f 7365   :py:meth:`my_se
+0002b420: 7373 696f 6e2e 6973 5f73 6974 655f 656e  ssion.is_site_en
+0002b430: 6162 6c65 6460 0a0a 2020 2020 2020 2020  abled`..        
+0002b440: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0002b450: 2020 2020 2065 6e61 626c 6520 2862 6f6f       enable (boo
+0002b460: 6c29 3a20 426f 6f6c 6561 6e20 7661 6c75  l): Boolean valu
+0002b470: 6520 7468 6174 2072 6574 7572 6e73 2077  e that returns w
+0002b480: 6865 7468 6572 2074 6865 2073 6974 6520  hether the site 
+0002b490: 6973 2065 6e61 626c 6564 206f 7220 6469  is enabled or di
+0002b4a0: 7361 626c 6564 2e0a 0a20 2020 2020 2020  sabled...       
+0002b4b0: 2027 2727 0a20 2020 2020 2020 2065 6e61   '''.        ena
+0002b4c0: 626c 6520 3d20 7365 6c66 2e5f 696e 7465  ble = self._inte
+0002b4d0: 7270 7265 7465 722e 6973 5f73 6974 655f  rpreter.is_site_
+0002b4e0: 656e 6162 6c65 6428 7365 6c66 2e5f 7265  enabled(self._re
+0002b4f0: 7065 6174 6564 5f63 6170 6162 696c 6974  peated_capabilit
+0002b500: 7929 0a20 2020 2020 2020 2072 6574 7572  y).        retur
+0002b510: 6e20 656e 6162 6c65 0a0a 2020 2020 6465  n enable..    de
+0002b520: 6620 6c6f 636b 2873 656c 6629 3a0a 2020  f lock(self):.  
+0002b530: 2020 2020 2020 2727 276c 6f63 6b0a 0a20        '''lock.. 
+0002b540: 2020 2020 2020 204f 6274 6169 6e73 2061         Obtains a
+0002b550: 206d 756c 7469 7468 7265 6164 206c 6f63   multithread loc
+0002b560: 6b20 6f6e 2074 6865 2064 6576 6963 6520  k on the device 
+0002b570: 7365 7373 696f 6e2e 2042 6566 6f72 6520  session. Before 
+0002b580: 646f 696e 6720 736f 2c20 7468 650a 2020  doing so, the.  
+0002b590: 2020 2020 2020 736f 6674 7761 7265 2077        software w
+0002b5a0: 6169 7473 2075 6e74 696c 2061 6c6c 206f  aits until all o
+0002b5b0: 7468 6572 2065 7865 6375 7469 6f6e 2074  ther execution t
+0002b5c0: 6872 6561 6473 2072 656c 6561 7365 2074  hreads release t
+0002b5d0: 6865 6972 206c 6f63 6b73 0a20 2020 2020  heir locks.     
+0002b5e0: 2020 206f 6e20 7468 6520 6465 7669 6365     on the device
+0002b5f0: 2073 6573 7369 6f6e 2e0a 0a20 2020 2020   session...     
+0002b600: 2020 204f 7468 6572 2074 6872 6561 6473     Other threads
+0002b610: 206d 6179 2068 6176 6520 6f62 7461 696e   may have obtain
+0002b620: 6564 2061 206c 6f63 6b20 6f6e 2074 6869  ed a lock on thi
+0002b630: 7320 7365 7373 696f 6e20 666f 7220 7468  s session for th
+0002b640: 650a 2020 2020 2020 2020 666f 6c6c 6f77  e.        follow
+0002b650: 696e 6720 7265 6173 6f6e 733a 0a0a 2020  ing reasons:..  
+0002b660: 2020 2020 2020 2020 2020 2d20 2054 6865            -  The
+0002b670: 2061 7070 6c69 6361 7469 6f6e 2063 616c   application cal
+0002b680: 6c65 6420 7468 6520 6c6f 636b 206d 6574  led the lock met
+0002b690: 686f 642e 0a20 2020 2020 2020 2020 2020  hod..           
+0002b6a0: 202d 2020 4120 6361 6c6c 2074 6f20 4e49   -  A call to NI
+0002b6b0: 2d44 6967 6974 616c 2050 6174 7465 726e  -Digital Pattern
+0002b6c0: 2044 7269 7665 7220 6c6f 636b 6564 2074   Driver locked t
+0002b6d0: 6865 2073 6573 7369 6f6e 2e0a 2020 2020  he session..    
+0002b6e0: 2020 2020 2020 2020 2d20 2041 6674 6572          -  After
+0002b6f0: 2061 2063 616c 6c20 746f 2074 6865 206c   a call to the l
+0002b700: 6f63 6b20 6d65 7468 6f64 2072 6574 7572  ock method retur
+0002b710: 6e73 0a20 2020 2020 2020 2020 2020 2020  ns.             
+0002b720: 2020 7375 6363 6573 7366 756c 6c79 2c20    successfully, 
+0002b730: 6e6f 206f 7468 6572 2074 6872 6561 6473  no other threads
+0002b740: 2063 616e 2061 6363 6573 7320 7468 6520   can access the 
+0002b750: 6465 7669 6365 2073 6573 7369 6f6e 2075  device session u
+0002b760: 6e74 696c 0a20 2020 2020 2020 2020 2020  ntil.           
+0002b770: 2020 2020 796f 7520 6361 6c6c 2074 6865      you call the
+0002b780: 2075 6e6c 6f63 6b20 6d65 7468 6f64 206f   unlock method o
+0002b790: 7220 6578 6974 206f 7574 206f 6620 7468  r exit out of th
+0002b7a0: 6520 7769 7468 2062 6c6f 636b 2077 6865  e with block whe
+0002b7b0: 6e20 7573 696e 670a 2020 2020 2020 2020  n using.        
+0002b7c0: 2020 2020 2020 206c 6f63 6b20 636f 6e74         lock cont
+0002b7d0: 6578 7420 6d61 6e61 6765 722e 0a20 2020  ext manager..   
+0002b7e0: 2020 2020 2020 2020 202d 2020 5573 6520           -  Use 
+0002b7f0: 7468 6520 6c6f 636b 206d 6574 686f 6420  the lock method 
+0002b800: 616e 6420 7468 650a 2020 2020 2020 2020  and the.        
+0002b810: 2020 2020 2020 2075 6e6c 6f63 6b20 6d65         unlock me
+0002b820: 7468 6f64 2061 726f 756e 6420 6120 7365  thod around a se
+0002b830: 7175 656e 6365 206f 6620 6361 6c6c 7320  quence of calls 
+0002b840: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
+0002b850: 2020 696e 7374 7275 6d65 6e74 2064 7269    instrument dri
+0002b860: 7665 7220 6d65 7468 6f64 7320 6966 2079  ver methods if y
+0002b870: 6f75 2072 6571 7569 7265 2074 6861 7420  ou require that 
+0002b880: 7468 6520 6465 7669 6365 2072 6574 6169  the device retai
+0002b890: 6e20 6974 730a 2020 2020 2020 2020 2020  n its.          
+0002b8a0: 2020 2020 2073 6574 7469 6e67 7320 7468       settings th
+0002b8b0: 726f 7567 6820 7468 6520 656e 6420 6f66  rough the end of
+0002b8c0: 2074 6865 2073 6571 7565 6e63 652e 0a0a   the sequence...
+0002b8d0: 2020 2020 2020 2020 596f 7520 6361 6e20          You can 
+0002b8e0: 7361 6665 6c79 206d 616b 6520 6e65 7374  safely make nest
+0002b8f0: 6564 2063 616c 6c73 2074 6f20 7468 6520  ed calls to the 
+0002b900: 6c6f 636b 206d 6574 686f 640a 2020 2020  lock method.    
+0002b910: 2020 2020 7769 7468 696e 2074 6865 2073      within the s
+0002b920: 616d 6520 7468 7265 6164 2e20 546f 2063  ame thread. To c
+0002b930: 6f6d 706c 6574 656c 7920 756e 6c6f 636b  ompletely unlock
+0002b940: 2074 6865 2073 6573 7369 6f6e 2c20 796f   the session, yo
+0002b950: 7520 6d75 7374 0a20 2020 2020 2020 2062  u must.        b
+0002b960: 616c 616e 6365 2065 6163 6820 6361 6c6c  alance each call
+0002b970: 2074 6f20 7468 6520 6c6f 636b 206d 6574   to the lock met
+0002b980: 686f 6420 7769 7468 2061 2063 616c 6c20  hod with a call 
+0002b990: 746f 0a20 2020 2020 2020 2074 6865 2075  to.        the u
+0002b9a0: 6e6c 6f63 6b20 6d65 7468 6f64 2e0a 0a20  nlock method... 
+0002b9b0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0002b9c0: 2020 2020 2020 2020 2020 2020 6c6f 636b              lock
+0002b9d0: 2028 636f 6e74 6578 7420 6d61 6e61 6765   (context manage
+0002b9e0: 7229 3a20 5768 656e 2075 7365 6420 696e  r): When used in
+0002b9f0: 2061 2077 6974 6820 7374 6174 656d 656e   a with statemen
+0002ba00: 742c 206e 6964 6967 6974 616c 2e53 6573  t, nidigital.Ses
+0002ba10: 7369 6f6e 2e6c 6f63 6b20 6163 7473 2061  sion.lock acts a
+0002ba20: 730a 2020 2020 2020 2020 2020 2020 6120  s.            a 
+0002ba30: 636f 6e74 6578 7420 6d61 6e61 6765 7220  context manager 
+0002ba40: 616e 6420 756e 6c6f 636b 2077 696c 6c20  and unlock will 
+0002ba50: 6265 2063 616c 6c65 6420 7768 656e 2074  be called when t
+0002ba60: 6865 2077 6974 6820 626c 6f63 6b20 6973  he with block is
+0002ba70: 2065 7869 7465 640a 2020 2020 2020 2020   exited.        
+0002ba80: 2727 270a 2020 2020 2020 2020 7365 6c66  '''.        self
+0002ba90: 2e5f 696e 7465 7270 7265 7465 722e 6c6f  ._interpreter.lo
+0002baa0: 636b 2829 2020 2320 5765 2064 6f20 6e6f  ck()  # We do no
+0002bab0: 7420 6361 6c6c 2074 6869 7320 696e 2074  t call this in t
+0002bac0: 6865 2063 6f6e 7465 7874 206d 616e 6167  he context manag
+0002bad0: 6572 2073 6f20 7468 6174 2074 6869 7320  er so that this 
+0002bae0: 6675 6e63 7469 6f6e 2063 616e 0a20 2020  function can.   
+0002baf0: 2020 2020 2023 2061 6374 2073 7461 6e64       # act stand
+0002bb00: 616c 6f6e 6520 6173 2077 656c 6c20 616e  alone as well an
+0002bb10: 6420 6c65 7420 7468 6520 636c 6965 6e74  d let the client
+0002bb20: 2063 616c 6c20 756e 6c6f 636b 2829 2065   call unlock() e
+0002bb30: 7870 6c69 6369 746c 792e 2049 6620 7468  xplicitly. If th
+0002bb40: 6579 2064 6f20 7573 6520 7468 6520 636f  ey do use the co
+0002bb50: 6e74 6578 7420 6d61 6e61 6765 722c 0a20  ntext manager,. 
+0002bb60: 2020 2020 2020 2023 2074 6861 7420 7769         # that wi
+0002bb70: 6c6c 2068 616e 646c 6520 7468 6520 756e  ll handle the un
+0002bb80: 6c6f 636b 2066 6f72 2074 6865 6d0a 2020  lock for them.  
+0002bb90: 2020 2020 2020 7265 7475 726e 205f 4c6f        return _Lo
+0002bba0: 636b 2873 656c 6629 0a0a 2020 2020 4069  ck(self)..    @i
+0002bbb0: 7669 5f73 796e 6368 726f 6e69 7a65 640a  vi_synchronized.
+0002bbc0: 2020 2020 6465 6620 7070 6d75 5f6d 6561      def ppmu_mea
+0002bbd0: 7375 7265 2873 656c 662c 206d 6561 7375  sure(self, measu
+0002bbe0: 7265 6d65 6e74 5f74 7970 6529 3a0a 2020  rement_type):.  
+0002bbf0: 2020 2020 2020 7227 2727 7070 6d75 5f6d        r'''ppmu_m
+0002bc00: 6561 7375 7265 0a0a 2020 2020 2020 2020  easure..        
+0002bc10: 496e 7374 7275 6374 7320 7468 6520 5050  Instructs the PP
+0002bc20: 4d55 2074 6f20 6d65 6173 7572 6520 766f  MU to measure vo
+0002bc30: 6c74 6167 6520 6f72 2063 7572 7265 6e74  ltage or current
+0002bc40: 2e20 5468 6973 206d 6574 686f 6420 6361  . This method ca
+0002bc50: 6e20 6265 2063 616c 6c65 6420 746f 2074  n be called to t
+0002bc60: 616b 6520 6120 766f 6c74 6167 6520 6d65  ake a voltage me
+0002bc70: 6173 7572 656d 656e 7420 6576 656e 2069  asurement even i
+0002bc80: 6620 7468 6520 7069 6e20 6d65 7468 6f64  f the pin method
+0002bc90: 2069 7320 6e6f 7420 7365 7420 746f 2050   is not set to P
+0002bca0: 504d 552e 0a0a 2020 2020 2020 2020 5469  PMU...        Ti
+0002bcb0: 703a 0a20 2020 2020 2020 2054 6869 7320  p:.        This 
+0002bcc0: 6d65 7468 6f64 2063 616e 2062 6520 6361  method can be ca
+0002bcd0: 6c6c 6564 206f 6e20 7370 6563 6966 6963  lled on specific
+0002bce0: 2063 6861 6e6e 656c 7320 7769 7468 696e   channels within
+0002bcf0: 2079 6f75 7220 3a70 793a 636c 6173 733a   your :py:class:
+0002bd00: 606e 6964 6967 6974 616c 2e53 6573 7369  `nidigital.Sessi
+0002bd10: 6f6e 6020 696e 7374 616e 6365 2e0a 2020  on` instance..  
+0002bd20: 2020 2020 2020 5573 6520 5079 7468 6f6e        Use Python
+0002bd30: 2069 6e64 6578 206e 6f74 6174 696f 6e20   index notation 
+0002bd40: 6f6e 2074 6865 2072 6570 6561 7465 6420  on the repeated 
+0002bd50: 6361 7061 6269 6c69 7469 6573 2063 6f6e  capabilities con
+0002bd60: 7461 696e 6572 2063 6861 6e6e 656c 7320  tainer channels 
+0002bd70: 746f 2073 7065 6369 6679 2061 2073 7562  to specify a sub
+0002bd80: 7365 742c 0a20 2020 2020 2020 2061 6e64  set,.        and
+0002bd90: 2074 6865 6e20 6361 6c6c 2074 6869 7320   then call this 
+0002bda0: 6d65 7468 6f64 206f 6e20 7468 6520 7265  method on the re
+0002bdb0: 7375 6c74 2e0a 0a20 2020 2020 2020 2045  sult...        E
+0002bdc0: 7861 6d70 6c65 3a20 3a70 793a 6d65 7468  xample: :py:meth
+0002bdd0: 3a60 6d79 5f73 6573 7369 6f6e 2e63 6861  :`my_session.cha
+0002bde0: 6e6e 656c 735b 202e 2e2e 205d 2e70 706d  nnels[ ... ].ppm
+0002bdf0: 755f 6d65 6173 7572 6560 0a0a 2020 2020  u_measure`..    
+0002be00: 2020 2020 546f 2063 616c 6c20 7468 6520      To call the 
+0002be10: 6d65 7468 6f64 206f 6e20 616c 6c20 6368  method on all ch
+0002be20: 616e 6e65 6c73 2c20 796f 7520 6361 6e20  annels, you can 
+0002be30: 6361 6c6c 2069 7420 6469 7265 6374 6c79  call it directly
+0002be40: 206f 6e20 7468 6520 3a70 793a 636c 6173   on the :py:clas
+0002be50: 733a 606e 6964 6967 6974 616c 2e53 6573  s:`nidigital.Ses
+0002be60: 7369 6f6e 602e 0a0a 2020 2020 2020 2020  sion`...        
+0002be70: 4578 616d 706c 653a 203a 7079 3a6d 6574  Example: :py:met
+0002be80: 683a 606d 795f 7365 7373 696f 6e2e 7070  h:`my_session.pp
+0002be90: 6d75 5f6d 6561 7375 7265 600a 0a20 2020  mu_measure`..   
+0002bea0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0002beb0: 2020 2020 2020 206d 6561 7375 7265 6d65         measureme
+0002bec0: 6e74 5f74 7970 6520 2865 6e75 6d73 2e50  nt_type (enums.P
+0002bed0: 504d 554d 6561 7375 7265 6d65 6e74 5479  PMUMeasurementTy
+0002bee0: 7065 293a 2050 6172 616d 6574 6572 2074  pe): Parameter t
+0002bef0: 6861 7420 7370 6563 6966 6965 7320 7768  hat specifies wh
+0002bf00: 6574 6865 7220 7468 6520 5050 4d55 206d  ether the PPMU m
+0002bf10: 6561 7375 7265 7320 766f 6c74 6167 6520  easures voltage 
+0002bf20: 6f72 2063 7572 7265 6e74 2066 726f 6d20  or current from 
+0002bf30: 7468 6520 4455 542e 0a0a 2020 2020 2020  the DUT...      
+0002bf40: 2020 2020 2020 2020 2020 2d20 2020 5050            -   PP
+0002bf50: 4d55 4d65 6173 7572 656d 656e 7454 7970  MUMeasurementTyp
+0002bf60: 652e 4355 5252 454e 543a 2054 6865 2050  e.CURRENT: The P
+0002bf70: 504d 5520 6d65 6173 7572 6573 2063 7572  PMU measures cur
+0002bf80: 7265 6e74 2066 726f 6d20 7468 6520 4455  rent from the DU
+0002bf90: 542e 0a20 2020 2020 2020 2020 2020 2020  T..             
+0002bfa0: 2020 202d 2020 2050 504d 554d 6561 7375     -   PPMUMeasu
+0002bfb0: 7265 6d65 6e74 5479 7065 2e56 4f4c 5441  rementType.VOLTA
+0002bfc0: 4745 3a20 5468 6520 5050 4d55 206d 6561  GE: The PPMU mea
+0002bfd0: 7375 7265 7320 766f 6c74 6167 6520 6672  sures voltage fr
+0002bfe0: 6f6d 2074 6865 2044 5554 2e0a 0a0a 2020  om the DUT....  
+0002bff0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+0002c000: 2020 2020 2020 2020 2020 206d 6561 7375             measu
+0002c010: 7265 6d65 6e74 7320 286c 6973 7420 6f66  rements (list of
+0002c020: 2066 6c6f 6174 293a 2054 6865 2072 6574   float): The ret
+0002c030: 7572 6e65 6420 6172 7261 7920 6f66 206d  urned array of m
+0002c040: 6561 7375 7265 6d65 6e74 7320 696e 2074  easurements in t
+0002c050: 6865 206f 7264 6572 2079 6f75 2073 7065  he order you spe
+0002c060: 6369 6679 2069 6e20 7468 6520 7265 7065  cify in the repe
+0002c070: 6174 6564 2063 6170 6162 696c 6974 6965  ated capabilitie
+0002c080: 732e 2049 6620 6120 7369 7465 2069 7320  s. If a site is 
+0002c090: 6469 7361 626c 6564 2c20 7468 6520 6d65  disabled, the me
+0002c0a0: 7468 6f64 2064 6f65 7320 6e6f 7420 7265  thod does not re
+0002c0b0: 7475 726e 2064 6174 6120 666f 7220 7468  turn data for th
+0002c0c0: 6174 2073 6974 652e 2059 6f75 2063 616e  at site. You can
+0002c0d0: 2061 6c73 6f20 7573 6520 7468 6520 6765   also use the ge
+0002c0e0: 745f 7069 6e5f 7265 7375 6c74 735f 7069  t_pin_results_pi
+0002c0f0: 6e5f 696e 666f 726d 6174 696f 6e20 6d65  n_information me
+0002c100: 7468 6f64 2074 6f20 6f62 7461 696e 2061  thod to obtain a
+0002c110: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
+0002c120: 7265 7475 726e 6564 2073 6974 6573 2061  returned sites a
+0002c130: 6e64 2063 6861 6e6e 656c 732e 0a0a 2020  nd channels...  
+0002c140: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+0002c150: 2020 6966 2074 7970 6528 6d65 6173 7572    if type(measur
+0002c160: 656d 656e 745f 7479 7065 2920 6973 206e  ement_type) is n
+0002c170: 6f74 2065 6e75 6d73 2e50 504d 554d 6561  ot enums.PPMUMea
+0002c180: 7375 7265 6d65 6e74 5479 7065 3a0a 2020  surementType:.  
+0002c190: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0002c1a0: 5479 7065 4572 726f 7228 2750 6172 616d  TypeError('Param
+0002c1b0: 6574 6572 206d 6561 7375 7265 6d65 6e74  eter measurement
+0002c1c0: 5f74 7970 6520 6d75 7374 2062 6520 6f66  _type must be of
+0002c1d0: 2074 7970 6520 2720 2b20 7374 7228 656e   type ' + str(en
+0002c1e0: 756d 732e 5050 4d55 4d65 6173 7572 656d  ums.PPMUMeasurem
+0002c1f0: 656e 7454 7970 6529 290a 2020 2020 2020  entType)).      
+0002c200: 2020 6d65 6173 7572 656d 656e 7473 203d    measurements =
+0002c210: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
+0002c220: 6572 2e70 706d 755f 6d65 6173 7572 6528  er.ppmu_measure(
+0002c230: 7365 6c66 2e5f 7265 7065 6174 6564 5f63  self._repeated_c
+0002c240: 6170 6162 696c 6974 792c 206d 6561 7375  apability, measu
+0002c250: 7265 6d65 6e74 5f74 7970 6529 0a20 2020  rement_type).   
+0002c260: 2020 2020 2072 6574 7572 6e20 6d65 6173       return meas
+0002c270: 7572 656d 656e 7473 0a0a 2020 2020 4069  urements..    @i
+0002c280: 7669 5f73 796e 6368 726f 6e69 7a65 640a  vi_synchronized.
+0002c290: 2020 2020 6465 6620 7070 6d75 5f73 6f75      def ppmu_sou
+0002c2a0: 7263 6528 7365 6c66 293a 0a20 2020 2020  rce(self):.     
+0002c2b0: 2020 2072 2727 2770 706d 755f 736f 7572     r'''ppmu_sour
+0002c2c0: 6365 0a0a 2020 2020 2020 2020 5374 6172  ce..        Star
+0002c2d0: 7473 2073 6f75 7263 696e 6720 766f 6c74  ts sourcing volt
+0002c2e0: 6167 6520 6f72 2063 7572 7265 6e74 2066  age or current f
+0002c2f0: 726f 6d20 7468 6520 5050 4d55 2e20 5468  rom the PPMU. Th
+0002c300: 6973 206d 6574 686f 6420 6175 746f 6d61  is method automa
+0002c310: 7469 6361 6c6c 7920 7365 6c65 6374 7320  tically selects 
+0002c320: 7468 6520 5050 4d55 206d 6574 686f 642e  the PPMU method.
+0002c330: 2043 6861 6e67 6573 2074 6f20 5050 4d55   Changes to PPMU
+0002c340: 2073 6f75 7263 6520 7365 7474 696e 6773   source settings
+0002c350: 2064 6f20 6e6f 7420 7461 6b65 2065 6666   do not take eff
+0002c360: 6563 7420 756e 7469 6c20 796f 7520 6361  ect until you ca
+0002c370: 6c6c 2074 6869 7320 6d65 7468 6f64 2e20  ll this method. 
+0002c380: 4966 2079 6f75 206d 6f64 6966 7920 736f  If you modify so
+0002c390: 7572 6365 2073 6574 7469 6e67 7320 6166  urce settings af
+0002c3a0: 7465 7220 796f 7520 6361 6c6c 2074 6869  ter you call thi
+0002c3b0: 7320 6d65 7468 6f64 2c20 796f 7520 6d75  s method, you mu
+0002c3c0: 7374 2063 616c 6c20 7468 6973 206d 6574  st call this met
+0002c3d0: 686f 6420 6167 6169 6e20 666f 7220 6368  hod again for ch
+0002c3e0: 616e 6765 7320 696e 2074 6865 2063 6f6e  anges in the con
+0002c3f0: 6669 6775 7261 7469 6f6e 2074 6f20 7461  figuration to ta
+0002c400: 6b65 2065 6666 6563 742e 0a0a 2020 2020  ke effect...    
+0002c410: 2020 2020 5469 703a 0a20 2020 2020 2020      Tip:.       
+0002c420: 2054 6869 7320 6d65 7468 6f64 2063 616e   This method can
+0002c430: 2062 6520 6361 6c6c 6564 206f 6e20 7370   be called on sp
+0002c440: 6563 6966 6963 2063 6861 6e6e 656c 7320  ecific channels 
+0002c450: 7769 7468 696e 2079 6f75 7220 3a70 793a  within your :py:
+0002c460: 636c 6173 733a 606e 6964 6967 6974 616c  class:`nidigital
+0002c470: 2e53 6573 7369 6f6e 6020 696e 7374 616e  .Session` instan
+0002c480: 6365 2e0a 2020 2020 2020 2020 5573 6520  ce..        Use 
+0002c490: 5079 7468 6f6e 2069 6e64 6578 206e 6f74  Python index not
+0002c4a0: 6174 696f 6e20 6f6e 2074 6865 2072 6570  ation on the rep
+0002c4b0: 6561 7465 6420 6361 7061 6269 6c69 7469  eated capabiliti
+0002c4c0: 6573 2063 6f6e 7461 696e 6572 2063 6861  es container cha
+0002c4d0: 6e6e 656c 7320 746f 2073 7065 6369 6679  nnels to specify
+0002c4e0: 2061 2073 7562 7365 742c 0a20 2020 2020   a subset,.     
+0002c4f0: 2020 2061 6e64 2074 6865 6e20 6361 6c6c     and then call
+0002c500: 2074 6869 7320 6d65 7468 6f64 206f 6e20   this method on 
+0002c510: 7468 6520 7265 7375 6c74 2e0a 0a20 2020  the result...   
+0002c520: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
+0002c530: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
+0002c540: 6f6e 2e63 6861 6e6e 656c 735b 202e 2e2e  on.channels[ ...
+0002c550: 205d 2e70 706d 755f 736f 7572 6365 600a   ].ppmu_source`.
+0002c560: 0a20 2020 2020 2020 2054 6f20 6361 6c6c  .        To call
+0002c570: 2074 6865 206d 6574 686f 6420 6f6e 2061   the method on a
+0002c580: 6c6c 2063 6861 6e6e 656c 732c 2079 6f75  ll channels, you
+0002c590: 2063 616e 2063 616c 6c20 6974 2064 6972   can call it dir
+0002c5a0: 6563 746c 7920 6f6e 2074 6865 203a 7079  ectly on the :py
+0002c5b0: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
+0002c5c0: 6c2e 5365 7373 696f 6e60 2e0a 0a20 2020  l.Session`...   
+0002c5d0: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
+0002c5e0: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
+0002c5f0: 6f6e 2e70 706d 755f 736f 7572 6365 600a  on.ppmu_source`.
+0002c600: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+0002c610: 2020 2020 7365 6c66 2e5f 696e 7465 7270      self._interp
+0002c620: 7265 7465 722e 7070 6d75 5f73 6f75 7263  reter.ppmu_sourc
+0002c630: 6528 7365 6c66 2e5f 7265 7065 6174 6564  e(self._repeated
+0002c640: 5f63 6170 6162 696c 6974 7929 0a0a 2020  _capability)..  
+0002c650: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
+0002c660: 7a65 640a 2020 2020 6465 6620 7265 6164  zed.    def read
+0002c670: 5f73 7461 7469 6328 7365 6c66 293a 0a20  _static(self):. 
+0002c680: 2020 2020 2020 2072 2727 2772 6561 645f         r'''read_
+0002c690: 7374 6174 6963 0a0a 2020 2020 2020 2020  static..        
+0002c6a0: 5265 6164 7320 7468 6520 6375 7272 656e  Reads the curren
+0002c6b0: 7420 7374 6174 6520 6f66 2063 6f6d 7061  t state of compa
+0002c6c0: 7261 746f 7273 2066 6f72 2070 696e 7320  rators for pins 
+0002c6d0: 796f 7520 7370 6563 6966 7920 696e 2074  you specify in t
+0002c6e0: 6865 2072 6570 6561 7465 6420 6361 7061  he repeated capa
+0002c6f0: 6269 6c69 7469 6573 2e20 4966 2074 6865  bilities. If the
+0002c700: 7265 2061 7265 2075 6e63 6f6d 6d69 7474  re are uncommitt
+0002c710: 6564 2063 6861 6e67 6573 2074 6f20 6c65  ed changes to le
+0002c720: 7665 6c73 206f 7220 7468 6520 7465 726d  vels or the term
+0002c730: 696e 6174 696f 6e20 6d6f 6465 2c20 7468  ination mode, th
+0002c740: 6973 206d 6574 686f 6420 636f 6d6d 6974  is method commit
+0002c750: 7320 7468 6520 6368 616e 6765 7320 746f  s the changes to
+0002c760: 2074 6865 2070 696e 732e 0a0a 2020 2020   the pins...    
+0002c770: 2020 2020 5469 703a 0a20 2020 2020 2020      Tip:.       
+0002c780: 2054 6869 7320 6d65 7468 6f64 2063 616e   This method can
+0002c790: 2062 6520 6361 6c6c 6564 206f 6e20 7370   be called on sp
+0002c7a0: 6563 6966 6963 2063 6861 6e6e 656c 7320  ecific channels 
+0002c7b0: 7769 7468 696e 2079 6f75 7220 3a70 793a  within your :py:
+0002c7c0: 636c 6173 733a 606e 6964 6967 6974 616c  class:`nidigital
+0002c7d0: 2e53 6573 7369 6f6e 6020 696e 7374 616e  .Session` instan
+0002c7e0: 6365 2e0a 2020 2020 2020 2020 5573 6520  ce..        Use 
+0002c7f0: 5079 7468 6f6e 2069 6e64 6578 206e 6f74  Python index not
+0002c800: 6174 696f 6e20 6f6e 2074 6865 2072 6570  ation on the rep
+0002c810: 6561 7465 6420 6361 7061 6269 6c69 7469  eated capabiliti
+0002c820: 6573 2063 6f6e 7461 696e 6572 2063 6861  es container cha
+0002c830: 6e6e 656c 7320 746f 2073 7065 6369 6679  nnels to specify
+0002c840: 2061 2073 7562 7365 742c 0a20 2020 2020   a subset,.     
+0002c850: 2020 2061 6e64 2074 6865 6e20 6361 6c6c     and then call
+0002c860: 2074 6869 7320 6d65 7468 6f64 206f 6e20   this method on 
+0002c870: 7468 6520 7265 7375 6c74 2e0a 0a20 2020  the result...   
+0002c880: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
+0002c890: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
+0002c8a0: 6f6e 2e63 6861 6e6e 656c 735b 202e 2e2e  on.channels[ ...
+0002c8b0: 205d 2e72 6561 645f 7374 6174 6963 600a   ].read_static`.
+0002c8c0: 0a20 2020 2020 2020 2054 6f20 6361 6c6c  .        To call
+0002c8d0: 2074 6865 206d 6574 686f 6420 6f6e 2061   the method on a
+0002c8e0: 6c6c 2063 6861 6e6e 656c 732c 2079 6f75  ll channels, you
+0002c8f0: 2063 616e 2063 616c 6c20 6974 2064 6972   can call it dir
+0002c900: 6563 746c 7920 6f6e 2074 6865 203a 7079  ectly on the :py
+0002c910: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
+0002c920: 6c2e 5365 7373 696f 6e60 2e0a 0a20 2020  l.Session`...   
+0002c930: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
+0002c940: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
+0002c950: 6f6e 2e72 6561 645f 7374 6174 6963 600a  on.read_static`.
+0002c960: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0002c970: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+0002c980: 7461 2028 6c69 7374 206f 6620 656e 756d  ta (list of enum
+0002c990: 732e 5069 6e53 7461 7465 293a 2054 6865  s.PinState): The
+0002c9a0: 2072 6574 7572 6e65 6420 6172 7261 7920   returned array 
+0002c9b0: 6f66 2070 696e 2073 7461 7465 7320 7265  of pin states re
+0002c9c0: 6164 2066 726f 6d20 7468 6520 6368 616e  ad from the chan
+0002c9d0: 6e65 6c73 2069 6e20 7468 6520 7265 7065  nels in the repe
+0002c9e0: 6174 6564 2063 6170 6162 696c 6974 6965  ated capabilitie
+0002c9f0: 732e 2044 6174 6120 6973 2072 6574 7572  s. Data is retur
+0002ca00: 6e65 6420 696e 2074 6865 206f 7264 6572  ned in the order
+0002ca10: 2079 6f75 2073 7065 6369 6679 2069 6e20   you specify in 
+0002ca20: 7468 6520 7265 7065 6174 6564 2063 6170  the repeated cap
+0002ca30: 6162 696c 6974 6965 732e 2049 6620 6120  abilities. If a 
+0002ca40: 7369 7465 2069 7320 6469 7361 626c 6564  site is disabled
+0002ca50: 2c20 7468 6520 6d65 7468 6f64 2064 6f65  , the method doe
+0002ca60: 7320 6e6f 7420 7265 7475 726e 2064 6174  s not return dat
+0002ca70: 6120 666f 7220 7468 6174 2073 6974 652e  a for that site.
+0002ca80: 2059 6f75 2063 616e 2061 6c73 6f20 7573   You can also us
+0002ca90: 6520 7468 6520 6765 745f 7069 6e5f 7265  e the get_pin_re
+0002caa0: 7375 6c74 735f 7069 6e5f 696e 666f 726d  sults_pin_inform
+0002cab0: 6174 696f 6e20 6d65 7468 6f64 2074 6f20  ation method to 
+0002cac0: 6f62 7461 696e 2061 2073 6f72 7465 6420  obtain a sorted 
+0002cad0: 6c69 7374 206f 6620 7265 7475 726e 6564  list of returned
+0002cae0: 2073 6974 6573 2061 6e64 2063 6861 6e6e   sites and chann
+0002caf0: 656c 732e 0a0a 2020 2020 2020 2020 2020  els...          
+0002cb00: 2020 2020 2020 2d20 2020 5069 6e53 7461        -   PinSta
+0002cb10: 7465 2e4c 3a20 5468 6520 636f 6d70 6172  te.L: The compar
+0002cb20: 6174 6f72 7320 7265 6164 2061 206c 6f67  ators read a log
+0002cb30: 6963 206c 6f77 2070 696e 2073 7461 7465  ic low pin state
+0002cb40: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0002cb50: 2020 2d20 2020 5069 6e53 7461 7465 2e48    -   PinState.H
+0002cb60: 3a20 5468 6520 636f 6d70 6172 6174 6f72  : The comparator
+0002cb70: 7320 7265 6164 2061 206c 6f67 6963 2068  s read a logic h
+0002cb80: 6967 6820 7069 6e20 7374 6174 652e 0a20  igh pin state.. 
+0002cb90: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+0002cba0: 2020 2050 696e 5374 6174 652e 4d3a 2054     PinState.M: T
+0002cbb0: 6865 2063 6f6d 7061 7261 746f 7273 2072  he comparators r
+0002cbc0: 6561 6420 6120 6d69 6462 616e 6420 7069  ead a midband pi
+0002cbd0: 6e20 7374 6174 652e 0a20 2020 2020 2020  n state..       
+0002cbe0: 2020 2020 2020 2020 202d 2020 2050 696e           -   Pin
+0002cbf0: 5374 6174 652e 563a 2054 6865 2063 6f6d  State.V: The com
+0002cc00: 7061 7261 746f 7273 2072 6561 6420 6120  parators read a 
+0002cc10: 7661 6c75 6520 7468 6174 2069 7320 6162  value that is ab
+0002cc20: 6f76 6520 564f 4820 616e 6420 6265 6c6f  ove VOH and belo
+0002cc30: 7720 564f 4c2c 2077 6869 6368 2063 616e  w VOL, which can
+0002cc40: 206f 6363 7572 2077 6865 6e20 796f 7520   occur when you 
+0002cc50: 7365 7420 564f 4c20 6869 6768 6572 2074  set VOL higher t
+0002cc60: 6861 6e20 564f 482e 0a0a 2020 2020 2020  han VOH...      
+0002cc70: 2020 2727 270a 2020 2020 2020 2020 6461    '''.        da
+0002cc80: 7461 203d 2073 656c 662e 5f69 6e74 6572  ta = self._inter
+0002cc90: 7072 6574 6572 2e72 6561 645f 7374 6174  preter.read_stat
+0002cca0: 6963 2873 656c 662e 5f72 6570 6561 7465  ic(self._repeate
+0002ccb0: 645f 6361 7061 6269 6c69 7479 290a 2020  d_capability).  
+0002ccc0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
+0002ccd0: 610a 0a20 2020 2040 6976 695f 7379 6e63  a..    @ivi_sync
+0002cce0: 6872 6f6e 697a 6564 0a20 2020 2064 6566  hronized.    def
+0002ccf0: 205f 7365 745f 6174 7472 6962 7574 655f   _set_attribute_
+0002cd00: 7669 5f62 6f6f 6c65 616e 2873 656c 662c  vi_boolean(self,
+0002cd10: 2061 7474 7269 6275 7465 2c20 7661 6c75   attribute, valu
+0002cd20: 6529 3a0a 2020 2020 2020 2020 7227 2727  e):.        r'''
+0002cd30: 5f73 6574 5f61 7474 7269 6275 7465 5f76  _set_attribute_v
+0002cd40: 695f 626f 6f6c 6561 6e0a 0a20 2020 2020  i_boolean..     
+0002cd50: 2020 2053 6574 7320 7468 6520 7661 6c75     Sets the valu
+0002cd60: 6520 6f66 2061 2056 6942 6f6f 6c65 616e  e of a ViBoolean
+0002cd70: 2070 726f 7065 7274 792e 2055 7365 2074   property. Use t
+0002cd80: 6869 7320 6d65 7468 6f64 2074 6f20 7365  his method to se
+0002cd90: 7420 7468 6520 7661 6c75 6573 206f 6620  t the values of 
+0002cda0: 6469 6769 7461 6c20 7061 7474 6572 6e20  digital pattern 
+0002cdb0: 696e 7374 7275 6d65 6e74 2d73 7065 6369  instrument-speci
+0002cdc0: 6669 6320 7072 6f70 6572 7469 6573 2061  fic properties a
+0002cdd0: 6e64 2069 6e68 6572 656e 7420 4956 4920  nd inherent IVI 
+0002cde0: 7072 6f70 6572 7469 6573 2e0a 0a20 2020  properties...   
+0002cdf0: 2020 2020 2054 6970 3a0a 2020 2020 2020       Tip:.      
+0002ce00: 2020 5468 6973 206d 6574 686f 6420 6361    This method ca
+0002ce10: 6e20 6265 2063 616c 6c65 6420 6f6e 2073  n be called on s
+0002ce20: 7065 6369 6669 6320 6368 616e 6e65 6c73  pecific channels
+0002ce30: 2077 6974 6869 6e20 796f 7572 203a 7079   within your :py
+0002ce40: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
+0002ce50: 6c2e 5365 7373 696f 6e60 2069 6e73 7461  l.Session` insta
+0002ce60: 6e63 652e 0a20 2020 2020 2020 2055 7365  nce..        Use
+0002ce70: 2050 7974 686f 6e20 696e 6465 7820 6e6f   Python index no
+0002ce80: 7461 7469 6f6e 206f 6e20 7468 6520 7265  tation on the re
+0002ce90: 7065 6174 6564 2063 6170 6162 696c 6974  peated capabilit
+0002cea0: 6965 7320 636f 6e74 6169 6e65 7220 6368  ies container ch
+0002ceb0: 616e 6e65 6c73 2074 6f20 7370 6563 6966  annels to specif
+0002cec0: 7920 6120 7375 6273 6574 2c0a 2020 2020  y a subset,.    
+0002ced0: 2020 2020 616e 6420 7468 656e 2063 616c      and then cal
+0002cee0: 6c20 7468 6973 206d 6574 686f 6420 6f6e  l this method on
+0002cef0: 2074 6865 2072 6573 756c 742e 0a0a 2020   the result...  
+0002cf00: 2020 2020 2020 4578 616d 706c 653a 203a        Example: :
+0002cf10: 7079 3a6d 6574 683a 606d 795f 7365 7373  py:meth:`my_sess
+0002cf20: 696f 6e2e 6368 616e 6e65 6c73 5b20 2e2e  ion.channels[ ..
+0002cf30: 2e20 5d2e 5f73 6574 5f61 7474 7269 6275  . ]._set_attribu
+0002cf40: 7465 5f76 695f 626f 6f6c 6561 6e60 0a0a  te_vi_boolean`..
+0002cf50: 2020 2020 2020 2020 546f 2063 616c 6c20          To call 
+0002cf60: 7468 6520 6d65 7468 6f64 206f 6e20 616c  the method on al
+0002cf70: 6c20 6368 616e 6e65 6c73 2c20 796f 7520  l channels, you 
+0002cf80: 6361 6e20 6361 6c6c 2069 7420 6469 7265  can call it dire
+0002cf90: 6374 6c79 206f 6e20 7468 6520 3a70 793a  ctly on the :py:
+0002cfa0: 636c 6173 733a 606e 6964 6967 6974 616c  class:`nidigital
+0002cfb0: 2e53 6573 7369 6f6e 602e 0a0a 2020 2020  .Session`...    
+0002cfc0: 2020 2020 4578 616d 706c 653a 203a 7079      Example: :py
+0002cfd0: 3a6d 6574 683a 606d 795f 7365 7373 696f  :meth:`my_sessio
+0002cfe0: 6e2e 5f73 6574 5f61 7474 7269 6275 7465  n._set_attribute
+0002cff0: 5f76 695f 626f 6f6c 6561 6e60 0a0a 2020  _vi_boolean`..  
+0002d000: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0002d010: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
+0002d020: 6520 2869 6e74 293a 2054 6865 2049 4420  e (int): The ID 
+0002d030: 6f66 2061 2070 726f 7065 7274 792e 0a0a  of a property...
+0002d040: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+0002d050: 6520 2862 6f6f 6c29 3a20 5468 6520 7661  e (bool): The va
+0002d060: 6c75 6520 746f 2077 6869 6368 2079 6f75  lue to which you
+0002d070: 2077 616e 7420 746f 2073 6574 2074 6865   want to set the
+0002d080: 2070 726f 7065 7274 793b 2073 6f6d 6520   property; some 
+0002d090: 6f66 2074 6865 2076 616c 7565 7320 6d69  of the values mi
+0002d0a0: 6768 7420 6e6f 7420 6265 2076 616c 6964  ght not be valid
+0002d0b0: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
+0002d0c0: 6520 6375 7272 656e 7420 7365 7474 696e  e current settin
+0002d0d0: 6773 206f 6620 7468 6520 696e 7374 7275  gs of the instru
+0002d0e0: 6d65 6e74 2073 6573 7369 6f6e 2e0a 0a20  ment session... 
+0002d0f0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0002d100: 2020 2073 656c 662e 5f69 6e74 6572 7072     self._interpr
+0002d110: 6574 6572 2e73 6574 5f61 7474 7269 6275  eter.set_attribu
+0002d120: 7465 5f76 695f 626f 6f6c 6561 6e28 7365  te_vi_boolean(se
+0002d130: 6c66 2e5f 7265 7065 6174 6564 5f63 6170  lf._repeated_cap
+0002d140: 6162 696c 6974 792c 2061 7474 7269 6275  ability, attribu
+0002d150: 7465 2c20 7661 6c75 6529 0a0a 2020 2020  te, value)..    
+0002d160: 4069 7669 5f73 796e 6368 726f 6e69 7a65  @ivi_synchronize
+0002d170: 640a 2020 2020 6465 6620 5f73 6574 5f61  d.    def _set_a
+0002d180: 7474 7269 6275 7465 5f76 695f 696e 7433  ttribute_vi_int3
+0002d190: 3228 7365 6c66 2c20 6174 7472 6962 7574  2(self, attribut
+0002d1a0: 652c 2076 616c 7565 293a 0a20 2020 2020  e, value):.     
+0002d1b0: 2020 2072 2727 275f 7365 745f 6174 7472     r'''_set_attr
+0002d1c0: 6962 7574 655f 7669 5f69 6e74 3332 0a0a  ibute_vi_int32..
+0002d1d0: 2020 2020 2020 2020 5365 7473 2074 6865          Sets the
+0002d1e0: 2076 616c 7565 206f 6620 6120 5669 496e   value of a ViIn
+0002d1f0: 7433 3220 7072 6f70 6572 7479 2e20 5573  t32 property. Us
+0002d200: 6520 7468 6973 206d 6574 686f 6420 746f  e this method to
+0002d210: 2073 6574 2074 6865 2076 616c 7565 7320   set the values 
+0002d220: 6f66 2064 6967 6974 616c 2070 6174 7465  of digital patte
+0002d230: 726e 2069 6e73 7472 756d 656e 742d 7370  rn instrument-sp
+0002d240: 6563 6966 6963 2070 726f 7065 7274 6965  ecific propertie
+0002d250: 7320 616e 6420 696e 6865 7265 6e74 2049  s and inherent I
+0002d260: 5649 2070 726f 7065 7274 6965 732e 0a0a  VI properties...
+0002d270: 2020 2020 2020 2020 5469 703a 0a20 2020          Tip:.   
+0002d280: 2020 2020 2054 6869 7320 6d65 7468 6f64       This method
+0002d290: 2063 616e 2062 6520 6361 6c6c 6564 206f   can be called o
+0002d2a0: 6e20 7370 6563 6966 6963 2063 6861 6e6e  n specific chann
+0002d2b0: 656c 7320 7769 7468 696e 2079 6f75 7220  els within your 
+0002d2c0: 3a70 793a 636c 6173 733a 606e 6964 6967  :py:class:`nidig
+0002d2d0: 6974 616c 2e53 6573 7369 6f6e 6020 696e  ital.Session` in
+0002d2e0: 7374 616e 6365 2e0a 2020 2020 2020 2020  stance..        
+0002d2f0: 5573 6520 5079 7468 6f6e 2069 6e64 6578  Use Python index
+0002d300: 206e 6f74 6174 696f 6e20 6f6e 2074 6865   notation on the
+0002d310: 2072 6570 6561 7465 6420 6361 7061 6269   repeated capabi
+0002d320: 6c69 7469 6573 2063 6f6e 7461 696e 6572  lities container
+0002d330: 2063 6861 6e6e 656c 7320 746f 2073 7065   channels to spe
+0002d340: 6369 6679 2061 2073 7562 7365 742c 0a20  cify a subset,. 
+0002d350: 2020 2020 2020 2061 6e64 2074 6865 6e20         and then 
+0002d360: 6361 6c6c 2074 6869 7320 6d65 7468 6f64  call this method
+0002d370: 206f 6e20 7468 6520 7265 7375 6c74 2e0a   on the result..
+0002d380: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+0002d390: 3a20 3a70 793a 6d65 7468 3a60 6d79 5f73  : :py:meth:`my_s
+0002d3a0: 6573 7369 6f6e 2e63 6861 6e6e 656c 735b  ession.channels[
+0002d3b0: 202e 2e2e 205d 2e5f 7365 745f 6174 7472   ... ]._set_attr
+0002d3c0: 6962 7574 655f 7669 5f69 6e74 3332 600a  ibute_vi_int32`.
+0002d3d0: 0a20 2020 2020 2020 2054 6f20 6361 6c6c  .        To call
+0002d3e0: 2074 6865 206d 6574 686f 6420 6f6e 2061   the method on a
+0002d3f0: 6c6c 2063 6861 6e6e 656c 732c 2079 6f75  ll channels, you
+0002d400: 2063 616e 2063 616c 6c20 6974 2064 6972   can call it dir
+0002d410: 6563 746c 7920 6f6e 2074 6865 203a 7079  ectly on the :py
+0002d420: 3a63 6c61 7373 3a60 6e69 6469 6769 7461  :class:`nidigita
+0002d430: 6c2e 5365 7373 696f 6e60 2e0a 0a20 2020  l.Session`...   
+0002d440: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
+0002d450: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
+0002d460: 6f6e 2e5f 7365 745f 6174 7472 6962 7574  on._set_attribut
+0002d470: 655f 7669 5f69 6e74 3332 600a 0a20 2020  e_vi_int32`..   
+0002d480: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0002d490: 2020 2020 2020 2061 7474 7269 6275 7465         attribute
+0002d4a0: 2028 696e 7429 3a20 5468 6520 4944 206f   (int): The ID o
+0002d4b0: 6620 6120 7072 6f70 6572 7479 2e0a 0a20  f a property... 
+0002d4c0: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0002d4d0: 2028 696e 7429 3a20 5468 6520 7661 6c75   (int): The valu
+0002d4e0: 6520 746f 2077 6869 6368 2079 6f75 2077  e to which you w
+0002d4f0: 616e 7420 746f 2073 6574 2074 6865 2070  ant to set the p
+0002d500: 726f 7065 7274 793b 2073 6f6d 6520 6f66  roperty; some of
+0002d510: 2074 6865 2076 616c 7565 7320 6d69 6768   the values migh
+0002d520: 7420 6e6f 7420 6265 2076 616c 6964 2064  t not be valid d
+0002d530: 6570 656e 6469 6e67 206f 6e20 7468 6520  epending on the 
+0002d540: 6375 7272 656e 7420 7365 7474 696e 6773  current settings
+0002d550: 206f 6620 7468 6520 696e 7374 7275 6d65   of the instrume
+0002d560: 6e74 2073 6573 7369 6f6e 2e0a 0a20 2020  nt session...   
+0002d570: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+0002d580: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
+0002d590: 6572 2e73 6574 5f61 7474 7269 6275 7465  er.set_attribute
+0002d5a0: 5f76 695f 696e 7433 3228 7365 6c66 2e5f  _vi_int32(self._
+0002d5b0: 7265 7065 6174 6564 5f63 6170 6162 696c  repeated_capabil
+0002d5c0: 6974 792c 2061 7474 7269 6275 7465 2c20  ity, attribute, 
+0002d5d0: 7661 6c75 6529 0a0a 2020 2020 4069 7669  value)..    @ivi
+0002d5e0: 5f73 796e 6368 726f 6e69 7a65 640a 2020  _synchronized.  
+0002d5f0: 2020 6465 6620 5f73 6574 5f61 7474 7269    def _set_attri
+0002d600: 6275 7465 5f76 695f 696e 7436 3428 7365  bute_vi_int64(se
+0002d610: 6c66 2c20 6174 7472 6962 7574 652c 2076  lf, attribute, v
+0002d620: 616c 7565 293a 0a20 2020 2020 2020 2072  alue):.        r
+0002d630: 2727 275f 7365 745f 6174 7472 6962 7574  '''_set_attribut
+0002d640: 655f 7669 5f69 6e74 3634 0a0a 2020 2020  e_vi_int64..    
+0002d650: 2020 2020 5365 7473 2074 6865 2076 616c      Sets the val
+0002d660: 7565 206f 6620 6120 5669 496e 7436 3420  ue of a ViInt64 
+0002d670: 7072 6f70 6572 7479 2e20 5573 6520 7468  property. Use th
+0002d680: 6973 206d 6574 686f 6420 746f 2073 6574  is method to set
+0002d690: 2074 6865 2076 616c 7565 7320 6f66 2064   the values of d
+0002d6a0: 6967 6974 616c 2070 6174 7465 726e 2069  igital pattern i
+0002d6b0: 6e73 7472 756d 656e 742d 7370 6563 6966  nstrument-specif
+0002d6c0: 6963 2070 726f 7065 7274 6965 7320 616e  ic properties an
+0002d6d0: 6420 696e 6865 7265 6e74 2049 5649 2070  d inherent IVI p
+0002d6e0: 726f 7065 7274 6965 732e 0a0a 2020 2020  roperties...    
+0002d6f0: 2020 2020 5469 703a 0a20 2020 2020 2020      Tip:.       
+0002d700: 2054 6869 7320 6d65 7468 6f64 2063 616e   This method can
+0002d710: 2062 6520 6361 6c6c 6564 206f 6e20 7370   be called on sp
+0002d720: 6563 6966 6963 2063 6861 6e6e 656c 7320  ecific channels 
+0002d730: 7769 7468 696e 2079 6f75 7220 3a70 793a  within your :py:
+0002d740: 636c 6173 733a 606e 6964 6967 6974 616c  class:`nidigital
+0002d750: 2e53 6573 7369 6f6e 6020 696e 7374 616e  .Session` instan
+0002d760: 6365 2e0a 2020 2020 2020 2020 5573 6520  ce..        Use 
+0002d770: 5079 7468 6f6e 2069 6e64 6578 206e 6f74  Python index not
+0002d780: 6174 696f 6e20 6f6e 2074 6865 2072 6570  ation on the rep
+0002d790: 6561 7465 6420 6361 7061 6269 6c69 7469  eated capabiliti
+0002d7a0: 6573 2063 6f6e 7461 696e 6572 2063 6861  es container cha
+0002d7b0: 6e6e 656c 7320 746f 2073 7065 6369 6679  nnels to specify
+0002d7c0: 2061 2073 7562 7365 742c 0a20 2020 2020   a subset,.     
+0002d7d0: 2020 2061 6e64 2074 6865 6e20 6361 6c6c     and then call
+0002d7e0: 2074 6869 7320 6d65 7468 6f64 206f 6e20   this method on 
+0002d7f0: 7468 6520 7265 7375 6c74 2e0a 0a20 2020  the result...   
+0002d800: 2020 2020 2045 7861 6d70 6c65 3a20 3a70       Example: :p
+0002d810: 793a 6d65 7468 3a60 6d79 5f73 6573 7369  y:meth:`my_sessi
+0002d820: 6f6e 2e63 6861 6e6e 656c 735b 202e 2e2e  on.channels[ ...
+0002d830: 205d 2e5f 7365 745f 6174 7472 6962 7574   ]._set_attribut
+0002d840: 655f 7669 5f69 6e74 3634 600a 0a20 2020  e_vi_int64`..   
+0002d850: 2020 2020 2054 6f20 6361 6c6c 2074 6865       To call the
+0002d860: 206d 6574 686f 6420 6f6e 2061 6c6c 2063   method on all c
+0002d870: 6861 6e6e 656c 732c 2079 6f75 2063 616e  hannels, you can
+0002d880: 2063 616c 6c20 6974 2064 6972 6563 746c   call it directl
+0002d890: 7920 6f6e 2074 6865 203a 7079 3a63 6c61  y on the :py:cla
+0002d8a0: 7373 3a60 6e69 6469 6769 7461 6c2e 5365  ss:`nidigital.Se
+0002d8b0: 7373 696f 6e60 2e0a 0a20 2020 2020 2020  ssion`...       
+0002d8c0: 2045 7861 6d70 6c65 3a20 3a70 793a 6d65   Example: :py:me
+0002d8d0: 7468 3a60 6d79 5f73 6573 7369 6f6e 2e5f  th:`my_session._
+0002d8e0: 7365 745f 6174 7472 6962 7574 655f 7669  set_attribute_vi
+0002d8f0: 5f69 6e74 3634 600a 0a20 2020 2020 2020  _int64`..       
+0002d900: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0002d910: 2020 2061 7474 7269 6275 7465 2028 696e     attribute (in
+0002d920: 7429 3a20 5468 6520 4944 206f 6620 6120  t): The ID of a 
+0002d930: 7072 6f70 6572 7479 2e0a 0a20 2020 2020  property...     
+0002d940: 2020 2020 2020 2076 616c 7565 2028 696e         value (in
+0002d950: 7429 3a20 5468 6520 7661 6c75 6520 746f  t): The value to
+0002d960: 2077 6869 6368 2079 6f75 2077 616e 7420   which you want 
+0002d970: 746f 2073 6574 2074 6865 2070 726f 7065  to set the prope
+0002d980: 7274 793b 2073 6f6d 6520 6f66 2074 6865  rty; some of the
+0002d990: 2076 616c 7565 7320 6d69 6768 7420 6e6f   values might no
+0002d9a0: 7420 6265 2076 616c 6964 2064 6570 656e  t be valid depen
+0002d9b0: 6469 6e67 206f 6e20 7468 6520 6375 7272  ding on the curr
+0002d9c0: 656e 7420 7365 7474 696e 6773 206f 6620  ent settings of 
+0002d9d0: 7468 6520 696e 7374 7275 6d65 6e74 2073  the instrument s
+0002d9e0: 6573 7369 6f6e 2e0a 0a20 2020 2020 2020  ession...       
+0002d9f0: 2027 2727 0a20 2020 2020 2020 2073 656c   '''.        sel
+0002da00: 662e 5f69 6e74 6572 7072 6574 6572 2e73  f._interpreter.s
+0002da10: 6574 5f61 7474 7269 6275 7465 5f76 695f  et_attribute_vi_
+0002da20: 696e 7436 3428 7365 6c66 2e5f 7265 7065  int64(self._repe
+0002da30: 6174 6564 5f63 6170 6162 696c 6974 792c  ated_capability,
+0002da40: 2061 7474 7269 6275 7465 2c20 7661 6c75   attribute, valu
+0002da50: 6529 0a0a 2020 2020 4069 7669 5f73 796e  e)..    @ivi_syn
+0002da60: 6368 726f 6e69 7a65 640a 2020 2020 6465  chronized.    de
+0002da70: 6620 5f73 6574 5f61 7474 7269 6275 7465  f _set_attribute
+0002da80: 5f76 695f 7265 616c 3634 2873 656c 662c  _vi_real64(self,
+0002da90: 2061 7474 7269 6275 7465 2c20 7661 6c75   attribute, valu
+0002daa0: 6529 3a0a 2020 2020 2020 2020 7227 2727  e):.        r'''
+0002dab0: 5f73 6574 5f61 7474 7269 6275 7465 5f76  _set_attribute_v
+0002dac0: 695f 7265 616c 3634 0a0a 2020 2020 2020  i_real64..      
+0002dad0: 2020 5365 7473 2074 6865 2076 616c 7565    Sets the value
+0002dae0: 206f 6620 6120 5669 496e 7452 6561 6c36   of a ViIntReal6
+0002daf0: 3420 7072 6f70 6572 7479 2e20 5573 6520  4 property. Use 
+0002db00: 7468 6973 206d 6574 686f 6420 746f 2073  this method to s
+0002db10: 6574 2074 6865 2076 616c 7565 7320 6f66  et the values of
+0002db20: 2064 6967 6974 616c 2070 6174 7465 726e   digital pattern
+0002db30: 2069 6e73 7472 756d 656e 742d 7370 6563   instrument-spec
+0002db40: 6966 6963 2070 726f 7065 7274 6965 7320  ific properties 
+0002db50: 616e 6420 696e 6865 7265 6e74 2049 5649  and inherent IVI
+0002db60: 2070 726f 7065 7274 6965 732e 0a0a 2020   properties...  
+0002db70: 2020 2020 2020 5469 703a 0a20 2020 2020        Tip:.     
+0002db80: 2020 2054 6869 7320 6d65 7468 6f64 2063     This method c
+0002db90: 616e 2062 6520 6361 6c6c 6564 206f 6e20  an be called on 
+0002dba0: 7370 6563 6966 6963 2063 6861 6e6e 656c  specific channel
+0002dbb0: 7320 7769 7468 696e 2079 6f75 7220 3a70  s within your :p
+0002dbc0: 793a 636c 6173 733a 606e 6964 6967 6974  y:class:`nidigit
+0002dbd0: 616c 2e53 6573 7369 6f6e 6020 696e 7374  al.Session` inst
+0002dbe0: 616e 6365 2e0a 2020 2020 2020 2020 5573  ance..        Us
+0002dbf0: 6520 5079 7468 6f6e 2069 6e64 6578 206e  e Python index n
+0002dc00: 6f74 6174 696f 6e20 6f6e 2074 6865 2072  otation on the r
+0002dc10: 6570 6561 7465 6420 6361 7061 6269 6c69  epeated capabili
+0002dc20: 7469 6573 2063 6f6e 7461 696e 6572 2063  ties container c
+0002dc30: 6861 6e6e 656c 7320 746f 2073 7065 6369  hannels to speci
+0002dc40: 6679 2061 2073 7562 7365 742c 0a20 2020  fy a subset,.   
+0002dc50: 2020 2020 2061 6e64 2074 6865 6e20 6361       and then ca
+0002dc60: 6c6c 2074 6869 7320 6d65 7468 6f64 206f  ll this method o
+0002dc70: 6e20 7468 6520 7265 7375 6c74 2e0a 0a20  n the result... 
+0002dc80: 2020 2020 2020 2045 7861 6d70 6c65 3a20         Example: 
+0002dc90: 3a70 793a 6d65 7468 3a60 6d79 5f73 6573  :py:meth:`my_ses
+0002dca0: 7369 6f6e 2e63 6861 6e6e 656c 735b 202e  sion.channels[ .
+0002dcb0: 2e2e 205d 2e5f 7365 745f 6174 7472 6962  .. ]._set_attrib
+0002dcc0: 7574 655f 7669 5f72 6561 6c36 3460 0a0a  ute_vi_real64`..
+0002dcd0: 2020 2020 2020 2020 546f 2063 616c 6c20          To call 
+0002dce0: 7468 6520 6d65 7468 6f64 206f 6e20 616c  the method on al
+0002dcf0: 6c20 6368 616e 6e65 6c73 2c20 796f 7520  l channels, you 
+0002dd00: 6361 6e20 6361 6c6c 2069 7420 6469 7265  can call it dire
+0002dd10: 6374 6c79 206f 6e20 7468 6520 3a70 793a  ctly on the :py:
+0002dd20: 636c 6173 733a 606e 6964 6967 6974 616c  class:`nidigital
+0002dd30: 2e53 6573 7369 6f6e 602e 0a0a 2020 2020  .Session`...    
+0002dd40: 2020 2020 4578 616d 706c 653a 203a 7079      Example: :py
+0002dd50: 3a6d 6574 683a 606d 795f 7365 7373 696f  :meth:`my_sessio
+0002dd60: 6e2e 5f73 6574 5f61 7474 7269 6275 7465  n._set_attribute
+0002dd70: 5f76 695f 7265 616c 3634 600a 0a20 2020  _vi_real64`..   
+0002dd80: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0002dd90: 2020 2020 2020 2061 7474 7269 6275 7465         attribute
+0002dda0: 2028 696e 7429 3a20 5468 6520 4944 206f   (int): The ID o
+0002ddb0: 6620 6120 7072 6f70 6572 7479 2e0a 0a20  f a property... 
+0002ddc0: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0002ddd0: 2028 666c 6f61 7429 3a20 5468 6520 7661   (float): The va
+0002dde0: 6c75 6520 746f 2077 6869 6368 2079 6f75  lue to which you
+0002ddf0: 2077 616e 7420 746f 2073 6574 2074 6865   want to set the
+0002de00: 2070 726f 7065 7274 793b 2073 6f6d 6520   property; some 
+0002de10: 6f66 2074 6865 2076 616c 7565 7320 6d69  of the values mi
+0002de20: 6768 7420 6e6f 7420 6265 2076 616c 6964  ght not be valid
+0002de30: 2064 6570 656e 6469 6e67 206f 6e20 7468   depending on th
+0002de40: 6520 6375 7272 656e 7420 7365 7474 696e  e current settin
+0002de50: 6773 206f 6620 7468 6520 696e 7374 7275  gs of the instru
+0002de60: 6d65 6e74 2073 6573 7369 6f6e 2e0a 0a20  ment session... 
+0002de70: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+0002de80: 2020 2073 656c 662e 5f69 6e74 6572 7072     self._interpr
+0002de90: 6574 6572 2e73 6574 5f61 7474 7269 6275  eter.set_attribu
+0002dea0: 7465 5f76 695f 7265 616c 3634 2873 656c  te_vi_real64(sel
+0002deb0: 662e 5f72 6570 6561 7465 645f 6361 7061  f._repeated_capa
+0002dec0: 6269 6c69 7479 2c20 6174 7472 6962 7574  bility, attribut
+0002ded0: 652c 2076 616c 7565 290a 0a20 2020 2040  e, value)..    @
+0002dee0: 6976 695f 7379 6e63 6872 6f6e 697a 6564  ivi_synchronized
+0002def0: 0a20 2020 2064 6566 205f 7365 745f 6174  .    def _set_at
+0002df00: 7472 6962 7574 655f 7669 5f73 7472 696e  tribute_vi_strin
+0002df10: 6728 7365 6c66 2c20 6174 7472 6962 7574  g(self, attribut
+0002df20: 652c 2076 616c 7565 293a 0a20 2020 2020  e, value):.     
+0002df30: 2020 2072 2727 275f 7365 745f 6174 7472     r'''_set_attr
+0002df40: 6962 7574 655f 7669 5f73 7472 696e 670a  ibute_vi_string.
+0002df50: 0a20 2020 2020 2020 2053 6574 7320 7468  .        Sets th
+0002df60: 6520 7661 6c75 6520 6f66 2061 2056 6953  e value of a ViS
+0002df70: 7472 696e 6720 7072 6f70 6572 7479 2e20  tring property. 
+0002df80: 5573 6520 7468 6973 206d 6574 686f 6420  Use this method 
+0002df90: 746f 2073 6574 2074 6865 2076 616c 7565  to set the value
+0002dfa0: 7320 6f66 2064 6967 6974 616c 2070 6174  s of digital pat
+0002dfb0: 7465 726e 2069 6e73 7472 756d 656e 742d  tern instrument-
+0002dfc0: 7370 6563 6966 6963 2070 726f 7065 7274  specific propert
+0002dfd0: 6965 7320 616e 6420 696e 6865 7265 6e74  ies and inherent
+0002dfe0: 2049 5649 2070 726f 7065 7274 6965 732e   IVI properties.
+0002dff0: 0a0a 2020 2020 2020 2020 5469 703a 0a20  ..        Tip:. 
+0002e000: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
+0002e010: 6f64 2063 616e 2062 6520 6361 6c6c 6564  od can be called
+0002e020: 206f 6e20 7370 6563 6966 6963 2063 6861   on specific cha
+0002e030: 6e6e 656c 7320 7769 7468 696e 2079 6f75  nnels within you
+0002e040: 7220 3a70 793a 636c 6173 733a 606e 6964  r :py:class:`nid
+0002e050: 6967 6974 616c 2e53 6573 7369 6f6e 6020  igital.Session` 
+0002e060: 696e 7374 616e 6365 2e0a 2020 2020 2020  instance..      
+0002e070: 2020 5573 6520 5079 7468 6f6e 2069 6e64    Use Python ind
+0002e080: 6578 206e 6f74 6174 696f 6e20 6f6e 2074  ex notation on t
+0002e090: 6865 2072 6570 6561 7465 6420 6361 7061  he repeated capa
+0002e0a0: 6269 6c69 7469 6573 2063 6f6e 7461 696e  bilities contain
+0002e0b0: 6572 2063 6861 6e6e 656c 7320 746f 2073  er channels to s
+0002e0c0: 7065 6369 6679 2061 2073 7562 7365 742c  pecify a subset,
+0002e0d0: 0a20 2020 2020 2020 2061 6e64 2074 6865  .        and the
+0002e0e0: 6e20 6361 6c6c 2074 6869 7320 6d65 7468  n call this meth
+0002e0f0: 6f64 206f 6e20 7468 6520 7265 7375 6c74  od on the result
+0002e100: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+0002e110: 6c65 3a20 3a70 793a 6d65 7468 3a60 6d79  le: :py:meth:`my
+0002e120: 5f73 6573 7369 6f6e 2e63 6861 6e6e 656c  _session.channel
+0002e130: 735b 202e 2e2e 205d 2e5f 7365 745f 6174  s[ ... ]._set_at
+0002e140: 7472 6962 7574 655f 7669 5f73 7472 696e  tribute_vi_strin
+0002e150: 6760 0a0a 2020 2020 2020 2020 546f 2063  g`..        To c
+0002e160: 616c 6c20 7468 6520 6d65 7468 6f64 206f  all the method o
+0002e170: 6e20 616c 6c20 6368 616e 6e65 6c73 2c20  n all channels, 
+0002e180: 796f 7520 6361 6e20 6361 6c6c 2069 7420  you can call it 
+0002e190: 6469 7265 6374 6c79 206f 6e20 7468 6520  directly on the 
+0002e1a0: 3a70 793a 636c 6173 733a 606e 6964 6967  :py:class:`nidig
+0002e1b0: 6974 616c 2e53 6573 7369 6f6e 602e 0a0a  ital.Session`...
+0002e1c0: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+0002e1d0: 203a 7079 3a6d 6574 683a 606d 795f 7365   :py:meth:`my_se
+0002e1e0: 7373 696f 6e2e 5f73 6574 5f61 7474 7269  ssion._set_attri
+0002e1f0: 6275 7465 5f76 695f 7374 7269 6e67 600a  bute_vi_string`.
+0002e200: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0002e210: 2020 2020 2020 2020 2020 2061 7474 7269             attri
+0002e220: 6275 7465 2028 696e 7429 3a20 5468 6520  bute (int): The 
+0002e230: 4944 206f 6620 6120 7072 6f70 6572 7479  ID of a property
+0002e240: 2e0a 0a20 2020 2020 2020 2020 2020 2076  ...            v
+0002e250: 616c 7565 2028 7374 7229 3a20 5468 6520  alue (str): The 
+0002e260: 7661 6c75 6520 746f 2077 6869 6368 2079  value to which y
+0002e270: 6f75 2077 616e 7420 746f 2073 6574 2074  ou want to set t
+0002e280: 6865 2070 726f 7065 7274 793b 2073 6f6d  he property; som
+0002e290: 6520 6f66 2074 6865 2076 616c 7565 7320  e of the values 
+0002e2a0: 6d69 6768 7420 6e6f 7420 6265 2076 616c  might not be val
+0002e2b0: 6964 2064 6570 656e 6469 6e67 206f 6e20  id depending on 
+0002e2c0: 7468 6520 6375 7272 656e 7420 7365 7474  the current sett
+0002e2d0: 696e 6773 206f 6620 7468 6520 696e 7374  ings of the inst
+0002e2e0: 7275 6d65 6e74 2073 6573 7369 6f6e 2e0a  rument session..
+0002e2f0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+0002e300: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
+0002e310: 7072 6574 6572 2e73 6574 5f61 7474 7269  preter.set_attri
+0002e320: 6275 7465 5f76 695f 7374 7269 6e67 2873  bute_vi_string(s
+0002e330: 656c 662e 5f72 6570 6561 7465 645f 6361  elf._repeated_ca
+0002e340: 7061 6269 6c69 7479 2c20 6174 7472 6962  pability, attrib
+0002e350: 7574 652c 2076 616c 7565 290a 0a20 2020  ute, value)..   
+0002e360: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
+0002e370: 6564 0a20 2020 2064 6566 2074 6472 2873  ed.    def tdr(s
+0002e380: 656c 662c 2061 7070 6c79 5f6f 6666 7365  elf, apply_offse
+0002e390: 7473 3d54 7275 6529 3a0a 2020 2020 2020  ts=True):.      
+0002e3a0: 2020 7227 2727 7464 720a 0a20 2020 2020    r'''tdr..     
+0002e3b0: 2020 204d 6561 7375 7265 7320 7072 6f70     Measures prop
+0002e3c0: 6167 6174 696f 6e20 6465 6c61 7973 2074  agation delays t
+0002e3d0: 6872 6f75 6768 2063 6162 6c65 732c 2063  hrough cables, c
+0002e3e0: 6f6e 6e65 6374 6f72 732c 2061 6e64 206c  onnectors, and l
+0002e3f0: 6f61 6420 626f 6172 6473 2075 7369 6e67  oad boards using
+0002e400: 2054 696d 652d 446f 6d61 696e 2052 6566   Time-Domain Ref
+0002e410: 6c65 6374 6f6d 6574 7279 2028 5444 5229  lectometry (TDR)
+0002e420: 2e20 456e 7375 7265 2074 6861 7420 7468  . Ensure that th
+0002e430: 6520 6368 616e 6e65 6c73 2061 6e64 2070  e channels and p
+0002e440: 696e 7320 796f 7520 7365 6c65 6374 2061  ins you select a
+0002e450: 7265 2063 6f6e 6e65 6374 6564 2074 6f20  re connected to 
+0002e460: 616e 206f 7065 6e20 6369 7263 7569 742e  an open circuit.
+0002e470: 0a0a 2020 2020 2020 2020 5469 703a 0a20  ..        Tip:. 
+0002e480: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
+0002e490: 6f64 2063 616e 2062 6520 6361 6c6c 6564  od can be called
+0002e4a0: 206f 6e20 7370 6563 6966 6963 2063 6861   on specific cha
+0002e4b0: 6e6e 656c 7320 7769 7468 696e 2079 6f75  nnels within you
+0002e4c0: 7220 3a70 793a 636c 6173 733a 606e 6964  r :py:class:`nid
+0002e4d0: 6967 6974 616c 2e53 6573 7369 6f6e 6020  igital.Session` 
+0002e4e0: 696e 7374 616e 6365 2e0a 2020 2020 2020  instance..      
+0002e4f0: 2020 5573 6520 5079 7468 6f6e 2069 6e64    Use Python ind
+0002e500: 6578 206e 6f74 6174 696f 6e20 6f6e 2074  ex notation on t
+0002e510: 6865 2072 6570 6561 7465 6420 6361 7061  he repeated capa
+0002e520: 6269 6c69 7469 6573 2063 6f6e 7461 696e  bilities contain
+0002e530: 6572 2063 6861 6e6e 656c 7320 746f 2073  er channels to s
+0002e540: 7065 6369 6679 2061 2073 7562 7365 742c  pecify a subset,
+0002e550: 0a20 2020 2020 2020 2061 6e64 2074 6865  .        and the
+0002e560: 6e20 6361 6c6c 2074 6869 7320 6d65 7468  n call this meth
+0002e570: 6f64 206f 6e20 7468 6520 7265 7375 6c74  od on the result
+0002e580: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+0002e590: 6c65 3a20 3a70 793a 6d65 7468 3a60 6d79  le: :py:meth:`my
+0002e5a0: 5f73 6573 7369 6f6e 2e63 6861 6e6e 656c  _session.channel
+0002e5b0: 735b 202e 2e2e 205d 2e74 6472 600a 0a20  s[ ... ].tdr`.. 
+0002e5c0: 2020 2020 2020 2054 6f20 6361 6c6c 2074         To call t
+0002e5d0: 6865 206d 6574 686f 6420 6f6e 2061 6c6c  he method on all
+0002e5e0: 2063 6861 6e6e 656c 732c 2079 6f75 2063   channels, you c
+0002e5f0: 616e 2063 616c 6c20 6974 2064 6972 6563  an call it direc
+0002e600: 746c 7920 6f6e 2074 6865 203a 7079 3a63  tly on the :py:c
+0002e610: 6c61 7373 3a60 6e69 6469 6769 7461 6c2e  lass:`nidigital.
+0002e620: 5365 7373 696f 6e60 2e0a 0a20 2020 2020  Session`...     
+0002e630: 2020 2045 7861 6d70 6c65 3a20 3a70 793a     Example: :py:
+0002e640: 6d65 7468 3a60 6d79 5f73 6573 7369 6f6e  meth:`my_session
+0002e650: 2e74 6472 600a 0a20 2020 2020 2020 2041  .tdr`..        A
+0002e660: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0002e670: 2061 7070 6c79 5f6f 6666 7365 7473 2028   apply_offsets (
+0002e680: 626f 6f6c 293a 2041 2042 6f6f 6c65 616e  bool): A Boolean
+0002e690: 2074 6861 7420 7370 6563 6966 6965 7320   that specifies 
+0002e6a0: 7768 6574 6865 7220 746f 2061 7070 6c79  whether to apply
+0002e6b0: 2074 6865 206d 6561 7375 7265 6420 5444   the measured TD
+0002e6c0: 5220 6f66 6673 6574 732e 2049 6620 796f  R offsets. If yo
+0002e6d0: 7520 6e65 6564 2074 6f20 6164 6a75 7374  u need to adjust
+0002e6e0: 2074 6865 206d 6561 7375 7265 6420 6f66   the measured of
+0002e6f0: 6673 6574 7320 7072 696f 7220 746f 2061  fsets prior to a
+0002e700: 7070 6c79 696e 672c 2073 6574 2074 6869  pplying, set thi
+0002e710: 7320 696e 7075 7420 746f 2046 616c 7365  s input to False
+0002e720: 2c20 616e 6420 6361 6c6c 2074 6865 2061  , and call the a
+0002e730: 7070 6c79 5f74 6472 5f6f 6666 7365 7473  pply_tdr_offsets
+0002e740: 206d 6574 686f 6420 746f 2073 7065 6369   method to speci
+0002e750: 6679 2074 6865 2061 646a 7573 7465 6420  fy the adjusted 
+0002e760: 5444 5220 6f66 6673 6574 7320 7661 6c75  TDR offsets valu
+0002e770: 6573 2e0a 0a0a 2020 2020 2020 2020 5265  es....        Re
+0002e780: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0002e790: 2020 206f 6666 7365 7473 2028 6c69 7374     offsets (list
+0002e7a0: 206f 6620 6869 6768 7469 6d65 2e74 696d   of hightime.tim
+0002e7b0: 6564 656c 7461 293a 204d 6561 7375 7265  edelta): Measure
+0002e7c0: 6420 5444 5220 6f66 6673 6574 7320 7370  d TDR offsets sp
+0002e7d0: 6563 6966 6965 6420 696e 2073 6563 6f6e  ecified in secon
+0002e7e0: 6473 2e0a 0a20 2020 2020 2020 2027 2727  ds...        '''
+0002e7f0: 0a20 2020 2020 2020 206f 6666 7365 7473  .        offsets
+0002e800: 203d 2073 656c 662e 5f69 6e74 6572 7072   = self._interpr
+0002e810: 6574 6572 2e74 6472 2873 656c 662e 5f72  eter.tdr(self._r
+0002e820: 6570 6561 7465 645f 6361 7061 6269 6c69  epeated_capabili
+0002e830: 7479 2c20 6170 706c 795f 6f66 6673 6574  ty, apply_offset
+0002e840: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+0002e850: 6e20 5f63 6f6e 7665 7274 6572 732e 636f  n _converters.co
+0002e860: 6e76 6572 745f 7365 636f 6e64 735f 7265  nvert_seconds_re
+0002e870: 616c 3634 5f74 6f5f 7469 6d65 6465 6c74  al64_to_timedelt
+0002e880: 6173 286f 6666 7365 7473 290a 0a20 2020  as(offsets)..   
+0002e890: 2064 6566 2075 6e6c 6f63 6b28 7365 6c66   def unlock(self
+0002e8a0: 293a 0a20 2020 2020 2020 2027 2727 756e  ):.        '''un
+0002e8b0: 6c6f 636b 0a0a 2020 2020 2020 2020 5265  lock..        Re
+0002e8c0: 6c65 6173 6573 2061 206c 6f63 6b20 7468  leases a lock th
+0002e8d0: 6174 2079 6f75 2061 6371 7569 7265 6420  at you acquired 
+0002e8e0: 6f6e 2061 6e20 6465 7669 6365 2073 6573  on an device ses
+0002e8f0: 7369 6f6e 2075 7369 6e67 0a20 2020 2020  sion using.     
+0002e900: 2020 206c 6f63 6b2e 2052 6566 6572 2074     lock. Refer t
+0002e910: 6f20 6c6f 636b 2066 6f72 2061 6464 6974  o lock for addit
+0002e920: 696f 6e61 6c0a 2020 2020 2020 2020 696e  ional.        in
+0002e930: 666f 726d 6174 696f 6e20 6f6e 2073 6573  formation on ses
+0002e940: 7369 6f6e 206c 6f63 6b73 2e0a 2020 2020  sion locks..    
+0002e950: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+0002e960: 7365 6c66 2e5f 696e 7465 7270 7265 7465  self._interprete
+0002e970: 722e 756e 6c6f 636b 2829 0a0a 2020 2020  r.unlock()..    
+0002e980: 4069 7669 5f73 796e 6368 726f 6e69 7a65  @ivi_synchronize
+0002e990: 640a 2020 2020 6465 6620 5f77 7269 7465  d.    def _write
+0002e9a0: 5f73 6f75 7263 655f 7761 7665 666f 726d  _source_waveform
+0002e9b0: 5f73 6974 655f 756e 6971 7565 5f75 3332  _site_unique_u32
+0002e9c0: 2873 656c 662c 2077 6176 6566 6f72 6d5f  (self, waveform_
+0002e9d0: 6e61 6d65 2c20 6e75 6d5f 7761 7665 666f  name, num_wavefo
+0002e9e0: 726d 732c 2073 616d 706c 6573 5f70 6572  rms, samples_per
+0002e9f0: 5f77 6176 6566 6f72 6d2c 2077 6176 6566  _waveform, wavef
+0002ea00: 6f72 6d5f 6461 7461 293a 0a20 2020 2020  orm_data):.     
+0002ea10: 2020 2072 2727 275f 7772 6974 655f 736f     r'''_write_so
+0002ea20: 7572 6365 5f77 6176 6566 6f72 6d5f 7369  urce_waveform_si
+0002ea30: 7465 5f75 6e69 7175 655f 7533 320a 0a20  te_unique_u32.. 
+0002ea40: 2020 2020 2020 2057 7269 7465 7320 6f6e         Writes on
+0002ea50: 6520 7761 7665 666f 726d 2070 6572 2073  e waveform per s
+0002ea60: 6974 652e 2055 7365 2074 6869 7320 7772  ite. Use this wr
+0002ea70: 6974 6520 6d65 7468 6f64 2069 6620 796f  ite method if yo
+0002ea80: 7520 7365 7420 7468 6520 7061 7261 6d65  u set the parame
+0002ea90: 7465 7220 6f66 2074 6865 2063 7265 6174  ter of the creat
+0002eaa0: 6520 736f 7572 6365 2077 6176 6566 6f72  e source wavefor
+0002eab0: 6d20 6d65 7468 6f64 2074 6f20 5369 7465  m method to Site
+0002eac0: 2055 6e69 7175 652e 0a0a 2020 2020 2020   Unique...      
+0002ead0: 2020 5469 703a 0a20 2020 2020 2020 2054    Tip:.        T
+0002eae0: 6869 7320 6d65 7468 6f64 2063 616e 2062  his method can b
+0002eaf0: 6520 6361 6c6c 6564 206f 6e20 7370 6563  e called on spec
+0002eb00: 6966 6963 2073 6974 6573 2077 6974 6869  ific sites withi
+0002eb10: 6e20 796f 7572 203a 7079 3a63 6c61 7373  n your :py:class
+0002eb20: 3a60 6e69 6469 6769 7461 6c2e 5365 7373  :`nidigital.Sess
+0002eb30: 696f 6e60 2069 6e73 7461 6e63 652e 0a20  ion` instance.. 
+0002eb40: 2020 2020 2020 2055 7365 2050 7974 686f         Use Pytho
+0002eb50: 6e20 696e 6465 7820 6e6f 7461 7469 6f6e  n index notation
+0002eb60: 206f 6e20 7468 6520 7265 7065 6174 6564   on the repeated
+0002eb70: 2063 6170 6162 696c 6974 6965 7320 636f   capabilities co
+0002eb80: 6e74 6169 6e65 7220 7369 7465 7320 746f  ntainer sites to
+0002eb90: 2073 7065 6369 6679 2061 2073 7562 7365   specify a subse
+0002eba0: 742c 0a20 2020 2020 2020 2061 6e64 2074  t,.        and t
+0002ebb0: 6865 6e20 6361 6c6c 2074 6869 7320 6d65  hen call this me
+0002ebc0: 7468 6f64 206f 6e20 7468 6520 7265 7375  thod on the resu
+0002ebd0: 6c74 2e0a 0a20 2020 2020 2020 2045 7861  lt...        Exa
+0002ebe0: 6d70 6c65 3a20 3a70 793a 6d65 7468 3a60  mple: :py:meth:`
+0002ebf0: 6d79 5f73 6573 7369 6f6e 2e73 6974 6573  my_session.sites
+0002ec00: 5b20 2e2e 2e20 5d2e 5f77 7269 7465 5f73  [ ... ]._write_s
+0002ec10: 6f75 7263 655f 7761 7665 666f 726d 5f73  ource_waveform_s
+0002ec20: 6974 655f 756e 6971 7565 5f75 3332 600a  ite_unique_u32`.
+0002ec30: 0a20 2020 2020 2020 2054 6f20 6361 6c6c  .        To call
+0002ec40: 2074 6865 206d 6574 686f 6420 6f6e 2061   the method on a
+0002ec50: 6c6c 2073 6974 6573 2c20 796f 7520 6361  ll sites, you ca
+0002ec60: 6e20 6361 6c6c 2069 7420 6469 7265 6374  n call it direct
+0002ec70: 6c79 206f 6e20 7468 6520 3a70 793a 636c  ly on the :py:cl
+0002ec80: 6173 733a 606e 6964 6967 6974 616c 2e53  ass:`nidigital.S
+0002ec90: 6573 7369 6f6e 602e 0a0a 2020 2020 2020  ession`...      
+0002eca0: 2020 4578 616d 706c 653a 203a 7079 3a6d    Example: :py:m
+0002ecb0: 6574 683a 606d 795f 7365 7373 696f 6e2e  eth:`my_session.
+0002ecc0: 5f77 7269 7465 5f73 6f75 7263 655f 7761  _write_source_wa
+0002ecd0: 7665 666f 726d 5f73 6974 655f 756e 6971  veform_site_uniq
+0002ece0: 7565 5f75 3332 600a 0a20 2020 2020 2020  ue_u32`..       
+0002ecf0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0002ed00: 2020 2077 6176 6566 6f72 6d5f 6e61 6d65     waveform_name
+0002ed10: 2028 7374 7229 3a20 5468 6520 6e61 6d65   (str): The name
+0002ed20: 2074 6f20 6173 7369 676e 2074 6f20 7468   to assign to th
+0002ed30: 6520 7761 7665 666f 726d 2e20 5573 6520  e waveform. Use 
+0002ed40: 7468 6520 7761 7665 666f 726d 5f6e 616d  the waveform_nam
+0002ed50: 6520 2077 6974 6820 736f 7572 6365 5f73  e  with source_s
+0002ed60: 7461 7274 206f 7063 6f64 6520 696e 2079  tart opcode in y
+0002ed70: 6f75 7220 7061 7474 6572 6e2e 0a0a 2020  our pattern...  
+0002ed80: 2020 2020 2020 2020 2020 6e75 6d5f 7761            num_wa
+0002ed90: 7665 666f 726d 7320 2869 6e74 293a 204e  veforms (int): N
+0002eda0: 756d 6265 7220 6f66 2077 6176 6566 6f72  umber of wavefor
+0002edb0: 6d73 2e0a 0a20 2020 2020 2020 2020 2020  ms...           
+0002edc0: 2073 616d 706c 6573 5f70 6572 5f77 6176   samples_per_wav
+0002edd0: 6566 6f72 6d20 2869 6e74 293a 204e 756d  eform (int): Num
+0002ede0: 6265 7220 6f66 2073 616d 706c 6573 2070  ber of samples p
+0002edf0: 6572 2077 6176 6566 6f72 6d2e 0a0a 2020  er waveform...  
+0002ee00: 2020 2020 2020 2020 2020 7761 7665 666f            wavefo
+0002ee10: 726d 5f64 6174 6120 2861 7272 6179 2e61  rm_data (array.a
+0002ee20: 7272 6179 2822 4c22 2929 3a20 416e 2061  rray("L")): An a
+0002ee30: 7272 6179 206f 6620 7361 6d70 6c65 7320  rray of samples 
+0002ee40: 746f 2075 7365 2061 7320 736f 7572 6365  to use as source
+0002ee50: 2064 6174 612e 2044 6174 6120 666f 7220   data. Data for 
+0002ee60: 6561 6368 2073 6974 6520 6d75 7374 2062  each site must b
+0002ee70: 6520 6170 7065 6e64 6564 2073 6571 7565  e appended seque
+0002ee80: 6e74 6961 6c6c 7920 696e 2074 6865 2061  ntially in the a
+0002ee90: 7272 6179 2028 6e6f 6e2d 696e 7465 726c  rray (non-interl
+0002eea0: 6561 7665 6429 2e0a 0a20 2020 2020 2020  eaved)...       
+0002eeb0: 2027 2727 0a20 2020 2020 2020 2073 656c   '''.        sel
+0002eec0: 662e 5f69 6e74 6572 7072 6574 6572 2e77  f._interpreter.w
+0002eed0: 7269 7465 5f73 6f75 7263 655f 7761 7665  rite_source_wave
+0002eee0: 666f 726d 5f73 6974 655f 756e 6971 7565  form_site_unique
+0002eef0: 5f75 3332 2873 656c 662e 5f72 6570 6561  _u32(self._repea
+0002ef00: 7465 645f 6361 7061 6269 6c69 7479 2c20  ted_capability, 
+0002ef10: 7761 7665 666f 726d 5f6e 616d 652c 206e  waveform_name, n
+0002ef20: 756d 5f77 6176 6566 6f72 6d73 2c20 7361  um_waveforms, sa
+0002ef30: 6d70 6c65 735f 7065 725f 7761 7665 666f  mples_per_wavefo
+0002ef40: 726d 2c20 7761 7665 666f 726d 5f64 6174  rm, waveform_dat
+0002ef50: 6129 0a0a 2020 2020 4069 7669 5f73 796e  a)..    @ivi_syn
+0002ef60: 6368 726f 6e69 7a65 640a 2020 2020 6465  chronized.    de
+0002ef70: 6620 7772 6974 655f 7374 6174 6963 2873  f write_static(s
+0002ef80: 656c 662c 2073 7461 7465 293a 0a20 2020  elf, state):.   
+0002ef90: 2020 2020 2072 2727 2777 7269 7465 5f73       r'''write_s
+0002efa0: 7461 7469 630a 0a20 2020 2020 2020 2057  tatic..        W
+0002efb0: 7269 7465 7320 6120 7374 6174 6963 2073  rites a static s
+0002efc0: 7461 7465 2074 6f20 7468 6520 7370 6563  tate to the spec
+0002efd0: 6966 6965 6420 7069 6e73 2e20 5468 6520  ified pins. The 
+0002efe0: 7365 6c65 6374 6564 2070 696e 7320 7265  selected pins re
+0002eff0: 6d61 696e 2069 6e20 7468 6520 7370 6563  main in the spec
+0002f000: 6966 6965 6420 7374 6174 6520 756e 7469  ified state unti
+0002f010: 6c20 7468 6520 6e65 7874 2070 6174 7465  l the next patte
+0002f020: 726e 2062 7572 7374 206f 7220 6361 6c6c  rn burst or call
+0002f030: 2074 6f20 7468 6973 206d 6574 686f 642e   to this method.
+0002f040: 2049 6620 7468 6572 6520 6172 6520 756e   If there are un
+0002f050: 636f 6d6d 6974 7465 6420 6368 616e 6765  committed change
+0002f060: 7320 746f 206c 6576 656c 7320 6f72 2074  s to levels or t
+0002f070: 6865 2074 6572 6d69 6e61 7469 6f6e 206d  he termination m
+0002f080: 6f64 652c 2074 6869 7320 6d65 7468 6f64  ode, this method
+0002f090: 2063 6f6d 6d69 7473 2074 6865 2063 6861   commits the cha
+0002f0a0: 6e67 6573 2074 6f20 7468 6520 7069 6e73  nges to the pins
+0002f0b0: 2e20 5468 6973 206d 6574 686f 6420 646f  . This method do
+0002f0c0: 6573 206e 6f74 2063 6861 6e67 6520 7468  es not change th
+0002f0d0: 6520 7365 6c65 6374 6564 2070 696e 206d  e selected pin m
+0002f0e0: 6574 686f 642e 2049 6620 796f 7520 7772  ethod. If you wr
+0002f0f0: 6974 6520 6120 7374 6174 6963 2073 7461  ite a static sta
+0002f100: 7465 2074 6f20 6120 7069 6e20 7468 6174  te to a pin that
+0002f110: 2064 6f65 7320 6e6f 7420 6861 7665 2074   does not have t
+0002f120: 6865 2044 6967 6974 616c 206d 6574 686f  he Digital metho
+0002f130: 6420 7365 6c65 6374 6564 2c20 7468 6520  d selected, the 
+0002f140: 6e65 7720 7374 6174 6963 2073 7461 7465  new static state
+0002f150: 2069 7320 7374 6f72 6564 2062 7920 7468   is stored by th
+0002f160: 6520 696e 7374 7275 6d65 6e74 2c20 616e  e instrument, an
+0002f170: 6420 6166 6665 6374 7320 7468 6520 7374  d affects the st
+0002f180: 6174 6520 6f66 2074 6865 2070 696e 2074  ate of the pin t
+0002f190: 6865 206e 6578 7420 7469 6d65 2079 6f75  he next time you
+0002f1a0: 2063 6861 6e67 6520 7468 6520 7365 6c65   change the sele
+0002f1b0: 6374 6564 206d 6574 686f 6420 746f 2044  cted method to D
+0002f1c0: 6967 6974 616c 2e0a 0a20 2020 2020 2020  igital...       
+0002f1d0: 2054 6970 3a0a 2020 2020 2020 2020 5468   Tip:.        Th
+0002f1e0: 6973 206d 6574 686f 6420 6361 6e20 6265  is method can be
+0002f1f0: 2063 616c 6c65 6420 6f6e 2073 7065 6369   called on speci
+0002f200: 6669 6320 6368 616e 6e65 6c73 2077 6974  fic channels wit
+0002f210: 6869 6e20 796f 7572 203a 7079 3a63 6c61  hin your :py:cla
+0002f220: 7373 3a60 6e69 6469 6769 7461 6c2e 5365  ss:`nidigital.Se
+0002f230: 7373 696f 6e60 2069 6e73 7461 6e63 652e  ssion` instance.
+0002f240: 0a20 2020 2020 2020 2055 7365 2050 7974  .        Use Pyt
+0002f250: 686f 6e20 696e 6465 7820 6e6f 7461 7469  hon index notati
+0002f260: 6f6e 206f 6e20 7468 6520 7265 7065 6174  on on the repeat
+0002f270: 6564 2063 6170 6162 696c 6974 6965 7320  ed capabilities 
+0002f280: 636f 6e74 6169 6e65 7220 6368 616e 6e65  container channe
+0002f290: 6c73 2074 6f20 7370 6563 6966 7920 6120  ls to specify a 
+0002f2a0: 7375 6273 6574 2c0a 2020 2020 2020 2020  subset,.        
+0002f2b0: 616e 6420 7468 656e 2063 616c 6c20 7468  and then call th
+0002f2c0: 6973 206d 6574 686f 6420 6f6e 2074 6865  is method on the
+0002f2d0: 2072 6573 756c 742e 0a0a 2020 2020 2020   result...      
+0002f2e0: 2020 4578 616d 706c 653a 203a 7079 3a6d    Example: :py:m
+0002f2f0: 6574 683a 606d 795f 7365 7373 696f 6e2e  eth:`my_session.
+0002f300: 6368 616e 6e65 6c73 5b20 2e2e 2e20 5d2e  channels[ ... ].
+0002f310: 7772 6974 655f 7374 6174 6963 600a 0a20  write_static`.. 
+0002f320: 2020 2020 2020 2054 6f20 6361 6c6c 2074         To call t
+0002f330: 6865 206d 6574 686f 6420 6f6e 2061 6c6c  he method on all
+0002f340: 2063 6861 6e6e 656c 732c 2079 6f75 2063   channels, you c
+0002f350: 616e 2063 616c 6c20 6974 2064 6972 6563  an call it direc
+0002f360: 746c 7920 6f6e 2074 6865 203a 7079 3a63  tly on the :py:c
+0002f370: 6c61 7373 3a60 6e69 6469 6769 7461 6c2e  lass:`nidigital.
+0002f380: 5365 7373 696f 6e60 2e0a 0a20 2020 2020  Session`...     
+0002f390: 2020 2045 7861 6d70 6c65 3a20 3a70 793a     Example: :py:
+0002f3a0: 6d65 7468 3a60 6d79 5f73 6573 7369 6f6e  meth:`my_session
+0002f3b0: 2e77 7269 7465 5f73 7461 7469 6360 0a0a  .write_static`..
+0002f3c0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0002f3d0: 2020 2020 2020 2020 2020 7374 6174 6520            state 
+0002f3e0: 2865 6e75 6d73 2e57 7269 7465 5374 6174  (enums.WriteStat
+0002f3f0: 6963 5069 6e53 7461 7465 293a 2050 6172  icPinState): Par
+0002f400: 616d 6574 6572 2074 6861 7420 7370 6563  ameter that spec
+0002f410: 6966 6965 7320 6f6e 6520 6f66 2074 6865  ifies one of the
+0002f420: 2066 6f6c 6c6f 7769 6e67 2064 6967 6974   following digit
+0002f430: 616c 2073 7461 7465 7320 746f 2061 7373  al states to ass
+0002f440: 6967 6e20 746f 2074 6865 2070 696e 2e0a  ign to the pin..
+0002f450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002f460: 202d 2020 2057 7269 7465 5374 6174 6963   -   WriteStatic
+0002f470: 5069 6e53 7461 7465 2e5a 4552 4f3a 2053  PinState.ZERO: S
+0002f480: 7065 6369 6669 6573 2074 6f20 6472 6976  pecifies to driv
+0002f490: 6520 6c6f 772e 0a20 2020 2020 2020 2020  e low..         
+0002f4a0: 2020 2020 2020 202d 2020 2057 7269 7465         -   Write
+0002f4b0: 5374 6174 6963 5069 6e53 7461 7465 2e4f  StaticPinState.O
+0002f4c0: 4e45 3a20 5370 6563 6966 6965 7320 746f  NE: Specifies to
+0002f4d0: 2064 7269 7665 2068 6967 682e 0a20 2020   drive high..   
+0002f4e0: 2020 2020 2020 2020 2020 2020 202d 2020               -  
+0002f4f0: 2057 7269 7465 5374 6174 6963 5069 6e53   WriteStaticPinS
+0002f500: 7461 7465 2e58 3a20 5370 6563 6966 6965  tate.X: Specifie
+0002f510: 7320 746f 206e 6f74 2064 7269 7665 2e0a  s to not drive..
+0002f520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002f530: 204e 6f74 653a 0a20 2020 2020 2020 2020   Note:.         
+0002f540: 2020 2020 2020 204f 6e65 206f 7220 6d6f         One or mo
+0002f550: 7265 206f 6620 7468 6520 7265 6665 7265  re of the refere
+0002f560: 6e63 6564 2076 616c 7565 7320 6172 6520  nced values are 
+0002f570: 6e6f 7420 696e 2074 6865 2050 7974 686f  not in the Pytho
+0002f580: 6e20 4150 4920 666f 7220 7468 6973 2064  n API for this d
+0002f590: 7269 7665 722e 2045 6e75 6d73 2074 6861  river. Enums tha
+0002f5a0: 7420 6f6e 6c79 2064 6566 696e 6520 7661  t only define va
+0002f5b0: 6c75 6573 2c20 6f72 2072 6570 7265 7365  lues, or represe
+0002f5c0: 6e74 2054 7275 652f 4661 6c73 652c 2068  nt True/False, h
+0002f5d0: 6176 6520 6265 656e 2072 656d 6f76 6564  ave been removed
+0002f5e0: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
+0002f5f0: 2020 2020 2020 2069 6620 7479 7065 2873         if type(s
+0002f600: 7461 7465 2920 6973 206e 6f74 2065 6e75  tate) is not enu
+0002f610: 6d73 2e57 7269 7465 5374 6174 6963 5069  ms.WriteStaticPi
+0002f620: 6e53 7461 7465 3a0a 2020 2020 2020 2020  nState:.        
+0002f630: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+0002f640: 726f 7228 2750 6172 616d 6574 6572 2073  ror('Parameter s
+0002f650: 7461 7465 206d 7573 7420 6265 206f 6620  tate must be of 
+0002f660: 7479 7065 2027 202b 2073 7472 2865 6e75  type ' + str(enu
+0002f670: 6d73 2e57 7269 7465 5374 6174 6963 5069  ms.WriteStaticPi
+0002f680: 6e53 7461 7465 2929 0a20 2020 2020 2020  nState)).       
+0002f690: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
+0002f6a0: 6572 2e77 7269 7465 5f73 7461 7469 6328  er.write_static(
+0002f6b0: 7365 6c66 2e5f 7265 7065 6174 6564 5f63  self._repeated_c
+0002f6c0: 6170 6162 696c 6974 792c 2073 7461 7465  apability, state
+0002f6d0: 290a 0a20 2020 2064 6566 205f 6572 726f  )..    def _erro
+0002f6e0: 725f 6d65 7373 6167 6528 7365 6c66 2c20  r_message(self, 
+0002f6f0: 6572 726f 725f 636f 6465 293a 0a20 2020  error_code):.   
+0002f700: 2020 2020 2072 2727 275f 6572 726f 725f       r'''_error_
+0002f710: 6d65 7373 6167 650a 0a20 2020 2020 2020  message..       
+0002f720: 2054 616b 6573 2074 6865 2065 7272 6f72   Takes the error
+0002f730: 2063 6f64 6520 7265 7475 726e 6564 2062   code returned b
+0002f740: 7920 7468 6520 6469 6769 7461 6c20 7061  y the digital pa
+0002f750: 7474 6572 6e20 696e 7374 7275 6d65 6e74  ttern instrument
+0002f760: 2064 7269 7665 7220 6d65 7468 6f64 732c   driver methods,
+0002f770: 2069 6e74 6572 7072 6574 7320 6974 2c20   interprets it, 
+0002f780: 616e 6420 7265 7475 726e 7320 6974 2061  and returns it a
+0002f790: 7320 6120 7573 6572 2072 6561 6461 626c  s a user readabl
+0002f7a0: 6520 7374 7269 6e67 2e0a 0a20 2020 2020  e string...     
+0002f7b0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0002f7c0: 2020 2020 2065 7272 6f72 5f63 6f64 6520       error_code 
+0002f7d0: 2869 6e74 293a 2054 6865 2073 7065 6369  (int): The speci
+0002f7e0: 6669 6564 2065 7272 6f72 2063 6f64 652e  fied error code.
+0002f7f0: 0a0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0002f800: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0002f810: 6572 726f 725f 6d65 7373 6167 6520 2873  error_message (s
+0002f820: 7472 293a 2054 6865 2065 7272 6f72 2069  tr): The error i
+0002f830: 6e66 6f72 6d61 7469 6f6e 2066 6f72 6d61  nformation forma
+0002f840: 7474 6564 2061 7320 6120 7374 7269 6e67  tted as a string
+0002f850: 2e20 5468 6520 6172 7261 7920 6d75 7374  . The array must
+0002f860: 2063 6f6e 7461 696e 2061 7420 6c65 6173   contain at leas
+0002f870: 7420 3235 3620 6368 6172 6163 7465 7273  t 256 characters
+0002f880: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
+0002f890: 2020 2020 2020 2065 7272 6f72 5f6d 6573         error_mes
+0002f8a0: 7361 6765 203d 2073 656c 662e 5f69 6e74  sage = self._int
+0002f8b0: 6572 7072 6574 6572 2e65 7272 6f72 5f6d  erpreter.error_m
+0002f8c0: 6573 7361 6765 2865 7272 6f72 5f63 6f64  essage(error_cod
+0002f8d0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+0002f8e0: 6e20 6572 726f 725f 6d65 7373 6167 650a  n error_message.
+0002f8f0: 0a0a 636c 6173 7320 5365 7373 696f 6e28  ..class Session(
+0002f900: 5f53 6573 7369 6f6e 4261 7365 293a 0a20  _SessionBase):. 
+0002f910: 2020 2027 2727 416e 204e 492d 4469 6769     '''An NI-Digi
+0002f920: 7461 6c20 5061 7474 6572 6e20 4472 6976  tal Pattern Driv
+0002f930: 6572 2073 6573 7369 6f6e 2727 270a 0a20  er session'''.. 
+0002f940: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0002f950: 7365 6c66 2c20 7265 736f 7572 6365 5f6e  self, resource_n
+0002f960: 616d 652c 2069 645f 7175 6572 793d 4661  ame, id_query=Fa
+0002f970: 6c73 652c 2072 6573 6574 5f64 6576 6963  lse, reset_devic
+0002f980: 653d 4661 6c73 652c 206f 7074 696f 6e73  e=False, options
+0002f990: 3d7b 7d2c 202a 2c20 6772 7063 5f6f 7074  ={}, *, grpc_opt
+0002f9a0: 696f 6e73 3d4e 6f6e 6529 3a0a 2020 2020  ions=None):.    
+0002f9b0: 2020 2020 7227 2727 416e 204e 492d 4469      r'''An NI-Di
+0002f9c0: 6769 7461 6c20 5061 7474 6572 6e20 4472  gital Pattern Dr
+0002f9d0: 6976 6572 2073 6573 7369 6f6e 0a0a 2020  iver session..  
+0002f9e0: 2020 2020 2020 4372 6561 7465 7320 616e        Creates an
+0002f9f0: 6420 7265 7475 726e 7320 6120 6e65 7720  d returns a new 
+0002fa00: 7365 7373 696f 6e20 746f 2074 6865 2073  session to the s
+0002fa10: 7065 6369 6669 6564 2064 6967 6974 616c  pecified digital
+0002fa20: 2070 6174 7465 726e 2069 6e73 7472 756d   pattern instrum
+0002fa30: 656e 7420 746f 2075 7365 2069 6e20 616c  ent to use in al
+0002fa40: 6c20 7375 6273 6571 7565 6e74 206d 6574  l subsequent met
+0002fa50: 686f 6420 6361 6c6c 732e 2054 6f20 706c  hod calls. To pl
+0002fa60: 6163 6520 7468 6520 696e 7374 7275 6d65  ace the instrume
+0002fa70: 6e74 2069 6e20 6120 6b6e 6f77 6e20 7374  nt in a known st
+0002fa80: 6172 7475 7020 7374 6174 6520 7768 656e  artup state when
+0002fa90: 2063 7265 6174 696e 6720 6120 6e65 7720   creating a new 
+0002faa0: 7365 7373 696f 6e2c 2073 6574 2074 6865  session, set the
+0002fab0: 2072 6573 6574 2070 6172 616d 6574 6572   reset parameter
+0002fac0: 2074 6f20 5472 7565 2c20 7768 6963 6820   to True, which 
+0002fad0: 6973 2065 7175 6976 616c 656e 7420 746f  is equivalent to
+0002fae0: 2063 616c 6c69 6e67 2074 6865 2072 6573   calling the res
+0002faf0: 6574 206d 6574 686f 6420 696d 6d65 6469  et method immedi
+0002fb00: 6174 656c 7920 6166 7465 7220 696e 6974  ately after init
+0002fb10: 6961 6c69 7a69 6e67 2074 6865 2073 6573  ializing the ses
+0002fb20: 7369 6f6e 2e0a 0a20 2020 2020 2020 2041  sion...        A
+0002fb30: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0002fb40: 2072 6573 6f75 7263 655f 6e61 6d65 2028   resource_name (
+0002fb50: 7374 7229 3a20 5468 6520 7370 6563 6966  str): The specif
+0002fb60: 6965 6420 7265 736f 7572 6365 206e 616d  ied resource nam
+0002fb70: 6520 7368 6f77 6e20 696e 204d 6561 7375  e shown in Measu
+0002fb80: 7265 6d65 6e74 2026 2041 7574 6f6d 6174  rement & Automat
+0002fb90: 696f 6e20 4578 706c 6f72 6572 2028 4d41  ion Explorer (MA
+0002fba0: 5829 2066 6f72 2061 2064 6967 6974 616c  X) for a digital
+0002fbb0: 2070 6174 7465 726e 2069 6e73 7472 756d   pattern instrum
+0002fbc0: 656e 742c 2066 6f72 2065 7861 6d70 6c65  ent, for example
+0002fbd0: 2c20 5058 4931 536c 6f74 332c 2077 6865  , PXI1Slot3, whe
+0002fbe0: 7265 2050 5849 3153 6c6f 7433 2069 7320  re PXI1Slot3 is 
+0002fbf0: 616e 2069 6e73 7472 756d 656e 7420 7265  an instrument re
+0002fc00: 736f 7572 6365 206e 616d 652e 202a 2a72  source name. **r
+0002fc10: 6573 6f75 7263 654e 616d 652a 2a20 6361  esourceName** ca
+0002fc20: 6e20 616c 736f 2062 6520 6120 6c6f 6769  n also be a logi
+0002fc30: 6361 6c20 4956 4920 6e61 6d65 2e20 5468  cal IVI name. Th
+0002fc40: 6973 2070 6172 616d 6574 6572 2061 6363  is parameter acc
+0002fc50: 6570 7473 2061 2063 6f6d 6d61 2d64 656c  epts a comma-del
+0002fc60: 696d 6974 6564 206c 6973 7420 6f66 2073  imited list of s
+0002fc70: 7472 696e 6773 2069 6e20 7468 6520 666f  trings in the fo
+0002fc80: 726d 2050 5849 3153 6c6f 7432 2c50 5849  rm PXI1Slot2,PXI
+0002fc90: 3153 6c6f 7433 2c20 7768 6572 6520 6060  1Slot3, where ``
+0002fca0: 5058 4931 536c 6f74 3260 6020 6973 206f  PXI1Slot2`` is o
+0002fcb0: 6e65 2069 6e73 7472 756d 656e 7420 7265  ne instrument re
+0002fcc0: 736f 7572 6365 206e 616d 6520 616e 6420  source name and 
+0002fcd0: 6060 5058 4931 536c 6f74 3360 6020 6973  ``PXI1Slot3`` is
+0002fce0: 2061 6e6f 7468 6572 2e20 5768 656e 2069   another. When i
+0002fcf0: 6e63 6c75 6469 6e67 206d 6f72 6520 7468  ncluding more th
+0002fd00: 616e 206f 6e65 2064 6967 6974 616c 2070  an one digital p
+0002fd10: 6174 7465 726e 2069 6e73 7472 756d 656e  attern instrumen
+0002fd20: 7420 696e 2074 6865 2063 6f6d 6d61 2d64  t in the comma-d
+0002fd30: 656c 696d 6974 6564 206c 6973 7420 6f66  elimited list of
+0002fd40: 2073 7472 696e 6773 2c20 6c69 7374 2074   strings, list t
+0002fd50: 6865 2069 6e73 7472 756d 656e 7473 2069  he instruments i
+0002fd60: 6e20 7468 6520 7361 6d65 206f 7264 6572  n the same order
+0002fd70: 2074 6865 7920 6170 7065 6172 2069 6e20   they appear in 
+0002fd80: 7468 6520 7069 6e20 6d61 702e 0a0a 2020  the pin map...  
+0002fd90: 2020 2020 2020 2020 2020 2020 2020 2b2d                +-
+0002fda0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
 0002fdb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fdc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fdd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fde0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fdf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fe00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fe10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fe20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fe30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fe40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fe50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0002fe60: 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020 2020  -------+.       
-0002fe70: 2020 2020 2020 2020 207c 207c 4e6f 7465           | |Note
-0002fe80: 7c20 7c20 4e6f 7465 c2a0 c2a0 2059 6f75  | | Note.... You
-0002fe90: 206f 6e6c 7920 6361 6e20 7370 6563 6966   only can specif
-0002fea0: 7920 6d75 6c74 6970 6c65 2069 6e73 7472  y multiple instr
-0002feb0: 756d 656e 7473 206f 6620 7468 6520 7361  uments of the sa
-0002fec0: 6d65 206d 6f64 656c 2e20 466f 7220 6578  me model. For ex
-0002fed0: 616d 706c 652c 2079 6f75 2063 616e 206c  ample, you can l
-0002fee0: 6973 7420 7477 6f20 5058 4965 2d36 3537  ist two PXIe-657
-0002fef0: 3073 2062 7574 206e 6f74 2061 2050 5849  0s but not a PXI
-0002ff00: 652d 3635 3730 2061 6e64 2050 5849 652d  e-6570 and PXIe-
-0002ff10: 3635 3731 2e20 5468 6520 696e 7374 7275  6571. The instru
-0002ff20: 6d65 6e74 7320 6d75 7374 2062 6520 696e  ments must be in
-0002ff30: 2074 6865 2073 616d 6520 6368 6173 7369   the same chassi
-0002ff40: 732e 207c 0a20 2020 2020 2020 2020 2020  s. |.           
-0002ff50: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2b2d       +--------+-
+0002fe60: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
+0002fe70: 2020 2020 2020 2020 7c20 7c4e 6f74 657c          | |Note|
+0002fe80: 207c 204e 6f74 65c2 a0c2 a020 596f 7520   | Note.... You 
+0002fe90: 6f6e 6c79 2063 616e 2073 7065 6369 6679  only can specify
+0002fea0: 206d 756c 7469 706c 6520 696e 7374 7275   multiple instru
+0002feb0: 6d65 6e74 7320 6f66 2074 6865 2073 616d  ments of the sam
+0002fec0: 6520 6d6f 6465 6c2e 2046 6f72 2065 7861  e model. For exa
+0002fed0: 6d70 6c65 2c20 796f 7520 6361 6e20 6c69  mple, you can li
+0002fee0: 7374 2074 776f 2050 5849 652d 3635 3730  st two PXIe-6570
+0002fef0: 7320 6275 7420 6e6f 7420 6120 5058 4965  s but not a PXIe
+0002ff00: 2d36 3537 3020 616e 6420 5058 4965 2d36  -6570 and PXIe-6
+0002ff10: 3537 312e 2054 6865 2069 6e73 7472 756d  571. The instrum
+0002ff20: 656e 7473 206d 7573 7420 6265 2069 6e20  ents must be in 
+0002ff30: 7468 6520 7361 6d65 2063 6861 7373 6973  the same chassis
+0002ff40: 2e20 7c0a 2020 2020 2020 2020 2020 2020  . |.            
+0002ff50: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d      +--------+--
 0002ff60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002ff70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002ff80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002ff90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002ffa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002ffb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002ffc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002ffd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002ffe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0002fff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00030000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00030010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a  -------------+..
-00030020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030030: 2e2e 207c 4e6f 7465 7c20 696d 6167 653a  .. |Note| image:
-00030040: 3a20 6e6f 7465 2e67 6966 0a0a 2020 2020  : note.gif..    
-00030050: 2020 2020 2020 2020 2020 2020 4e6f 7465              Note
-00030060: 3a0a 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00030070: 645f 7175 6572 7920 2862 6f6f 6c29 3a20  d_query (bool): 
-00030080: 4120 426f 6f6c 6561 6e20 7468 6174 2076  A Boolean that v
-00030090: 6572 6966 6965 7320 7468 6174 2074 6865  erifies that the
-000300a0: 2064 6967 6974 616c 2070 6174 7465 726e   digital pattern
-000300b0: 2069 6e73 7472 756d 656e 7420 796f 7520   instrument you 
-000300c0: 696e 6974 6961 6c69 7a65 2069 7320 7375  initialize is su
-000300d0: 7070 6f72 7465 6420 6279 204e 492d 4469  pported by NI-Di
-000300e0: 6769 7461 6c2e 204e 492d 4469 6769 7461  gital. NI-Digita
-000300f0: 6c20 6175 746f 6d61 7469 6361 6c6c 7920  l automatically 
-00030100: 7065 7266 6f72 6d73 2074 6869 7320 7175  performs this qu
-00030110: 6572 792c 2073 6f20 7365 7474 696e 6720  ery, so setting 
-00030120: 7468 6973 2070 6172 616d 6574 6572 2069  this parameter i
-00030130: 7320 6e6f 7420 6e65 6365 7373 6172 792e  s not necessary.
-00030140: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00030150: 7365 745f 6465 7669 6365 2028 626f 6f6c  set_device (bool
-00030160: 293a 2041 2042 6f6f 6c65 616e 2074 6861  ): A Boolean tha
-00030170: 7420 7370 6563 6966 6965 7320 7768 6574  t specifies whet
-00030180: 6865 7220 746f 2072 6573 6574 2061 2064  her to reset a d
-00030190: 6967 6974 616c 2070 6174 7465 726e 2069  igital pattern i
-000301a0: 6e73 7472 756d 656e 7420 746f 2061 206b  nstrument to a k
-000301b0: 6e6f 776e 2073 7461 7465 2077 6865 6e20  nown state when 
-000301c0: 7468 6520 7365 7373 696f 6e20 6973 2069  the session is i
-000301d0: 6e69 7469 616c 697a 6564 2e20 5365 7474  nitialized. Sett
-000301e0: 696e 6720 7468 6520 2a2a 7265 7365 7444  ing the **resetD
-000301f0: 6576 6963 652a 2a20 7661 6c75 6520 746f  evice** value to
-00030200: 2054 7275 6520 6973 2065 7175 6976 616c   True is equival
-00030210: 656e 7420 746f 2063 616c 6c69 6e67 2074  ent to calling t
-00030220: 6865 2072 6573 6574 206d 6574 686f 6420  he reset method 
-00030230: 696d 6d65 6469 6174 656c 7920 6166 7465  immediately afte
-00030240: 7220 696e 6974 6961 6c69 7a69 6e67 2074  r initializing t
-00030250: 6865 2073 6573 7369 6f6e 2e0a 0a20 2020  he session...   
-00030260: 2020 2020 2020 2020 206f 7074 696f 6e73           options
-00030270: 2028 6469 6374 293a 2053 7065 6369 6669   (dict): Specifi
-00030280: 6573 2074 6865 2069 6e69 7469 616c 2076  es the initial v
-00030290: 616c 7565 206f 6620 6365 7274 6169 6e20  alue of certain 
-000302a0: 7072 6f70 6572 7469 6573 2066 6f72 2074  properties for t
-000302b0: 6865 2073 6573 7369 6f6e 2e20 5468 650a  he session. The.
-000302c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000302d0: 7379 6e74 6178 2066 6f72 202a 2a6f 7074  syntax for **opt
-000302e0: 696f 6e73 2a2a 2069 7320 6120 6469 6374  ions** is a dict
-000302f0: 696f 6e61 7279 206f 6620 7072 6f70 6572  ionary of proper
-00030300: 7469 6573 2077 6974 6820 616e 2061 7373  ties with an ass
-00030310: 6967 6e65 640a 2020 2020 2020 2020 2020  igned.          
-00030320: 2020 2020 2020 7661 6c75 652e 2046 6f72        value. For
-00030330: 2065 7861 6d70 6c65 3a0a 0a20 2020 2020   example:..     
-00030340: 2020 2020 2020 2020 2020 207b 2027 7369             { 'si
-00030350: 6d75 6c61 7465 273a 2046 616c 7365 207d  mulate': False }
-00030360: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00030370: 2020 596f 7520 646f 206e 6f74 2068 6176    You do not hav
-00030380: 6520 746f 2073 7065 6369 6679 2061 2076  e to specify a v
-00030390: 616c 7565 2066 6f72 2061 6c6c 2074 6865  alue for all the
-000303a0: 2070 726f 7065 7274 6965 732e 2049 6620   properties. If 
-000303b0: 796f 7520 646f 206e 6f74 0a20 2020 2020  you do not.     
-000303c0: 2020 2020 2020 2020 2020 2073 7065 6369             speci
-000303d0: 6679 2061 2076 616c 7565 2066 6f72 2061  fy a value for a
-000303e0: 2070 726f 7065 7274 792c 2074 6865 2064   property, the d
-000303f0: 6566 6175 6c74 2076 616c 7565 2069 7320  efault value is 
-00030400: 7573 6564 2e0a 0a20 2020 2020 2020 2020  used...         
-00030410: 2020 2020 2020 2041 6476 616e 6365 6420         Advanced 
-00030420: 4578 616d 706c 653a 0a20 2020 2020 2020  Example:.       
-00030430: 2020 2020 2020 2020 207b 2027 7369 6d75           { 'simu
-00030440: 6c61 7465 273a 2054 7275 652c 2027 6472  late': True, 'dr
-00030450: 6976 6572 5f73 6574 7570 273a 207b 2027  iver_setup': { '
-00030460: 4d6f 6465 6c27 3a20 273c 6d6f 6465 6c20  Model': '<model 
-00030470: 6e75 6d62 6572 3e27 2c20 2027 426f 6172  number>',  'Boar
-00030480: 6454 7970 6527 3a20 273c 7479 7065 3e27  dType': '<type>'
-00030490: 207d 207d 0a0a 2020 2020 2020 2020 2020   } }..          
-000304a0: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
-000304b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000304c0: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
-000304d0: 2020 2020 2020 2020 2020 2020 7c20 5072              | Pr
-000304e0: 6f70 6572 7479 2020 2020 2020 2020 2020  operty          
-000304f0: 2020 2020 2020 7c20 4465 6661 756c 7420        | Default 
-00030500: 7c0a 2020 2020 2020 2020 2020 2020 2020  |.              
-00030510: 2020 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    +=============
-00030520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d  ============+===
-00030530: 3d3d 3d3d 3d3d 2b0a 2020 2020 2020 2020  ======+.        
-00030540: 2020 2020 2020 2020 7c20 7261 6e67 655f          | range_
-00030550: 6368 6563 6b20 2020 2020 2020 2020 2020  check           
-00030560: 2020 7c20 5472 7565 2020 2020 7c0a 2020    | True    |.  
-00030570: 2020 2020 2020 2020 2020 2020 2020 2b2d                +-
+00030010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 0a20  ------------+.. 
+00030020: 2020 2020 2020 2020 2020 2020 2020 202e                 .
+00030030: 2e20 7c4e 6f74 657c 2069 6d61 6765 3a3a  . |Note| image::
+00030040: 206e 6f74 652e 6769 660a 0a20 2020 2020   note.gif..     
+00030050: 2020 2020 2020 2020 2020 204e 6f74 653a             Note:
+00030060: 0a0a 2020 2020 2020 2020 2020 2020 6964  ..            id
+00030070: 5f71 7565 7279 2028 626f 6f6c 293a 2041  _query (bool): A
+00030080: 2042 6f6f 6c65 616e 2074 6861 7420 7665   Boolean that ve
+00030090: 7269 6669 6573 2074 6861 7420 7468 6520  rifies that the 
+000300a0: 6469 6769 7461 6c20 7061 7474 6572 6e20  digital pattern 
+000300b0: 696e 7374 7275 6d65 6e74 2079 6f75 2069  instrument you i
+000300c0: 6e69 7469 616c 697a 6520 6973 2073 7570  nitialize is sup
+000300d0: 706f 7274 6564 2062 7920 4e49 2d44 6967  ported by NI-Dig
+000300e0: 6974 616c 2e20 4e49 2d44 6967 6974 616c  ital. NI-Digital
+000300f0: 2061 7574 6f6d 6174 6963 616c 6c79 2070   automatically p
+00030100: 6572 666f 726d 7320 7468 6973 2071 7565  erforms this que
+00030110: 7279 2c20 736f 2073 6574 7469 6e67 2074  ry, so setting t
+00030120: 6869 7320 7061 7261 6d65 7465 7220 6973  his parameter is
+00030130: 206e 6f74 206e 6563 6573 7361 7279 2e0a   not necessary..
+00030140: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00030150: 6574 5f64 6576 6963 6520 2862 6f6f 6c29  et_device (bool)
+00030160: 3a20 4120 426f 6f6c 6561 6e20 7468 6174  : A Boolean that
+00030170: 2073 7065 6369 6669 6573 2077 6865 7468   specifies wheth
+00030180: 6572 2074 6f20 7265 7365 7420 6120 6469  er to reset a di
+00030190: 6769 7461 6c20 7061 7474 6572 6e20 696e  gital pattern in
+000301a0: 7374 7275 6d65 6e74 2074 6f20 6120 6b6e  strument to a kn
+000301b0: 6f77 6e20 7374 6174 6520 7768 656e 2074  own state when t
+000301c0: 6865 2073 6573 7369 6f6e 2069 7320 696e  he session is in
+000301d0: 6974 6961 6c69 7a65 642e 2053 6574 7469  itialized. Setti
+000301e0: 6e67 2074 6865 202a 2a72 6573 6574 4465  ng the **resetDe
+000301f0: 7669 6365 2a2a 2076 616c 7565 2074 6f20  vice** value to 
+00030200: 5472 7565 2069 7320 6571 7569 7661 6c65  True is equivale
+00030210: 6e74 2074 6f20 6361 6c6c 696e 6720 7468  nt to calling th
+00030220: 6520 7265 7365 7420 6d65 7468 6f64 2069  e reset method i
+00030230: 6d6d 6564 6961 7465 6c79 2061 6674 6572  mmediately after
+00030240: 2069 6e69 7469 616c 697a 696e 6720 7468   initializing th
+00030250: 6520 7365 7373 696f 6e2e 0a0a 2020 2020  e session...    
+00030260: 2020 2020 2020 2020 6f70 7469 6f6e 7320          options 
+00030270: 2864 6963 7429 3a20 5370 6563 6966 6965  (dict): Specifie
+00030280: 7320 7468 6520 696e 6974 6961 6c20 7661  s the initial va
+00030290: 6c75 6520 6f66 2063 6572 7461 696e 2070  lue of certain p
+000302a0: 726f 7065 7274 6965 7320 666f 7220 7468  roperties for th
+000302b0: 6520 7365 7373 696f 6e2e 2054 6865 0a20  e session. The. 
+000302c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000302d0: 796e 7461 7820 666f 7220 2a2a 6f70 7469  yntax for **opti
+000302e0: 6f6e 732a 2a20 6973 2061 2064 6963 7469  ons** is a dicti
+000302f0: 6f6e 6172 7920 6f66 2070 726f 7065 7274  onary of propert
+00030300: 6965 7320 7769 7468 2061 6e20 6173 7369  ies with an assi
+00030310: 676e 6564 0a20 2020 2020 2020 2020 2020  gned.           
+00030320: 2020 2020 2076 616c 7565 2e20 466f 7220       value. For 
+00030330: 6578 616d 706c 653a 0a0a 2020 2020 2020  example:..      
+00030340: 2020 2020 2020 2020 2020 7b20 2773 696d            { 'sim
+00030350: 756c 6174 6527 3a20 4661 6c73 6520 7d0a  ulate': False }.
+00030360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030370: 2059 6f75 2064 6f20 6e6f 7420 6861 7665   You do not have
+00030380: 2074 6f20 7370 6563 6966 7920 6120 7661   to specify a va
+00030390: 6c75 6520 666f 7220 616c 6c20 7468 6520  lue for all the 
+000303a0: 7072 6f70 6572 7469 6573 2e20 4966 2079  properties. If y
+000303b0: 6f75 2064 6f20 6e6f 740a 2020 2020 2020  ou do not.      
+000303c0: 2020 2020 2020 2020 2020 7370 6563 6966            specif
+000303d0: 7920 6120 7661 6c75 6520 666f 7220 6120  y a value for a 
+000303e0: 7072 6f70 6572 7479 2c20 7468 6520 6465  property, the de
+000303f0: 6661 756c 7420 7661 6c75 6520 6973 2075  fault value is u
+00030400: 7365 642e 0a0a 2020 2020 2020 2020 2020  sed...          
+00030410: 2020 2020 2020 4164 7661 6e63 6564 2045        Advanced E
+00030420: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
+00030430: 2020 2020 2020 2020 7b20 2773 696d 756c          { 'simul
+00030440: 6174 6527 3a20 5472 7565 2c20 2764 7269  ate': True, 'dri
+00030450: 7665 725f 7365 7475 7027 3a20 7b20 274d  ver_setup': { 'M
+00030460: 6f64 656c 273a 2027 3c6d 6f64 656c 206e  odel': '<model n
+00030470: 756d 6265 723e 272c 2020 2742 6f61 7264  umber>',  'Board
+00030480: 5479 7065 273a 2027 3c74 7970 653e 2720  Type': '<type>' 
+00030490: 7d20 7d0a 0a20 2020 2020 2020 2020 2020  } }..           
+000304a0: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d       +----------
+000304b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+000304c0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020  ---------+.     
+000304d0: 2020 2020 2020 2020 2020 207c 2050 726f             | Pro
+000304e0: 7065 7274 7920 2020 2020 2020 2020 2020  perty           
+000304f0: 2020 2020 207c 2044 6566 6175 6c74 207c       | Default |
+00030500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030510: 202b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   +==============
+00030520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  ===========+====
+00030530: 3d3d 3d3d 3d2b 0a20 2020 2020 2020 2020  =====+.         
+00030540: 2020 2020 2020 207c 2072 616e 6765 5f63         | range_c
+00030550: 6865 636b 2020 2020 2020 2020 2020 2020  heck            
+00030560: 207c 2054 7275 6520 2020 207c 0a20 2020   | True    |.   
+00030570: 2020 2020 2020 2020 2020 2020 202b 2d2d               +--
 00030580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00030590: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-000305a0: 2d2d 2b0a 2020 2020 2020 2020 2020 2020  --+.            
-000305b0: 2020 2020 7c20 7175 6572 795f 696e 7374      | query_inst
-000305c0: 7275 6d65 6e74 5f73 7461 7475 7320 7c20  rument_status | 
-000305d0: 4661 6c73 6520 2020 7c0a 2020 2020 2020  False   |.      
-000305e0: 2020 2020 2020 2020 2020 2b2d 2d2d 2d2d            +-----
+00030590: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000305a0: 2d2b 0a20 2020 2020 2020 2020 2020 2020  -+.             
+000305b0: 2020 207c 2071 7565 7279 5f69 6e73 7472     | query_instr
+000305c0: 756d 656e 745f 7374 6174 7573 207c 2046  ument_status | F
+000305d0: 616c 7365 2020 207c 0a20 2020 2020 2020  alse   |.       
+000305e0: 2020 2020 2020 2020 202b 2d2d 2d2d 2d2d           +------
 000305f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00030600: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a  ----+---------+.
-00030610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030620: 7c20 6361 6368 6520 2020 2020 2020 2020  | cache         
-00030630: 2020 2020 2020 2020 2020 7c20 5472 7565            | True
-00030640: 2020 2020 7c0a 2020 2020 2020 2020 2020      |.          
-00030650: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
-00030660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00030670: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
-00030680: 2020 2020 2020 2020 2020 2020 7c20 7369              | si
-00030690: 6d75 6c61 7465 2020 2020 2020 2020 2020  mulate          
-000306a0: 2020 2020 2020 7c20 4661 6c73 6520 2020        | False   
-000306b0: 7c0a 2020 2020 2020 2020 2020 2020 2020  |.              
-000306c0: 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    +-------------
-000306d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-000306e0: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
-000306f0: 2020 2020 2020 2020 7c20 7265 636f 7264          | record
-00030700: 5f76 616c 7565 5f63 6f65 7273 696f 6e73  _value_coersions
-00030710: 2020 7c20 4661 6c73 6520 2020 7c0a 2020    | False   |.  
-00030720: 2020 2020 2020 2020 2020 2020 2020 2b2d                +-
+00030600: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 0a20  ---+---------+. 
+00030610: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00030620: 2063 6163 6865 2020 2020 2020 2020 2020   cache          
+00030630: 2020 2020 2020 2020 207c 2054 7275 6520           | True 
+00030640: 2020 207c 0a20 2020 2020 2020 2020 2020     |.           
+00030650: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d       +----------
+00030660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00030670: 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020  ---------+.     
+00030680: 2020 2020 2020 2020 2020 207c 2073 696d             | sim
+00030690: 756c 6174 6520 2020 2020 2020 2020 2020  ulate           
+000306a0: 2020 2020 207c 2046 616c 7365 2020 207c       | False   |
+000306b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000306c0: 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   +--------------
+000306d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+000306e0: 2d2d 2d2d 2d2b 0a20 2020 2020 2020 2020  -----+.         
+000306f0: 2020 2020 2020 207c 2072 6563 6f72 645f         | record_
+00030700: 7661 6c75 655f 636f 6572 7369 6f6e 7320  value_coersions 
+00030710: 207c 2046 616c 7365 2020 207c 0a20 2020   | False   |.   
+00030720: 2020 2020 2020 2020 2020 2020 202b 2d2d               +--
 00030730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00030740: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00030750: 2d2d 2b0a 2020 2020 2020 2020 2020 2020  --+.            
-00030760: 2020 2020 7c20 6472 6976 6572 5f73 6574      | driver_set
-00030770: 7570 2020 2020 2020 2020 2020 2020 7c20  up            | 
-00030780: 7b7d 2020 2020 2020 7c0a 2020 2020 2020  {}      |.      
-00030790: 2020 2020 2020 2020 2020 2b2d 2d2d 2d2d            +-----
+00030740: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00030750: 2d2b 0a20 2020 2020 2020 2020 2020 2020  -+.             
+00030760: 2020 207c 2064 7269 7665 725f 7365 7475     | driver_setu
+00030770: 7020 2020 2020 2020 2020 2020 207c 207b  p            | {
+00030780: 7d20 2020 2020 207c 0a20 2020 2020 2020  }      |.       
+00030790: 2020 2020 2020 2020 202b 2d2d 2d2d 2d2d           +------
 000307a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000307b0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a  ----+---------+.
-000307c0: 0a20 2020 2020 2020 2020 2020 2067 7270  .            grp
-000307d0: 635f 6f70 7469 6f6e 7320 286e 6964 6967  c_options (nidig
-000307e0: 6974 616c 2e67 7270 635f 7365 7373 696f  ital.grpc_sessio
-000307f0: 6e5f 6f70 7469 6f6e 732e 4772 7063 5365  n_options.GrpcSe
-00030800: 7373 696f 6e4f 7074 696f 6e73 293a 204d  ssionOptions): M
-00030810: 6561 7375 7265 6d65 6e74 4c69 6e6b 2067  easurementLink g
-00030820: 5250 4320 7365 7373 696f 6e20 6f70 7469  RPC session opti
-00030830: 6f6e 730a 0a0a 2020 2020 2020 2020 5265  ons...        Re
-00030840: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00030850: 2020 206e 6577 5f76 6920 2869 6e74 293a     new_vi (int):
-00030860: 2054 6865 2072 6574 7572 6e65 6420 696e   The returned in
-00030870: 7374 7275 6d65 6e74 2073 6573 7369 6f6e  strument session
-00030880: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
-00030890: 2020 2020 2020 2069 6620 6772 7063 5f6f         if grpc_o
-000308a0: 7074 696f 6e73 3a0a 2020 2020 2020 2020  ptions:.        
-000308b0: 2020 2020 696d 706f 7274 206e 6964 6967      import nidig
-000308c0: 6974 616c 2e5f 6772 7063 5f73 7475 625f  ital._grpc_stub_
-000308d0: 696e 7465 7270 7265 7465 7220 6173 205f  interpreter as _
-000308e0: 6772 7063 5f73 7475 625f 696e 7465 7270  grpc_stub_interp
-000308f0: 7265 7465 720a 2020 2020 2020 2020 2020  reter.          
-00030900: 2020 696e 7465 7270 7265 7465 7220 3d20    interpreter = 
-00030910: 5f67 7270 635f 7374 7562 5f69 6e74 6572  _grpc_stub_inter
-00030920: 7072 6574 6572 2e47 7270 6353 7475 6249  preter.GrpcStubI
-00030930: 6e74 6572 7072 6574 6572 2867 7270 635f  nterpreter(grpc_
-00030940: 6f70 7469 6f6e 7329 0a20 2020 2020 2020  options).       
-00030950: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00030960: 2020 2069 6e74 6572 7072 6574 6572 203d     interpreter =
-00030970: 205f 6c69 6272 6172 795f 696e 7465 7270   _library_interp
-00030980: 7265 7465 722e 4c69 6272 6172 7949 6e74  reter.LibraryInt
-00030990: 6572 7072 6574 6572 2865 6e63 6f64 696e  erpreter(encodin
-000309a0: 673d 2777 696e 646f 7773 2d31 3235 3127  g='windows-1251'
-000309b0: 290a 0a20 2020 2020 2020 2023 2049 6e69  )..        # Ini
-000309c0: 7469 616c 697a 6520 7468 6520 7375 7065  tialize the supe
-000309d0: 7263 6c61 7373 2077 6974 6820 6465 6661  rclass with defa
-000309e0: 756c 7420 7661 6c75 6573 2066 6972 7374  ult values first
-000309f0: 2c20 706f 7075 6c61 7465 2074 6865 6d20  , populate them 
-00030a00: 6c61 7465 720a 2020 2020 2020 2020 7375  later.        su
-00030a10: 7065 7228 5365 7373 696f 6e2c 2073 656c  per(Session, sel
-00030a20: 6629 2e5f 5f69 6e69 745f 5f28 0a20 2020  f).__init__(.   
-00030a30: 2020 2020 2020 2020 2072 6570 6561 7465           repeate
-00030a40: 645f 6361 7061 6269 6c69 7479 5f6c 6973  d_capability_lis
-00030a50: 743d 5b5d 2c0a 2020 2020 2020 2020 2020  t=[],.          
-00030a60: 2020 696e 7465 7270 7265 7465 723d 696e    interpreter=in
-00030a70: 7465 7270 7265 7465 722c 0a20 2020 2020  terpreter,.     
-00030a80: 2020 2020 2020 2066 7265 657a 655f 6974         freeze_it
-00030a90: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00030aa0: 2020 2020 616c 6c5f 6368 616e 6e65 6c73      all_channels
-00030ab0: 5f69 6e5f 7365 7373 696f 6e3d 4e6f 6e65  _in_session=None
-00030ac0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00030ad0: 2020 206f 7074 696f 6e73 203d 205f 636f     options = _co
-00030ae0: 6e76 6572 7465 7273 2e63 6f6e 7665 7274  nverters.convert
-00030af0: 5f69 6e69 745f 7769 7468 5f6f 7074 696f  _init_with_optio
-00030b00: 6e73 5f64 6963 7469 6f6e 6172 7928 6f70  ns_dictionary(op
-00030b10: 7469 6f6e 7329 0a0a 2020 2020 2020 2020  tions)..        
-00030b20: 2320 4361 6c6c 2073 7065 6369 6669 6564  # Call specified
-00030b30: 2069 6e69 7420 6675 6e63 7469 6f6e 0a20   init function. 
-00030b40: 2020 2020 2020 2023 204e 6f74 6520 7468         # Note th
-00030b50: 6174 205f 696e 7465 7270 7265 7465 7220  at _interpreter 
-00030b60: 6465 6661 756c 742d 696e 6974 6961 6c69  default-initiali
-00030b70: 7a65 7320 7468 6520 7365 7373 696f 6e20  zes the session 
-00030b80: 6861 6e64 6c65 2069 6e20 6974 7320 636f  handle in its co
-00030b90: 6e73 7472 7563 746f 722c 2073 6f20 7468  nstructor, so th
-00030ba0: 6174 0a20 2020 2020 2020 2023 2069 6620  at.        # if 
-00030bb0: 5f69 6e69 745f 7769 7468 5f6f 7074 696f  _init_with_optio
-00030bc0: 6e73 2066 6169 6c73 2c20 7468 6520 6572  ns fails, the er
-00030bd0: 726f 7220 6861 6e64 6c65 7220 6361 6e20  ror handler can 
-00030be0: 7265 6665 7265 6e63 6520 6974 2e0a 2020  reference it..  
-00030bf0: 2020 2020 2020 2320 416e 6420 7468 656e        # And then
-00030c00: 2068 6572 652c 206f 6e63 6520 5f69 6e69   here, once _ini
-00030c10: 745f 7769 7468 5f6f 7074 696f 6e73 2073  t_with_options s
-00030c20: 7563 6365 6564 732c 2077 6520 6361 6c6c  ucceeds, we call
-00030c30: 2073 6574 5f73 6573 7369 6f6e 5f68 616e   set_session_han
-00030c40: 646c 650a 2020 2020 2020 2020 2320 7769  dle.        # wi
-00030c50: 7468 2074 6865 2061 6374 7561 6c20 7365  th the actual se
-00030c60: 7373 696f 6e20 6861 6e64 6c65 2e0a 2020  ssion handle..  
-00030c70: 2020 2020 2020 7365 6c66 2e5f 696e 7465        self._inte
-00030c80: 7270 7265 7465 722e 7365 745f 7365 7373  rpreter.set_sess
-00030c90: 696f 6e5f 6861 6e64 6c65 2873 656c 662e  ion_handle(self.
-00030ca0: 5f69 6e69 745f 7769 7468 5f6f 7074 696f  _init_with_optio
-00030cb0: 6e73 2872 6573 6f75 7263 655f 6e61 6d65  ns(resource_name
-00030cc0: 2c20 6964 5f71 7565 7279 2c20 7265 7365  , id_query, rese
-00030cd0: 745f 6465 7669 6365 2c20 6f70 7469 6f6e  t_device, option
-00030ce0: 7329 290a 0a20 2020 2020 2020 2023 204e  s))..        # N
-00030cf0: 492d 5443 6c6b 2064 6f65 7320 6e6f 7420  I-TClk does not 
-00030d00: 776f 726b 206f 7665 7220 4e49 2067 5250  work over NI gRP
-00030d10: 4320 4465 7669 6365 2053 6572 7665 720a  C Device Server.
-00030d20: 2020 2020 2020 2020 6966 206e 6f74 2067          if not g
-00030d30: 7270 635f 6f70 7469 6f6e 733a 0a20 2020  rpc_options:.   
-00030d40: 2020 2020 2020 2020 2073 656c 662e 7463           self.tc
-00030d50: 6c6b 203d 206e 6974 636c 6b2e 5365 7373  lk = nitclk.Sess
-00030d60: 696f 6e52 6566 6572 656e 6365 2873 656c  ionReference(sel
-00030d70: 662e 5f69 6e74 6572 7072 6574 6572 2e67  f._interpreter.g
-00030d80: 6574 5f73 6573 7369 6f6e 5f68 616e 646c  et_session_handl
-00030d90: 6528 2929 0a0a 2020 2020 2020 2020 2320  e())..        # 
-00030da0: 5374 6f72 6520 7468 6520 7061 7261 6d65  Store the parame
-00030db0: 7465 7220 6c69 7374 2066 6f72 206c 6174  ter list for lat
-00030dc0: 6572 2070 7269 6e74 696e 6720 696e 205f  er printing in _
-00030dd0: 5f72 6570 725f 5f0a 2020 2020 2020 2020  _repr__.        
-00030de0: 7061 7261 6d5f 6c69 7374 203d 205b 5d0a  param_list = [].
-00030df0: 2020 2020 2020 2020 7061 7261 6d5f 6c69          param_li
-00030e00: 7374 2e61 7070 656e 6428 2272 6573 6f75  st.append("resou
-00030e10: 7263 655f 6e61 6d65 3d22 202b 2070 702e  rce_name=" + pp.
-00030e20: 7066 6f72 6d61 7428 7265 736f 7572 6365  pformat(resource
-00030e30: 5f6e 616d 6529 290a 2020 2020 2020 2020  _name)).        
-00030e40: 7061 7261 6d5f 6c69 7374 2e61 7070 656e  param_list.appen
-00030e50: 6428 2272 6573 6574 5f64 6576 6963 653d  d("reset_device=
-00030e60: 2220 2b20 7070 2e70 666f 726d 6174 2872  " + pp.pformat(r
-00030e70: 6573 6574 5f64 6576 6963 6529 290a 2020  eset_device)).  
-00030e80: 2020 2020 2020 7061 7261 6d5f 6c69 7374        param_list
-00030e90: 2e61 7070 656e 6428 226f 7074 696f 6e73  .append("options
-00030ea0: 3d22 202b 2070 702e 7066 6f72 6d61 7428  =" + pp.pformat(
-00030eb0: 6f70 7469 6f6e 7329 290a 2020 2020 2020  options)).      
-00030ec0: 2020 7365 6c66 2e5f 7061 7261 6d5f 6c69    self._param_li
-00030ed0: 7374 203d 2027 2c20 272e 6a6f 696e 2870  st = ', '.join(p
-00030ee0: 6172 616d 5f6c 6973 7429 0a0a 2020 2020  aram_list)..    
-00030ef0: 2020 2020 2320 5374 6f72 6520 7468 6520      # Store the 
-00030f00: 6c69 7374 206f 6620 6368 616e 6e65 6c73  list of channels
-00030f10: 2069 6e20 7468 6520 5365 7373 696f 6e20   in the Session 
-00030f20: 7768 6963 6820 6973 206e 6565 6465 6420  which is needed 
-00030f30: 6279 2073 6f6d 6520 6e69 6d69 2d70 7974  by some nimi-pyt
-00030f40: 686f 6e20 6d6f 6475 6c65 732e 0a20 2020  hon modules..   
-00030f50: 2020 2020 2023 2055 7365 2074 7279 2f65       # Use try/e
-00030f60: 7863 6570 7420 6265 6361 7573 6520 6e6f  xcept because no
-00030f70: 7420 616c 6c20 7468 6520 6d6f 6475 6c65  t all the module
-00030f80: 7320 7375 7070 6f72 7420 6368 616e 6e65  s support channe
-00030f90: 6c73 2e0a 2020 2020 2020 2020 2320 7365  ls..        # se
-00030fa0: 6c66 2e67 6574 5f63 6861 6e6e 656c 5f6e  lf.get_channel_n
-00030fb0: 616d 6573 2829 2061 6e64 2073 656c 662e  ames() and self.
-00030fc0: 6368 616e 6e65 6c5f 636f 756e 7420 6361  channel_count ca
-00030fd0: 6e20 6f6e 6c79 2062 6520 6361 6c6c 6564  n only be called
-00030fe0: 2061 6674 6572 2074 6865 2073 6573 7369   after the sessi
-00030ff0: 6f6e 0a20 2020 2020 2020 2023 2068 616e  on.        # han
-00031000: 646c 6520 6973 2073 6574 0a20 2020 2020  dle is set.     
-00031010: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00031020: 2020 2020 7365 6c66 2e5f 616c 6c5f 6368      self._all_ch
-00031030: 616e 6e65 6c73 5f69 6e5f 7365 7373 696f  annels_in_sessio
-00031040: 6e20 3d20 7365 6c66 2e67 6574 5f63 6861  n = self.get_cha
-00031050: 6e6e 656c 5f6e 616d 6573 2872 616e 6765  nnel_names(range
-00031060: 2873 656c 662e 6368 616e 6e65 6c5f 636f  (self.channel_co
-00031070: 756e 7429 290a 2020 2020 2020 2020 6578  unt)).        ex
-00031080: 6365 7074 2041 7474 7269 6275 7465 4572  cept AttributeEr
-00031090: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-000310a0: 2073 656c 662e 5f61 6c6c 5f63 6861 6e6e   self._all_chann
-000310b0: 656c 735f 696e 5f73 6573 7369 6f6e 203d  els_in_session =
-000310c0: 204e 6f6e 650a 0a20 2020 2020 2020 2023   None..        #
-000310d0: 2046 696e 616c 6c79 2c20 7365 7420 5f69   Finally, set _i
-000310e0: 735f 6672 6f7a 656e 2074 6f20 5472 7565  s_frozen to True
-000310f0: 2077 6869 6368 2069 7320 7573 6564 2074   which is used t
-00031100: 6f20 7072 6576 656e 7420 636c 6965 6e74  o prevent client
-00031110: 7320 6672 6f6d 2061 6363 6964 656e 7461  s from accidenta
-00031120: 6c6c 7920 6164 6469 6e67 0a20 2020 2020  lly adding.     
-00031130: 2020 2023 206d 656d 6265 7273 2077 6865     # members whe
-00031140: 6e20 7472 7969 6e67 2074 6f20 7365 7420  n trying to set 
-00031150: 6120 7072 6f70 6572 7479 2077 6974 6820  a property with 
-00031160: 6120 7479 706f 2e0a 2020 2020 2020 2020  a typo..        
-00031170: 7365 6c66 2e5f 6973 5f66 726f 7a65 6e20  self._is_frozen 
-00031180: 3d20 5472 7565 0a0a 2020 2020 6465 6620  = True..    def 
-00031190: 5f5f 656e 7465 725f 5f28 7365 6c66 293a  __enter__(self):
-000311a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000311b0: 7365 6c66 0a0a 2020 2020 6465 6620 5f5f  self..    def __
-000311c0: 6578 6974 5f5f 2873 656c 662c 2065 7863  exit__(self, exc
-000311d0: 5f74 7970 652c 2065 7863 5f76 616c 7565  _type, exc_value
-000311e0: 2c20 7472 6163 6562 6163 6b29 3a0a 2020  , traceback):.  
-000311f0: 2020 2020 2020 6966 2073 656c 662e 5f69        if self._i
-00031200: 6e74 6572 7072 6574 6572 2e5f 636c 6f73  nterpreter._clos
-00031210: 655f 6f6e 5f65 7869 743a 0a20 2020 2020  e_on_exit:.     
-00031220: 2020 2020 2020 2073 656c 662e 636c 6f73         self.clos
-00031230: 6528 290a 0a20 2020 2064 6566 2069 6e69  e()..    def ini
-00031240: 7469 6174 6528 7365 6c66 293a 0a20 2020  tiate(self):.   
-00031250: 2020 2020 2027 2727 696e 6974 6961 7465       '''initiate
-00031260: 0a0a 2020 2020 2020 2020 5374 6172 7473  ..        Starts
-00031270: 2062 7572 7374 696e 6720 7468 6520 7061   bursting the pa
-00031280: 7474 6572 6e20 636f 6e66 6967 7572 6564  ttern configured
-00031290: 2062 7920 7374 6172 745f 6c61 6265 6c2c   by start_label,
-000312a0: 2063 6175 7369 6e67 2074 6865 204e 492d   causing the NI-
-000312b0: 4469 6769 7461 6c20 7365 7373 696f 6e20  Digital session 
-000312c0: 746f 2062 6520 636f 6d6d 6974 7465 642e  to be committed.
-000312d0: 2054 6f20 7374 6f70 2074 6865 2070 6174   To stop the pat
-000312e0: 7465 726e 2062 7572 7374 2c20 6361 6c6c  tern burst, call
-000312f0: 2061 626f 7274 2e20 4966 206b 6565 7020   abort. If keep 
-00031300: 616c 6976 6520 7061 7474 6572 6e20 6973  alive pattern is
-00031310: 2062 7572 7374 696e 6720 7768 656e 2061   bursting when a
-00031320: 626f 7274 2069 7320 6361 6c6c 6564 206f  bort is called o
-00031330: 7220 7570 6f6e 2065 7869 7469 6e67 2074  r upon exiting t
-00031340: 6865 2063 6f6e 7465 7874 206d 616e 6167  he context manag
-00031350: 6572 2c20 6b65 6570 2061 6c69 7665 2070  er, keep alive p
-00031360: 6174 7465 726e 2077 696c 6c20 6e6f 7420  attern will not 
-00031370: 6265 2073 746f 7070 6564 2e20 546f 2073  be stopped. To s
-00031380: 746f 7020 7468 6520 6b65 6570 2061 6c69  top the keep ali
-00031390: 7665 2070 6174 7465 726e 2c20 6361 6c6c  ve pattern, call
-000313a0: 2061 626f 7274 5f6b 6565 705f 616c 6976   abort_keep_aliv
-000313b0: 652e 0a0a 2020 2020 2020 2020 4e6f 7465  e...        Note
-000313c0: 3a0a 2020 2020 2020 2020 5468 6973 206d  :.        This m
-000313d0: 6574 686f 6420 7769 6c6c 2072 6574 7572  ethod will retur
-000313e0: 6e20 6120 5079 7468 6f6e 2063 6f6e 7465  n a Python conte
-000313f0: 7874 206d 616e 6167 6572 2074 6861 7420  xt manager that 
-00031400: 7769 6c6c 2069 6e69 7469 6174 6520 6f6e  will initiate on
-00031410: 2065 6e74 6572 696e 6720 616e 6420 6162   entering and ab
-00031420: 6f72 7420 6f6e 2065 7869 742e 0a20 2020  ort on exit..   
-00031430: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00031440: 2072 6574 7572 6e20 5f42 7572 7374 2873   return _Burst(s
-00031450: 656c 6629 0a0a 2020 2020 6465 6620 636c  elf)..    def cl
-00031460: 6f73 6528 7365 6c66 293a 0a20 2020 2020  ose(self):.     
-00031470: 2020 2027 2727 636c 6f73 650a 0a20 2020     '''close..   
-00031480: 2020 2020 2043 6c6f 7365 7320 7468 6520       Closes the 
-00031490: 7370 6563 6966 6965 6420 696e 7374 7275  specified instru
-000314a0: 6d65 6e74 2073 6573 7369 6f6e 2074 6f20  ment session to 
-000314b0: 6120 6469 6769 7461 6c20 7061 7474 6572  a digital patter
-000314c0: 6e20 696e 7374 7275 6d65 6e74 2c20 6162  n instrument, ab
-000314d0: 6f72 7473 2070 6174 7465 726e 2065 7865  orts pattern exe
-000314e0: 6375 7469 6f6e 2c20 616e 6420 756e 6c6f  cution, and unlo
-000314f0: 6164 7320 7061 7474 6572 6e20 6d65 6d6f  ads pattern memo
-00031500: 7279 2e20 5468 6520 6368 616e 6e65 6c73  ry. The channels
-00031510: 206f 6e20 6120 6469 6769 7461 6c20 7061   on a digital pa
-00031520: 7474 6572 6e20 696e 7374 7275 6d65 6e74  ttern instrument
-00031530: 2072 656d 6169 6e20 696e 2074 6865 6972   remain in their
-00031540: 2063 7572 7265 6e74 2073 7461 7465 2e0a   current state..
-00031550: 0a20 2020 2020 2020 204e 6f74 653a 0a20  .        Note:. 
-00031560: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
-00031570: 6f64 2069 7320 6e6f 7420 6e65 6564 6564  od is not needed
-00031580: 2077 6865 6e20 7573 696e 6720 7468 6520   when using the 
-00031590: 7365 7373 696f 6e20 636f 6e74 6578 7420  session context 
-000315a0: 6d61 6e61 6765 720a 2020 2020 2020 2020  manager.        
-000315b0: 2727 270a 2020 2020 2020 2020 7472 793a  '''.        try:
-000315c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000315d0: 662e 5f63 6c6f 7365 2829 0a20 2020 2020  f._close().     
-000315e0: 2020 2065 7863 6570 7420 6572 726f 7273     except errors
-000315f0: 2e44 7269 7665 7245 7272 6f72 3a0a 2020  .DriverError:.  
-00031600: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00031610: 696e 7465 7270 7265 7465 722e 7365 745f  interpreter.set_
-00031620: 7365 7373 696f 6e5f 6861 6e64 6c65 2829  session_handle()
-00031630: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00031640: 7365 0a20 2020 2020 2020 2073 656c 662e  se.        self.
-00031650: 5f69 6e74 6572 7072 6574 6572 2e73 6574  _interpreter.set
-00031660: 5f73 6573 7369 6f6e 5f68 616e 646c 6528  _session_handle(
-00031670: 290a 0a20 2020 2027 2727 2054 6865 7365  )..    ''' These
-00031680: 2061 7265 2063 6f64 652d 6765 6e65 7261   are code-genera
-00031690: 7465 6420 2727 270a 0a20 2020 2040 6976  ted '''..    @iv
-000316a0: 695f 7379 6e63 6872 6f6e 697a 6564 0a20  i_synchronized. 
-000316b0: 2020 2064 6566 2061 626f 7274 2873 656c     def abort(sel
-000316c0: 6629 3a0a 2020 2020 2020 2020 7227 2727  f):.        r'''
-000316d0: 6162 6f72 740a 0a20 2020 2020 2020 2053  abort..        S
-000316e0: 746f 7073 2062 7572 7374 696e 6720 7468  tops bursting th
-000316f0: 6520 7061 7474 6572 6e2e 0a20 2020 2020  e pattern..     
-00031700: 2020 2027 2727 0a20 2020 2020 2020 2073     '''.        s
-00031710: 656c 662e 5f69 6e74 6572 7072 6574 6572  elf._interpreter
-00031720: 2e61 626f 7274 2829 0a0a 2020 2020 4069  .abort()..    @i
-00031730: 7669 5f73 796e 6368 726f 6e69 7a65 640a  vi_synchronized.
-00031740: 2020 2020 6465 6620 6162 6f72 745f 6b65      def abort_ke
-00031750: 6570 5f61 6c69 7665 2873 656c 6629 3a0a  ep_alive(self):.
-00031760: 2020 2020 2020 2020 7227 2727 6162 6f72          r'''abor
-00031770: 745f 6b65 6570 5f61 6c69 7665 0a0a 2020  t_keep_alive..  
-00031780: 2020 2020 2020 5374 6f70 7320 7468 6520        Stops the 
-00031790: 6b65 6570 2061 6c69 7665 2070 6174 7465  keep alive patte
-000317a0: 726e 2069 6620 6974 2069 7320 6375 7272  rn if it is curr
-000317b0: 656e 746c 7920 7275 6e6e 696e 672e 2049  ently running. I
-000317c0: 6620 6120 7061 7474 6572 6e20 6275 7273  f a pattern burs
-000317d0: 7420 6973 2069 6e20 7072 6f67 7265 7373  t is in progress
-000317e0: 2c20 7468 6520 6d65 7468 6f64 2061 626f  , the method abo
-000317f0: 7274 7320 7468 6520 7061 7474 6572 6e20  rts the pattern 
-00031800: 6275 7273 742e 2049 6620 796f 7520 7374  burst. If you st
-00031810: 6172 7420 6120 6e65 7720 7061 7474 6572  art a new patter
-00031820: 6e20 6275 7273 7420 7768 696c 6520 6120  n burst while a 
-00031830: 6b65 6570 2061 6c69 7665 2070 6174 7465  keep alive patte
-00031840: 726e 2069 7320 7275 6e6e 696e 672c 2074  rn is running, t
-00031850: 6865 206b 6565 7020 616c 6976 6520 7061  he keep alive pa
-00031860: 7474 6572 6e20 7275 6e73 2074 6f20 7468  ttern runs to th
-00031870: 6520 6c61 7374 206b 6565 7020 616c 6976  e last keep aliv
-00031880: 6520 7665 6374 6f72 2c20 616e 6420 7468  e vector, and th
-00031890: 6520 6e65 7720 7061 7474 6572 6e20 6275  e new pattern bu
-000318a0: 7273 7420 7374 6172 7473 206f 6e20 7468  rst starts on th
-000318b0: 6520 6e65 7874 2063 7963 6c65 2e0a 2020  e next cycle..  
-000318c0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-000318d0: 2020 7365 6c66 2e5f 696e 7465 7270 7265    self._interpre
-000318e0: 7465 722e 6162 6f72 745f 6b65 6570 5f61  ter.abort_keep_a
-000318f0: 6c69 7665 2829 0a0a 2020 2020 4069 7669  live()..    @ivi
-00031900: 5f73 796e 6368 726f 6e69 7a65 640a 2020  _synchronized.  
-00031910: 2020 6465 6620 636f 6d6d 6974 2873 656c    def commit(sel
-00031920: 6629 3a0a 2020 2020 2020 2020 7227 2727  f):.        r'''
-00031930: 636f 6d6d 6974 0a0a 2020 2020 2020 2020  commit..        
-00031940: 4170 706c 6965 7320 616c 6c20 7072 6576  Applies all prev
-00031950: 696f 7573 6c79 2063 6f6e 6669 6775 7265  iously configure
-00031960: 6420 7069 6e20 6c65 7665 6c73 2c20 7465  d pin levels, te
-00031970: 726d 696e 6174 696f 6e20 6d6f 6465 732c  rmination modes,
-00031980: 2063 6c6f 636b 732c 2074 7269 6767 6572   clocks, trigger
-00031990: 732c 2061 6e64 2070 6174 7465 726e 2074  s, and pattern t
-000319a0: 696d 696e 6720 746f 2061 2064 6967 6974  iming to a digit
-000319b0: 616c 2070 6174 7465 726e 2069 6e73 7472  al pattern instr
-000319c0: 756d 656e 742e 2049 6620 796f 7520 646f  ument. If you do
-000319d0: 206e 6f74 2063 616c 6c20 7468 6520 636f   not call the co
-000319e0: 6d6d 6974 206d 6574 686f 642c 2074 6865  mmit method, the
-000319f0: 6e20 7468 6520 696e 6974 6961 7465 206d  n the initiate m
-00031a00: 6574 686f 6420 6f72 2074 6865 2062 7572  ethod or the bur
-00031a10: 7374 5f70 6174 7465 726e 206d 6574 686f  st_pattern metho
-00031a20: 6420 7769 6c6c 2069 6d70 6c69 6369 746c  d will implicitl
-00031a30: 7920 6361 6c6c 2074 6869 7320 6d65 7468  y call this meth
-00031a40: 6f64 2066 6f72 2079 6f75 2e20 4361 6c6c  od for you. Call
-00031a50: 696e 6720 7468 6973 206d 6574 686f 6420  ing this method 
-00031a60: 6d6f 7665 7320 7468 6520 7365 7373 696f  moves the sessio
-00031a70: 6e20 6672 6f6d 2074 6865 2055 6e63 6f6d  n from the Uncom
-00031a80: 6d69 7474 6564 2073 7461 7465 2074 6f20  mitted state to 
-00031a90: 7468 6520 436f 6d6d 6974 7465 6420 7374  the Committed st
-00031aa0: 6174 652e 0a20 2020 2020 2020 2027 2727  ate..        '''
-00031ab0: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
-00031ac0: 6e74 6572 7072 6574 6572 2e63 6f6d 6d69  nterpreter.commi
-00031ad0: 7428 290a 0a20 2020 2040 6976 695f 7379  t()..    @ivi_sy
-00031ae0: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
-00031af0: 6566 2063 6f6e 6669 6775 7265 5f74 696d  ef configure_tim
-00031b00: 655f 7365 745f 7065 7269 6f64 2873 656c  e_set_period(sel
-00031b10: 662c 2074 696d 655f 7365 745f 6e61 6d65  f, time_set_name
-00031b20: 2c20 7065 7269 6f64 293a 0a20 2020 2020  , period):.     
-00031b30: 2020 2072 2727 2763 6f6e 6669 6775 7265     r'''configure
-00031b40: 5f74 696d 655f 7365 745f 7065 7269 6f64  _time_set_period
-00031b50: 0a0a 2020 2020 2020 2020 436f 6e66 6967  ..        Config
-00031b60: 7572 6573 2074 6865 2070 6572 696f 6420  ures the period 
-00031b70: 6f66 2061 2074 696d 6520 7365 742e 2055  of a time set. U
-00031b80: 7365 2074 6869 7320 6d65 7468 6f64 2074  se this method t
-00031b90: 6f20 6d6f 6469 6679 2074 696d 6520 7365  o modify time se
-00031ba0: 7420 7661 6c75 6573 2061 6674 6572 2061  t values after a
-00031bb0: 7070 6c79 696e 6720 6120 7469 6d69 6e67  pplying a timing
-00031bc0: 2073 6865 6574 2077 6974 6820 7468 6520   sheet with the 
-00031bd0: 6170 706c 795f 6c65 7665 6c73 5f61 6e64  apply_levels_and
-00031be0: 5f74 696d 696e 6720 6d65 7468 6f64 2c20  _timing method, 
-00031bf0: 6f72 2074 6f20 6372 6561 7465 2074 696d  or to create tim
-00031c00: 6520 7365 7473 2070 726f 6772 616d 6d61  e sets programma
-00031c10: 7469 6361 6c6c 7920 7769 7468 6f75 7420  tically without 
-00031c20: 7468 6520 7573 6520 6f66 2074 696d 696e  the use of timin
-00031c30: 6720 7368 6565 7473 2e20 5468 6973 206d  g sheets. This m
-00031c40: 6574 686f 6420 646f 6573 206e 6f74 206d  ethod does not m
-00031c50: 6f64 6966 7920 7468 6520 7469 6d69 6e67  odify the timing
-00031c60: 2073 6865 6574 2066 696c 6520 6f72 2074   sheet file or t
-00031c70: 6865 2074 696d 696e 6720 7368 6565 7420  he timing sheet 
-00031c80: 636f 6e74 656e 7473 2074 6861 7420 7769  contents that wi
-00031c90: 6c6c 2062 6520 7573 6564 2069 6e20 6675  ll be used in fu
-00031ca0: 7475 7265 2063 616c 6c73 2074 6f20 6170  ture calls to ap
-00031cb0: 706c 795f 6c65 7665 6c73 5f61 6e64 5f74  ply_levels_and_t
-00031cc0: 696d 696e 673b 2069 7420 6f6e 6c79 2061  iming; it only a
-00031cd0: 6666 6563 7473 2074 6865 2076 616c 7565  ffects the value
-00031ce0: 7320 6f66 2074 6865 2063 7572 7265 6e74  s of the current
-00031cf0: 2074 696d 696e 6720 636f 6e74 6578 742e   timing context.
-00031d00: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00031d10: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00031d20: 5f73 6574 5f6e 616d 6520 2873 7472 293a  _set_name (str):
-00031d30: 2054 6865 2073 7065 6369 6669 6564 2074   The specified t
-00031d40: 696d 6520 7365 7420 6e61 6d65 2e0a 0a20  ime set name... 
-00031d50: 2020 2020 2020 2020 2020 2070 6572 696f             perio
-00031d60: 6420 2868 6967 6874 696d 652e 7469 6d65  d (hightime.time
-00031d70: 6465 6c74 612c 2064 6174 6574 696d 652e  delta, datetime.
-00031d80: 7469 6d65 6465 6c74 612c 206f 7220 666c  timedelta, or fl
-00031d90: 6f61 7420 696e 2073 6563 6f6e 6473 293a  oat in seconds):
-00031da0: 2050 6572 696f 6420 666f 7220 7468 6973   Period for this
-00031db0: 2074 696d 6520 7365 742c 2069 6e20 7365   time set, in se
-00031dc0: 636f 6e64 732e 0a0a 2020 2020 2020 2020  conds...        
-00031dd0: 2727 270a 2020 2020 2020 2020 7065 7269  '''.        peri
-00031de0: 6f64 203d 205f 636f 6e76 6572 7465 7273  od = _converters
-00031df0: 2e63 6f6e 7665 7274 5f74 696d 6564 656c  .convert_timedel
-00031e00: 7461 5f74 6f5f 7365 636f 6e64 735f 7265  ta_to_seconds_re
-00031e10: 616c 3634 2870 6572 696f 6429 0a20 2020  al64(period).   
-00031e20: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
-00031e30: 7072 6574 6572 2e63 6f6e 6669 6775 7265  preter.configure
-00031e40: 5f74 696d 655f 7365 745f 7065 7269 6f64  _time_set_period
-00031e50: 2874 696d 655f 7365 745f 6e61 6d65 2c20  (time_set_name, 
-00031e60: 7065 7269 6f64 290a 0a20 2020 2040 6976  period)..    @iv
-00031e70: 695f 7379 6e63 6872 6f6e 697a 6564 0a20  i_synchronized. 
-00031e80: 2020 2064 6566 2063 7265 6174 655f 6361     def create_ca
-00031e90: 7074 7572 655f 7761 7665 666f 726d 5f66  pture_waveform_f
-00031ea0: 726f 6d5f 6669 6c65 5f64 6967 6963 6170  rom_file_digicap
-00031eb0: 7475 7265 2873 656c 662c 2077 6176 6566  ture(self, wavef
-00031ec0: 6f72 6d5f 6e61 6d65 2c20 7761 7665 666f  orm_name, wavefo
-00031ed0: 726d 5f66 696c 655f 7061 7468 293a 0a20  rm_file_path):. 
-00031ee0: 2020 2020 2020 2072 2727 2763 7265 6174         r'''creat
-00031ef0: 655f 6361 7074 7572 655f 7761 7665 666f  e_capture_wavefo
-00031f00: 726d 5f66 726f 6d5f 6669 6c65 5f64 6967  rm_from_file_dig
-00031f10: 6963 6170 7475 7265 0a0a 2020 2020 2020  icapture..      
-00031f20: 2020 4372 6561 7465 7320 6120 6361 7074    Creates a capt
-00031f30: 7572 6520 7761 7665 666f 726d 2077 6974  ure waveform wit
-00031f40: 6820 7468 6520 636f 6e66 6967 7572 6174  h the configurat
-00031f50: 696f 6e20 696e 666f 726d 6174 696f 6e20  ion information 
-00031f60: 6672 6f6d 2061 2044 6967 6963 6170 7475  from a Digicaptu
-00031f70: 7265 2066 696c 6520 6765 6e65 7261 7465  re file generate
-00031f80: 6420 6279 2074 6865 2044 6967 6974 616c  d by the Digital
-00031f90: 2050 6174 7465 726e 2045 6469 746f 722e   Pattern Editor.
-00031fa0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00031fb0: 2020 2020 2020 2020 2020 2020 7761 7665              wave
-00031fc0: 666f 726d 5f6e 616d 6520 2873 7472 293a  form_name (str):
-00031fd0: 2057 6176 6566 6f72 6d20 6e61 6d65 2079   Waveform name y
-00031fe0: 6f75 2077 616e 7420 746f 2075 7365 2e20  ou want to use. 
-00031ff0: 596f 7520 6d75 7374 2073 7065 6369 6679  You must specify
-00032000: 2077 6176 6566 6f72 6d5f 6e61 6d65 2069   waveform_name i
-00032010: 6620 7468 6520 6669 6c65 2063 6f6e 7461  f the file conta
-00032020: 696e 7320 6d75 6c74 6970 6c65 2077 6176  ins multiple wav
-00032030: 6566 6f72 6d73 2e20 5573 6520 7468 6520  eforms. Use the 
-00032040: 7761 7665 666f 726d 5f6e 616d 6520 7769  waveform_name wi
-00032050: 7468 2074 6865 2063 6170 7475 7265 5f73  th the capture_s
-00032060: 7461 7274 206f 7063 6f64 6520 696e 2079  tart opcode in y
-00032070: 6f75 7220 7061 7474 6572 6e2e 0a0a 2020  our pattern...  
-00032080: 2020 2020 2020 2020 2020 7761 7665 666f            wavefo
-00032090: 726d 5f66 696c 655f 7061 7468 2028 7374  rm_file_path (st
-000320a0: 7229 3a20 4162 736f 6c75 7465 2066 696c  r): Absolute fil
-000320b0: 6520 7061 7468 2074 6f20 7468 6520 6361  e path to the ca
-000320c0: 7074 7572 6520 7761 7665 666f 726d 2066  pture waveform f
-000320d0: 696c 6520 282e 6469 6769 6361 7074 7572  ile (.digicaptur
-000320e0: 6529 2079 6f75 2077 616e 7420 746f 206c  e) you want to l
-000320f0: 6f61 642e 0a0a 2020 2020 2020 2020 2727  oad...        ''
-00032100: 270a 2020 2020 2020 2020 7365 6c66 2e5f  '.        self._
-00032110: 696e 7465 7270 7265 7465 722e 6372 6561  interpreter.crea
-00032120: 7465 5f63 6170 7475 7265 5f77 6176 6566  te_capture_wavef
-00032130: 6f72 6d5f 6672 6f6d 5f66 696c 655f 6469  orm_from_file_di
-00032140: 6769 6361 7074 7572 6528 7761 7665 666f  gicapture(wavefo
-00032150: 726d 5f6e 616d 652c 2077 6176 6566 6f72  rm_name, wavefor
-00032160: 6d5f 6669 6c65 5f70 6174 6829 0a0a 2020  m_file_path)..  
-00032170: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
-00032180: 7a65 640a 2020 2020 6465 6620 6372 6561  zed.    def crea
-00032190: 7465 5f73 6f75 7263 655f 7761 7665 666f  te_source_wavefo
-000321a0: 726d 5f66 726f 6d5f 6669 6c65 5f74 646d  rm_from_file_tdm
-000321b0: 7328 7365 6c66 2c20 7761 7665 666f 726d  s(self, waveform
-000321c0: 5f6e 616d 652c 2077 6176 6566 6f72 6d5f  _name, waveform_
-000321d0: 6669 6c65 5f70 6174 682c 2077 7269 7465  file_path, write
-000321e0: 5f77 6176 6566 6f72 6d5f 6461 7461 3d54  _waveform_data=T
-000321f0: 7275 6529 3a0a 2020 2020 2020 2020 7227  rue):.        r'
-00032200: 2727 6372 6561 7465 5f73 6f75 7263 655f  ''create_source_
-00032210: 7761 7665 666f 726d 5f66 726f 6d5f 6669  waveform_from_fi
-00032220: 6c65 5f74 646d 730a 0a20 2020 2020 2020  le_tdms..       
-00032230: 2043 7265 6174 6573 2061 2073 6f75 7263   Creates a sourc
-00032240: 6520 7761 7665 666f 726d 2077 6974 6820  e waveform with 
-00032250: 636f 6e66 6967 7572 6174 696f 6e20 696e  configuration in
-00032260: 666f 726d 6174 696f 6e20 6672 6f6d 2061  formation from a
-00032270: 2054 444d 5320 6669 6c65 2067 656e 6572   TDMS file gener
-00032280: 6174 6564 2062 7920 7468 6520 4469 6769  ated by the Digi
-00032290: 7461 6c20 5061 7474 6572 6e20 4564 6974  tal Pattern Edit
-000322a0: 6f72 2e20 4974 2061 6c73 6f20 6f70 7469  or. It also opti
-000322b0: 6f6e 616c 6c79 2077 7269 7465 7320 7761  onally writes wa
-000322c0: 7665 666f 726d 2064 6174 6120 6672 6f6d  veform data from
-000322d0: 2074 6865 2066 696c 652e 0a0a 2020 2020   the file...    
-000322e0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000322f0: 2020 2020 2020 7761 7665 666f 726d 5f6e        waveform_n
-00032300: 616d 6520 2873 7472 293a 2054 6865 2077  ame (str): The w
-00032310: 6176 6566 6f72 6d20 6e61 6d65 2079 6f75  aveform name you
-00032320: 2077 616e 7420 746f 2075 7365 2066 726f   want to use fro
-00032330: 6d20 7468 6520 6669 6c65 2e20 596f 7520  m the file. You 
-00032340: 6d75 7374 2073 7065 6369 6679 2077 6176  must specify wav
-00032350: 6566 6f72 6d5f 6e61 6d65 2069 6620 7468  eform_name if th
-00032360: 6520 6669 6c65 2063 6f6e 7461 696e 7320  e file contains 
-00032370: 6d75 6c74 6970 6c65 2077 6176 6566 6f72  multiple wavefor
-00032380: 6d73 2e20 5573 6520 7468 6520 7761 7665  ms. Use the wave
-00032390: 666f 726d 5f6e 616d 6520 7769 7468 2074  form_name with t
-000323a0: 6865 2073 6f75 7263 655f 7374 6172 7420  he source_start 
-000323b0: 6f70 636f 6465 2069 6e20 796f 7572 2070  opcode in your p
-000323c0: 6174 7465 726e 2e0a 0a20 2020 2020 2020  attern...       
-000323d0: 2020 2020 2077 6176 6566 6f72 6d5f 6669       waveform_fi
-000323e0: 6c65 5f70 6174 6820 2873 7472 293a 2041  le_path (str): A
-000323f0: 6273 6f6c 7574 6520 6669 6c65 2070 6174  bsolute file pat
-00032400: 6820 746f 2074 6865 206c 6f61 6420 736f  h to the load so
-00032410: 7572 6365 2077 6176 6566 6f72 6d20 6669  urce waveform fi
-00032420: 6c65 2028 2e74 646d 7329 2e0a 0a20 2020  le (.tdms)...   
-00032430: 2020 2020 2020 2020 2077 7269 7465 5f77           write_w
-00032440: 6176 6566 6f72 6d5f 6461 7461 2028 626f  aveform_data (bo
-00032450: 6f6c 293a 2041 2042 6f6f 6c65 616e 2074  ol): A Boolean t
-00032460: 6861 7420 7772 6974 6573 2077 6176 6566  hat writes wavef
-00032470: 6f72 6d20 6461 7461 2074 6f20 736f 7572  orm data to sour
-00032480: 6365 206d 656d 6f72 7920 6966 2054 7275  ce memory if Tru
-00032490: 6520 616e 6420 7468 6520 7761 7665 666f  e and the wavefo
-000324a0: 726d 2064 6174 6120 6973 2069 6e20 7468  rm data is in th
-000324b0: 6520 6669 6c65 2e0a 0a20 2020 2020 2020  e file...       
-000324c0: 2027 2727 0a20 2020 2020 2020 2073 656c   '''.        sel
-000324d0: 662e 5f69 6e74 6572 7072 6574 6572 2e63  f._interpreter.c
-000324e0: 7265 6174 655f 736f 7572 6365 5f77 6176  reate_source_wav
-000324f0: 6566 6f72 6d5f 6672 6f6d 5f66 696c 655f  eform_from_file_
-00032500: 7464 6d73 2877 6176 6566 6f72 6d5f 6e61  tdms(waveform_na
-00032510: 6d65 2c20 7761 7665 666f 726d 5f66 696c  me, waveform_fil
-00032520: 655f 7061 7468 2c20 7772 6974 655f 7761  e_path, write_wa
-00032530: 7665 666f 726d 5f64 6174 6129 0a0a 2020  veform_data)..  
-00032540: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
-00032550: 7a65 640a 2020 2020 6465 6620 6372 6561  zed.    def crea
-00032560: 7465 5f74 696d 655f 7365 7428 7365 6c66  te_time_set(self
-00032570: 2c20 6e61 6d65 293a 0a20 2020 2020 2020  , name):.       
-00032580: 2072 2727 2763 7265 6174 655f 7469 6d65   r'''create_time
-00032590: 5f73 6574 0a0a 2020 2020 2020 2020 4372  _set..        Cr
-000325a0: 6561 7465 7320 6120 7469 6d65 2073 6574  eates a time set
-000325b0: 2077 6974 6820 7468 6520 6e61 6d65 2074   with the name t
-000325c0: 6861 7420 796f 7520 7370 6563 6966 792e  hat you specify.
-000325d0: 2055 7365 2074 6869 7320 6d65 7468 6f64   Use this method
-000325e0: 2077 6865 6e20 796f 7520 7761 6e74 2074   when you want t
-000325f0: 6f20 6372 6561 7465 2074 696d 6520 7365  o create time se
-00032600: 7473 2070 726f 6772 616d 6d61 7469 6361  ts programmatica
-00032610: 6c6c 7920 7261 7468 6572 2074 6861 6e20  lly rather than 
-00032620: 7769 7468 2061 2074 696d 696e 6720 7368  with a timing sh
-00032630: 6565 742e 0a0a 2020 2020 2020 2020 4172  eet...        Ar
-00032640: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00032650: 6e61 6d65 2028 7374 7229 3a20 5468 6520  name (str): The 
-00032660: 7370 6563 6966 6965 6420 6e61 6d65 206f  specified name o
-00032670: 6620 7468 6520 6e65 7720 7469 6d65 2073  f the new time s
-00032680: 6574 2e0a 0a20 2020 2020 2020 2027 2727  et...        '''
-00032690: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
-000326a0: 6e74 6572 7072 6574 6572 2e63 7265 6174  nterpreter.creat
-000326b0: 655f 7469 6d65 5f73 6574 286e 616d 6529  e_time_set(name)
-000326c0: 0a0a 2020 2020 4069 7669 5f73 796e 6368  ..    @ivi_synch
-000326d0: 726f 6e69 7a65 640a 2020 2020 6465 6620  ronized.    def 
-000326e0: 6465 6c65 7465 5f61 6c6c 5f74 696d 655f  delete_all_time_
-000326f0: 7365 7473 2873 656c 6629 3a0a 2020 2020  sets(self):.    
-00032700: 2020 2020 7227 2727 6465 6c65 7465 5f61      r'''delete_a
-00032710: 6c6c 5f74 696d 655f 7365 7473 0a0a 2020  ll_time_sets..  
-00032720: 2020 2020 2020 4465 6c65 7465 7320 616c        Deletes al
-00032730: 6c20 7469 6d65 2073 6574 7320 6672 6f6d  l time sets from
-00032740: 2069 6e73 7472 756d 656e 7420 6d65 6d6f   instrument memo
-00032750: 7279 2e0a 2020 2020 2020 2020 2727 270a  ry..        '''.
-00032760: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
-00032770: 7465 7270 7265 7465 722e 6465 6c65 7465  terpreter.delete
-00032780: 5f61 6c6c 5f74 696d 655f 7365 7473 2829  _all_time_sets()
-00032790: 0a0a 2020 2020 4069 7669 5f73 796e 6368  ..    @ivi_synch
-000327a0: 726f 6e69 7a65 640a 2020 2020 6465 6620  ronized.    def 
-000327b0: 6c6f 6164 5f73 7065 6369 6669 6361 7469  load_specificati
-000327c0: 6f6e 735f 6c65 7665 6c73 5f61 6e64 5f74  ons_levels_and_t
-000327d0: 696d 696e 6728 7365 6c66 2c20 7370 6563  iming(self, spec
-000327e0: 6966 6963 6174 696f 6e73 5f66 696c 655f  ifications_file_
-000327f0: 7061 7468 733d 4e6f 6e65 2c20 6c65 7665  paths=None, leve
-00032800: 6c73 5f66 696c 655f 7061 7468 733d 4e6f  ls_file_paths=No
-00032810: 6e65 2c20 7469 6d69 6e67 5f66 696c 655f  ne, timing_file_
-00032820: 7061 7468 733d 4e6f 6e65 293a 0a20 2020  paths=None):.   
-00032830: 2020 2020 2027 2727 6c6f 6164 5f73 7065       '''load_spe
-00032840: 6369 6669 6361 7469 6f6e 735f 6c65 7665  cifications_leve
-00032850: 6c73 5f61 6e64 5f74 696d 696e 670a 0a20  ls_and_timing.. 
-00032860: 2020 2020 2020 204c 6f61 6473 2073 6574         Loads set
-00032870: 7469 6e67 7320 696e 2073 7065 6369 6669  tings in specifi
-00032880: 6361 7469 6f6e 732c 206c 6576 656c 732c  cations, levels,
-00032890: 2061 6e64 2074 696d 696e 6720 7368 6565   and timing shee
-000328a0: 7473 2e20 5468 6573 6520 7365 7474 696e  ts. These settin
-000328b0: 6773 2061 7265 206e 6f74 0a20 2020 2020  gs are not.     
-000328c0: 2020 2061 7070 6c69 6564 2074 6f20 7468     applied to th
-000328d0: 6520 6469 6769 7461 6c20 7061 7474 6572  e digital patter
-000328e0: 6e20 696e 7374 7275 6d65 6e74 2075 6e74  n instrument unt
-000328f0: 696c 2061 7070 6c79 5f6c 6576 656c 735f  il apply_levels_
-00032900: 616e 645f 7469 6d69 6e67 2069 7320 6361  and_timing is ca
-00032910: 6c6c 6564 2e0a 0a20 2020 2020 2020 2049  lled...        I
-00032920: 6620 7468 6520 6c65 7665 6c73 2061 6e64  f the levels and
-00032930: 2074 696d 696e 6720 7368 6565 7473 2063   timing sheets c
-00032940: 6f6e 7461 696e 7320 666f 726d 756c 6173  ontains formulas
-00032950: 2c20 7468 6579 2061 7265 2065 7661 6c75  , they are evalu
-00032960: 6174 6564 2061 7420 6c6f 6164 2074 696d  ated at load tim
-00032970: 652e 0a20 2020 2020 2020 2049 6620 7468  e..        If th
-00032980: 6520 666f 726d 756c 6173 2072 6566 6572  e formulas refer
-00032990: 2074 6f20 7661 7269 6162 6c65 732c 2074   to variables, t
-000329a0: 6865 2073 7065 6369 6669 6361 7469 6f6e  he specification
-000329b0: 7320 7368 6565 7473 2074 6861 7420 6465  s sheets that de
-000329c0: 6669 6e65 2074 686f 7365 0a20 2020 2020  fine those.     
-000329d0: 2020 2076 6172 6961 626c 6573 206d 7573     variables mus
-000329e0: 7420 6265 206c 6f61 6465 6420 6569 7468  t be loaded eith
-000329f0: 6572 2066 6972 7374 2c20 6f72 2061 7420  er first, or at 
-00032a00: 7468 6520 7361 6d65 2074 696d 6520 6173  the same time as
-00032a10: 2074 6865 206c 6576 656c 7320 616e 6420   the levels and 
-00032a20: 7469 6d69 6e67 2073 6865 6574 732e 0a0a  timing sheets...
-00032a30: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00032a40: 2020 2020 2020 2020 2020 7370 6563 6966            specif
-00032a50: 6963 6174 696f 6e73 5f66 696c 655f 7061  ications_file_pa
-00032a60: 7468 7320 2873 7472 206f 7220 6261 7369  ths (str or basi
-00032a70: 6320 7365 7175 656e 6365 206f 6620 7374  c sequence of st
-00032a80: 7229 3a20 4162 736f 6c75 7465 2066 696c  r): Absolute fil
-00032a90: 6520 7061 7468 206f 6620 6f6e 6520 6f72  e path of one or
-00032aa0: 206d 6f72 6520 7370 6563 6966 6963 6174   more specificat
-00032ab0: 696f 6e73 2066 696c 6573 2e0a 0a20 2020  ions files...   
-00032ac0: 2020 2020 2020 2020 206c 6576 656c 735f           levels_
-00032ad0: 6669 6c65 5f70 6174 6873 2028 7374 7220  file_paths (str 
-00032ae0: 6f72 2062 6173 6963 2073 6571 7565 6e63  or basic sequenc
-00032af0: 6520 6f66 2073 7472 293a 2041 6273 6f6c  e of str): Absol
-00032b00: 7574 6520 6669 6c65 2070 6174 6820 6f66  ute file path of
-00032b10: 206f 6e65 206f 7220 6d6f 7265 206c 6576   one or more lev
-00032b20: 656c 7320 7368 6565 7420 6669 6c65 732e  els sheet files.
-00032b30: 0a0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-00032b40: 6d69 6e67 5f66 696c 655f 7061 7468 7320  ming_file_paths 
-00032b50: 2873 7472 206f 7220 6261 7369 6320 7365  (str or basic se
-00032b60: 7175 656e 6365 206f 6620 7374 7229 3a20  quence of str): 
-00032b70: 4162 736f 6c75 7465 2066 696c 6520 7061  Absolute file pa
-00032b80: 7468 206f 6620 6f6e 6520 6f72 206d 6f72  th of one or mor
-00032b90: 6520 7469 6d69 6e67 2073 6865 6574 2066  e timing sheet f
-00032ba0: 696c 6573 2e0a 0a20 2020 2020 2020 2027  iles...        '
-00032bb0: 2727 0a20 2020 2020 2020 2073 656c 662e  ''.        self.
-00032bc0: 5f63 616c 6c5f 6d65 7468 6f64 5f77 6974  _call_method_wit
-00032bd0: 685f 6974 6572 6162 6c65 2873 656c 662e  h_iterable(self.
-00032be0: 5f6c 6f61 645f 7370 6563 6966 6963 6174  _load_specificat
-00032bf0: 696f 6e73 2c20 7370 6563 6966 6963 6174  ions, specificat
-00032c00: 696f 6e73 5f66 696c 655f 7061 7468 7329  ions_file_paths)
-00032c10: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-00032c20: 616c 6c5f 6d65 7468 6f64 5f77 6974 685f  all_method_with_
-00032c30: 6974 6572 6162 6c65 2873 656c 662e 5f6c  iterable(self._l
-00032c40: 6f61 645f 6c65 7665 6c73 2c20 6c65 7665  oad_levels, leve
-00032c50: 6c73 5f66 696c 655f 7061 7468 7329 0a20  ls_file_paths). 
-00032c60: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
-00032c70: 6c5f 6d65 7468 6f64 5f77 6974 685f 6974  l_method_with_it
-00032c80: 6572 6162 6c65 2873 656c 662e 5f6c 6f61  erable(self._loa
-00032c90: 645f 7469 6d69 6e67 2c20 7469 6d69 6e67  d_timing, timing
-00032ca0: 5f66 696c 655f 7061 7468 7329 0a0a 2020  _file_paths)..  
-00032cb0: 2020 6465 6620 5f63 616c 6c5f 6d65 7468    def _call_meth
-00032cc0: 6f64 5f77 6974 685f 6974 6572 6162 6c65  od_with_iterable
-00032cd0: 2873 656c 662c 206d 6574 686f 642c 2066  (self, method, f
-00032ce0: 696c 6573 293a 0a20 2020 2020 2020 2069  iles):.        i
-00032cf0: 6620 6669 6c65 7320 6973 204e 6f6e 653a  f files is None:
-00032d00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00032d10: 7572 6e0a 2020 2020 2020 2020 6966 2069  urn.        if i
-00032d20: 7369 6e73 7461 6e63 6528 6669 6c65 732c  sinstance(files,
-00032d30: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-00032d40: 2020 2066 696c 6573 203d 205b 6669 6c65     files = [file
-00032d50: 735d 0a20 2020 2020 2020 2066 6f72 2066  s].        for f
-00032d60: 2069 6e20 6669 6c65 733a 0a20 2020 2020   in files:.     
-00032d70: 2020 2020 2020 206d 6574 686f 6428 6629         method(f)
-00032d80: 0a0a 2020 2020 4069 7669 5f73 796e 6368  ..    @ivi_synch
-00032d90: 726f 6e69 7a65 640a 2020 2020 6465 6620  ronized.    def 
-00032da0: 7365 6c66 5f74 6573 7428 7365 6c66 293a  self_test(self):
-00032db0: 0a20 2020 2020 2020 2027 2727 7365 6c66  .        '''self
-00032dc0: 5f74 6573 740a 0a20 2020 2020 2020 2052  _test..        R
-00032dd0: 6574 7572 6e73 2073 656c 6620 7465 7374  eturns self test
-00032de0: 2072 6573 756c 7473 2066 726f 6d20 6120   results from a 
-00032df0: 6469 6769 7461 6c20 7061 7474 6572 6e20  digital pattern 
-00032e00: 696e 7374 7275 6d65 6e74 2e20 5468 6973  instrument. This
-00032e10: 2074 6573 7420 7265 7175 6972 6573 2073   test requires s
-00032e20: 6576 6572 616c 206d 696e 7574 6573 2074  everal minutes t
-00032e30: 6f20 6578 6563 7574 652e 0a0a 2020 2020  o execute...    
-00032e40: 2020 2020 5261 6973 6573 2060 5365 6c66      Raises `Self
-00032e50: 5465 7374 4572 726f 7260 206f 6e20 7365  TestError` on se
-00032e60: 6c66 2074 6573 7420 6661 696c 7572 652e  lf test failure.
-00032e70: 2050 726f 7065 7274 6965 7320 6f6e 2065   Properties on e
-00032e80: 7863 6570 7469 6f6e 206f 626a 6563 743a  xception object:
-00032e90: 0a0a 2020 2020 2020 2020 2d20 636f 6465  ..        - code
-00032ea0: 202d 2066 6169 6c75 7265 2063 6f64 6520   - failure code 
-00032eb0: 6672 6f6d 2064 7269 7665 720a 2020 2020  from driver.    
-00032ec0: 2020 2020 2d20 6d65 7373 6167 6520 2d20      - message - 
-00032ed0: 7374 6174 7573 206d 6573 7361 6765 2066  status message f
-00032ee0: 726f 6d20 6472 6976 6572 0a0a 2020 2020  rom driver..    
-00032ef0: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d      +-----------
-00032f00: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00032f10: 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020  ---------+.     
-00032f20: 2020 207c 2053 656c 662d 5465 7374 2043     | Self-Test C
-00032f30: 6f64 6520 7c20 4465 7363 7269 7074 696f  ode | Descriptio
-00032f40: 6e20 2020 2020 2020 7c0a 2020 2020 2020  n       |.      
-00032f50: 2020 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    +=============
-00032f60: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ===+============
-00032f70: 3d3d 3d3d 3d3d 3d2b 0a20 2020 2020 2020  =======+.       
-00032f80: 207c 2030 2020 2020 2020 2020 2020 2020   | 0            
-00032f90: 2020 7c20 5365 6c66 2074 6573 7420 7061    | Self test pa
-00032fa0: 7373 6564 2e20 7c0a 2020 2020 2020 2020  ssed. |.        
-00032fb0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00032fc0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00032fd0: 2d2d 2d2d 2d2b 0a20 2020 2020 2020 207c  -----+.        |
-00032fe0: 2031 2020 2020 2020 2020 2020 2020 2020   1              
-00032ff0: 7c20 5365 6c66 2074 6573 7420 6661 696c  | Self test fail
-00033000: 6564 2e20 7c0a 2020 2020 2020 2020 2b2d  ed. |.        +-
-00033010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+000307b0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a  ---+---------+..
+000307c0: 2020 2020 2020 2020 2020 2020 6772 7063              grpc
+000307d0: 5f6f 7074 696f 6e73 2028 6e69 6469 6769  _options (nidigi
+000307e0: 7461 6c2e 6772 7063 5f73 6573 7369 6f6e  tal.grpc_session
+000307f0: 5f6f 7074 696f 6e73 2e47 7270 6353 6573  _options.GrpcSes
+00030800: 7369 6f6e 4f70 7469 6f6e 7329 3a20 4d65  sionOptions): Me
+00030810: 6173 7572 656d 656e 744c 696e 6b20 6752  asurementLink gR
+00030820: 5043 2073 6573 7369 6f6e 206f 7074 696f  PC session optio
+00030830: 6e73 0a0a 0a20 2020 2020 2020 2052 6574  ns...        Ret
+00030840: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00030850: 2020 6e65 775f 7669 2028 696e 7429 3a20    new_vi (int): 
+00030860: 5468 6520 7265 7475 726e 6564 2069 6e73  The returned ins
+00030870: 7472 756d 656e 7420 7365 7373 696f 6e2e  trument session.
+00030880: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00030890: 2020 2020 2020 6966 2067 7270 635f 6f70        if grpc_op
+000308a0: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
+000308b0: 2020 2069 6d70 6f72 7420 6e69 6469 6769     import nidigi
+000308c0: 7461 6c2e 5f67 7270 635f 7374 7562 5f69  tal._grpc_stub_i
+000308d0: 6e74 6572 7072 6574 6572 2061 7320 5f67  nterpreter as _g
+000308e0: 7270 635f 7374 7562 5f69 6e74 6572 7072  rpc_stub_interpr
+000308f0: 6574 6572 0a20 2020 2020 2020 2020 2020  eter.           
+00030900: 2069 6e74 6572 7072 6574 6572 203d 205f   interpreter = _
+00030910: 6772 7063 5f73 7475 625f 696e 7465 7270  grpc_stub_interp
+00030920: 7265 7465 722e 4772 7063 5374 7562 496e  reter.GrpcStubIn
+00030930: 7465 7270 7265 7465 7228 6772 7063 5f6f  terpreter(grpc_o
+00030940: 7074 696f 6e73 290a 2020 2020 2020 2020  ptions).        
+00030950: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00030960: 2020 696e 7465 7270 7265 7465 7220 3d20    interpreter = 
+00030970: 5f6c 6962 7261 7279 5f69 6e74 6572 7072  _library_interpr
+00030980: 6574 6572 2e4c 6962 7261 7279 496e 7465  eter.LibraryInte
+00030990: 7270 7265 7465 7228 656e 636f 6469 6e67  rpreter(encoding
+000309a0: 3d27 7769 6e64 6f77 732d 3132 3531 2729  ='windows-1251')
+000309b0: 0a0a 2020 2020 2020 2020 2320 496e 6974  ..        # Init
+000309c0: 6961 6c69 7a65 2074 6865 2073 7570 6572  ialize the super
+000309d0: 636c 6173 7320 7769 7468 2064 6566 6175  class with defau
+000309e0: 6c74 2076 616c 7565 7320 6669 7273 742c  lt values first,
+000309f0: 2070 6f70 756c 6174 6520 7468 656d 206c   populate them l
+00030a00: 6174 6572 0a20 2020 2020 2020 2073 7570  ater.        sup
+00030a10: 6572 2853 6573 7369 6f6e 2c20 7365 6c66  er(Session, self
+00030a20: 292e 5f5f 696e 6974 5f5f 280a 2020 2020  ).__init__(.    
+00030a30: 2020 2020 2020 2020 7265 7065 6174 6564          repeated
+00030a40: 5f63 6170 6162 696c 6974 795f 6c69 7374  _capability_list
+00030a50: 3d5b 5d2c 0a20 2020 2020 2020 2020 2020  =[],.           
+00030a60: 2069 6e74 6572 7072 6574 6572 3d69 6e74   interpreter=int
+00030a70: 6572 7072 6574 6572 2c0a 2020 2020 2020  erpreter,.      
+00030a80: 2020 2020 2020 6672 6565 7a65 5f69 743d        freeze_it=
+00030a90: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+00030aa0: 2020 2061 6c6c 5f63 6861 6e6e 656c 735f     all_channels_
+00030ab0: 696e 5f73 6573 7369 6f6e 3d4e 6f6e 650a  in_session=None.
+00030ac0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00030ad0: 2020 6f70 7469 6f6e 7320 3d20 5f63 6f6e    options = _con
+00030ae0: 7665 7274 6572 732e 636f 6e76 6572 745f  verters.convert_
+00030af0: 696e 6974 5f77 6974 685f 6f70 7469 6f6e  init_with_option
+00030b00: 735f 6469 6374 696f 6e61 7279 286f 7074  s_dictionary(opt
+00030b10: 696f 6e73 290a 0a20 2020 2020 2020 2023  ions)..        #
+00030b20: 2043 616c 6c20 7370 6563 6966 6965 6420   Call specified 
+00030b30: 696e 6974 2066 756e 6374 696f 6e0a 2020  init function.  
+00030b40: 2020 2020 2020 2320 4e6f 7465 2074 6861        # Note tha
+00030b50: 7420 5f69 6e74 6572 7072 6574 6572 2064  t _interpreter d
+00030b60: 6566 6175 6c74 2d69 6e69 7469 616c 697a  efault-initializ
+00030b70: 6573 2074 6865 2073 6573 7369 6f6e 2068  es the session h
+00030b80: 616e 646c 6520 696e 2069 7473 2063 6f6e  andle in its con
+00030b90: 7374 7275 6374 6f72 2c20 736f 2074 6861  structor, so tha
+00030ba0: 740a 2020 2020 2020 2020 2320 6966 205f  t.        # if _
+00030bb0: 696e 6974 5f77 6974 685f 6f70 7469 6f6e  init_with_option
+00030bc0: 7320 6661 696c 732c 2074 6865 2065 7272  s fails, the err
+00030bd0: 6f72 2068 616e 646c 6572 2063 616e 2072  or handler can r
+00030be0: 6566 6572 656e 6365 2069 742e 0a20 2020  eference it..   
+00030bf0: 2020 2020 2023 2041 6e64 2074 6865 6e20       # And then 
+00030c00: 6865 7265 2c20 6f6e 6365 205f 696e 6974  here, once _init
+00030c10: 5f77 6974 685f 6f70 7469 6f6e 7320 7375  _with_options su
+00030c20: 6363 6565 6473 2c20 7765 2063 616c 6c20  cceeds, we call 
+00030c30: 7365 745f 7365 7373 696f 6e5f 6861 6e64  set_session_hand
+00030c40: 6c65 0a20 2020 2020 2020 2023 2077 6974  le.        # wit
+00030c50: 6820 7468 6520 6163 7475 616c 2073 6573  h the actual ses
+00030c60: 7369 6f6e 2068 616e 646c 652e 0a20 2020  sion handle..   
+00030c70: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
+00030c80: 7072 6574 6572 2e73 6574 5f73 6573 7369  preter.set_sessi
+00030c90: 6f6e 5f68 616e 646c 6528 7365 6c66 2e5f  on_handle(self._
+00030ca0: 696e 6974 5f77 6974 685f 6f70 7469 6f6e  init_with_option
+00030cb0: 7328 7265 736f 7572 6365 5f6e 616d 652c  s(resource_name,
+00030cc0: 2069 645f 7175 6572 792c 2072 6573 6574   id_query, reset
+00030cd0: 5f64 6576 6963 652c 206f 7074 696f 6e73  _device, options
+00030ce0: 2929 0a0a 2020 2020 2020 2020 2320 4e49  ))..        # NI
+00030cf0: 2d54 436c 6b20 646f 6573 206e 6f74 2077  -TClk does not w
+00030d00: 6f72 6b20 6f76 6572 204e 4920 6752 5043  ork over NI gRPC
+00030d10: 2044 6576 6963 6520 5365 7276 6572 0a20   Device Server. 
+00030d20: 2020 2020 2020 2069 6620 6e6f 7420 6772         if not gr
+00030d30: 7063 5f6f 7074 696f 6e73 3a0a 2020 2020  pc_options:.    
+00030d40: 2020 2020 2020 2020 7365 6c66 2e74 636c          self.tcl
+00030d50: 6b20 3d20 6e69 7463 6c6b 2e53 6573 7369  k = nitclk.Sessi
+00030d60: 6f6e 5265 6665 7265 6e63 6528 7365 6c66  onReference(self
+00030d70: 2e5f 696e 7465 7270 7265 7465 722e 6765  ._interpreter.ge
+00030d80: 745f 7365 7373 696f 6e5f 6861 6e64 6c65  t_session_handle
+00030d90: 2829 290a 0a20 2020 2020 2020 2023 2053  ())..        # S
+00030da0: 746f 7265 2074 6865 2070 6172 616d 6574  tore the paramet
+00030db0: 6572 206c 6973 7420 666f 7220 6c61 7465  er list for late
+00030dc0: 7220 7072 696e 7469 6e67 2069 6e20 5f5f  r printing in __
+00030dd0: 7265 7072 5f5f 0a20 2020 2020 2020 2070  repr__.        p
+00030de0: 6172 616d 5f6c 6973 7420 3d20 5b5d 0a20  aram_list = []. 
+00030df0: 2020 2020 2020 2070 6172 616d 5f6c 6973         param_lis
+00030e00: 742e 6170 7065 6e64 2822 7265 736f 7572  t.append("resour
+00030e10: 6365 5f6e 616d 653d 2220 2b20 7070 2e70  ce_name=" + pp.p
+00030e20: 666f 726d 6174 2872 6573 6f75 7263 655f  format(resource_
+00030e30: 6e61 6d65 2929 0a20 2020 2020 2020 2070  name)).        p
+00030e40: 6172 616d 5f6c 6973 742e 6170 7065 6e64  aram_list.append
+00030e50: 2822 7265 7365 745f 6465 7669 6365 3d22  ("reset_device="
+00030e60: 202b 2070 702e 7066 6f72 6d61 7428 7265   + pp.pformat(re
+00030e70: 7365 745f 6465 7669 6365 2929 0a20 2020  set_device)).   
+00030e80: 2020 2020 2070 6172 616d 5f6c 6973 742e       param_list.
+00030e90: 6170 7065 6e64 2822 6f70 7469 6f6e 733d  append("options=
+00030ea0: 2220 2b20 7070 2e70 666f 726d 6174 286f  " + pp.pformat(o
+00030eb0: 7074 696f 6e73 2929 0a20 2020 2020 2020  ptions)).       
+00030ec0: 2073 656c 662e 5f70 6172 616d 5f6c 6973   self._param_lis
+00030ed0: 7420 3d20 272c 2027 2e6a 6f69 6e28 7061  t = ', '.join(pa
+00030ee0: 7261 6d5f 6c69 7374 290a 0a20 2020 2020  ram_list)..     
+00030ef0: 2020 2023 2053 746f 7265 2074 6865 206c     # Store the l
+00030f00: 6973 7420 6f66 2063 6861 6e6e 656c 7320  ist of channels 
+00030f10: 696e 2074 6865 2053 6573 7369 6f6e 2077  in the Session w
+00030f20: 6869 6368 2069 7320 6e65 6564 6564 2062  hich is needed b
+00030f30: 7920 736f 6d65 206e 696d 692d 7079 7468  y some nimi-pyth
+00030f40: 6f6e 206d 6f64 756c 6573 2e0a 2020 2020  on modules..    
+00030f50: 2020 2020 2320 5573 6520 7472 792f 6578      # Use try/ex
+00030f60: 6365 7074 2062 6563 6175 7365 206e 6f74  cept because not
+00030f70: 2061 6c6c 2074 6865 206d 6f64 756c 6573   all the modules
+00030f80: 2073 7570 706f 7274 2063 6861 6e6e 656c   support channel
+00030f90: 732e 0a20 2020 2020 2020 2023 2073 656c  s..        # sel
+00030fa0: 662e 6765 745f 6368 616e 6e65 6c5f 6e61  f.get_channel_na
+00030fb0: 6d65 7328 2920 616e 6420 7365 6c66 2e63  mes() and self.c
+00030fc0: 6861 6e6e 656c 5f63 6f75 6e74 2063 616e  hannel_count can
+00030fd0: 206f 6e6c 7920 6265 2063 616c 6c65 6420   only be called 
+00030fe0: 6166 7465 7220 7468 6520 7365 7373 696f  after the sessio
+00030ff0: 6e0a 2020 2020 2020 2020 2320 6861 6e64  n.        # hand
+00031000: 6c65 2069 7320 7365 740a 2020 2020 2020  le is set.      
+00031010: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00031020: 2020 2073 656c 662e 5f61 6c6c 5f63 6861     self._all_cha
+00031030: 6e6e 656c 735f 696e 5f73 6573 7369 6f6e  nnels_in_session
+00031040: 203d 2073 656c 662e 6765 745f 6368 616e   = self.get_chan
+00031050: 6e65 6c5f 6e61 6d65 7328 7261 6e67 6528  nel_names(range(
+00031060: 7365 6c66 2e63 6861 6e6e 656c 5f63 6f75  self.channel_cou
+00031070: 6e74 2929 0a20 2020 2020 2020 2065 7863  nt)).        exc
+00031080: 6570 7420 4174 7472 6962 7574 6545 7272  ept AttributeErr
+00031090: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+000310a0: 7365 6c66 2e5f 616c 6c5f 6368 616e 6e65  self._all_channe
+000310b0: 6c73 5f69 6e5f 7365 7373 696f 6e20 3d20  ls_in_session = 
+000310c0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2320  None..        # 
+000310d0: 4669 6e61 6c6c 792c 2073 6574 205f 6973  Finally, set _is
+000310e0: 5f66 726f 7a65 6e20 746f 2054 7275 6520  _frozen to True 
+000310f0: 7768 6963 6820 6973 2075 7365 6420 746f  which is used to
+00031100: 2070 7265 7665 6e74 2063 6c69 656e 7473   prevent clients
+00031110: 2066 726f 6d20 6163 6369 6465 6e74 616c   from accidental
+00031120: 6c79 2061 6464 696e 670a 2020 2020 2020  ly adding.      
+00031130: 2020 2320 6d65 6d62 6572 7320 7768 656e    # members when
+00031140: 2074 7279 696e 6720 746f 2073 6574 2061   trying to set a
+00031150: 2070 726f 7065 7274 7920 7769 7468 2061   property with a
+00031160: 2074 7970 6f2e 0a20 2020 2020 2020 2073   typo..        s
+00031170: 656c 662e 5f69 735f 6672 6f7a 656e 203d  elf._is_frozen =
+00031180: 2054 7275 650a 0a20 2020 2064 6566 205f   True..    def _
+00031190: 5f65 6e74 6572 5f5f 2873 656c 6629 3a0a  _enter__(self):.
+000311a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000311b0: 656c 660a 0a20 2020 2064 6566 205f 5f65  elf..    def __e
+000311c0: 7869 745f 5f28 7365 6c66 2c20 6578 635f  xit__(self, exc_
+000311d0: 7479 7065 2c20 6578 635f 7661 6c75 652c  type, exc_value,
+000311e0: 2074 7261 6365 6261 636b 293a 0a20 2020   traceback):.   
+000311f0: 2020 2020 2069 6620 7365 6c66 2e5f 696e       if self._in
+00031200: 7465 7270 7265 7465 722e 5f63 6c6f 7365  terpreter._close
+00031210: 5f6f 6e5f 6578 6974 3a0a 2020 2020 2020  _on_exit:.      
+00031220: 2020 2020 2020 7365 6c66 2e63 6c6f 7365        self.close
+00031230: 2829 0a0a 2020 2020 6465 6620 696e 6974  ()..    def init
+00031240: 6961 7465 2873 656c 6629 3a0a 2020 2020  iate(self):.    
+00031250: 2020 2020 2727 2769 6e69 7469 6174 650a      '''initiate.
+00031260: 0a20 2020 2020 2020 2053 7461 7274 7320  .        Starts 
+00031270: 6275 7273 7469 6e67 2074 6865 2070 6174  bursting the pat
+00031280: 7465 726e 2063 6f6e 6669 6775 7265 6420  tern configured 
+00031290: 6279 2073 7461 7274 5f6c 6162 656c 2c20  by start_label, 
+000312a0: 6361 7573 696e 6720 7468 6520 4e49 2d44  causing the NI-D
+000312b0: 6967 6974 616c 2073 6573 7369 6f6e 2074  igital session t
+000312c0: 6f20 6265 2063 6f6d 6d69 7474 6564 2e20  o be committed. 
+000312d0: 546f 2073 746f 7020 7468 6520 7061 7474  To stop the patt
+000312e0: 6572 6e20 6275 7273 742c 2063 616c 6c20  ern burst, call 
+000312f0: 6162 6f72 742e 2049 6620 6b65 6570 2061  abort. If keep a
+00031300: 6c69 7665 2070 6174 7465 726e 2069 7320  live pattern is 
+00031310: 6275 7273 7469 6e67 2077 6865 6e20 6162  bursting when ab
+00031320: 6f72 7420 6973 2063 616c 6c65 6420 6f72  ort is called or
+00031330: 2075 706f 6e20 6578 6974 696e 6720 7468   upon exiting th
+00031340: 6520 636f 6e74 6578 7420 6d61 6e61 6765  e context manage
+00031350: 722c 206b 6565 7020 616c 6976 6520 7061  r, keep alive pa
+00031360: 7474 6572 6e20 7769 6c6c 206e 6f74 2062  ttern will not b
+00031370: 6520 7374 6f70 7065 642e 2054 6f20 7374  e stopped. To st
+00031380: 6f70 2074 6865 206b 6565 7020 616c 6976  op the keep aliv
+00031390: 6520 7061 7474 6572 6e2c 2063 616c 6c20  e pattern, call 
+000313a0: 6162 6f72 745f 6b65 6570 5f61 6c69 7665  abort_keep_alive
+000313b0: 2e0a 0a20 2020 2020 2020 204e 6f74 653a  ...        Note:
+000313c0: 0a20 2020 2020 2020 2054 6869 7320 6d65  .        This me
+000313d0: 7468 6f64 2077 696c 6c20 7265 7475 726e  thod will return
+000313e0: 2061 2050 7974 686f 6e20 636f 6e74 6578   a Python contex
+000313f0: 7420 6d61 6e61 6765 7220 7468 6174 2077  t manager that w
+00031400: 696c 6c20 696e 6974 6961 7465 206f 6e20  ill initiate on 
+00031410: 656e 7465 7269 6e67 2061 6e64 2061 626f  entering and abo
+00031420: 7274 206f 6e20 6578 6974 2e0a 2020 2020  rt on exit..    
+00031430: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00031440: 7265 7475 726e 205f 4275 7273 7428 7365  return _Burst(se
+00031450: 6c66 290a 0a20 2020 2064 6566 2063 6c6f  lf)..    def clo
+00031460: 7365 2873 656c 6629 3a0a 2020 2020 2020  se(self):.      
+00031470: 2020 2727 2763 6c6f 7365 0a0a 2020 2020    '''close..    
+00031480: 2020 2020 436c 6f73 6573 2074 6865 2073      Closes the s
+00031490: 7065 6369 6669 6564 2069 6e73 7472 756d  pecified instrum
+000314a0: 656e 7420 7365 7373 696f 6e20 746f 2061  ent session to a
+000314b0: 2064 6967 6974 616c 2070 6174 7465 726e   digital pattern
+000314c0: 2069 6e73 7472 756d 656e 742c 2061 626f   instrument, abo
+000314d0: 7274 7320 7061 7474 6572 6e20 6578 6563  rts pattern exec
+000314e0: 7574 696f 6e2c 2061 6e64 2075 6e6c 6f61  ution, and unloa
+000314f0: 6473 2070 6174 7465 726e 206d 656d 6f72  ds pattern memor
+00031500: 792e 2054 6865 2063 6861 6e6e 656c 7320  y. The channels 
+00031510: 6f6e 2061 2064 6967 6974 616c 2070 6174  on a digital pat
+00031520: 7465 726e 2069 6e73 7472 756d 656e 7420  tern instrument 
+00031530: 7265 6d61 696e 2069 6e20 7468 6569 7220  remain in their 
+00031540: 6375 7272 656e 7420 7374 6174 652e 0a0a  current state...
+00031550: 2020 2020 2020 2020 4e6f 7465 3a0a 2020          Note:.  
+00031560: 2020 2020 2020 5468 6973 206d 6574 686f        This metho
+00031570: 6420 6973 206e 6f74 206e 6565 6465 6420  d is not needed 
+00031580: 7768 656e 2075 7369 6e67 2074 6865 2073  when using the s
+00031590: 6573 7369 6f6e 2063 6f6e 7465 7874 206d  ession context m
+000315a0: 616e 6167 6572 0a20 2020 2020 2020 2027  anager.        '
+000315b0: 2727 0a20 2020 2020 2020 2074 7279 3a0a  ''.        try:.
+000315c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000315d0: 2e5f 636c 6f73 6528 290a 2020 2020 2020  ._close().      
+000315e0: 2020 6578 6365 7074 2065 7272 6f72 732e    except errors.
+000315f0: 4472 6976 6572 4572 726f 723a 0a20 2020  DriverError:.   
+00031600: 2020 2020 2020 2020 2073 656c 662e 5f69           self._i
+00031610: 6e74 6572 7072 6574 6572 2e73 6574 5f73  nterpreter.set_s
+00031620: 6573 7369 6f6e 5f68 616e 646c 6528 290a  ession_handle().
+00031630: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00031640: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00031650: 696e 7465 7270 7265 7465 722e 7365 745f  interpreter.set_
+00031660: 7365 7373 696f 6e5f 6861 6e64 6c65 2829  session_handle()
+00031670: 0a0a 2020 2020 2727 2720 5468 6573 6520  ..    ''' These 
+00031680: 6172 6520 636f 6465 2d67 656e 6572 6174  are code-generat
+00031690: 6564 2027 2727 0a0a 2020 2020 4069 7669  ed '''..    @ivi
+000316a0: 5f73 796e 6368 726f 6e69 7a65 640a 2020  _synchronized.  
+000316b0: 2020 6465 6620 6162 6f72 7428 7365 6c66    def abort(self
+000316c0: 293a 0a20 2020 2020 2020 2072 2727 2761  ):.        r'''a
+000316d0: 626f 7274 0a0a 2020 2020 2020 2020 5374  bort..        St
+000316e0: 6f70 7320 6275 7273 7469 6e67 2074 6865  ops bursting the
+000316f0: 2070 6174 7465 726e 2e0a 2020 2020 2020   pattern..      
+00031700: 2020 2727 270a 2020 2020 2020 2020 7365    '''.        se
+00031710: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
+00031720: 6162 6f72 7428 290a 0a20 2020 2040 6976  abort()..    @iv
+00031730: 695f 7379 6e63 6872 6f6e 697a 6564 0a20  i_synchronized. 
+00031740: 2020 2064 6566 2061 626f 7274 5f6b 6565     def abort_kee
+00031750: 705f 616c 6976 6528 7365 6c66 293a 0a20  p_alive(self):. 
+00031760: 2020 2020 2020 2072 2727 2761 626f 7274         r'''abort
+00031770: 5f6b 6565 705f 616c 6976 650a 0a20 2020  _keep_alive..   
+00031780: 2020 2020 2053 746f 7073 2074 6865 206b       Stops the k
+00031790: 6565 7020 616c 6976 6520 7061 7474 6572  eep alive patter
+000317a0: 6e20 6966 2069 7420 6973 2063 7572 7265  n if it is curre
+000317b0: 6e74 6c79 2072 756e 6e69 6e67 2e20 4966  ntly running. If
+000317c0: 2061 2070 6174 7465 726e 2062 7572 7374   a pattern burst
+000317d0: 2069 7320 696e 2070 726f 6772 6573 732c   is in progress,
+000317e0: 2074 6865 206d 6574 686f 6420 6162 6f72   the method abor
+000317f0: 7473 2074 6865 2070 6174 7465 726e 2062  ts the pattern b
+00031800: 7572 7374 2e20 4966 2079 6f75 2073 7461  urst. If you sta
+00031810: 7274 2061 206e 6577 2070 6174 7465 726e  rt a new pattern
+00031820: 2062 7572 7374 2077 6869 6c65 2061 206b   burst while a k
+00031830: 6565 7020 616c 6976 6520 7061 7474 6572  eep alive patter
+00031840: 6e20 6973 2072 756e 6e69 6e67 2c20 7468  n is running, th
+00031850: 6520 6b65 6570 2061 6c69 7665 2070 6174  e keep alive pat
+00031860: 7465 726e 2072 756e 7320 746f 2074 6865  tern runs to the
+00031870: 206c 6173 7420 6b65 6570 2061 6c69 7665   last keep alive
+00031880: 2076 6563 746f 722c 2061 6e64 2074 6865   vector, and the
+00031890: 206e 6577 2070 6174 7465 726e 2062 7572   new pattern bur
+000318a0: 7374 2073 7461 7274 7320 6f6e 2074 6865  st starts on the
+000318b0: 206e 6578 7420 6379 636c 652e 0a20 2020   next cycle..   
+000318c0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+000318d0: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
+000318e0: 6572 2e61 626f 7274 5f6b 6565 705f 616c  er.abort_keep_al
+000318f0: 6976 6528 290a 0a20 2020 2040 6976 695f  ive()..    @ivi_
+00031900: 7379 6e63 6872 6f6e 697a 6564 0a20 2020  synchronized.   
+00031910: 2064 6566 2063 6f6d 6d69 7428 7365 6c66   def commit(self
+00031920: 293a 0a20 2020 2020 2020 2072 2727 2763  ):.        r'''c
+00031930: 6f6d 6d69 740a 0a20 2020 2020 2020 2041  ommit..        A
+00031940: 7070 6c69 6573 2061 6c6c 2070 7265 7669  pplies all previ
+00031950: 6f75 736c 7920 636f 6e66 6967 7572 6564  ously configured
+00031960: 2070 696e 206c 6576 656c 732c 2074 6572   pin levels, ter
+00031970: 6d69 6e61 7469 6f6e 206d 6f64 6573 2c20  mination modes, 
+00031980: 636c 6f63 6b73 2c20 7472 6967 6765 7273  clocks, triggers
+00031990: 2c20 616e 6420 7061 7474 6572 6e20 7469  , and pattern ti
+000319a0: 6d69 6e67 2074 6f20 6120 6469 6769 7461  ming to a digita
+000319b0: 6c20 7061 7474 6572 6e20 696e 7374 7275  l pattern instru
+000319c0: 6d65 6e74 2e20 4966 2079 6f75 2064 6f20  ment. If you do 
+000319d0: 6e6f 7420 6361 6c6c 2074 6865 2063 6f6d  not call the com
+000319e0: 6d69 7420 6d65 7468 6f64 2c20 7468 656e  mit method, then
+000319f0: 2074 6865 2069 6e69 7469 6174 6520 6d65   the initiate me
+00031a00: 7468 6f64 206f 7220 7468 6520 6275 7273  thod or the burs
+00031a10: 745f 7061 7474 6572 6e20 6d65 7468 6f64  t_pattern method
+00031a20: 2077 696c 6c20 696d 706c 6963 6974 6c79   will implicitly
+00031a30: 2063 616c 6c20 7468 6973 206d 6574 686f   call this metho
+00031a40: 6420 666f 7220 796f 752e 2043 616c 6c69  d for you. Calli
+00031a50: 6e67 2074 6869 7320 6d65 7468 6f64 206d  ng this method m
+00031a60: 6f76 6573 2074 6865 2073 6573 7369 6f6e  oves the session
+00031a70: 2066 726f 6d20 7468 6520 556e 636f 6d6d   from the Uncomm
+00031a80: 6974 7465 6420 7374 6174 6520 746f 2074  itted state to t
+00031a90: 6865 2043 6f6d 6d69 7474 6564 2073 7461  he Committed sta
+00031aa0: 7465 2e0a 2020 2020 2020 2020 2727 270a  te..        '''.
+00031ab0: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
+00031ac0: 7465 7270 7265 7465 722e 636f 6d6d 6974  terpreter.commit
+00031ad0: 2829 0a0a 2020 2020 4069 7669 5f73 796e  ()..    @ivi_syn
+00031ae0: 6368 726f 6e69 7a65 640a 2020 2020 6465  chronized.    de
+00031af0: 6620 636f 6e66 6967 7572 655f 7469 6d65  f configure_time
+00031b00: 5f73 6574 5f70 6572 696f 6428 7365 6c66  _set_period(self
+00031b10: 2c20 7469 6d65 5f73 6574 5f6e 616d 652c  , time_set_name,
+00031b20: 2070 6572 696f 6429 3a0a 2020 2020 2020   period):.      
+00031b30: 2020 7227 2727 636f 6e66 6967 7572 655f    r'''configure_
+00031b40: 7469 6d65 5f73 6574 5f70 6572 696f 640a  time_set_period.
+00031b50: 0a20 2020 2020 2020 2043 6f6e 6669 6775  .        Configu
+00031b60: 7265 7320 7468 6520 7065 7269 6f64 206f  res the period o
+00031b70: 6620 6120 7469 6d65 2073 6574 2e20 5573  f a time set. Us
+00031b80: 6520 7468 6973 206d 6574 686f 6420 746f  e this method to
+00031b90: 206d 6f64 6966 7920 7469 6d65 2073 6574   modify time set
+00031ba0: 2076 616c 7565 7320 6166 7465 7220 6170   values after ap
+00031bb0: 706c 7969 6e67 2061 2074 696d 696e 6720  plying a timing 
+00031bc0: 7368 6565 7420 7769 7468 2074 6865 2061  sheet with the a
+00031bd0: 7070 6c79 5f6c 6576 656c 735f 616e 645f  pply_levels_and_
+00031be0: 7469 6d69 6e67 206d 6574 686f 642c 206f  timing method, o
+00031bf0: 7220 746f 2063 7265 6174 6520 7469 6d65  r to create time
+00031c00: 2073 6574 7320 7072 6f67 7261 6d6d 6174   sets programmat
+00031c10: 6963 616c 6c79 2077 6974 686f 7574 2074  ically without t
+00031c20: 6865 2075 7365 206f 6620 7469 6d69 6e67  he use of timing
+00031c30: 2073 6865 6574 732e 2054 6869 7320 6d65   sheets. This me
+00031c40: 7468 6f64 2064 6f65 7320 6e6f 7420 6d6f  thod does not mo
+00031c50: 6469 6679 2074 6865 2074 696d 696e 6720  dify the timing 
+00031c60: 7368 6565 7420 6669 6c65 206f 7220 7468  sheet file or th
+00031c70: 6520 7469 6d69 6e67 2073 6865 6574 2063  e timing sheet c
+00031c80: 6f6e 7465 6e74 7320 7468 6174 2077 696c  ontents that wil
+00031c90: 6c20 6265 2075 7365 6420 696e 2066 7574  l be used in fut
+00031ca0: 7572 6520 6361 6c6c 7320 746f 2061 7070  ure calls to app
+00031cb0: 6c79 5f6c 6576 656c 735f 616e 645f 7469  ly_levels_and_ti
+00031cc0: 6d69 6e67 3b20 6974 206f 6e6c 7920 6166  ming; it only af
+00031cd0: 6665 6374 7320 7468 6520 7661 6c75 6573  fects the values
+00031ce0: 206f 6620 7468 6520 6375 7272 656e 7420   of the current 
+00031cf0: 7469 6d69 6e67 2063 6f6e 7465 7874 2e0a  timing context..
+00031d00: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00031d10: 2020 2020 2020 2020 2020 2074 696d 655f             time_
+00031d20: 7365 745f 6e61 6d65 2028 7374 7229 3a20  set_name (str): 
+00031d30: 5468 6520 7370 6563 6966 6965 6420 7469  The specified ti
+00031d40: 6d65 2073 6574 206e 616d 652e 0a0a 2020  me set name...  
+00031d50: 2020 2020 2020 2020 2020 7065 7269 6f64            period
+00031d60: 2028 6869 6768 7469 6d65 2e74 696d 6564   (hightime.timed
+00031d70: 656c 7461 2c20 6461 7465 7469 6d65 2e74  elta, datetime.t
+00031d80: 696d 6564 656c 7461 2c20 6f72 2066 6c6f  imedelta, or flo
+00031d90: 6174 2069 6e20 7365 636f 6e64 7329 3a20  at in seconds): 
+00031da0: 5065 7269 6f64 2066 6f72 2074 6869 7320  Period for this 
+00031db0: 7469 6d65 2073 6574 2c20 696e 2073 6563  time set, in sec
+00031dc0: 6f6e 6473 2e0a 0a20 2020 2020 2020 2027  onds...        '
+00031dd0: 2727 0a20 2020 2020 2020 2070 6572 696f  ''.        perio
+00031de0: 6420 3d20 5f63 6f6e 7665 7274 6572 732e  d = _converters.
+00031df0: 636f 6e76 6572 745f 7469 6d65 6465 6c74  convert_timedelt
+00031e00: 615f 746f 5f73 6563 6f6e 6473 5f72 6561  a_to_seconds_rea
+00031e10: 6c36 3428 7065 7269 6f64 290a 2020 2020  l64(period).    
+00031e20: 2020 2020 7365 6c66 2e5f 696e 7465 7270      self._interp
+00031e30: 7265 7465 722e 636f 6e66 6967 7572 655f  reter.configure_
+00031e40: 7469 6d65 5f73 6574 5f70 6572 696f 6428  time_set_period(
+00031e50: 7469 6d65 5f73 6574 5f6e 616d 652c 2070  time_set_name, p
+00031e60: 6572 696f 6429 0a0a 2020 2020 4069 7669  eriod)..    @ivi
+00031e70: 5f73 796e 6368 726f 6e69 7a65 640a 2020  _synchronized.  
+00031e80: 2020 6465 6620 6372 6561 7465 5f63 6170    def create_cap
+00031e90: 7475 7265 5f77 6176 6566 6f72 6d5f 6672  ture_waveform_fr
+00031ea0: 6f6d 5f66 696c 655f 6469 6769 6361 7074  om_file_digicapt
+00031eb0: 7572 6528 7365 6c66 2c20 7761 7665 666f  ure(self, wavefo
+00031ec0: 726d 5f6e 616d 652c 2077 6176 6566 6f72  rm_name, wavefor
+00031ed0: 6d5f 6669 6c65 5f70 6174 6829 3a0a 2020  m_file_path):.  
+00031ee0: 2020 2020 2020 7227 2727 6372 6561 7465        r'''create
+00031ef0: 5f63 6170 7475 7265 5f77 6176 6566 6f72  _capture_wavefor
+00031f00: 6d5f 6672 6f6d 5f66 696c 655f 6469 6769  m_from_file_digi
+00031f10: 6361 7074 7572 650a 0a20 2020 2020 2020  capture..       
+00031f20: 2043 7265 6174 6573 2061 2063 6170 7475   Creates a captu
+00031f30: 7265 2077 6176 6566 6f72 6d20 7769 7468  re waveform with
+00031f40: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
+00031f50: 6f6e 2069 6e66 6f72 6d61 7469 6f6e 2066  on information f
+00031f60: 726f 6d20 6120 4469 6769 6361 7074 7572  rom a Digicaptur
+00031f70: 6520 6669 6c65 2067 656e 6572 6174 6564  e file generated
+00031f80: 2062 7920 7468 6520 4469 6769 7461 6c20   by the Digital 
+00031f90: 5061 7474 6572 6e20 4564 6974 6f72 2e0a  Pattern Editor..
+00031fa0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00031fb0: 2020 2020 2020 2020 2020 2077 6176 6566             wavef
+00031fc0: 6f72 6d5f 6e61 6d65 2028 7374 7229 3a20  orm_name (str): 
+00031fd0: 5761 7665 666f 726d 206e 616d 6520 796f  Waveform name yo
+00031fe0: 7520 7761 6e74 2074 6f20 7573 652e 2059  u want to use. Y
+00031ff0: 6f75 206d 7573 7420 7370 6563 6966 7920  ou must specify 
+00032000: 7761 7665 666f 726d 5f6e 616d 6520 6966  waveform_name if
+00032010: 2074 6865 2066 696c 6520 636f 6e74 6169   the file contai
+00032020: 6e73 206d 756c 7469 706c 6520 7761 7665  ns multiple wave
+00032030: 666f 726d 732e 2055 7365 2074 6865 2077  forms. Use the w
+00032040: 6176 6566 6f72 6d5f 6e61 6d65 2077 6974  aveform_name wit
+00032050: 6820 7468 6520 6361 7074 7572 655f 7374  h the capture_st
+00032060: 6172 7420 6f70 636f 6465 2069 6e20 796f  art opcode in yo
+00032070: 7572 2070 6174 7465 726e 2e0a 0a20 2020  ur pattern...   
+00032080: 2020 2020 2020 2020 2077 6176 6566 6f72           wavefor
+00032090: 6d5f 6669 6c65 5f70 6174 6820 2873 7472  m_file_path (str
+000320a0: 293a 2041 6273 6f6c 7574 6520 6669 6c65  ): Absolute file
+000320b0: 2070 6174 6820 746f 2074 6865 2063 6170   path to the cap
+000320c0: 7475 7265 2077 6176 6566 6f72 6d20 6669  ture waveform fi
+000320d0: 6c65 2028 2e64 6967 6963 6170 7475 7265  le (.digicapture
+000320e0: 2920 796f 7520 7761 6e74 2074 6f20 6c6f  ) you want to lo
+000320f0: 6164 2e0a 0a20 2020 2020 2020 2027 2727  ad...        '''
+00032100: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+00032110: 6e74 6572 7072 6574 6572 2e63 7265 6174  nterpreter.creat
+00032120: 655f 6361 7074 7572 655f 7761 7665 666f  e_capture_wavefo
+00032130: 726d 5f66 726f 6d5f 6669 6c65 5f64 6967  rm_from_file_dig
+00032140: 6963 6170 7475 7265 2877 6176 6566 6f72  icapture(wavefor
+00032150: 6d5f 6e61 6d65 2c20 7761 7665 666f 726d  m_name, waveform
+00032160: 5f66 696c 655f 7061 7468 290a 0a20 2020  _file_path)..   
+00032170: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
+00032180: 6564 0a20 2020 2064 6566 2063 7265 6174  ed.    def creat
+00032190: 655f 736f 7572 6365 5f77 6176 6566 6f72  e_source_wavefor
+000321a0: 6d5f 6672 6f6d 5f66 696c 655f 7464 6d73  m_from_file_tdms
+000321b0: 2873 656c 662c 2077 6176 6566 6f72 6d5f  (self, waveform_
+000321c0: 6e61 6d65 2c20 7761 7665 666f 726d 5f66  name, waveform_f
+000321d0: 696c 655f 7061 7468 2c20 7772 6974 655f  ile_path, write_
+000321e0: 7761 7665 666f 726d 5f64 6174 613d 5472  waveform_data=Tr
+000321f0: 7565 293a 0a20 2020 2020 2020 2072 2727  ue):.        r''
+00032200: 2763 7265 6174 655f 736f 7572 6365 5f77  'create_source_w
+00032210: 6176 6566 6f72 6d5f 6672 6f6d 5f66 696c  aveform_from_fil
+00032220: 655f 7464 6d73 0a0a 2020 2020 2020 2020  e_tdms..        
+00032230: 4372 6561 7465 7320 6120 736f 7572 6365  Creates a source
+00032240: 2077 6176 6566 6f72 6d20 7769 7468 2063   waveform with c
+00032250: 6f6e 6669 6775 7261 7469 6f6e 2069 6e66  onfiguration inf
+00032260: 6f72 6d61 7469 6f6e 2066 726f 6d20 6120  ormation from a 
+00032270: 5444 4d53 2066 696c 6520 6765 6e65 7261  TDMS file genera
+00032280: 7465 6420 6279 2074 6865 2044 6967 6974  ted by the Digit
+00032290: 616c 2050 6174 7465 726e 2045 6469 746f  al Pattern Edito
+000322a0: 722e 2049 7420 616c 736f 206f 7074 696f  r. It also optio
+000322b0: 6e61 6c6c 7920 7772 6974 6573 2077 6176  nally writes wav
+000322c0: 6566 6f72 6d20 6461 7461 2066 726f 6d20  eform data from 
+000322d0: 7468 6520 6669 6c65 2e0a 0a20 2020 2020  the file...     
+000322e0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000322f0: 2020 2020 2077 6176 6566 6f72 6d5f 6e61       waveform_na
+00032300: 6d65 2028 7374 7229 3a20 5468 6520 7761  me (str): The wa
+00032310: 7665 666f 726d 206e 616d 6520 796f 7520  veform name you 
+00032320: 7761 6e74 2074 6f20 7573 6520 6672 6f6d  want to use from
+00032330: 2074 6865 2066 696c 652e 2059 6f75 206d   the file. You m
+00032340: 7573 7420 7370 6563 6966 7920 7761 7665  ust specify wave
+00032350: 666f 726d 5f6e 616d 6520 6966 2074 6865  form_name if the
+00032360: 2066 696c 6520 636f 6e74 6169 6e73 206d   file contains m
+00032370: 756c 7469 706c 6520 7761 7665 666f 726d  ultiple waveform
+00032380: 732e 2055 7365 2074 6865 2077 6176 6566  s. Use the wavef
+00032390: 6f72 6d5f 6e61 6d65 2077 6974 6820 7468  orm_name with th
+000323a0: 6520 736f 7572 6365 5f73 7461 7274 206f  e source_start o
+000323b0: 7063 6f64 6520 696e 2079 6f75 7220 7061  pcode in your pa
+000323c0: 7474 6572 6e2e 0a0a 2020 2020 2020 2020  ttern...        
+000323d0: 2020 2020 7761 7665 666f 726d 5f66 696c      waveform_fil
+000323e0: 655f 7061 7468 2028 7374 7229 3a20 4162  e_path (str): Ab
+000323f0: 736f 6c75 7465 2066 696c 6520 7061 7468  solute file path
+00032400: 2074 6f20 7468 6520 6c6f 6164 2073 6f75   to the load sou
+00032410: 7263 6520 7761 7665 666f 726d 2066 696c  rce waveform fil
+00032420: 6520 282e 7464 6d73 292e 0a0a 2020 2020  e (.tdms)...    
+00032430: 2020 2020 2020 2020 7772 6974 655f 7761          write_wa
+00032440: 7665 666f 726d 5f64 6174 6120 2862 6f6f  veform_data (boo
+00032450: 6c29 3a20 4120 426f 6f6c 6561 6e20 7468  l): A Boolean th
+00032460: 6174 2077 7269 7465 7320 7761 7665 666f  at writes wavefo
+00032470: 726d 2064 6174 6120 746f 2073 6f75 7263  rm data to sourc
+00032480: 6520 6d65 6d6f 7279 2069 6620 5472 7565  e memory if True
+00032490: 2061 6e64 2074 6865 2077 6176 6566 6f72   and the wavefor
+000324a0: 6d20 6461 7461 2069 7320 696e 2074 6865  m data is in the
+000324b0: 2066 696c 652e 0a0a 2020 2020 2020 2020   file...        
+000324c0: 2727 270a 2020 2020 2020 2020 7365 6c66  '''.        self
+000324d0: 2e5f 696e 7465 7270 7265 7465 722e 6372  ._interpreter.cr
+000324e0: 6561 7465 5f73 6f75 7263 655f 7761 7665  eate_source_wave
+000324f0: 666f 726d 5f66 726f 6d5f 6669 6c65 5f74  form_from_file_t
+00032500: 646d 7328 7761 7665 666f 726d 5f6e 616d  dms(waveform_nam
+00032510: 652c 2077 6176 6566 6f72 6d5f 6669 6c65  e, waveform_file
+00032520: 5f70 6174 682c 2077 7269 7465 5f77 6176  _path, write_wav
+00032530: 6566 6f72 6d5f 6461 7461 290a 0a20 2020  eform_data)..   
+00032540: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
+00032550: 6564 0a20 2020 2064 6566 2063 7265 6174  ed.    def creat
+00032560: 655f 7469 6d65 5f73 6574 2873 656c 662c  e_time_set(self,
+00032570: 206e 616d 6529 3a0a 2020 2020 2020 2020   name):.        
+00032580: 7227 2727 6372 6561 7465 5f74 696d 655f  r'''create_time_
+00032590: 7365 740a 0a20 2020 2020 2020 2043 7265  set..        Cre
+000325a0: 6174 6573 2061 2074 696d 6520 7365 7420  ates a time set 
+000325b0: 7769 7468 2074 6865 206e 616d 6520 7468  with the name th
+000325c0: 6174 2079 6f75 2073 7065 6369 6679 2e20  at you specify. 
+000325d0: 5573 6520 7468 6973 206d 6574 686f 6420  Use this method 
+000325e0: 7768 656e 2079 6f75 2077 616e 7420 746f  when you want to
+000325f0: 2063 7265 6174 6520 7469 6d65 2073 6574   create time set
+00032600: 7320 7072 6f67 7261 6d6d 6174 6963 616c  s programmatical
+00032610: 6c79 2072 6174 6865 7220 7468 616e 2077  ly rather than w
+00032620: 6974 6820 6120 7469 6d69 6e67 2073 6865  ith a timing she
+00032630: 6574 2e0a 0a20 2020 2020 2020 2041 7267  et...        Arg
+00032640: 733a 0a20 2020 2020 2020 2020 2020 206e  s:.            n
+00032650: 616d 6520 2873 7472 293a 2054 6865 2073  ame (str): The s
+00032660: 7065 6369 6669 6564 206e 616d 6520 6f66  pecified name of
+00032670: 2074 6865 206e 6577 2074 696d 6520 7365   the new time se
+00032680: 742e 0a0a 2020 2020 2020 2020 2727 270a  t...        '''.
+00032690: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
+000326a0: 7465 7270 7265 7465 722e 6372 6561 7465  terpreter.create
+000326b0: 5f74 696d 655f 7365 7428 6e61 6d65 290a  _time_set(name).
+000326c0: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
+000326d0: 6f6e 697a 6564 0a20 2020 2064 6566 2064  onized.    def d
+000326e0: 656c 6574 655f 616c 6c5f 7469 6d65 5f73  elete_all_time_s
+000326f0: 6574 7328 7365 6c66 293a 0a20 2020 2020  ets(self):.     
+00032700: 2020 2072 2727 2764 656c 6574 655f 616c     r'''delete_al
+00032710: 6c5f 7469 6d65 5f73 6574 730a 0a20 2020  l_time_sets..   
+00032720: 2020 2020 2044 656c 6574 6573 2061 6c6c       Deletes all
+00032730: 2074 696d 6520 7365 7473 2066 726f 6d20   time sets from 
+00032740: 696e 7374 7275 6d65 6e74 206d 656d 6f72  instrument memor
+00032750: 792e 0a20 2020 2020 2020 2027 2727 0a20  y..        '''. 
+00032760: 2020 2020 2020 2073 656c 662e 5f69 6e74         self._int
+00032770: 6572 7072 6574 6572 2e64 656c 6574 655f  erpreter.delete_
+00032780: 616c 6c5f 7469 6d65 5f73 6574 7328 290a  all_time_sets().
+00032790: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
+000327a0: 6f6e 697a 6564 0a20 2020 2064 6566 206c  onized.    def l
+000327b0: 6f61 645f 7370 6563 6966 6963 6174 696f  oad_specificatio
+000327c0: 6e73 5f6c 6576 656c 735f 616e 645f 7469  ns_levels_and_ti
+000327d0: 6d69 6e67 2873 656c 662c 2073 7065 6369  ming(self, speci
+000327e0: 6669 6361 7469 6f6e 735f 6669 6c65 5f70  fications_file_p
+000327f0: 6174 6873 3d4e 6f6e 652c 206c 6576 656c  aths=None, level
+00032800: 735f 6669 6c65 5f70 6174 6873 3d4e 6f6e  s_file_paths=Non
+00032810: 652c 2074 696d 696e 675f 6669 6c65 5f70  e, timing_file_p
+00032820: 6174 6873 3d4e 6f6e 6529 3a0a 2020 2020  aths=None):.    
+00032830: 2020 2020 2727 276c 6f61 645f 7370 6563      '''load_spec
+00032840: 6966 6963 6174 696f 6e73 5f6c 6576 656c  ifications_level
+00032850: 735f 616e 645f 7469 6d69 6e67 0a0a 2020  s_and_timing..  
+00032860: 2020 2020 2020 4c6f 6164 7320 7365 7474        Loads sett
+00032870: 696e 6773 2069 6e20 7370 6563 6966 6963  ings in specific
+00032880: 6174 696f 6e73 2c20 6c65 7665 6c73 2c20  ations, levels, 
+00032890: 616e 6420 7469 6d69 6e67 2073 6865 6574  and timing sheet
+000328a0: 732e 2054 6865 7365 2073 6574 7469 6e67  s. These setting
+000328b0: 7320 6172 6520 6e6f 740a 2020 2020 2020  s are not.      
+000328c0: 2020 6170 706c 6965 6420 746f 2074 6865    applied to the
+000328d0: 2064 6967 6974 616c 2070 6174 7465 726e   digital pattern
+000328e0: 2069 6e73 7472 756d 656e 7420 756e 7469   instrument unti
+000328f0: 6c20 6170 706c 795f 6c65 7665 6c73 5f61  l apply_levels_a
+00032900: 6e64 5f74 696d 696e 6720 6973 2063 616c  nd_timing is cal
+00032910: 6c65 642e 0a0a 2020 2020 2020 2020 4966  led...        If
+00032920: 2074 6865 206c 6576 656c 7320 616e 6420   the levels and 
+00032930: 7469 6d69 6e67 2073 6865 6574 7320 636f  timing sheets co
+00032940: 6e74 6169 6e73 2066 6f72 6d75 6c61 732c  ntains formulas,
+00032950: 2074 6865 7920 6172 6520 6576 616c 7561   they are evalua
+00032960: 7465 6420 6174 206c 6f61 6420 7469 6d65  ted at load time
+00032970: 2e0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
+00032980: 2066 6f72 6d75 6c61 7320 7265 6665 7220   formulas refer 
+00032990: 746f 2076 6172 6961 626c 6573 2c20 7468  to variables, th
+000329a0: 6520 7370 6563 6966 6963 6174 696f 6e73  e specifications
+000329b0: 2073 6865 6574 7320 7468 6174 2064 6566   sheets that def
+000329c0: 696e 6520 7468 6f73 650a 2020 2020 2020  ine those.      
+000329d0: 2020 7661 7269 6162 6c65 7320 6d75 7374    variables must
+000329e0: 2062 6520 6c6f 6164 6564 2065 6974 6865   be loaded eithe
+000329f0: 7220 6669 7273 742c 206f 7220 6174 2074  r first, or at t
+00032a00: 6865 2073 616d 6520 7469 6d65 2061 7320  he same time as 
+00032a10: 7468 6520 6c65 7665 6c73 2061 6e64 2074  the levels and t
+00032a20: 696d 696e 6720 7368 6565 7473 2e0a 0a20  iming sheets... 
+00032a30: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00032a40: 2020 2020 2020 2020 2073 7065 6369 6669           specifi
+00032a50: 6361 7469 6f6e 735f 6669 6c65 5f70 6174  cations_file_pat
+00032a60: 6873 2028 7374 7220 6f72 2062 6173 6963  hs (str or basic
+00032a70: 2073 6571 7565 6e63 6520 6f66 2073 7472   sequence of str
+00032a80: 293a 2041 6273 6f6c 7574 6520 6669 6c65  ): Absolute file
+00032a90: 2070 6174 6820 6f66 206f 6e65 206f 7220   path of one or 
+00032aa0: 6d6f 7265 2073 7065 6369 6669 6361 7469  more specificati
+00032ab0: 6f6e 7320 6669 6c65 732e 0a0a 2020 2020  ons files...    
+00032ac0: 2020 2020 2020 2020 6c65 7665 6c73 5f66          levels_f
+00032ad0: 696c 655f 7061 7468 7320 2873 7472 206f  ile_paths (str o
+00032ae0: 7220 6261 7369 6320 7365 7175 656e 6365  r basic sequence
+00032af0: 206f 6620 7374 7229 3a20 4162 736f 6c75   of str): Absolu
+00032b00: 7465 2066 696c 6520 7061 7468 206f 6620  te file path of 
+00032b10: 6f6e 6520 6f72 206d 6f72 6520 6c65 7665  one or more leve
+00032b20: 6c73 2073 6865 6574 2066 696c 6573 2e0a  ls sheet files..
+00032b30: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00032b40: 696e 675f 6669 6c65 5f70 6174 6873 2028  ing_file_paths (
+00032b50: 7374 7220 6f72 2062 6173 6963 2073 6571  str or basic seq
+00032b60: 7565 6e63 6520 6f66 2073 7472 293a 2041  uence of str): A
+00032b70: 6273 6f6c 7574 6520 6669 6c65 2070 6174  bsolute file pat
+00032b80: 6820 6f66 206f 6e65 206f 7220 6d6f 7265  h of one or more
+00032b90: 2074 696d 696e 6720 7368 6565 7420 6669   timing sheet fi
+00032ba0: 6c65 732e 0a0a 2020 2020 2020 2020 2727  les...        ''
+00032bb0: 270a 2020 2020 2020 2020 7365 6c66 2e5f  '.        self._
+00032bc0: 6361 6c6c 5f6d 6574 686f 645f 7769 7468  call_method_with
+00032bd0: 5f69 7465 7261 626c 6528 7365 6c66 2e5f  _iterable(self._
+00032be0: 6c6f 6164 5f73 7065 6369 6669 6361 7469  load_specificati
+00032bf0: 6f6e 732c 2073 7065 6369 6669 6361 7469  ons, specificati
+00032c00: 6f6e 735f 6669 6c65 5f70 6174 6873 290a  ons_file_paths).
+00032c10: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
+00032c20: 6c6c 5f6d 6574 686f 645f 7769 7468 5f69  ll_method_with_i
+00032c30: 7465 7261 626c 6528 7365 6c66 2e5f 6c6f  terable(self._lo
+00032c40: 6164 5f6c 6576 656c 732c 206c 6576 656c  ad_levels, level
+00032c50: 735f 6669 6c65 5f70 6174 6873 290a 2020  s_file_paths).  
+00032c60: 2020 2020 2020 7365 6c66 2e5f 6361 6c6c        self._call
+00032c70: 5f6d 6574 686f 645f 7769 7468 5f69 7465  _method_with_ite
+00032c80: 7261 626c 6528 7365 6c66 2e5f 6c6f 6164  rable(self._load
+00032c90: 5f74 696d 696e 672c 2074 696d 696e 675f  _timing, timing_
+00032ca0: 6669 6c65 5f70 6174 6873 290a 0a20 2020  file_paths)..   
+00032cb0: 2064 6566 205f 6361 6c6c 5f6d 6574 686f   def _call_metho
+00032cc0: 645f 7769 7468 5f69 7465 7261 626c 6528  d_with_iterable(
+00032cd0: 7365 6c66 2c20 6d65 7468 6f64 2c20 6669  self, method, fi
+00032ce0: 6c65 7329 3a0a 2020 2020 2020 2020 6966  les):.        if
+00032cf0: 2066 696c 6573 2069 7320 4e6f 6e65 3a0a   files is None:.
+00032d00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00032d10: 726e 0a20 2020 2020 2020 2069 6620 6973  rn.        if is
+00032d20: 696e 7374 616e 6365 2866 696c 6573 2c20  instance(files, 
+00032d30: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+00032d40: 2020 6669 6c65 7320 3d20 5b66 696c 6573    files = [files
+00032d50: 5d0a 2020 2020 2020 2020 666f 7220 6620  ].        for f 
+00032d60: 696e 2066 696c 6573 3a0a 2020 2020 2020  in files:.      
+00032d70: 2020 2020 2020 6d65 7468 6f64 2866 290a        method(f).
+00032d80: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
+00032d90: 6f6e 697a 6564 0a20 2020 2064 6566 2073  onized.    def s
+00032da0: 656c 665f 7465 7374 2873 656c 6629 3a0a  elf_test(self):.
+00032db0: 2020 2020 2020 2020 2727 2773 656c 665f          '''self_
+00032dc0: 7465 7374 0a0a 2020 2020 2020 2020 5265  test..        Re
+00032dd0: 7475 726e 7320 7365 6c66 2074 6573 7420  turns self test 
+00032de0: 7265 7375 6c74 7320 6672 6f6d 2061 2064  results from a d
+00032df0: 6967 6974 616c 2070 6174 7465 726e 2069  igital pattern i
+00032e00: 6e73 7472 756d 656e 742e 2054 6869 7320  nstrument. This 
+00032e10: 7465 7374 2072 6571 7569 7265 7320 7365  test requires se
+00032e20: 7665 7261 6c20 6d69 6e75 7465 7320 746f  veral minutes to
+00032e30: 2065 7865 6375 7465 2e0a 0a20 2020 2020   execute...     
+00032e40: 2020 2052 6169 7365 7320 6053 656c 6654     Raises `SelfT
+00032e50: 6573 7445 7272 6f72 6020 6f6e 2073 656c  estError` on sel
+00032e60: 6620 7465 7374 2066 6169 6c75 7265 2e20  f test failure. 
+00032e70: 5072 6f70 6572 7469 6573 206f 6e20 6578  Properties on ex
+00032e80: 6365 7074 696f 6e20 6f62 6a65 6374 3a0a  ception object:.
+00032e90: 0a20 2020 2020 2020 202d 2063 6f64 6520  .        - code 
+00032ea0: 2d20 6661 696c 7572 6520 636f 6465 2066  - failure code f
+00032eb0: 726f 6d20 6472 6976 6572 0a20 2020 2020  rom driver.     
+00032ec0: 2020 202d 206d 6573 7361 6765 202d 2073     - message - s
+00032ed0: 7461 7475 7320 6d65 7373 6167 6520 6672  tatus message fr
+00032ee0: 6f6d 2064 7269 7665 720a 0a20 2020 2020  om driver..     
+00032ef0: 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     +------------
+00032f00: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00032f10: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+00032f20: 2020 7c20 5365 6c66 2d54 6573 7420 436f    | Self-Test Co
+00032f30: 6465 207c 2044 6573 6372 6970 7469 6f6e  de | Description
+00032f40: 2020 2020 2020 207c 0a20 2020 2020 2020         |.       
+00032f50: 202b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   +==============
+00032f60: 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==+=============
+00032f70: 3d3d 3d3d 3d3d 2b0a 2020 2020 2020 2020  ======+.        
+00032f80: 7c20 3020 2020 2020 2020 2020 2020 2020  | 0             
+00032f90: 207c 2053 656c 6620 7465 7374 2070 6173   | Self test pas
+00032fa0: 7365 642e 207c 0a20 2020 2020 2020 202b  sed. |.        +
+00032fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00032fc0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00032fd0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 7c20  ----+.        | 
+00032fe0: 3120 2020 2020 2020 2020 2020 2020 207c  1              |
+00032ff0: 2053 656c 6620 7465 7374 2066 6169 6c65   Self test faile
+00033000: 642e 207c 0a20 2020 2020 2020 202b 2d2d  d. |.        +--
+00033010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
 00033020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00033030: 2d2d 2d2b 0a20 2020 2020 2020 2027 2727  ---+.        '''
-00033040: 0a20 2020 2020 2020 2063 6f64 652c 206d  .        code, m
-00033050: 7367 203d 2073 656c 662e 5f73 656c 665f  sg = self._self_
-00033060: 7465 7374 2829 0a20 2020 2020 2020 2069  test().        i
-00033070: 6620 636f 6465 3a0a 2020 2020 2020 2020  f code:.        
-00033080: 2020 2020 7261 6973 6520 6572 726f 7273      raise errors
-00033090: 2e53 656c 6654 6573 7445 7272 6f72 2863  .SelfTestError(c
-000330a0: 6f64 652c 206d 7367 290a 2020 2020 2020  ode, msg).      
-000330b0: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-000330c0: 2020 2040 6976 695f 7379 6e63 6872 6f6e     @ivi_synchron
-000330d0: 697a 6564 0a20 2020 2064 6566 2075 6e6c  ized.    def unl
-000330e0: 6f61 645f 7370 6563 6966 6963 6174 696f  oad_specificatio
-000330f0: 6e73 2873 656c 662c 2066 696c 655f 7061  ns(self, file_pa
-00033100: 7468 7329 3a0a 2020 2020 2020 2020 2727  ths):.        ''
-00033110: 2775 6e6c 6f61 645f 7370 6563 6966 6963  'unload_specific
-00033120: 6174 696f 6e73 0a0a 2020 2020 2020 2020  ations..        
-00033130: 556e 6c6f 6164 7320 7468 6520 6769 7665  Unloads the give
-00033140: 6e20 7370 6563 6966 6963 6174 696f 6e73  n specifications
-00033150: 2073 6865 6574 7320 7072 6573 656e 7420   sheets present 
-00033160: 696e 2074 6865 2070 7265 7669 6f75 736c  in the previousl
-00033170: 7920 6c6f 6164 6564 0a20 2020 2020 2020  y loaded.       
-00033180: 2073 7065 6369 6669 6361 7469 6f6e 7320   specifications 
-00033190: 6669 6c65 7320 7468 6174 2079 6f75 2073  files that you s
-000331a0: 656c 6563 742e 0a0a 2020 2020 2020 2020  elect...        
-000331b0: 596f 7520 6d75 7374 2063 616c 6c20 6c6f  You must call lo
-000331c0: 6164 5f73 7065 6369 6669 6361 7469 6f6e  ad_specification
-000331d0: 735f 6c65 7665 6c73 5f61 6e64 5f74 696d  s_levels_and_tim
-000331e0: 696e 6720 746f 2072 656c 6f61 6420 7468  ing to reload th
-000331f0: 6520 6669 6c65 7320 7769 7468 2075 7064  e files with upd
-00033200: 6174 6564 0a20 2020 2020 2020 2073 7065  ated.        spe
-00033210: 6369 6669 6361 7469 6f6e 7320 7661 6c75  cifications valu
-00033220: 6573 2e20 596f 7520 6d75 7374 2074 6865  es. You must the
-00033230: 6e20 6361 6c6c 2061 7070 6c79 5f6c 6576  n call apply_lev
-00033240: 656c 735f 616e 645f 7469 6d69 6e67 2069  els_and_timing i
-00033250: 6e20 6f72 6465 7220 746f 2061 7070 6c79  n order to apply
-00033260: 0a20 2020 2020 2020 2074 6865 206c 6576  .        the lev
-00033270: 656c 7320 616e 6420 7469 6d69 6e67 2076  els and timing v
-00033280: 616c 7565 7320 7468 6174 2072 6566 6572  alues that refer
-00033290: 656e 6365 2074 6865 2075 7064 6174 6564  ence the updated
-000332a0: 2073 7065 6369 6669 6361 7469 6f6e 7320   specifications 
-000332b0: 7661 6c75 6573 2e0a 0a20 2020 2020 2020  values...       
-000332c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-000332d0: 2020 2066 696c 655f 7061 7468 7320 2873     file_paths (s
-000332e0: 7472 206f 7220 6261 7369 6320 7365 7175  tr or basic sequ
-000332f0: 656e 6365 206f 6620 7374 7229 3a20 4162  ence of str): Ab
-00033300: 736f 6c75 7465 2066 696c 6520 7061 7468  solute file path
-00033310: 206f 6620 6f6e 6520 6f72 206d 6f72 6520   of one or more 
-00033320: 6c6f 6164 6564 2073 7065 6369 6669 6361  loaded specifica
-00033330: 7469 6f6e 7320 6669 6c65 732e 0a0a 2020  tions files...  
-00033340: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00033350: 2020 7365 6c66 2e5f 6361 6c6c 5f6d 6574    self._call_met
-00033360: 686f 645f 7769 7468 5f69 7465 7261 626c  hod_with_iterabl
-00033370: 6528 7365 6c66 2e5f 756e 6c6f 6164 5f73  e(self._unload_s
-00033380: 7065 6369 6669 6361 7469 6f6e 732c 2066  pecifications, f
-00033390: 696c 655f 7061 7468 7329 0a0a 2020 2020  ile_paths)..    
-000333a0: 4069 7669 5f73 796e 6368 726f 6e69 7a65  @ivi_synchronize
-000333b0: 640a 2020 2020 6465 6620 7772 6974 655f  d.    def write_
-000333c0: 736f 7572 6365 5f77 6176 6566 6f72 6d5f  source_waveform_
-000333d0: 7369 7465 5f75 6e69 7175 6528 7365 6c66  site_unique(self
-000333e0: 2c20 7761 7665 666f 726d 5f6e 616d 652c  , waveform_name,
-000333f0: 2077 6176 6566 6f72 6d5f 6461 7461 293a   waveform_data):
-00033400: 0a20 2020 2020 2020 2027 2727 7772 6974  .        '''writ
-00033410: 655f 736f 7572 6365 5f77 6176 6566 6f72  e_source_wavefor
-00033420: 6d5f 7369 7465 5f75 6e69 7175 650a 0a20  m_site_unique.. 
-00033430: 2020 2020 2020 2057 7269 7465 7320 6f6e         Writes on
-00033440: 6520 7761 7665 666f 726d 2070 6572 2073  e waveform per s
-00033450: 6974 652e 2055 7365 2074 6869 7320 7772  ite. Use this wr
-00033460: 6974 6520 6d65 7468 6f64 2069 6620 796f  ite method if yo
-00033470: 7520 7365 7420 7468 6520 7061 7261 6d65  u set the parame
-00033480: 7465 7220 6f66 2074 6865 2063 7265 6174  ter of the creat
-00033490: 6520 736f 7572 6365 2077 6176 6566 6f72  e source wavefor
-000334a0: 6d20 6d65 7468 6f64 2074 6f20 5369 7465  m method to Site
-000334b0: 2055 6e69 7175 652e 0a0a 2020 2020 2020   Unique...      
-000334c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000334d0: 2020 2020 7761 7665 666f 726d 5f6e 616d      waveform_nam
-000334e0: 6520 2873 7472 293a 2054 6865 206e 616d  e (str): The nam
-000334f0: 6520 746f 2061 7373 6967 6e20 746f 2074  e to assign to t
-00033500: 6865 2077 6176 6566 6f72 6d2e 2055 7365  he waveform. Use
-00033510: 2074 6865 2077 6176 6566 6f72 6d5f 6e61   the waveform_na
-00033520: 6d65 2077 6974 6820 736f 7572 6365 5f73  me with source_s
-00033530: 7461 7274 206f 7063 6f64 6520 696e 2079  tart opcode in y
-00033540: 6f75 7220 7061 7474 6572 6e2e 0a0a 2020  our pattern...  
-00033550: 2020 2020 2020 2020 2020 7761 7665 666f            wavefo
-00033560: 726d 5f64 6174 6120 287b 2069 6e74 3a20  rm_data ({ int: 
-00033570: 6261 7369 6320 7365 7175 656e 6365 206f  basic sequence o
-00033580: 6620 756e 7369 676e 6564 2069 6e74 2c20  f unsigned int, 
-00033590: 696e 743a 2062 6173 6963 2073 6571 7565  int: basic seque
-000335a0: 6e63 6520 6f66 2075 6e73 6967 6e65 6420  nce of unsigned 
-000335b0: 696e 742c 202e 2e2e 207d 293a 2044 6963  int, ... }): Dic
-000335c0: 7469 6f6e 6172 7920 7768 6572 6520 6561  tionary where ea
-000335d0: 6368 206b 6579 2069 7320 6120 7369 7465  ch key is a site
-000335e0: 206e 756d 6265 7220 616e 6420 7661 6c75   number and valu
-000335f0: 6520 6973 2061 2063 6f6c 6c65 6374 696f  e is a collectio
-00033600: 6e20 6f66 2073 616d 706c 6573 2074 6f20  n of samples to 
-00033610: 7573 6520 6173 2073 6f75 7263 6520 6461  use as source da
-00033620: 7461 0a0a 2020 2020 2020 2020 2727 270a  ta..        '''.
-00033630: 2020 2020 2020 2020 6672 6f6d 2063 6f6c          from col
-00033640: 6c65 6374 696f 6e73 2e61 6263 2069 6d70  lections.abc imp
-00033650: 6f72 7420 4d61 7070 696e 670a 2020 2020  ort Mapping.    
-00033660: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-00033670: 7461 6e63 6528 7761 7665 666f 726d 5f64  tance(waveform_d
-00033680: 6174 612c 204d 6170 7069 6e67 293a 0a20  ata, Mapping):. 
-00033690: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000336a0: 2054 7970 6545 7272 6f72 2822 4578 7065   TypeError("Expe
-000336b0: 6374 696e 6720 7761 7665 666f 726d 5f64  cting waveform_d
-000336c0: 6174 6120 746f 2062 6520 6120 6469 6374  ata to be a dict
-000336d0: 696f 6e61 7279 2062 7574 2067 6f74 207b  ionary but got {
-000336e0: 7d22 2e66 6f72 6d61 7428 7479 7065 2877  }".format(type(w
-000336f0: 6176 6566 6f72 6d5f 6461 7461 2929 290a  aveform_data))).
-00033700: 2020 2020 2020 2020 7369 7465 5f6c 6973          site_lis
-00033710: 7420 3d20 5b5d 0a20 2020 2020 2020 2023  t = [].        #
-00033720: 2057 6520 6173 7375 6d65 2061 6c6c 2074   We assume all t
-00033730: 6865 2065 6e74 7269 6573 2061 7265 2074  he entries are t
-00033740: 6865 2073 616d 6520 6c65 6e67 7468 2028  he same length (
-00033750: 7765 276c 6c20 6368 6563 6b20 6c61 7465  we'll check late
-00033760: 7229 2074 6f20 6d61 6b65 2074 6865 2061  r) to make the a
-00033770: 7272 6179 2074 6865 2063 6f72 7265 6374  rray the correct
-00033780: 2073 697a 650a 2020 2020 2020 2020 2320   size.        # 
-00033790: 4765 7420 616e 2065 6e74 7279 2066 726f  Get an entry fro
-000337a0: 6d20 7468 6520 6469 6374 696f 6e61 7279  m the dictionary
-000337b0: 2066 726f 6d20 6874 7470 733a 2f2f 7374   from https://st
-000337c0: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
-000337d0: 7175 6573 7469 6f6e 732f 3330 3336 3233  questions/303623
-000337e0: 3931 2f68 6f77 2d64 6f2d 796f 752d 6669  91/how-do-you-fi
-000337f0: 6e64 2d74 6865 2d66 6972 7374 2d6b 6579  nd-the-first-key
-00033800: 2d69 6e2d 612d 6469 6374 696f 6e61 7279  -in-a-dictionary
-00033810: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00033820: 7761 7665 666f 726d 5f64 6174 6129 203d  waveform_data) =
-00033830: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00033840: 2061 6374 7561 6c5f 7361 6d70 6c65 735f   actual_samples_
-00033850: 7065 725f 7761 7665 666f 726d 203d 2030  per_waveform = 0
-00033860: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00033870: 2020 2020 2020 2020 2020 2061 6374 7561             actua
-00033880: 6c5f 7361 6d70 6c65 735f 7065 725f 7761  l_samples_per_wa
-00033890: 7665 666f 726d 203d 206c 656e 2877 6176  veform = len(wav
-000338a0: 6566 6f72 6d5f 6461 7461 5b6e 6578 7428  eform_data[next(
-000338b0: 6974 6572 2877 6176 6566 6f72 6d5f 6461  iter(waveform_da
-000338c0: 7461 2929 5d29 0a20 2020 2020 2020 2064  ta))]).        d
-000338d0: 6174 6120 3d20 6172 7261 792e 6172 7261  ata = array.arra
-000338e0: 7928 274c 272c 205b 305d 202a 2028 6c65  y('L', [0] * (le
-000338f0: 6e28 7761 7665 666f 726d 5f64 6174 6129  n(waveform_data)
-00033900: 202a 2061 6374 7561 6c5f 7361 6d70 6c65   * actual_sample
-00033910: 735f 7065 725f 7761 7665 666f 726d 2929  s_per_waveform))
-00033920: 0a20 2020 2020 2020 206d 7620 3d20 6d65  .        mv = me
-00033930: 6d6f 7279 7669 6577 2864 6174 6129 0a0a  moryview(data)..
-00033940: 2020 2020 2020 2020 6920 3d20 300a 2020          i = 0.  
-00033950: 2020 2020 2020 666f 7220 7369 7465 2069        for site i
-00033960: 6e20 7761 7665 666f 726d 5f64 6174 613a  n waveform_data:
-00033970: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00033980: 6c65 6e28 7761 7665 666f 726d 5f64 6174  len(waveform_dat
-00033990: 615b 7369 7465 5d29 2021 3d20 6163 7475  a[site]) != actu
-000339a0: 616c 5f73 616d 706c 6573 5f70 6572 5f77  al_samples_per_w
-000339b0: 6176 6566 6f72 6d3a 0a20 2020 2020 2020  aveform:.       
-000339c0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-000339d0: 616c 7565 4572 726f 7228 274d 6973 6d61  alueError('Misma
-000339e0: 7463 6865 6420 6c65 6e67 7468 206f 6620  tched length of 
-000339f0: 7761 7665 666f 726d 732e 2041 6c6c 206d  waveforms. All m
-00033a00: 7573 7420 6265 2074 6865 2073 616d 6520  ust be the same 
-00033a10: 6c65 6e67 7468 2e27 290a 2020 2020 2020  length.').      
-00033a20: 2020 2020 2020 2320 4368 6563 6b20 7468        # Check th
-00033a30: 6520 7479 7065 2062 7920 7573 696e 6720  e type by using 
-00033a40: 7374 7269 6e67 2063 6f6d 7061 7269 736f  string compariso
-00033a50: 6e20 736f 2074 6861 7420 7765 2064 6f6e  n so that we don
-00033a60: 2774 2069 6d70 6f72 7420 6e75 6d70 7920  't import numpy 
-00033a70: 756e 6e65 6365 7373 6172 696c 792e 0a20  unnecessarily.. 
-00033a80: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-00033a90: 7228 7479 7065 2877 6176 6566 6f72 6d5f  r(type(waveform_
-00033aa0: 6461 7461 5b73 6974 655d 2929 2e66 696e  data[site])).fin
-00033ab0: 6428 2227 6e75 6d70 792e 6e64 6172 7261  d("'numpy.ndarra
-00033ac0: 7927 2229 2021 3d20 2d31 3a0a 2020 2020  y'") != -1:.    
-00033ad0: 2020 2020 2020 2020 2020 2020 696d 706f              impo
-00033ae0: 7274 206e 756d 7079 0a20 2020 2020 2020  rt numpy.       
-00033af0: 2020 2020 2020 2020 2069 6620 7761 7665           if wave
-00033b00: 666f 726d 5f64 6174 615b 7369 7465 5d2e  form_data[site].
-00033b10: 6474 7970 6520 3d3d 206e 756d 7079 2e75  dtype == numpy.u
-00033b20: 696e 7433 323a 0a20 2020 2020 2020 2020  int32:.         
-00033b30: 2020 2020 2020 2020 2020 2077 666d 203d             wfm =
-00033b40: 2061 7272 6179 2e61 7272 6179 2827 4c27   array.array('L'
-00033b50: 2c20 7761 7665 666f 726d 5f64 6174 615b  , waveform_data[
-00033b60: 7369 7465 5d29 0a20 2020 2020 2020 2020  site]).         
-00033b70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00033030: 2d2d 2b0a 2020 2020 2020 2020 2727 270a  --+.        '''.
+00033040: 2020 2020 2020 2020 636f 6465 2c20 6d73          code, ms
+00033050: 6720 3d20 7365 6c66 2e5f 7365 6c66 5f74  g = self._self_t
+00033060: 6573 7428 290a 2020 2020 2020 2020 6966  est().        if
+00033070: 2063 6f64 653a 0a20 2020 2020 2020 2020   code:.         
+00033080: 2020 2072 6169 7365 2065 7272 6f72 732e     raise errors.
+00033090: 5365 6c66 5465 7374 4572 726f 7228 636f  SelfTestError(co
+000330a0: 6465 2c20 6d73 6729 0a20 2020 2020 2020  de, msg).       
+000330b0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+000330c0: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
+000330d0: 7a65 640a 2020 2020 6465 6620 756e 6c6f  zed.    def unlo
+000330e0: 6164 5f73 7065 6369 6669 6361 7469 6f6e  ad_specification
+000330f0: 7328 7365 6c66 2c20 6669 6c65 5f70 6174  s(self, file_pat
+00033100: 6873 293a 0a20 2020 2020 2020 2027 2727  hs):.        '''
+00033110: 756e 6c6f 6164 5f73 7065 6369 6669 6361  unload_specifica
+00033120: 7469 6f6e 730a 0a20 2020 2020 2020 2055  tions..        U
+00033130: 6e6c 6f61 6473 2074 6865 2067 6976 656e  nloads the given
+00033140: 2073 7065 6369 6669 6361 7469 6f6e 7320   specifications 
+00033150: 7368 6565 7473 2070 7265 7365 6e74 2069  sheets present i
+00033160: 6e20 7468 6520 7072 6576 696f 7573 6c79  n the previously
+00033170: 206c 6f61 6465 640a 2020 2020 2020 2020   loaded.        
+00033180: 7370 6563 6966 6963 6174 696f 6e73 2066  specifications f
+00033190: 696c 6573 2074 6861 7420 796f 7520 7365  iles that you se
+000331a0: 6c65 6374 2e0a 0a20 2020 2020 2020 2059  lect...        Y
+000331b0: 6f75 206d 7573 7420 6361 6c6c 206c 6f61  ou must call loa
+000331c0: 645f 7370 6563 6966 6963 6174 696f 6e73  d_specifications
+000331d0: 5f6c 6576 656c 735f 616e 645f 7469 6d69  _levels_and_timi
+000331e0: 6e67 2074 6f20 7265 6c6f 6164 2074 6865  ng to reload the
+000331f0: 2066 696c 6573 2077 6974 6820 7570 6461   files with upda
+00033200: 7465 640a 2020 2020 2020 2020 7370 6563  ted.        spec
+00033210: 6966 6963 6174 696f 6e73 2076 616c 7565  ifications value
+00033220: 732e 2059 6f75 206d 7573 7420 7468 656e  s. You must then
+00033230: 2063 616c 6c20 6170 706c 795f 6c65 7665   call apply_leve
+00033240: 6c73 5f61 6e64 5f74 696d 696e 6720 696e  ls_and_timing in
+00033250: 206f 7264 6572 2074 6f20 6170 706c 790a   order to apply.
+00033260: 2020 2020 2020 2020 7468 6520 6c65 7665          the leve
+00033270: 6c73 2061 6e64 2074 696d 696e 6720 7661  ls and timing va
+00033280: 6c75 6573 2074 6861 7420 7265 6665 7265  lues that refere
+00033290: 6e63 6520 7468 6520 7570 6461 7465 6420  nce the updated 
+000332a0: 7370 6563 6966 6963 6174 696f 6e73 2076  specifications v
+000332b0: 616c 7565 732e 0a0a 2020 2020 2020 2020  alues...        
+000332c0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+000332d0: 2020 6669 6c65 5f70 6174 6873 2028 7374    file_paths (st
+000332e0: 7220 6f72 2062 6173 6963 2073 6571 7565  r or basic seque
+000332f0: 6e63 6520 6f66 2073 7472 293a 2041 6273  nce of str): Abs
+00033300: 6f6c 7574 6520 6669 6c65 2070 6174 6820  olute file path 
+00033310: 6f66 206f 6e65 206f 7220 6d6f 7265 206c  of one or more l
+00033320: 6f61 6465 6420 7370 6563 6966 6963 6174  oaded specificat
+00033330: 696f 6e73 2066 696c 6573 2e0a 0a20 2020  ions files...   
+00033340: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00033350: 2073 656c 662e 5f63 616c 6c5f 6d65 7468   self._call_meth
+00033360: 6f64 5f77 6974 685f 6974 6572 6162 6c65  od_with_iterable
+00033370: 2873 656c 662e 5f75 6e6c 6f61 645f 7370  (self._unload_sp
+00033380: 6563 6966 6963 6174 696f 6e73 2c20 6669  ecifications, fi
+00033390: 6c65 5f70 6174 6873 290a 0a20 2020 2040  le_paths)..    @
+000333a0: 6976 695f 7379 6e63 6872 6f6e 697a 6564  ivi_synchronized
+000333b0: 0a20 2020 2064 6566 2077 7269 7465 5f73  .    def write_s
+000333c0: 6f75 7263 655f 7761 7665 666f 726d 5f73  ource_waveform_s
+000333d0: 6974 655f 756e 6971 7565 2873 656c 662c  ite_unique(self,
+000333e0: 2077 6176 6566 6f72 6d5f 6e61 6d65 2c20   waveform_name, 
+000333f0: 7761 7665 666f 726d 5f64 6174 6129 3a0a  waveform_data):.
+00033400: 2020 2020 2020 2020 2727 2777 7269 7465          '''write
+00033410: 5f73 6f75 7263 655f 7761 7665 666f 726d  _source_waveform
+00033420: 5f73 6974 655f 756e 6971 7565 0a0a 2020  _site_unique..  
+00033430: 2020 2020 2020 5772 6974 6573 206f 6e65        Writes one
+00033440: 2077 6176 6566 6f72 6d20 7065 7220 7369   waveform per si
+00033450: 7465 2e20 5573 6520 7468 6973 2077 7269  te. Use this wri
+00033460: 7465 206d 6574 686f 6420 6966 2079 6f75  te method if you
+00033470: 2073 6574 2074 6865 2070 6172 616d 6574   set the paramet
+00033480: 6572 206f 6620 7468 6520 6372 6561 7465  er of the create
+00033490: 2073 6f75 7263 6520 7761 7665 666f 726d   source waveform
+000334a0: 206d 6574 686f 6420 746f 2053 6974 6520   method to Site 
+000334b0: 556e 6971 7565 2e0a 0a20 2020 2020 2020  Unique...       
+000334c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+000334d0: 2020 2077 6176 6566 6f72 6d5f 6e61 6d65     waveform_name
+000334e0: 2028 7374 7229 3a20 5468 6520 6e61 6d65   (str): The name
+000334f0: 2074 6f20 6173 7369 676e 2074 6f20 7468   to assign to th
+00033500: 6520 7761 7665 666f 726d 2e20 5573 6520  e waveform. Use 
+00033510: 7468 6520 7761 7665 666f 726d 5f6e 616d  the waveform_nam
+00033520: 6520 7769 7468 2073 6f75 7263 655f 7374  e with source_st
+00033530: 6172 7420 6f70 636f 6465 2069 6e20 796f  art opcode in yo
+00033540: 7572 2070 6174 7465 726e 2e0a 0a20 2020  ur pattern...   
+00033550: 2020 2020 2020 2020 2077 6176 6566 6f72           wavefor
+00033560: 6d5f 6461 7461 2028 7b20 696e 743a 2062  m_data ({ int: b
+00033570: 6173 6963 2073 6571 7565 6e63 6520 6f66  asic sequence of
+00033580: 2075 6e73 6967 6e65 6420 696e 742c 2069   unsigned int, i
+00033590: 6e74 3a20 6261 7369 6320 7365 7175 656e  nt: basic sequen
+000335a0: 6365 206f 6620 756e 7369 676e 6564 2069  ce of unsigned i
+000335b0: 6e74 2c20 2e2e 2e20 7d29 3a20 4469 6374  nt, ... }): Dict
+000335c0: 696f 6e61 7279 2077 6865 7265 2065 6163  ionary where eac
+000335d0: 6820 6b65 7920 6973 2061 2073 6974 6520  h key is a site 
+000335e0: 6e75 6d62 6572 2061 6e64 2076 616c 7565  number and value
+000335f0: 2069 7320 6120 636f 6c6c 6563 7469 6f6e   is a collection
+00033600: 206f 6620 7361 6d70 6c65 7320 746f 2075   of samples to u
+00033610: 7365 2061 7320 736f 7572 6365 2064 6174  se as source dat
+00033620: 610a 0a20 2020 2020 2020 2027 2727 0a20  a..        '''. 
+00033630: 2020 2020 2020 2066 726f 6d20 636f 6c6c         from coll
+00033640: 6563 7469 6f6e 732e 6162 6320 696d 706f  ections.abc impo
+00033650: 7274 204d 6170 7069 6e67 0a20 2020 2020  rt Mapping.     
+00033660: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+00033670: 616e 6365 2877 6176 6566 6f72 6d5f 6461  ance(waveform_da
+00033680: 7461 2c20 4d61 7070 696e 6729 3a0a 2020  ta, Mapping):.  
+00033690: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000336a0: 5479 7065 4572 726f 7228 2245 7870 6563  TypeError("Expec
+000336b0: 7469 6e67 2077 6176 6566 6f72 6d5f 6461  ting waveform_da
+000336c0: 7461 2074 6f20 6265 2061 2064 6963 7469  ta to be a dicti
+000336d0: 6f6e 6172 7920 6275 7420 676f 7420 7b7d  onary but got {}
+000336e0: 222e 666f 726d 6174 2874 7970 6528 7761  ".format(type(wa
+000336f0: 7665 666f 726d 5f64 6174 6129 2929 0a20  veform_data))). 
+00033700: 2020 2020 2020 2073 6974 655f 6c69 7374         site_list
+00033710: 203d 205b 5d0a 2020 2020 2020 2020 2320   = [].        # 
+00033720: 5765 2061 7373 756d 6520 616c 6c20 7468  We assume all th
+00033730: 6520 656e 7472 6965 7320 6172 6520 7468  e entries are th
+00033740: 6520 7361 6d65 206c 656e 6774 6820 2877  e same length (w
+00033750: 6527 6c6c 2063 6865 636b 206c 6174 6572  e'll check later
+00033760: 2920 746f 206d 616b 6520 7468 6520 6172  ) to make the ar
+00033770: 7261 7920 7468 6520 636f 7272 6563 7420  ray the correct 
+00033780: 7369 7a65 0a20 2020 2020 2020 2023 2047  size.        # G
+00033790: 6574 2061 6e20 656e 7472 7920 6672 6f6d  et an entry from
+000337a0: 2074 6865 2064 6963 7469 6f6e 6172 7920   the dictionary 
+000337b0: 6672 6f6d 2068 7474 7073 3a2f 2f73 7461  from https://sta
+000337c0: 636b 6f76 6572 666c 6f77 2e63 6f6d 2f71  ckoverflow.com/q
+000337d0: 7565 7374 696f 6e73 2f33 3033 3632 3339  uestions/3036239
+000337e0: 312f 686f 772d 646f 2d79 6f75 2d66 696e  1/how-do-you-fin
+000337f0: 642d 7468 652d 6669 7273 742d 6b65 792d  d-the-first-key-
+00033800: 696e 2d61 2d64 6963 7469 6f6e 6172 790a  in-a-dictionary.
+00033810: 2020 2020 2020 2020 6966 206c 656e 2877          if len(w
+00033820: 6176 6566 6f72 6d5f 6461 7461 2920 3d3d  aveform_data) ==
+00033830: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00033840: 6163 7475 616c 5f73 616d 706c 6573 5f70  actual_samples_p
+00033850: 6572 5f77 6176 6566 6f72 6d20 3d20 300a  er_waveform = 0.
+00033860: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00033870: 2020 2020 2020 2020 2020 6163 7475 616c            actual
+00033880: 5f73 616d 706c 6573 5f70 6572 5f77 6176  _samples_per_wav
+00033890: 6566 6f72 6d20 3d20 6c65 6e28 7761 7665  eform = len(wave
+000338a0: 666f 726d 5f64 6174 615b 6e65 7874 2869  form_data[next(i
+000338b0: 7465 7228 7761 7665 666f 726d 5f64 6174  ter(waveform_dat
+000338c0: 6129 295d 290a 2020 2020 2020 2020 6461  a))]).        da
+000338d0: 7461 203d 2061 7272 6179 2e61 7272 6179  ta = array.array
+000338e0: 2827 4c27 2c20 5b30 5d20 2a20 286c 656e  ('L', [0] * (len
+000338f0: 2877 6176 6566 6f72 6d5f 6461 7461 2920  (waveform_data) 
+00033900: 2a20 6163 7475 616c 5f73 616d 706c 6573  * actual_samples
+00033910: 5f70 6572 5f77 6176 6566 6f72 6d29 290a  _per_waveform)).
+00033920: 2020 2020 2020 2020 6d76 203d 206d 656d          mv = mem
+00033930: 6f72 7976 6965 7728 6461 7461 290a 0a20  oryview(data).. 
+00033940: 2020 2020 2020 2069 203d 2030 0a20 2020         i = 0.   
+00033950: 2020 2020 2066 6f72 2073 6974 6520 696e       for site in
+00033960: 2077 6176 6566 6f72 6d5f 6461 7461 3a0a   waveform_data:.
+00033970: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00033980: 656e 2877 6176 6566 6f72 6d5f 6461 7461  en(waveform_data
+00033990: 5b73 6974 655d 2920 213d 2061 6374 7561  [site]) != actua
+000339a0: 6c5f 7361 6d70 6c65 735f 7065 725f 7761  l_samples_per_wa
+000339b0: 7665 666f 726d 3a0a 2020 2020 2020 2020  veform:.        
+000339c0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+000339d0: 6c75 6545 7272 6f72 2827 4d69 736d 6174  lueError('Mismat
+000339e0: 6368 6564 206c 656e 6774 6820 6f66 2077  ched length of w
+000339f0: 6176 6566 6f72 6d73 2e20 416c 6c20 6d75  aveforms. All mu
+00033a00: 7374 2062 6520 7468 6520 7361 6d65 206c  st be the same l
+00033a10: 656e 6774 682e 2729 0a20 2020 2020 2020  ength.').       
+00033a20: 2020 2020 2023 2043 6865 636b 2074 6865       # Check the
+00033a30: 2074 7970 6520 6279 2075 7369 6e67 2073   type by using s
+00033a40: 7472 696e 6720 636f 6d70 6172 6973 6f6e  tring comparison
+00033a50: 2073 6f20 7468 6174 2077 6520 646f 6e27   so that we don'
+00033a60: 7420 696d 706f 7274 206e 756d 7079 2075  t import numpy u
+00033a70: 6e6e 6563 6573 7361 7269 6c79 2e0a 2020  nnecessarily..  
+00033a80: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+00033a90: 2874 7970 6528 7761 7665 666f 726d 5f64  (type(waveform_d
+00033aa0: 6174 615b 7369 7465 5d29 292e 6669 6e64  ata[site])).find
+00033ab0: 2822 276e 756d 7079 2e6e 6461 7272 6179  ("'numpy.ndarray
+00033ac0: 2722 2920 213d 202d 313a 0a20 2020 2020  '") != -1:.     
+00033ad0: 2020 2020 2020 2020 2020 2069 6d70 6f72             impor
+00033ae0: 7420 6e75 6d70 790a 2020 2020 2020 2020  t numpy.        
+00033af0: 2020 2020 2020 2020 6966 2077 6176 6566          if wavef
+00033b00: 6f72 6d5f 6461 7461 5b73 6974 655d 2e64  orm_data[site].d
+00033b10: 7479 7065 203d 3d20 6e75 6d70 792e 7569  type == numpy.ui
+00033b20: 6e74 3332 3a0a 2020 2020 2020 2020 2020  nt32:.          
+00033b30: 2020 2020 2020 2020 2020 7766 6d20 3d20            wfm = 
+00033b40: 6172 7261 792e 6172 7261 7928 274c 272c  array.array('L',
+00033b50: 2077 6176 6566 6f72 6d5f 6461 7461 5b73   waveform_data[s
+00033b60: 6974 655d 290a 2020 2020 2020 2020 2020  ite]).          
+00033b70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 00033b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033b90: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-00033ba0: 2822 556e 7375 7070 6f72 7465 6420 6474  ("Unsupported dt
-00033bb0: 7970 6520 666f 7220 7761 7665 666f 726d  ype for waveform
-00033bc0: 5f64 6174 6120 6172 7261 7920 656c 656d  _data array elem
-00033bd0: 656e 7420 7479 7065 2e20 4973 207b 307d  ent type. Is {0}
-00033be0: 2c20 6578 7065 6374 6564 207b 317d 222e  , expected {1}".
-00033bf0: 666f 726d 6174 2877 6176 6566 6f72 6d5f  format(waveform_
-00033c00: 6461 7461 5b73 6974 655d 2e64 7479 7065  data[site].dtype
-00033c10: 2c20 6e75 6d70 792e 696e 7433 3229 290a  , numpy.int32)).
-00033c20: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00033c30: 6620 6973 696e 7374 616e 6365 2877 6176  f isinstance(wav
-00033c40: 6566 6f72 6d5f 6461 7461 5b73 6974 655d  eform_data[site]
-00033c50: 2c20 6172 7261 792e 6172 7261 7929 3a0a  , array.array):.
-00033c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033c70: 6966 2077 6176 6566 6f72 6d5f 6461 7461  if waveform_data
-00033c80: 5b73 6974 655d 2e74 7970 6563 6f64 6520  [site].typecode 
-00033c90: 3d3d 2027 4c27 3a0a 2020 2020 2020 2020  == 'L':.        
-00033ca0: 2020 2020 2020 2020 2020 2020 7766 6d20              wfm 
-00033cb0: 3d20 7761 7665 666f 726d 5f64 6174 615b  = waveform_data[
-00033cc0: 7369 7465 5d0a 2020 2020 2020 2020 2020  site].          
-00033cd0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00033ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033cf0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-00033d00: 2757 726f 6e67 2077 6176 6566 6f72 6d5f  'Wrong waveform_
-00033d10: 6461 7461 2061 7272 6179 2065 6c65 6d65  data array eleme
-00033d20: 6e74 2074 7970 652e 204d 7573 7420 6265  nt type. Must be
-00033d30: 2075 6e73 6967 6e65 6420 3332 2062 6974   unsigned 32 bit
-00033d40: 2069 6e74 2028 224c 2229 2c20 7761 7320   int ("L"), was 
-00033d50: 7b7d 272e 666f 726d 6174 2877 6176 6566  {}'.format(wavef
-00033d60: 6f72 6d5f 6461 7461 5b73 6974 655d 2e74  orm_data[site].t
-00033d70: 7970 6563 6f64 6529 290a 0a20 2020 2020  ypecode))..     
-00033d80: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-00033d90: 7374 616e 6365 2877 6176 6566 6f72 6d5f  stance(waveform_
-00033da0: 6461 7461 5b73 6974 655d 2c20 6c69 7374  data[site], list
-00033db0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00033dc0: 2020 2077 666d 203d 2061 7272 6179 2e61     wfm = array.a
-00033dd0: 7272 6179 2827 4c27 2c20 7761 7665 666f  rray('L', wavefo
-00033de0: 726d 5f64 6174 615b 7369 7465 5d29 0a0a  rm_data[site])..
-00033df0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00033e00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00033e10: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-00033e20: 7228 2755 6e6b 6e6f 776e 2061 7272 6179  r('Unknown array
-00033e30: 2074 7970 653a 207b 7d27 2e66 6f72 6d61   type: {}'.forma
-00033e40: 7428 7479 7065 2877 6176 6566 6f72 6d5f  t(type(waveform_
-00033e50: 6461 7461 5b73 6974 655d 2929 290a 0a20  data[site]))).. 
-00033e60: 2020 2020 2020 2020 2020 2073 6974 655f             site_
-00033e70: 6c69 7374 2e61 7070 656e 6428 7369 7465  list.append(site
-00033e80: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00033e90: 7461 7274 203d 2069 202a 2061 6374 7561  tart = i * actua
-00033ea0: 6c5f 7361 6d70 6c65 735f 7065 725f 7761  l_samples_per_wa
-00033eb0: 7665 666f 726d 0a20 2020 2020 2020 2020  veform.         
-00033ec0: 2020 2065 6e64 203d 2073 7461 7274 202b     end = start +
-00033ed0: 2061 6374 7561 6c5f 7361 6d70 6c65 735f   actual_samples_
-00033ee0: 7065 725f 7761 7665 666f 726d 0a20 2020  per_waveform.   
-00033ef0: 2020 2020 2020 2020 206d 765b 7374 6172           mv[star
-00033f00: 743a 656e 645d 203d 2077 666d 0a0a 2020  t:end] = wfm..  
-00033f10: 2020 2020 2020 2020 2020 6920 2b3d 2031            i += 1
-00033f20: 0a0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00033f30: 6974 6573 5b73 6974 655f 6c69 7374 5d2e  ites[site_list].
-00033f40: 5f77 7269 7465 5f73 6f75 7263 655f 7761  _write_source_wa
-00033f50: 7665 666f 726d 5f73 6974 655f 756e 6971  veform_site_uniq
-00033f60: 7565 5f75 3332 2877 6176 6566 6f72 6d5f  ue_u32(waveform_
-00033f70: 6e61 6d65 2c20 6c65 6e28 7761 7665 666f  name, len(wavefo
-00033f80: 726d 5f64 6174 6129 2c20 6163 7475 616c  rm_data), actual
-00033f90: 5f73 616d 706c 6573 5f70 6572 5f77 6176  _samples_per_wav
-00033fa0: 6566 6f72 6d2c 2064 6174 6129 0a0a 2020  eform, data)..  
-00033fb0: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
-00033fc0: 7a65 640a 2020 2020 6465 6620 6765 745f  zed.    def get_
-00033fd0: 7061 7474 6572 6e5f 7069 6e5f 6e61 6d65  pattern_pin_name
-00033fe0: 7328 7365 6c66 2c20 7374 6172 745f 6c61  s(self, start_la
-00033ff0: 6265 6c29 3a0a 2020 2020 2020 2020 7227  bel):.        r'
-00034000: 2727 6765 745f 7061 7474 6572 6e5f 7069  ''get_pattern_pi
-00034010: 6e5f 6e61 6d65 730a 0a20 2020 2020 2020  n_names..       
-00034020: 2052 6574 7572 6e73 2074 6865 2070 6174   Returns the pat
-00034030: 7465 726e 2070 696e 206c 6973 742e 0a0a  tern pin list...
-00034040: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00034050: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-00034060: 6c61 6265 6c20 2873 7472 293a 2050 6174  label (str): Pat
-00034070: 7465 726e 206e 616d 6520 6f72 2065 7870  tern name or exp
-00034080: 6f72 7465 6420 7061 7474 6572 6e20 6c61  orted pattern la
-00034090: 6265 6c20 6672 6f6d 2077 6869 6368 2074  bel from which t
-000340a0: 6f20 6765 7420 7468 6520 7069 6e20 6e61  o get the pin na
-000340b0: 6d65 7320 7468 6174 2074 6865 2070 6174  mes that the pat
-000340c0: 7465 726e 2072 6566 6572 656e 6365 732e  tern references.
-000340d0: 0a0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000340e0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-000340f0: 7069 6e5f 6c69 7374 2028 6c69 7374 206f  pin_list (list o
-00034100: 6620 7374 7229 3a20 4c69 7374 206f 6620  f str): List of 
-00034110: 7069 6e73 2072 6566 6572 656e 6365 6420  pins referenced 
-00034120: 6279 2074 6865 2070 6174 7465 726e 2077  by the pattern w
-00034130: 6974 6820 7468 6520 2a2a 7374 6172 744c  ith the **startL
-00034140: 6162 656c 2a2a 2e0a 0a20 2020 2020 2020  abel**...       
-00034150: 2027 2727 0a20 2020 2020 2020 2070 696e   '''.        pin
-00034160: 5f6c 6973 7420 3d20 7365 6c66 2e5f 696e  _list = self._in
-00034170: 7465 7270 7265 7465 722e 6765 745f 7061  terpreter.get_pa
-00034180: 7474 6572 6e5f 7069 6e5f 6e61 6d65 7328  ttern_pin_names(
-00034190: 7374 6172 745f 6c61 6265 6c29 0a20 2020  start_label).   
-000341a0: 2020 2020 2072 6574 7572 6e20 5f63 6f6e       return _con
-000341b0: 7665 7274 6572 732e 636f 6e76 6572 745f  verters.convert_
-000341c0: 636f 6d6d 615f 7365 7061 7261 7465 645f  comma_separated_
-000341d0: 7374 7269 6e67 5f74 6f5f 6c69 7374 2870  string_to_list(p
-000341e0: 696e 5f6c 6973 7429 0a0a 2020 2020 4069  in_list)..    @i
-000341f0: 7669 5f73 796e 6368 726f 6e69 7a65 640a  vi_synchronized.
-00034200: 2020 2020 6465 6620 6765 745f 7469 6d65      def get_time
-00034210: 5f73 6574 5f70 6572 696f 6428 7365 6c66  _set_period(self
-00034220: 2c20 7469 6d65 5f73 6574 5f6e 616d 6529  , time_set_name)
-00034230: 3a0a 2020 2020 2020 2020 7227 2727 6765  :.        r'''ge
-00034240: 745f 7469 6d65 5f73 6574 5f70 6572 696f  t_time_set_perio
-00034250: 640a 0a20 2020 2020 2020 2052 6574 7572  d..        Retur
-00034260: 6e73 2074 6865 2070 6572 696f 6420 6f66  ns the period of
-00034270: 2074 6865 2073 7065 6369 6669 6564 2074   the specified t
-00034280: 696d 6520 7365 742e 0a0a 2020 2020 2020  ime set...      
-00034290: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000342a0: 2020 2020 7469 6d65 5f73 6574 5f6e 616d      time_set_nam
-000342b0: 6520 2873 7472 293a 2054 6865 2073 7065  e (str): The spe
-000342c0: 6369 6669 6564 2074 696d 6520 7365 7420  cified time set 
-000342d0: 6e61 6d65 2e0a 0a0a 2020 2020 2020 2020  name....        
-000342e0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-000342f0: 2020 2020 2070 6572 696f 6420 2868 6967       period (hig
-00034300: 6874 696d 652e 7469 6d65 6465 6c74 6129  htime.timedelta)
-00034310: 3a20 5265 7475 726e 6564 2070 6572 696f  : Returned perio
-00034320: 642c 2069 6e20 7365 636f 6e64 732c 2074  d, in seconds, t
-00034330: 6861 7420 7468 6520 6564 6765 2069 7320  hat the edge is 
-00034340: 636f 6e66 6967 7572 6564 2074 6f2e 0a0a  configured to...
-00034350: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00034360: 2020 2020 7065 7269 6f64 203d 2073 656c      period = sel
-00034370: 662e 5f69 6e74 6572 7072 6574 6572 2e67  f._interpreter.g
-00034380: 6574 5f74 696d 655f 7365 745f 7065 7269  et_time_set_peri
-00034390: 6f64 2874 696d 655f 7365 745f 6e61 6d65  od(time_set_name
-000343a0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000343b0: 205f 636f 6e76 6572 7465 7273 2e63 6f6e   _converters.con
-000343c0: 7665 7274 5f73 6563 6f6e 6473 5f72 6561  vert_seconds_rea
-000343d0: 6c36 345f 746f 5f74 696d 6564 656c 7461  l64_to_timedelta
-000343e0: 2870 6572 696f 6429 0a0a 2020 2020 6465  (period)..    de
-000343f0: 6620 5f69 6e69 745f 7769 7468 5f6f 7074  f _init_with_opt
-00034400: 696f 6e73 2873 656c 662c 2072 6573 6f75  ions(self, resou
-00034410: 7263 655f 6e61 6d65 2c20 6964 5f71 7565  rce_name, id_que
-00034420: 7279 3d46 616c 7365 2c20 7265 7365 745f  ry=False, reset_
-00034430: 6465 7669 6365 3d46 616c 7365 2c20 6f70  device=False, op
-00034440: 7469 6f6e 5f73 7472 696e 673d 2222 293a  tion_string=""):
-00034450: 0a20 2020 2020 2020 2072 2727 275f 696e  .        r'''_in
-00034460: 6974 5f77 6974 685f 6f70 7469 6f6e 730a  it_with_options.
-00034470: 0a20 2020 2020 2020 2043 7265 6174 6573  .        Creates
-00034480: 2061 6e64 2072 6574 7572 6e73 2061 206e   and returns a n
-00034490: 6577 2073 6573 7369 6f6e 2074 6f20 7468  ew session to th
-000344a0: 6520 7370 6563 6966 6965 6420 6469 6769  e specified digi
-000344b0: 7461 6c20 7061 7474 6572 6e20 696e 7374  tal pattern inst
-000344c0: 7275 6d65 6e74 2074 6f20 7573 6520 696e  rument to use in
-000344d0: 2061 6c6c 2073 7562 7365 7175 656e 7420   all subsequent 
-000344e0: 6d65 7468 6f64 2063 616c 6c73 2e20 546f  method calls. To
-000344f0: 2070 6c61 6365 2074 6865 2069 6e73 7472   place the instr
-00034500: 756d 656e 7420 696e 2061 206b 6e6f 776e  ument in a known
-00034510: 2073 7461 7274 7570 2073 7461 7465 2077   startup state w
-00034520: 6865 6e20 6372 6561 7469 6e67 2061 206e  hen creating a n
-00034530: 6577 2073 6573 7369 6f6e 2c20 7365 7420  ew session, set 
-00034540: 7468 6520 7265 7365 7420 7061 7261 6d65  the reset parame
-00034550: 7465 7220 746f 2054 7275 652c 2077 6869  ter to True, whi
-00034560: 6368 2069 7320 6571 7569 7661 6c65 6e74  ch is equivalent
-00034570: 2074 6f20 6361 6c6c 696e 6720 7468 6520   to calling the 
-00034580: 7265 7365 7420 6d65 7468 6f64 2069 6d6d  reset method imm
-00034590: 6564 6961 7465 6c79 2061 6674 6572 2069  ediately after i
-000345a0: 6e69 7469 616c 697a 696e 6720 7468 6520  nitializing the 
-000345b0: 7365 7373 696f 6e2e 0a0a 2020 2020 2020  session...      
-000345c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000345d0: 2020 2020 7265 736f 7572 6365 5f6e 616d      resource_nam
-000345e0: 6520 2873 7472 293a 2054 6865 2073 7065  e (str): The spe
-000345f0: 6369 6669 6564 2072 6573 6f75 7263 6520  cified resource 
-00034600: 6e61 6d65 2073 686f 776e 2069 6e20 4d65  name shown in Me
-00034610: 6173 7572 656d 656e 7420 2620 4175 746f  asurement & Auto
-00034620: 6d61 7469 6f6e 2045 7870 6c6f 7265 7220  mation Explorer 
-00034630: 284d 4158 2920 666f 7220 6120 6469 6769  (MAX) for a digi
-00034640: 7461 6c20 7061 7474 6572 6e20 696e 7374  tal pattern inst
-00034650: 7275 6d65 6e74 2c20 666f 7220 6578 616d  rument, for exam
-00034660: 706c 652c 2050 5849 3153 6c6f 7433 2c20  ple, PXI1Slot3, 
-00034670: 7768 6572 6520 5058 4931 536c 6f74 3320  where PXI1Slot3 
-00034680: 6973 2061 6e20 696e 7374 7275 6d65 6e74  is an instrument
-00034690: 2072 6573 6f75 7263 6520 6e61 6d65 2e20   resource name. 
-000346a0: 2a2a 7265 736f 7572 6365 4e61 6d65 2a2a  **resourceName**
-000346b0: 2063 616e 2061 6c73 6f20 6265 2061 206c   can also be a l
-000346c0: 6f67 6963 616c 2049 5649 206e 616d 652e  ogical IVI name.
-000346d0: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
-000346e0: 6163 6365 7074 7320 6120 636f 6d6d 612d  accepts a comma-
-000346f0: 6465 6c69 6d69 7465 6420 6c69 7374 206f  delimited list o
-00034700: 6620 7374 7269 6e67 7320 696e 2074 6865  f strings in the
-00034710: 2066 6f72 6d20 5058 4931 536c 6f74 322c   form PXI1Slot2,
-00034720: 5058 4931 536c 6f74 332c 2077 6865 7265  PXI1Slot3, where
-00034730: 2060 6050 5849 3153 6c6f 7432 6060 2069   ``PXI1Slot2`` i
-00034740: 7320 6f6e 6520 696e 7374 7275 6d65 6e74  s one instrument
-00034750: 2072 6573 6f75 7263 6520 6e61 6d65 2061   resource name a
-00034760: 6e64 2060 6050 5849 3153 6c6f 7433 6060  nd ``PXI1Slot3``
-00034770: 2069 7320 616e 6f74 6865 722e 2057 6865   is another. Whe
-00034780: 6e20 696e 636c 7564 696e 6720 6d6f 7265  n including more
-00034790: 2074 6861 6e20 6f6e 6520 6469 6769 7461   than one digita
-000347a0: 6c20 7061 7474 6572 6e20 696e 7374 7275  l pattern instru
-000347b0: 6d65 6e74 2069 6e20 7468 6520 636f 6d6d  ment in the comm
-000347c0: 612d 6465 6c69 6d69 7465 6420 6c69 7374  a-delimited list
-000347d0: 206f 6620 7374 7269 6e67 732c 206c 6973   of strings, lis
-000347e0: 7420 7468 6520 696e 7374 7275 6d65 6e74  t the instrument
-000347f0: 7320 696e 2074 6865 2073 616d 6520 6f72  s in the same or
-00034800: 6465 7220 7468 6579 2061 7070 6561 7220  der they appear 
-00034810: 696e 2074 6865 2070 696e 206d 6170 2e0a  in the pin map..
-00034820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00034830: 202b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d   +--------+-----
+00033b90: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00033ba0: 2255 6e73 7570 706f 7274 6564 2064 7479  "Unsupported dty
+00033bb0: 7065 2066 6f72 2077 6176 6566 6f72 6d5f  pe for waveform_
+00033bc0: 6461 7461 2061 7272 6179 2065 6c65 6d65  data array eleme
+00033bd0: 6e74 2074 7970 652e 2049 7320 7b30 7d2c  nt type. Is {0},
+00033be0: 2065 7870 6563 7465 6420 7b31 7d22 2e66   expected {1}".f
+00033bf0: 6f72 6d61 7428 7761 7665 666f 726d 5f64  ormat(waveform_d
+00033c00: 6174 615b 7369 7465 5d2e 6474 7970 652c  ata[site].dtype,
+00033c10: 206e 756d 7079 2e69 6e74 3332 2929 0a0a   numpy.int32))..
+00033c20: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00033c30: 2069 7369 6e73 7461 6e63 6528 7761 7665   isinstance(wave
+00033c40: 666f 726d 5f64 6174 615b 7369 7465 5d2c  form_data[site],
+00033c50: 2061 7272 6179 2e61 7272 6179 293a 0a20   array.array):. 
+00033c60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00033c70: 6620 7761 7665 666f 726d 5f64 6174 615b  f waveform_data[
+00033c80: 7369 7465 5d2e 7479 7065 636f 6465 203d  site].typecode =
+00033c90: 3d20 274c 273a 0a20 2020 2020 2020 2020  = 'L':.         
+00033ca0: 2020 2020 2020 2020 2020 2077 666d 203d             wfm =
+00033cb0: 2077 6176 6566 6f72 6d5f 6461 7461 5b73   waveform_data[s
+00033cc0: 6974 655d 0a20 2020 2020 2020 2020 2020  ite].           
+00033cd0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00033ce0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00033cf0: 6169 7365 2054 7970 6545 7272 6f72 2827  aise TypeError('
+00033d00: 5772 6f6e 6720 7761 7665 666f 726d 5f64  Wrong waveform_d
+00033d10: 6174 6120 6172 7261 7920 656c 656d 656e  ata array elemen
+00033d20: 7420 7479 7065 2e20 4d75 7374 2062 6520  t type. Must be 
+00033d30: 756e 7369 676e 6564 2033 3220 6269 7420  unsigned 32 bit 
+00033d40: 696e 7420 2822 4c22 292c 2077 6173 207b  int ("L"), was {
+00033d50: 7d27 2e66 6f72 6d61 7428 7761 7665 666f  }'.format(wavefo
+00033d60: 726d 5f64 6174 615b 7369 7465 5d2e 7479  rm_data[site].ty
+00033d70: 7065 636f 6465 2929 0a0a 2020 2020 2020  pecode))..      
+00033d80: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00033d90: 7461 6e63 6528 7761 7665 666f 726d 5f64  tance(waveform_d
+00033da0: 6174 615b 7369 7465 5d2c 206c 6973 7429  ata[site], list)
+00033db0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00033dc0: 2020 7766 6d20 3d20 6172 7261 792e 6172    wfm = array.ar
+00033dd0: 7261 7928 274c 272c 2077 6176 6566 6f72  ray('L', wavefor
+00033de0: 6d5f 6461 7461 5b73 6974 655d 290a 0a20  m_data[site]).. 
+00033df0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00033e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00033e10: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+00033e20: 2827 556e 6b6e 6f77 6e20 6172 7261 7920  ('Unknown array 
+00033e30: 7479 7065 3a20 7b7d 272e 666f 726d 6174  type: {}'.format
+00033e40: 2874 7970 6528 7761 7665 666f 726d 5f64  (type(waveform_d
+00033e50: 6174 615b 7369 7465 5d29 2929 0a0a 2020  ata[site])))..  
+00033e60: 2020 2020 2020 2020 2020 7369 7465 5f6c            site_l
+00033e70: 6973 742e 6170 7065 6e64 2873 6974 6529  ist.append(site)
+00033e80: 0a0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00033e90: 6172 7420 3d20 6920 2a20 6163 7475 616c  art = i * actual
+00033ea0: 5f73 616d 706c 6573 5f70 6572 5f77 6176  _samples_per_wav
+00033eb0: 6566 6f72 6d0a 2020 2020 2020 2020 2020  eform.          
+00033ec0: 2020 656e 6420 3d20 7374 6172 7420 2b20    end = start + 
+00033ed0: 6163 7475 616c 5f73 616d 706c 6573 5f70  actual_samples_p
+00033ee0: 6572 5f77 6176 6566 6f72 6d0a 2020 2020  er_waveform.    
+00033ef0: 2020 2020 2020 2020 6d76 5b73 7461 7274          mv[start
+00033f00: 3a65 6e64 5d20 3d20 7766 6d0a 0a20 2020  :end] = wfm..   
+00033f10: 2020 2020 2020 2020 2069 202b 3d20 310a           i += 1.
+00033f20: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
+00033f30: 7465 735b 7369 7465 5f6c 6973 745d 2e5f  tes[site_list]._
+00033f40: 7772 6974 655f 736f 7572 6365 5f77 6176  write_source_wav
+00033f50: 6566 6f72 6d5f 7369 7465 5f75 6e69 7175  eform_site_uniqu
+00033f60: 655f 7533 3228 7761 7665 666f 726d 5f6e  e_u32(waveform_n
+00033f70: 616d 652c 206c 656e 2877 6176 6566 6f72  ame, len(wavefor
+00033f80: 6d5f 6461 7461 292c 2061 6374 7561 6c5f  m_data), actual_
+00033f90: 7361 6d70 6c65 735f 7065 725f 7761 7665  samples_per_wave
+00033fa0: 666f 726d 2c20 6461 7461 290a 0a20 2020  form, data)..   
+00033fb0: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
+00033fc0: 6564 0a20 2020 2064 6566 2067 6574 5f70  ed.    def get_p
+00033fd0: 6174 7465 726e 5f70 696e 5f6e 616d 6573  attern_pin_names
+00033fe0: 2873 656c 662c 2073 7461 7274 5f6c 6162  (self, start_lab
+00033ff0: 656c 293a 0a20 2020 2020 2020 2072 2727  el):.        r''
+00034000: 2767 6574 5f70 6174 7465 726e 5f70 696e  'get_pattern_pin
+00034010: 5f6e 616d 6573 0a0a 2020 2020 2020 2020  _names..        
+00034020: 5265 7475 726e 7320 7468 6520 7061 7474  Returns the patt
+00034030: 6572 6e20 7069 6e20 6c69 7374 2e0a 0a20  ern pin list... 
+00034040: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00034050: 2020 2020 2020 2020 2073 7461 7274 5f6c           start_l
+00034060: 6162 656c 2028 7374 7229 3a20 5061 7474  abel (str): Patt
+00034070: 6572 6e20 6e61 6d65 206f 7220 6578 706f  ern name or expo
+00034080: 7274 6564 2070 6174 7465 726e 206c 6162  rted pattern lab
+00034090: 656c 2066 726f 6d20 7768 6963 6820 746f  el from which to
+000340a0: 2067 6574 2074 6865 2070 696e 206e 616d   get the pin nam
+000340b0: 6573 2074 6861 7420 7468 6520 7061 7474  es that the patt
+000340c0: 6572 6e20 7265 6665 7265 6e63 6573 2e0a  ern references..
+000340d0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000340e0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+000340f0: 696e 5f6c 6973 7420 286c 6973 7420 6f66  in_list (list of
+00034100: 2073 7472 293a 204c 6973 7420 6f66 2070   str): List of p
+00034110: 696e 7320 7265 6665 7265 6e63 6564 2062  ins referenced b
+00034120: 7920 7468 6520 7061 7474 6572 6e20 7769  y the pattern wi
+00034130: 7468 2074 6865 202a 2a73 7461 7274 4c61  th the **startLa
+00034140: 6265 6c2a 2a2e 0a0a 2020 2020 2020 2020  bel**...        
+00034150: 2727 270a 2020 2020 2020 2020 7069 6e5f  '''.        pin_
+00034160: 6c69 7374 203d 2073 656c 662e 5f69 6e74  list = self._int
+00034170: 6572 7072 6574 6572 2e67 6574 5f70 6174  erpreter.get_pat
+00034180: 7465 726e 5f70 696e 5f6e 616d 6573 2873  tern_pin_names(s
+00034190: 7461 7274 5f6c 6162 656c 290a 2020 2020  tart_label).    
+000341a0: 2020 2020 7265 7475 726e 205f 636f 6e76      return _conv
+000341b0: 6572 7465 7273 2e63 6f6e 7665 7274 5f63  erters.convert_c
+000341c0: 6f6d 6d61 5f73 6570 6172 6174 6564 5f73  omma_separated_s
+000341d0: 7472 696e 675f 746f 5f6c 6973 7428 7069  tring_to_list(pi
+000341e0: 6e5f 6c69 7374 290a 0a20 2020 2040 6976  n_list)..    @iv
+000341f0: 695f 7379 6e63 6872 6f6e 697a 6564 0a20  i_synchronized. 
+00034200: 2020 2064 6566 2067 6574 5f74 696d 655f     def get_time_
+00034210: 7365 745f 7065 7269 6f64 2873 656c 662c  set_period(self,
+00034220: 2074 696d 655f 7365 745f 6e61 6d65 293a   time_set_name):
+00034230: 0a20 2020 2020 2020 2072 2727 2767 6574  .        r'''get
+00034240: 5f74 696d 655f 7365 745f 7065 7269 6f64  _time_set_period
+00034250: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00034260: 7320 7468 6520 7065 7269 6f64 206f 6620  s the period of 
+00034270: 7468 6520 7370 6563 6966 6965 6420 7469  the specified ti
+00034280: 6d65 2073 6574 2e0a 0a20 2020 2020 2020  me set...       
+00034290: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+000342a0: 2020 2074 696d 655f 7365 745f 6e61 6d65     time_set_name
+000342b0: 2028 7374 7229 3a20 5468 6520 7370 6563   (str): The spec
+000342c0: 6966 6965 6420 7469 6d65 2073 6574 206e  ified time set n
+000342d0: 616d 652e 0a0a 0a20 2020 2020 2020 2052  ame....        R
+000342e0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+000342f0: 2020 2020 7065 7269 6f64 2028 6869 6768      period (high
+00034300: 7469 6d65 2e74 696d 6564 656c 7461 293a  time.timedelta):
+00034310: 2052 6574 7572 6e65 6420 7065 7269 6f64   Returned period
+00034320: 2c20 696e 2073 6563 6f6e 6473 2c20 7468  , in seconds, th
+00034330: 6174 2074 6865 2065 6467 6520 6973 2063  at the edge is c
+00034340: 6f6e 6669 6775 7265 6420 746f 2e0a 0a20  onfigured to... 
+00034350: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00034360: 2020 2070 6572 696f 6420 3d20 7365 6c66     period = self
+00034370: 2e5f 696e 7465 7270 7265 7465 722e 6765  ._interpreter.ge
+00034380: 745f 7469 6d65 5f73 6574 5f70 6572 696f  t_time_set_perio
+00034390: 6428 7469 6d65 5f73 6574 5f6e 616d 6529  d(time_set_name)
+000343a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000343b0: 5f63 6f6e 7665 7274 6572 732e 636f 6e76  _converters.conv
+000343c0: 6572 745f 7365 636f 6e64 735f 7265 616c  ert_seconds_real
+000343d0: 3634 5f74 6f5f 7469 6d65 6465 6c74 6128  64_to_timedelta(
+000343e0: 7065 7269 6f64 290a 0a20 2020 2064 6566  period)..    def
+000343f0: 205f 696e 6974 5f77 6974 685f 6f70 7469   _init_with_opti
+00034400: 6f6e 7328 7365 6c66 2c20 7265 736f 7572  ons(self, resour
+00034410: 6365 5f6e 616d 652c 2069 645f 7175 6572  ce_name, id_quer
+00034420: 793d 4661 6c73 652c 2072 6573 6574 5f64  y=False, reset_d
+00034430: 6576 6963 653d 4661 6c73 652c 206f 7074  evice=False, opt
+00034440: 696f 6e5f 7374 7269 6e67 3d22 2229 3a0a  ion_string=""):.
+00034450: 2020 2020 2020 2020 7227 2727 5f69 6e69          r'''_ini
+00034460: 745f 7769 7468 5f6f 7074 696f 6e73 0a0a  t_with_options..
+00034470: 2020 2020 2020 2020 4372 6561 7465 7320          Creates 
+00034480: 616e 6420 7265 7475 726e 7320 6120 6e65  and returns a ne
+00034490: 7720 7365 7373 696f 6e20 746f 2074 6865  w session to the
+000344a0: 2073 7065 6369 6669 6564 2064 6967 6974   specified digit
+000344b0: 616c 2070 6174 7465 726e 2069 6e73 7472  al pattern instr
+000344c0: 756d 656e 7420 746f 2075 7365 2069 6e20  ument to use in 
+000344d0: 616c 6c20 7375 6273 6571 7565 6e74 206d  all subsequent m
+000344e0: 6574 686f 6420 6361 6c6c 732e 2054 6f20  ethod calls. To 
+000344f0: 706c 6163 6520 7468 6520 696e 7374 7275  place the instru
+00034500: 6d65 6e74 2069 6e20 6120 6b6e 6f77 6e20  ment in a known 
+00034510: 7374 6172 7475 7020 7374 6174 6520 7768  startup state wh
+00034520: 656e 2063 7265 6174 696e 6720 6120 6e65  en creating a ne
+00034530: 7720 7365 7373 696f 6e2c 2073 6574 2074  w session, set t
+00034540: 6865 2072 6573 6574 2070 6172 616d 6574  he reset paramet
+00034550: 6572 2074 6f20 5472 7565 2c20 7768 6963  er to True, whic
+00034560: 6820 6973 2065 7175 6976 616c 656e 7420  h is equivalent 
+00034570: 746f 2063 616c 6c69 6e67 2074 6865 2072  to calling the r
+00034580: 6573 6574 206d 6574 686f 6420 696d 6d65  eset method imme
+00034590: 6469 6174 656c 7920 6166 7465 7220 696e  diately after in
+000345a0: 6974 6961 6c69 7a69 6e67 2074 6865 2073  itializing the s
+000345b0: 6573 7369 6f6e 2e0a 0a20 2020 2020 2020  ession...       
+000345c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+000345d0: 2020 2072 6573 6f75 7263 655f 6e61 6d65     resource_name
+000345e0: 2028 7374 7229 3a20 5468 6520 7370 6563   (str): The spec
+000345f0: 6966 6965 6420 7265 736f 7572 6365 206e  ified resource n
+00034600: 616d 6520 7368 6f77 6e20 696e 204d 6561  ame shown in Mea
+00034610: 7375 7265 6d65 6e74 2026 2041 7574 6f6d  surement & Autom
+00034620: 6174 696f 6e20 4578 706c 6f72 6572 2028  ation Explorer (
+00034630: 4d41 5829 2066 6f72 2061 2064 6967 6974  MAX) for a digit
+00034640: 616c 2070 6174 7465 726e 2069 6e73 7472  al pattern instr
+00034650: 756d 656e 742c 2066 6f72 2065 7861 6d70  ument, for examp
+00034660: 6c65 2c20 5058 4931 536c 6f74 332c 2077  le, PXI1Slot3, w
+00034670: 6865 7265 2050 5849 3153 6c6f 7433 2069  here PXI1Slot3 i
+00034680: 7320 616e 2069 6e73 7472 756d 656e 7420  s an instrument 
+00034690: 7265 736f 7572 6365 206e 616d 652e 202a  resource name. *
+000346a0: 2a72 6573 6f75 7263 654e 616d 652a 2a20  *resourceName** 
+000346b0: 6361 6e20 616c 736f 2062 6520 6120 6c6f  can also be a lo
+000346c0: 6769 6361 6c20 4956 4920 6e61 6d65 2e20  gical IVI name. 
+000346d0: 5468 6973 2070 6172 616d 6574 6572 2061  This parameter a
+000346e0: 6363 6570 7473 2061 2063 6f6d 6d61 2d64  ccepts a comma-d
+000346f0: 656c 696d 6974 6564 206c 6973 7420 6f66  elimited list of
+00034700: 2073 7472 696e 6773 2069 6e20 7468 6520   strings in the 
+00034710: 666f 726d 2050 5849 3153 6c6f 7432 2c50  form PXI1Slot2,P
+00034720: 5849 3153 6c6f 7433 2c20 7768 6572 6520  XI1Slot3, where 
+00034730: 6060 5058 4931 536c 6f74 3260 6020 6973  ``PXI1Slot2`` is
+00034740: 206f 6e65 2069 6e73 7472 756d 656e 7420   one instrument 
+00034750: 7265 736f 7572 6365 206e 616d 6520 616e  resource name an
+00034760: 6420 6060 5058 4931 536c 6f74 3360 6020  d ``PXI1Slot3`` 
+00034770: 6973 2061 6e6f 7468 6572 2e20 5768 656e  is another. When
+00034780: 2069 6e63 6c75 6469 6e67 206d 6f72 6520   including more 
+00034790: 7468 616e 206f 6e65 2064 6967 6974 616c  than one digital
+000347a0: 2070 6174 7465 726e 2069 6e73 7472 756d   pattern instrum
+000347b0: 656e 7420 696e 2074 6865 2063 6f6d 6d61  ent in the comma
+000347c0: 2d64 656c 696d 6974 6564 206c 6973 7420  -delimited list 
+000347d0: 6f66 2073 7472 696e 6773 2c20 6c69 7374  of strings, list
+000347e0: 2074 6865 2069 6e73 7472 756d 656e 7473   the instruments
+000347f0: 2069 6e20 7468 6520 7361 6d65 206f 7264   in the same ord
+00034800: 6572 2074 6865 7920 6170 7065 6172 2069  er they appear i
+00034810: 6e20 7468 6520 7069 6e20 6d61 702e 0a0a  n the pin map...
+00034820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00034830: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
 00034840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000348a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000348b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000348c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000348d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000348e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000348f0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020  ---------+.     
-00034900: 2020 2020 2020 2020 2020 207c 207c 4e6f             | |No
-00034910: 7465 7c20 7c20 4e6f 7465 c2a0 c2a0 2059  te| | Note.... Y
-00034920: 6f75 206f 6e6c 7920 6361 6e20 7370 6563  ou only can spec
-00034930: 6966 7920 6d75 6c74 6970 6c65 2069 6e73  ify multiple ins
-00034940: 7472 756d 656e 7473 206f 6620 7468 6520  truments of the 
-00034950: 7361 6d65 206d 6f64 656c 2e20 466f 7220  same model. For 
-00034960: 6578 616d 706c 652c 2079 6f75 2063 616e  example, you can
-00034970: 206c 6973 7420 7477 6f20 5058 4965 2d36   list two PXIe-6
-00034980: 3537 3073 2062 7574 206e 6f74 2061 2050  570s but not a P
-00034990: 5849 652d 3635 3730 2061 6e64 2050 5849  XIe-6570 and PXI
-000349a0: 652d 3635 3731 2e20 5468 6520 696e 7374  e-6571. The inst
-000349b0: 7275 6d65 6e74 7320 6d75 7374 2062 6520  ruments must be 
-000349c0: 696e 2074 6865 2073 616d 6520 6368 6173  in the same chas
-000349d0: 7369 732e 207c 0a20 2020 2020 2020 2020  sis. |.         
-000349e0: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
-000349f0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+000348f0: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+00034900: 2020 2020 2020 2020 2020 7c20 7c4e 6f74            | |Not
+00034910: 657c 207c 204e 6f74 65c2 a0c2 a020 596f  e| | Note.... Yo
+00034920: 7520 6f6e 6c79 2063 616e 2073 7065 6369  u only can speci
+00034930: 6679 206d 756c 7469 706c 6520 696e 7374  fy multiple inst
+00034940: 7275 6d65 6e74 7320 6f66 2074 6865 2073  ruments of the s
+00034950: 616d 6520 6d6f 6465 6c2e 2046 6f72 2065  ame model. For e
+00034960: 7861 6d70 6c65 2c20 796f 7520 6361 6e20  xample, you can 
+00034970: 6c69 7374 2074 776f 2050 5849 652d 3635  list two PXIe-65
+00034980: 3730 7320 6275 7420 6e6f 7420 6120 5058  70s but not a PX
+00034990: 4965 2d36 3537 3020 616e 6420 5058 4965  Ie-6570 and PXIe
+000349a0: 2d36 3537 312e 2054 6865 2069 6e73 7472  -6571. The instr
+000349b0: 756d 656e 7473 206d 7573 7420 6265 2069  uments must be i
+000349c0: 6e20 7468 6520 7361 6d65 2063 6861 7373  n the same chass
+000349d0: 6973 2e20 7c0a 2020 2020 2020 2020 2020  is. |.          
+000349e0: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2b        +--------+
+000349f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00034a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00034aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00034ab0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00034ac0: 2020 2e2e 207c 4e6f 7465 7c20 696d 6167    .. |Note| imag
-00034ad0: 653a 3a20 6e6f 7465 2e67 6966 0a0a 2020  e:: note.gif..  
-00034ae0: 2020 2020 2020 2020 2020 2020 2020 4e6f                No
-00034af0: 7465 3a0a 0a20 2020 2020 2020 2020 2020  te:..           
-00034b00: 2069 645f 7175 6572 7920 2862 6f6f 6c29   id_query (bool)
-00034b10: 3a20 4120 426f 6f6c 6561 6e20 7468 6174  : A Boolean that
-00034b20: 2076 6572 6966 6965 7320 7468 6174 2074   verifies that t
-00034b30: 6865 2064 6967 6974 616c 2070 6174 7465  he digital patte
-00034b40: 726e 2069 6e73 7472 756d 656e 7420 796f  rn instrument yo
-00034b50: 7520 696e 6974 6961 6c69 7a65 2069 7320  u initialize is 
-00034b60: 7375 7070 6f72 7465 6420 6279 204e 492d  supported by NI-
-00034b70: 4469 6769 7461 6c2e 204e 492d 4469 6769  Digital. NI-Digi
-00034b80: 7461 6c20 6175 746f 6d61 7469 6361 6c6c  tal automaticall
-00034b90: 7920 7065 7266 6f72 6d73 2074 6869 7320  y performs this 
-00034ba0: 7175 6572 792c 2073 6f20 7365 7474 696e  query, so settin
-00034bb0: 6720 7468 6973 2070 6172 616d 6574 6572  g this parameter
-00034bc0: 2069 7320 6e6f 7420 6e65 6365 7373 6172   is not necessar
-00034bd0: 792e 0a0a 2020 2020 2020 2020 2020 2020  y...            
-00034be0: 7265 7365 745f 6465 7669 6365 2028 626f  reset_device (bo
-00034bf0: 6f6c 293a 2041 2042 6f6f 6c65 616e 2074  ol): A Boolean t
-00034c00: 6861 7420 7370 6563 6966 6965 7320 7768  hat specifies wh
-00034c10: 6574 6865 7220 746f 2072 6573 6574 2061  ether to reset a
-00034c20: 2064 6967 6974 616c 2070 6174 7465 726e   digital pattern
-00034c30: 2069 6e73 7472 756d 656e 7420 746f 2061   instrument to a
-00034c40: 206b 6e6f 776e 2073 7461 7465 2077 6865   known state whe
-00034c50: 6e20 7468 6520 7365 7373 696f 6e20 6973  n the session is
-00034c60: 2069 6e69 7469 616c 697a 6564 2e20 5365   initialized. Se
-00034c70: 7474 696e 6720 7468 6520 2a2a 7265 7365  tting the **rese
-00034c80: 7444 6576 6963 652a 2a20 7661 6c75 6520  tDevice** value 
-00034c90: 746f 2054 7275 6520 6973 2065 7175 6976  to True is equiv
-00034ca0: 616c 656e 7420 746f 2063 616c 6c69 6e67  alent to calling
-00034cb0: 2074 6865 2072 6573 6574 206d 6574 686f   the reset metho
-00034cc0: 6420 696d 6d65 6469 6174 656c 7920 6166  d immediately af
-00034cd0: 7465 7220 696e 6974 6961 6c69 7a69 6e67  ter initializing
-00034ce0: 2074 6865 2073 6573 7369 6f6e 2e0a 0a20   the session... 
-00034cf0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00034d00: 6e5f 7374 7269 6e67 2028 6469 6374 293a  n_string (dict):
-00034d10: 2054 6865 2069 6e69 7469 616c 2076 616c   The initial val
-00034d20: 7565 7320 6f66 2063 6572 7461 696e 2070  ues of certain p
-00034d30: 726f 7065 7274 6965 7320 666f 7220 7468  roperties for th
-00034d40: 6520 4e49 2d44 6967 6974 616c 2050 6174  e NI-Digital Pat
-00034d50: 7465 726e 2044 7269 7665 7220 7365 7373  tern Driver sess
-00034d60: 696f 6e2e 2054 6865 2073 7472 696e 6720  ion. The string 
-00034d70: 6361 6e20 6265 2065 6d70 7479 2e20 596f  can be empty. Yo
-00034d80: 7520 6361 6e20 7573 6520 7468 6520 4472  u can use the Dr
-00034d90: 6976 6572 5365 7475 7020 666c 6167 2074  iverSetup flag t
-00034da0: 6f20 7369 6d75 6c61 7465 2061 2064 6967  o simulate a dig
-00034db0: 6974 616c 2070 6174 7465 726e 2069 6e73  ital pattern ins
-00034dc0: 7472 756d 656e 742e 2057 6865 6e20 7369  trument. When si
-00034dd0: 6d75 6c61 7469 6e67 2061 2064 6967 6974  mulating a digit
-00034de0: 616c 2070 6174 7465 726e 2069 6e73 7472  al pattern instr
-00034df0: 756d 656e 742c 2079 6f75 206d 7573 7420  ument, you must 
-00034e00: 7370 6563 6966 7920 7468 6520 6d6f 6465  specify the mode
-00034e10: 6c20 796f 7520 7761 6e74 2074 6f20 7369  l you want to si
-00034e20: 6d75 6c61 7465 2e20 466f 7220 6578 616d  mulate. For exam
-00034e30: 706c 652c 2053 696d 756c 6174 6520 3d20  ple, Simulate = 
-00034e40: 312c 2044 7269 7665 7253 6574 7570 203d  1, DriverSetup =
-00034e50: 204d 6f64 656c 3a36 3537 302e 0a0a 0a20   Model:6570.... 
-00034e60: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00034e70: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00034e80: 7669 2028 696e 7429 3a20 5468 6520 7265  vi (int): The re
-00034e90: 7475 726e 6564 2069 6e73 7472 756d 656e  turned instrumen
-00034ea0: 7420 7365 7373 696f 6e2e 0a0a 2020 2020  t session...    
-00034eb0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00034ec0: 6f70 7469 6f6e 5f73 7472 696e 6720 3d20  option_string = 
-00034ed0: 5f63 6f6e 7665 7274 6572 732e 636f 6e76  _converters.conv
-00034ee0: 6572 745f 696e 6974 5f77 6974 685f 6f70  ert_init_with_op
-00034ef0: 7469 6f6e 735f 6469 6374 696f 6e61 7279  tions_dictionary
-00034f00: 286f 7074 696f 6e5f 7374 7269 6e67 290a  (option_string).
-00034f10: 2020 2020 2020 2020 6e65 775f 7669 203d          new_vi =
-00034f20: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
-00034f30: 6572 2e69 6e69 745f 7769 7468 5f6f 7074  er.init_with_opt
-00034f40: 696f 6e73 2872 6573 6f75 7263 655f 6e61  ions(resource_na
-00034f50: 6d65 2c20 6964 5f71 7565 7279 2c20 7265  me, id_query, re
-00034f60: 7365 745f 6465 7669 6365 2c20 6f70 7469  set_device, opti
-00034f70: 6f6e 5f73 7472 696e 6729 0a20 2020 2020  on_string).     
-00034f80: 2020 2072 6574 7572 6e20 6e65 775f 7669     return new_vi
-00034f90: 0a0a 2020 2020 4069 7669 5f73 796e 6368  ..    @ivi_synch
-00034fa0: 726f 6e69 7a65 640a 2020 2020 6465 6620  ronized.    def 
-00034fb0: 5f69 6e69 7469 6174 6528 7365 6c66 293a  _initiate(self):
-00034fc0: 0a20 2020 2020 2020 2072 2727 275f 696e  .        r'''_in
-00034fd0: 6974 6961 7465 0a0a 2020 2020 2020 2020  itiate..        
-00034fe0: 5374 6172 7473 2062 7572 7374 696e 6720  Starts bursting 
-00034ff0: 7468 6520 7061 7474 6572 6e20 636f 6e66  the pattern conf
-00035000: 6967 7572 6564 2062 7920 7374 6172 745f  igured by start_
-00035010: 6c61 6265 6c2c 2063 6175 7369 6e67 2074  label, causing t
-00035020: 6865 204e 492d 4469 6769 7461 6c20 7365  he NI-Digital se
-00035030: 7373 696f 6e20 746f 2062 6520 636f 6d6d  ssion to be comm
-00035040: 6974 7465 642e 2054 6f20 7374 6f70 2074  itted. To stop t
-00035050: 6865 2070 6174 7465 726e 2062 7572 7374  he pattern burst
-00035060: 2c20 6361 6c6c 2061 626f 7274 2e20 4966  , call abort. If
-00035070: 206b 6565 7020 616c 6976 6520 7061 7474   keep alive patt
-00035080: 6572 6e20 6973 2062 7572 7374 696e 6720  ern is bursting 
-00035090: 7768 656e 2061 626f 7274 2069 7320 6361  when abort is ca
-000350a0: 6c6c 6564 206f 7220 7570 6f6e 2065 7869  lled or upon exi
-000350b0: 7469 6e67 2074 6865 2063 6f6e 7465 7874  ting the context
-000350c0: 206d 616e 6167 6572 2c20 6b65 6570 2061   manager, keep a
-000350d0: 6c69 7665 2070 6174 7465 726e 2077 696c  live pattern wil
-000350e0: 6c20 6e6f 7420 6265 2073 746f 7070 6564  l not be stopped
-000350f0: 2e20 546f 2073 746f 7020 7468 6520 6b65  . To stop the ke
-00035100: 6570 2061 6c69 7665 2070 6174 7465 726e  ep alive pattern
-00035110: 2c20 6361 6c6c 2061 626f 7274 5f6b 6565  , call abort_kee
-00035120: 705f 616c 6976 652e 0a20 2020 2020 2020  p_alive..       
-00035130: 2027 2727 0a20 2020 2020 2020 2073 656c   '''.        sel
-00035140: 662e 5f69 6e74 6572 7072 6574 6572 2e69  f._interpreter.i
-00035150: 6e69 7469 6174 6528 290a 0a20 2020 2040  nitiate()..    @
-00035160: 6976 695f 7379 6e63 6872 6f6e 697a 6564  ivi_synchronized
-00035170: 0a20 2020 2064 6566 2069 735f 646f 6e65  .    def is_done
-00035180: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00035190: 7227 2727 6973 5f64 6f6e 650a 0a20 2020  r'''is_done..   
-000351a0: 2020 2020 2043 6865 636b 7320 7468 6520       Checks the 
-000351b0: 6861 7264 7761 7265 2074 6f20 6465 7465  hardware to dete
-000351c0: 726d 696e 6520 6966 2074 6865 2070 6174  rmine if the pat
-000351d0: 7465 726e 2062 7572 7374 2068 6173 2063  tern burst has c
-000351e0: 6f6d 706c 6574 6564 206f 7220 6966 2061  ompleted or if a
-000351f0: 6e79 2065 7272 6f72 7320 6861 7665 206f  ny errors have o
-00035200: 6363 7572 7265 642e 0a0a 2020 2020 2020  ccurred...      
-00035210: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00035220: 2020 2020 2020 2064 6f6e 6520 2862 6f6f         done (boo
-00035230: 6c29 3a20 4120 426f 6f6c 6561 6e20 7468  l): A Boolean th
-00035240: 6174 2069 6e64 6963 6174 6573 2077 6865  at indicates whe
-00035250: 7468 6572 2074 6865 2070 6174 7465 726e  ther the pattern
-00035260: 2062 7572 7374 2063 6f6d 706c 6574 6564   burst completed
-00035270: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
-00035280: 2020 2020 2020 2064 6f6e 6520 3d20 7365         done = se
-00035290: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
-000352a0: 6973 5f64 6f6e 6528 290a 2020 2020 2020  is_done().      
-000352b0: 2020 7265 7475 726e 2064 6f6e 650a 0a20    return done.. 
-000352c0: 2020 2040 6976 695f 7379 6e63 6872 6f6e     @ivi_synchron
-000352d0: 697a 6564 0a20 2020 2064 6566 205f 6c6f  ized.    def _lo
-000352e0: 6164 5f6c 6576 656c 7328 7365 6c66 2c20  ad_levels(self, 
-000352f0: 6669 6c65 5f70 6174 6829 3a0a 2020 2020  file_path):.    
-00035300: 2020 2020 7227 2727 5f6c 6f61 645f 6c65      r'''_load_le
-00035310: 7665 6c73 0a0a 2020 2020 2020 2020 4c6f  vels..        Lo
-00035320: 6164 7320 6120 6c65 7665 6c73 2073 6865  ads a levels she
-00035330: 6574 2066 726f 6d20 6120 7370 6563 6966  et from a specif
-00035340: 6965 6420 6669 6c65 2e0a 0a20 2020 2020  ied file...     
-00035350: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00035360: 2020 2020 2066 696c 655f 7061 7468 2028       file_path (
-00035370: 7374 7229 3a20 4162 736f 6c75 7465 2066  str): Absolute f
-00035380: 696c 6520 7061 7468 2074 6f20 7468 6520  ile path to the 
-00035390: 7370 6563 6966 6965 6420 6c65 7665 6c73  specified levels
-000353a0: 2073 6865 6574 2066 696c 652e 0a0a 2020   sheet file...  
-000353b0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-000353c0: 2020 7365 6c66 2e5f 696e 7465 7270 7265    self._interpre
-000353d0: 7465 722e 6c6f 6164 5f6c 6576 656c 7328  ter.load_levels(
-000353e0: 6669 6c65 5f70 6174 6829 0a0a 2020 2020  file_path)..    
-000353f0: 4069 7669 5f73 796e 6368 726f 6e69 7a65  @ivi_synchronize
-00035400: 640a 2020 2020 6465 6620 6c6f 6164 5f70  d.    def load_p
-00035410: 6174 7465 726e 2873 656c 662c 2066 696c  attern(self, fil
-00035420: 655f 7061 7468 293a 0a20 2020 2020 2020  e_path):.       
-00035430: 2072 2727 276c 6f61 645f 7061 7474 6572   r'''load_patter
-00035440: 6e0a 0a20 2020 2020 2020 204c 6f61 6473  n..        Loads
-00035450: 2074 6865 2073 7065 6369 6669 6564 2070   the specified p
-00035460: 6174 7465 726e 2066 696c 652e 0a0a 2020  attern file...  
-00035470: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00035480: 2020 2020 2020 2020 6669 6c65 5f70 6174          file_pat
-00035490: 6820 2873 7472 293a 2041 6273 6f6c 7574  h (str): Absolut
-000354a0: 6520 6669 6c65 2070 6174 6820 6f66 2074  e file path of t
-000354b0: 6865 2062 696e 6172 7920 2e64 6967 6970  he binary .digip
-000354c0: 6174 2070 6174 7465 726e 2066 696c 6520  at pattern file 
-000354d0: 746f 206c 6f61 642e 2053 7065 6369 6679  to load. Specify
-000354e0: 2074 6865 2070 6174 7465 726e 2074 6f20   the pattern to 
-000354f0: 6275 7273 7420 7573 696e 6720 7374 6172  burst using star
-00035500: 745f 6c61 6265 6c20 6f72 2074 6865 2073  t_label or the s
-00035510: 7461 7274 5f6c 6162 656c 2070 6172 616d  tart_label param
-00035520: 6574 6572 206f 6620 7468 6520 6275 7273  eter of the burs
-00035530: 745f 7061 7474 6572 6e20 6d65 7468 6f64  t_pattern method
-00035540: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
-00035550: 2020 2020 2020 2073 656c 662e 5f69 6e74         self._int
-00035560: 6572 7072 6574 6572 2e6c 6f61 645f 7061  erpreter.load_pa
-00035570: 7474 6572 6e28 6669 6c65 5f70 6174 6829  ttern(file_path)
-00035580: 0a0a 2020 2020 4069 7669 5f73 796e 6368  ..    @ivi_synch
-00035590: 726f 6e69 7a65 640a 2020 2020 6465 6620  ronized.    def 
-000355a0: 6c6f 6164 5f70 696e 5f6d 6170 2873 656c  load_pin_map(sel
-000355b0: 662c 2066 696c 655f 7061 7468 293a 0a20  f, file_path):. 
-000355c0: 2020 2020 2020 2072 2727 276c 6f61 645f         r'''load_
-000355d0: 7069 6e5f 6d61 700a 0a20 2020 2020 2020  pin_map..       
-000355e0: 204c 6f61 6473 2061 2070 696e 206d 6170   Loads a pin map
-000355f0: 2066 696c 652e 2059 6f75 2063 616e 206c   file. You can l
-00035600: 6f61 6420 6f6e 6c79 2061 2073 696e 676c  oad only a singl
-00035610: 6520 7069 6e20 616e 6420 6368 616e 6e65  e pin and channe
-00035620: 6c20 6d61 7020 6669 6c65 2064 7572 696e  l map file durin
-00035630: 6720 616e 204e 492d 4469 6769 7461 6c20  g an NI-Digital 
-00035640: 5061 7474 6572 6e20 4472 6976 6572 2073  Pattern Driver s
-00035650: 6573 7369 6f6e 2e20 546f 2073 7769 7463  ession. To switc
-00035660: 6820 7069 6e20 6d61 7073 2c20 6372 6561  h pin maps, crea
-00035670: 7465 2061 206e 6577 2073 6573 7369 6f6e  te a new session
-00035680: 206f 7220 6361 6c6c 2074 6865 2072 6573   or call the res
-00035690: 6574 206d 6574 686f 642e 0a0a 2020 2020  et method...    
-000356a0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000356b0: 2020 2020 2020 6669 6c65 5f70 6174 6820        file_path 
-000356c0: 2873 7472 293a 2041 6273 6f6c 7574 6520  (str): Absolute 
-000356d0: 6669 6c65 2070 6174 6820 746f 2061 2070  file path to a p
-000356e0: 696e 206d 6170 2066 696c 6520 6372 6561  in map file crea
-000356f0: 7465 6420 7769 7468 2074 6865 2044 6967  ted with the Dig
-00035700: 6974 616c 2050 6174 7465 726e 2045 6469  ital Pattern Edi
-00035710: 746f 7220 6f72 2074 6865 204e 4920 5465  tor or the NI Te
-00035720: 7374 5374 616e 6420 5365 6d69 636f 6e64  stStand Semicond
-00035730: 7563 746f 7220 4d6f 6475 6c65 2e0a 0a20  uctor Module... 
-00035740: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00035750: 2020 2073 656c 662e 5f69 6e74 6572 7072     self._interpr
-00035760: 6574 6572 2e6c 6f61 645f 7069 6e5f 6d61  eter.load_pin_ma
-00035770: 7028 6669 6c65 5f70 6174 6829 0a0a 2020  p(file_path)..  
-00035780: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
-00035790: 7a65 640a 2020 2020 6465 6620 5f6c 6f61  zed.    def _loa
-000357a0: 645f 7370 6563 6966 6963 6174 696f 6e73  d_specifications
-000357b0: 2873 656c 662c 2066 696c 655f 7061 7468  (self, file_path
-000357c0: 293a 0a20 2020 2020 2020 2072 2727 275f  ):.        r'''_
-000357d0: 6c6f 6164 5f73 7065 6369 6669 6361 7469  load_specificati
-000357e0: 6f6e 730a 0a20 2020 2020 2020 204c 6f61  ons..        Loa
-000357f0: 6473 2061 2073 7065 6369 6669 6361 7469  ds a specificati
-00035800: 6f6e 7320 7368 6565 7420 6672 6f6d 2061  ons sheet from a
-00035810: 2073 7065 6369 6669 6564 2066 696c 652e   specified file.
-00035820: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00035830: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00035840: 5f70 6174 6820 2873 7472 293a 2041 6273  _path (str): Abs
-00035850: 6f6c 7574 6520 6669 6c65 2070 6174 6820  olute file path 
-00035860: 746f 2061 2073 7065 6369 6669 6361 7469  to a specificati
-00035870: 6f6e 7320 6669 6c65 2e0a 0a20 2020 2020  ons file...     
-00035880: 2020 2027 2727 0a20 2020 2020 2020 2073     '''.        s
-00035890: 656c 662e 5f69 6e74 6572 7072 6574 6572  elf._interpreter
-000358a0: 2e6c 6f61 645f 7370 6563 6966 6963 6174  .load_specificat
-000358b0: 696f 6e73 2866 696c 655f 7061 7468 290a  ions(file_path).
-000358c0: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
-000358d0: 6f6e 697a 6564 0a20 2020 2064 6566 205f  onized.    def _
-000358e0: 6c6f 6164 5f74 696d 696e 6728 7365 6c66  load_timing(self
-000358f0: 2c20 6669 6c65 5f70 6174 6829 3a0a 2020  , file_path):.  
-00035900: 2020 2020 2020 7227 2727 5f6c 6f61 645f        r'''_load_
-00035910: 7469 6d69 6e67 0a0a 2020 2020 2020 2020  timing..        
-00035920: 4c6f 6164 7320 6120 7469 6d69 6e67 2073  Loads a timing s
-00035930: 6865 6574 2066 726f 6d20 6120 7370 6563  heet from a spec
-00035940: 6966 6965 6420 6669 6c65 2e0a 0a20 2020  ified file...   
-00035950: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00035960: 2020 2020 2020 2066 696c 655f 7061 7468         file_path
-00035970: 2028 7374 7229 3a20 4162 736f 6c75 7465   (str): Absolute
-00035980: 2066 696c 6520 7061 7468 2074 6f20 7468   file path to th
-00035990: 6520 7370 6563 6966 6965 6420 7469 6d69  e specified timi
-000359a0: 6e67 2073 6865 6574 2066 696c 652e 0a0a  ng sheet file...
-000359b0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000359c0: 2020 2020 7365 6c66 2e5f 696e 7465 7270      self._interp
-000359d0: 7265 7465 722e 6c6f 6164 5f74 696d 696e  reter.load_timin
-000359e0: 6728 6669 6c65 5f70 6174 6829 0a0a 2020  g(file_path)..  
-000359f0: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
-00035a00: 7a65 640a 2020 2020 6465 6620 7265 6164  zed.    def read
-00035a10: 5f73 6571 7565 6e63 6572 5f66 6c61 6728  _sequencer_flag(
-00035a20: 7365 6c66 2c20 666c 6167 293a 0a20 2020  self, flag):.   
-00035a30: 2020 2020 2072 2727 2772 6561 645f 7365       r'''read_se
-00035a40: 7175 656e 6365 725f 666c 6167 0a0a 2020  quencer_flag..  
-00035a50: 2020 2020 2020 5265 6164 7320 7468 6520        Reads the 
-00035a60: 7374 6174 6520 6f66 2061 2070 6174 7465  state of a patte
-00035a70: 726e 2073 6571 7565 6e63 6572 2066 6c61  rn sequencer fla
-00035a80: 672e 2055 7365 2070 6174 7465 726e 2073  g. Use pattern s
-00035a90: 6571 7565 6e63 6572 2066 6c61 6773 2074  equencer flags t
-00035aa0: 6f20 636f 6f72 6469 6e61 7465 2065 7865  o coordinate exe
-00035ab0: 6375 7469 6f6e 2062 6574 7765 656e 2074  cution between t
-00035ac0: 6865 2070 6174 7465 726e 2073 6571 7565  he pattern seque
-00035ad0: 6e63 6572 2061 6e64 2061 2072 756e 7469  ncer and a runti
-00035ae0: 6d65 2074 6573 7420 7072 6f67 7261 6d2e  me test program.
-00035af0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00035b00: 2020 2020 2020 2020 2020 2020 666c 6167              flag
-00035b10: 2028 656e 756d 732e 5365 7175 656e 6365   (enums.Sequence
-00035b20: 7246 6c61 6729 3a20 5468 6520 7061 7474  rFlag): The patt
-00035b30: 6572 6e20 7365 7175 656e 6365 7220 666c  ern sequencer fl
-00035b40: 6167 2079 6f75 2077 616e 7420 746f 2072  ag you want to r
-00035b50: 6561 642e 0a0a 2020 2020 2020 2020 2020  ead...          
-00035b60: 2020 2020 2020 2d20 2020 5365 7175 656e        -   Sequen
-00035b70: 6365 7246 6c61 672e 464c 4147 3020 2822  cerFlag.FLAG0 ("
-00035b80: 7365 7166 6c61 6730 2229 3a20 5265 6164  seqflag0"): Read
-00035b90: 7320 7061 7474 6572 6e20 7365 7175 656e  s pattern sequen
-00035ba0: 6365 7220 666c 6167 2030 2e0a 2020 2020  cer flag 0..    
-00035bb0: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
-00035bc0: 5365 7175 656e 6365 7246 6c61 672e 464c  SequencerFlag.FL
-00035bd0: 4147 3120 2822 7365 7166 6c61 6731 2229  AG1 ("seqflag1")
-00035be0: 3a20 5265 6164 7320 7061 7474 6572 6e20  : Reads pattern 
-00035bf0: 7365 7175 656e 6365 7220 666c 6167 2031  sequencer flag 1
-00035c00: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00035c10: 2020 2d20 2020 5365 7175 656e 6365 7246    -   SequencerF
-00035c20: 6c61 672e 464c 4147 3220 2822 7365 7166  lag.FLAG2 ("seqf
-00035c30: 6c61 6732 2229 3a20 5265 6164 7320 7061  lag2"): Reads pa
-00035c40: 7474 6572 6e20 7365 7175 656e 6365 7220  ttern sequencer 
-00035c50: 666c 6167 2032 2e0a 2020 2020 2020 2020  flag 2..        
-00035c60: 2020 2020 2020 2020 2d20 2020 5365 7175          -   Sequ
-00035c70: 656e 6365 7246 6c61 672e 464c 4147 3320  encerFlag.FLAG3 
-00035c80: 2822 7365 7166 6c61 6733 2229 3a20 5265  ("seqflag3"): Re
-00035c90: 6164 7320 7061 7474 6572 6e20 7365 7175  ads pattern sequ
-00035ca0: 656e 6365 7220 666c 6167 2033 2e0a 0a0a  encer flag 3....
-00035cb0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00035cc0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00035cd0: 7565 2028 626f 6f6c 293a 2041 2042 6f6f  ue (bool): A Boo
-00035ce0: 6c65 616e 2074 6861 7420 696e 6469 6361  lean that indica
-00035cf0: 7465 7320 7468 6520 7374 6174 6520 6f66  tes the state of
-00035d00: 2074 6865 2070 6174 7465 726e 2073 6571   the pattern seq
-00035d10: 7565 6e63 6572 2066 6c61 6720 796f 7520  uencer flag you 
-00035d20: 7370 6563 6966 792e 0a0a 2020 2020 2020  specify...      
-00035d30: 2020 2727 270a 2020 2020 2020 2020 6966    '''.        if
-00035d40: 2074 7970 6528 666c 6167 2920 6973 206e   type(flag) is n
-00035d50: 6f74 2065 6e75 6d73 2e53 6571 7565 6e63  ot enums.Sequenc
-00035d60: 6572 466c 6167 3a0a 2020 2020 2020 2020  erFlag:.        
-00035d70: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
-00035d80: 726f 7228 2750 6172 616d 6574 6572 2066  ror('Parameter f
-00035d90: 6c61 6720 6d75 7374 2062 6520 6f66 2074  lag must be of t
-00035da0: 7970 6520 2720 2b20 7374 7228 656e 756d  ype ' + str(enum
-00035db0: 732e 5365 7175 656e 6365 7246 6c61 6729  s.SequencerFlag)
-00035dc0: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
-00035dd0: 3d20 7365 6c66 2e5f 696e 7465 7270 7265  = self._interpre
-00035de0: 7465 722e 7265 6164 5f73 6571 7565 6e63  ter.read_sequenc
-00035df0: 6572 5f66 6c61 6728 666c 6167 290a 2020  er_flag(flag).  
-00035e00: 2020 2020 2020 7265 7475 726e 2076 616c        return val
-00035e10: 7565 0a0a 2020 2020 4069 7669 5f73 796e  ue..    @ivi_syn
-00035e20: 6368 726f 6e69 7a65 640a 2020 2020 6465  chronized.    de
-00035e30: 6620 7265 6164 5f73 6571 7565 6e63 6572  f read_sequencer
-00035e40: 5f72 6567 6973 7465 7228 7365 6c66 2c20  _register(self, 
-00035e50: 7265 6729 3a0a 2020 2020 2020 2020 7227  reg):.        r'
-00035e60: 2727 7265 6164 5f73 6571 7565 6e63 6572  ''read_sequencer
-00035e70: 5f72 6567 6973 7465 720a 0a20 2020 2020  _register..     
-00035e80: 2020 2052 6561 6473 2074 6865 2076 616c     Reads the val
-00035e90: 7565 206f 6620 6120 7061 7474 6572 6e20  ue of a pattern 
-00035ea0: 7365 7175 656e 6365 7220 7265 6769 7374  sequencer regist
-00035eb0: 6572 2e20 5573 6520 7061 7474 6572 6e20  er. Use pattern 
-00035ec0: 7365 7175 656e 6365 7220 7265 6769 7374  sequencer regist
-00035ed0: 6572 7320 746f 2070 6173 7320 6e75 6d65  ers to pass nume
-00035ee0: 7269 6320 7661 6c75 6573 2062 6574 7765  ric values betwe
-00035ef0: 656e 2074 6865 2070 6174 7465 726e 2073  en the pattern s
-00035f00: 6571 7565 6e63 6572 2061 6e64 2061 2072  equencer and a r
-00035f10: 756e 7469 6d65 2074 6573 7420 7072 6f67  untime test prog
-00035f20: 7261 6d2e 2046 6f72 2065 7861 6d70 6c65  ram. For example
-00035f30: 2c20 796f 7520 6361 6e20 7573 6520 7468  , you can use th
-00035f40: 6973 206d 6574 686f 6420 746f 2072 6561  is method to rea
-00035f50: 6420 6120 7265 6769 7374 6572 206d 6f64  d a register mod
-00035f60: 6966 6965 6420 6279 2074 6865 2077 7269  ified by the wri
-00035f70: 7465 5f72 6567 206f 7063 6f64 6520 6475  te_reg opcode du
-00035f80: 7269 6e67 2061 2070 6174 7465 726e 2062  ring a pattern b
-00035f90: 7572 7374 2e0a 0a20 2020 2020 2020 2041  urst...        A
-00035fa0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00035fb0: 2072 6567 2028 656e 756d 732e 5365 7175   reg (enums.Sequ
-00035fc0: 656e 6365 7252 6567 6973 7465 7229 3a20  encerRegister): 
-00035fd0: 5468 6520 7365 7175 656e 6365 7220 7265  The sequencer re
-00035fe0: 6769 7374 6572 2074 6f20 7265 6164 2066  gister to read f
-00035ff0: 726f 6d2e 0a0a 2020 2020 2020 2020 2020  rom...          
-00036000: 2020 2020 2020 2d20 2020 5365 7175 656e        -   Sequen
-00036010: 6365 7252 6567 6973 7465 722e 5245 4749  cerRegister.REGI
-00036020: 5354 4552 3020 2822 7265 6730 2229 3a20  STER0 ("reg0"): 
-00036030: 5265 6164 7320 7365 7175 656e 6365 7220  Reads sequencer 
-00036040: 7265 6769 7374 6572 2030 2e0a 2020 2020  register 0..    
-00036050: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
-00036060: 5365 7175 656e 6365 7252 6567 6973 7465  SequencerRegiste
-00036070: 722e 5245 4749 5354 4552 3120 2822 7265  r.REGISTER1 ("re
-00036080: 6731 2229 3a20 5265 6164 7320 7365 7175  g1"): Reads sequ
-00036090: 656e 6365 7220 7265 6769 7374 6572 2031  encer register 1
-000360a0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000360b0: 2020 2d20 2020 5365 7175 656e 6365 7252    -   SequencerR
-000360c0: 6567 6973 7465 722e 5245 4749 5354 4552  egister.REGISTER
-000360d0: 3220 2822 7265 6732 2229 3a20 5265 6164  2 ("reg2"): Read
-000360e0: 7320 7365 7175 656e 6365 7220 7265 6769  s sequencer regi
-000360f0: 7374 6572 2032 2e0a 2020 2020 2020 2020  ster 2..        
-00036100: 2020 2020 2020 2020 2d20 2020 5365 7175          -   Sequ
-00036110: 656e 6365 7252 6567 6973 7465 722e 5245  encerRegister.RE
-00036120: 4749 5354 4552 3320 2822 7265 6733 2229  GISTER3 ("reg3")
-00036130: 3a20 5265 6164 7320 7365 7175 656e 6365  : Reads sequence
-00036140: 7220 7265 6769 7374 6572 2033 2e0a 2020  r register 3..  
-00036150: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00036160: 2020 5365 7175 656e 6365 7252 6567 6973    SequencerRegis
-00036170: 7465 722e 5245 4749 5354 4552 3420 2822  ter.REGISTER4 ("
-00036180: 7265 6734 2229 3a20 5265 6164 7320 7365  reg4"): Reads se
-00036190: 7175 656e 6365 7220 7265 6769 7374 6572  quencer register
-000361a0: 2034 2e0a 2020 2020 2020 2020 2020 2020   4..            
-000361b0: 2020 2020 2d20 2020 5365 7175 656e 6365      -   Sequence
-000361c0: 7252 6567 6973 7465 722e 5245 4749 5354  rRegister.REGIST
-000361d0: 4552 3520 2822 7265 6735 2229 3a20 5265  ER5 ("reg5"): Re
-000361e0: 6164 7320 7365 7175 656e 6365 7220 7265  ads sequencer re
-000361f0: 6769 7374 6572 2035 2e0a 2020 2020 2020  gister 5..      
-00036200: 2020 2020 2020 2020 2020 2d20 2020 5365            -   Se
-00036210: 7175 656e 6365 7252 6567 6973 7465 722e  quencerRegister.
-00036220: 5245 4749 5354 4552 3620 2822 7265 6736  REGISTER6 ("reg6
-00036230: 2229 3a20 5265 6164 7320 7365 7175 656e  "): Reads sequen
-00036240: 6365 7220 7265 6769 7374 6572 2036 2e0a  cer register 6..
-00036250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036260: 2d20 2020 5365 7175 656e 6365 7252 6567  -   SequencerReg
-00036270: 6973 7465 722e 5245 4749 5354 4552 3720  ister.REGISTER7 
-00036280: 2822 7265 6737 2229 3a20 5265 6164 7320  ("reg7"): Reads 
-00036290: 7365 7175 656e 6365 7220 7265 6769 7374  sequencer regist
-000362a0: 6572 2037 2e0a 2020 2020 2020 2020 2020  er 7..          
-000362b0: 2020 2020 2020 2d20 2020 5365 7175 656e        -   Sequen
-000362c0: 6365 7252 6567 6973 7465 722e 5245 4749  cerRegister.REGI
-000362d0: 5354 4552 3820 2822 7265 6738 2229 3a20  STER8 ("reg8"): 
-000362e0: 5265 6164 7320 7365 7175 656e 6365 7220  Reads sequencer 
-000362f0: 7265 6769 7374 6572 2038 2e0a 2020 2020  register 8..    
-00036300: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
-00036310: 5365 7175 656e 6365 7252 6567 6973 7465  SequencerRegiste
-00036320: 722e 5245 4749 5354 4552 3920 2822 7265  r.REGISTER9 ("re
-00036330: 6739 2229 3a20 5265 6164 7320 7365 7175  g9"): Reads sequ
-00036340: 656e 6365 7220 7265 6769 7374 6572 2039  encer register 9
-00036350: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00036360: 2020 2d20 2020 5365 7175 656e 6365 7252    -   SequencerR
-00036370: 6567 6973 7465 722e 5245 4749 5354 4552  egister.REGISTER
-00036380: 3130 2028 2272 6567 3130 2229 3a20 5265  10 ("reg10"): Re
-00036390: 6164 7320 7365 7175 656e 6365 7220 7265  ads sequencer re
-000363a0: 6769 7374 6572 2031 302e 0a20 2020 2020  gister 10..     
-000363b0: 2020 2020 2020 2020 2020 202d 2020 2053             -   S
-000363c0: 6571 7565 6e63 6572 5265 6769 7374 6572  equencerRegister
-000363d0: 2e52 4547 4953 5445 5231 3120 2822 7265  .REGISTER11 ("re
-000363e0: 6731 3122 293a 2052 6561 6473 2073 6571  g11"): Reads seq
-000363f0: 7565 6e63 6572 2072 6567 6973 7465 7220  uencer register 
-00036400: 3131 2e0a 2020 2020 2020 2020 2020 2020  11..            
-00036410: 2020 2020 2d20 2020 5365 7175 656e 6365      -   Sequence
-00036420: 7252 6567 6973 7465 722e 5245 4749 5354  rRegister.REGIST
-00036430: 4552 3132 2028 2272 6567 3132 2229 3a20  ER12 ("reg12"): 
-00036440: 5265 6164 7320 7365 7175 656e 6365 7220  Reads sequencer 
-00036450: 7265 6769 7374 6572 2031 322e 0a20 2020  register 12..   
-00036460: 2020 2020 2020 2020 2020 2020 202d 2020               -  
-00036470: 2053 6571 7565 6e63 6572 5265 6769 7374   SequencerRegist
-00036480: 6572 2e52 4547 4953 5445 5231 3320 2822  er.REGISTER13 ("
-00036490: 7265 6731 3322 293a 2052 6561 6473 2073  reg13"): Reads s
-000364a0: 6571 7565 6e63 6572 2072 6567 6973 7465  equencer registe
-000364b0: 7220 3133 2e0a 2020 2020 2020 2020 2020  r 13..          
-000364c0: 2020 2020 2020 2d20 2020 5365 7175 656e        -   Sequen
-000364d0: 6365 7252 6567 6973 7465 722e 5245 4749  cerRegister.REGI
-000364e0: 5354 4552 3134 2028 2272 6567 3134 2229  STER14 ("reg14")
-000364f0: 3a20 5265 6164 7320 7365 7175 656e 6365  : Reads sequence
-00036500: 7220 7265 6769 7374 6572 2031 342e 0a20  r register 14.. 
-00036510: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00036520: 2020 2053 6571 7565 6e63 6572 5265 6769     SequencerRegi
-00036530: 7374 6572 2e52 4547 4953 5445 5231 3520  ster.REGISTER15 
-00036540: 2822 7265 6731 3522 293a 2052 6561 6473  ("reg15"): Reads
-00036550: 2073 6571 7565 6e63 6572 2072 6567 6973   sequencer regis
-00036560: 7465 7220 3135 2e0a 0a0a 2020 2020 2020  ter 15....      
-00036570: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00036580: 2020 2020 2020 2076 616c 7565 2028 696e         value (in
-00036590: 7429 3a20 5661 6c75 6520 7265 6164 2066  t): Value read f
-000365a0: 726f 6d20 7468 6520 7365 7175 656e 6365  rom the sequence
-000365b0: 7220 7265 6769 7374 6572 2e0a 0a20 2020  r register...   
-000365c0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-000365d0: 2069 6620 7479 7065 2872 6567 2920 6973   if type(reg) is
-000365e0: 206e 6f74 2065 6e75 6d73 2e53 6571 7565   not enums.Seque
-000365f0: 6e63 6572 5265 6769 7374 6572 3a0a 2020  ncerRegister:.  
-00036600: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00036610: 5479 7065 4572 726f 7228 2750 6172 616d  TypeError('Param
-00036620: 6574 6572 2072 6567 206d 7573 7420 6265  eter reg must be
-00036630: 206f 6620 7479 7065 2027 202b 2073 7472   of type ' + str
-00036640: 2865 6e75 6d73 2e53 6571 7565 6e63 6572  (enums.Sequencer
-00036650: 5265 6769 7374 6572 2929 0a20 2020 2020  Register)).     
-00036660: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
-00036670: 5f69 6e74 6572 7072 6574 6572 2e72 6561  _interpreter.rea
-00036680: 645f 7365 7175 656e 6365 725f 7265 6769  d_sequencer_regi
-00036690: 7374 6572 2872 6567 290a 2020 2020 2020  ster(reg).      
-000366a0: 2020 7265 7475 726e 2076 616c 7565 0a0a    return value..
-000366b0: 2020 2020 4069 7669 5f73 796e 6368 726f      @ivi_synchro
-000366c0: 6e69 7a65 640a 2020 2020 6465 6620 7265  nized.    def re
-000366d0: 7365 745f 6465 7669 6365 2873 656c 6629  set_device(self)
-000366e0: 3a0a 2020 2020 2020 2020 7227 2727 7265  :.        r'''re
-000366f0: 7365 745f 6465 7669 6365 0a0a 2020 2020  set_device..    
-00036700: 2020 2020 5265 7475 726e 7320 6120 6469      Returns a di
-00036710: 6769 7461 6c20 7061 7474 6572 6e20 696e  gital pattern in
-00036720: 7374 7275 6d65 6e74 2074 6f20 6120 6b6e  strument to a kn
-00036730: 6f77 6e20 7374 6174 652e 2054 6869 7320  own state. This 
-00036740: 6d65 7468 6f64 2070 6572 666f 726d 7320  method performs 
-00036750: 7468 6520 666f 6c6c 6f77 696e 6720 6163  the following ac
-00036760: 7469 6f6e 733a 0a0a 2020 2020 2020 2020  tions:..        
-00036770: 2d20 4162 6f72 7473 2070 6174 7465 726e  - Aborts pattern
-00036780: 2065 7865 6375 7469 6f6e 2e0a 2020 2020   execution..    
-00036790: 2020 2020 2d20 436c 6561 7273 2070 696e      - Clears pin
-000367a0: 206d 6170 732c 2074 696d 6520 7365 7473   maps, time sets
-000367b0: 2c20 736f 7572 6365 2061 6e64 2063 6170  , source and cap
-000367c0: 7475 7265 2077 6176 6566 6f72 6d73 2c20  ture waveforms, 
-000367d0: 616e 6420 7061 7474 6572 6e73 2e0a 2020  and patterns..  
-000367e0: 2020 2020 2020 2d20 5265 7365 7473 2061        - Resets a
-000367f0: 6c6c 2070 726f 7065 7274 6965 7320 746f  ll properties to
-00036800: 2064 6566 6175 6c74 2076 616c 7565 732c   default values,
-00036810: 2069 6e63 6c75 6469 6e67 2074 6865 2073   including the s
-00036820: 656c 6563 7465 645f 6675 6e63 7469 6f6e  elected_function
-00036830: 2070 726f 7065 7274 7920 7468 6174 2069   property that i
-00036840: 7320 7365 7420 746f 2053 656c 6563 7465  s set to Selecte
-00036850: 6446 756e 6374 696f 6e2e 4449 5343 4f4e  dFunction.DISCON
-00036860: 4e45 4354 2c20 6361 7573 696e 6720 7468  NECT, causing th
-00036870: 6520 492f 4f20 7377 6974 6368 6573 2074  e I/O switches t
-00036880: 6f20 6f70 656e 2e0a 2020 2020 2020 2020  o open..        
-00036890: 2d20 5374 6f70 7320 6578 706f 7274 206f  - Stops export o
-000368a0: 6620 616c 6c20 6578 7465 726e 616c 2073  f all external s
-000368b0: 6967 6e61 6c73 2061 6e64 2065 7665 6e74  ignals and event
-000368c0: 732e 0a20 2020 2020 2020 202d 2043 6c65  s..        - Cle
-000368d0: 6172 7320 6f76 6572 2d74 656d 7065 7261  ars over-tempera
-000368e0: 7475 7265 2061 6e64 206f 7665 722d 706f  ture and over-po
-000368f0: 7765 7220 636f 6e64 6974 696f 6e73 2e0a  wer conditions..
-00036900: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00036910: 2020 2020 7365 6c66 2e5f 696e 7465 7270      self._interp
-00036920: 7265 7465 722e 7265 7365 745f 6465 7669  reter.reset_devi
-00036930: 6365 2829 0a0a 2020 2020 4069 7669 5f73  ce()..    @ivi_s
-00036940: 796e 6368 726f 6e69 7a65 640a 2020 2020  ynchronized.    
-00036950: 6465 6620 7365 6c66 5f63 616c 6962 7261  def self_calibra
-00036960: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00036970: 2020 7227 2727 7365 6c66 5f63 616c 6962    r'''self_calib
-00036980: 7261 7465 0a0a 2020 2020 2020 2020 5065  rate..        Pe
-00036990: 7266 6f72 6d73 2073 656c 662d 6361 6c69  rforms self-cali
-000369a0: 6272 6174 696f 6e20 6f6e 2061 2064 6967  bration on a dig
-000369b0: 6974 616c 2070 6174 7465 726e 2069 6e73  ital pattern ins
-000369c0: 7472 756d 656e 742e 0a20 2020 2020 2020  trument..       
-000369d0: 2027 2727 0a20 2020 2020 2020 2073 656c   '''.        sel
-000369e0: 662e 5f69 6e74 6572 7072 6574 6572 2e73  f._interpreter.s
-000369f0: 656c 665f 6361 6c69 6272 6174 6528 290a  elf_calibrate().
-00036a00: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
-00036a10: 6f6e 697a 6564 0a20 2020 2064 6566 2073  onized.    def s
-00036a20: 656e 645f 736f 6674 7761 7265 5f65 6467  end_software_edg
-00036a30: 655f 7472 6967 6765 7228 7365 6c66 2c20  e_trigger(self, 
-00036a40: 7472 6967 6765 722c 2074 7269 6767 6572  trigger, trigger
-00036a50: 5f69 6465 6e74 6966 6965 7229 3a0a 2020  _identifier):.  
-00036a60: 2020 2020 2020 7227 2727 7365 6e64 5f73        r'''send_s
-00036a70: 6f66 7477 6172 655f 6564 6765 5f74 7269  oftware_edge_tri
-00036a80: 6767 6572 0a0a 2020 2020 2020 2020 466f  gger..        Fo
-00036a90: 7263 6573 2061 2070 6172 7469 6375 6c61  rces a particula
-00036aa0: 7220 6564 6765 2d62 6173 6564 2074 7269  r edge-based tri
-00036ab0: 6767 6572 2074 6f20 6f63 6375 7220 7265  gger to occur re
-00036ac0: 6761 7264 6c65 7373 206f 6620 686f 7720  gardless of how 
-00036ad0: 7468 6520 7370 6563 6966 6965 6420 7472  the specified tr
-00036ae0: 6967 6765 7220 6973 2063 6f6e 6669 6775  igger is configu
-00036af0: 7265 642e 2059 6f75 2063 616e 2075 7365  red. You can use
-00036b00: 2074 6869 7320 6d65 7468 6f64 2061 7320   this method as 
-00036b10: 6120 736f 6674 7761 7265 206f 7665 7272  a software overr
-00036b20: 6964 652e 0a0a 2020 2020 2020 2020 4172  ide...        Ar
-00036b30: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00036b40: 7472 6967 6765 7220 2865 6e75 6d73 2e53  trigger (enums.S
-00036b50: 6f66 7477 6172 6554 7269 6767 6572 293a  oftwareTrigger):
-00036b60: 2054 7269 6767 6572 2073 7065 6369 6669   Trigger specifi
-00036b70: 6573 2074 6865 2074 7269 6767 6572 2079  es the trigger y
-00036b80: 6f75 2077 616e 7420 746f 206f 7665 7272  ou want to overr
-00036b90: 6964 652e 0a0a 2020 2020 2020 2020 2020  ide...          
-00036ba0: 2020 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2d        +---------
+00034aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
+00034ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00034ac0: 202e 2e20 7c4e 6f74 657c 2069 6d61 6765   .. |Note| image
+00034ad0: 3a3a 206e 6f74 652e 6769 660a 0a20 2020  :: note.gif..   
+00034ae0: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
+00034af0: 653a 0a0a 2020 2020 2020 2020 2020 2020  e:..            
+00034b00: 6964 5f71 7565 7279 2028 626f 6f6c 293a  id_query (bool):
+00034b10: 2041 2042 6f6f 6c65 616e 2074 6861 7420   A Boolean that 
+00034b20: 7665 7269 6669 6573 2074 6861 7420 7468  verifies that th
+00034b30: 6520 6469 6769 7461 6c20 7061 7474 6572  e digital patter
+00034b40: 6e20 696e 7374 7275 6d65 6e74 2079 6f75  n instrument you
+00034b50: 2069 6e69 7469 616c 697a 6520 6973 2073   initialize is s
+00034b60: 7570 706f 7274 6564 2062 7920 4e49 2d44  upported by NI-D
+00034b70: 6967 6974 616c 2e20 4e49 2d44 6967 6974  igital. NI-Digit
+00034b80: 616c 2061 7574 6f6d 6174 6963 616c 6c79  al automatically
+00034b90: 2070 6572 666f 726d 7320 7468 6973 2071   performs this q
+00034ba0: 7565 7279 2c20 736f 2073 6574 7469 6e67  uery, so setting
+00034bb0: 2074 6869 7320 7061 7261 6d65 7465 7220   this parameter 
+00034bc0: 6973 206e 6f74 206e 6563 6573 7361 7279  is not necessary
+00034bd0: 2e0a 0a20 2020 2020 2020 2020 2020 2072  ...            r
+00034be0: 6573 6574 5f64 6576 6963 6520 2862 6f6f  eset_device (boo
+00034bf0: 6c29 3a20 4120 426f 6f6c 6561 6e20 7468  l): A Boolean th
+00034c00: 6174 2073 7065 6369 6669 6573 2077 6865  at specifies whe
+00034c10: 7468 6572 2074 6f20 7265 7365 7420 6120  ther to reset a 
+00034c20: 6469 6769 7461 6c20 7061 7474 6572 6e20  digital pattern 
+00034c30: 696e 7374 7275 6d65 6e74 2074 6f20 6120  instrument to a 
+00034c40: 6b6e 6f77 6e20 7374 6174 6520 7768 656e  known state when
+00034c50: 2074 6865 2073 6573 7369 6f6e 2069 7320   the session is 
+00034c60: 696e 6974 6961 6c69 7a65 642e 2053 6574  initialized. Set
+00034c70: 7469 6e67 2074 6865 202a 2a72 6573 6574  ting the **reset
+00034c80: 4465 7669 6365 2a2a 2076 616c 7565 2074  Device** value t
+00034c90: 6f20 5472 7565 2069 7320 6571 7569 7661  o True is equiva
+00034ca0: 6c65 6e74 2074 6f20 6361 6c6c 696e 6720  lent to calling 
+00034cb0: 7468 6520 7265 7365 7420 6d65 7468 6f64  the reset method
+00034cc0: 2069 6d6d 6564 6961 7465 6c79 2061 6674   immediately aft
+00034cd0: 6572 2069 6e69 7469 616c 697a 696e 6720  er initializing 
+00034ce0: 7468 6520 7365 7373 696f 6e2e 0a0a 2020  the session...  
+00034cf0: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+00034d00: 5f73 7472 696e 6720 2864 6963 7429 3a20  _string (dict): 
+00034d10: 5468 6520 696e 6974 6961 6c20 7661 6c75  The initial valu
+00034d20: 6573 206f 6620 6365 7274 6169 6e20 7072  es of certain pr
+00034d30: 6f70 6572 7469 6573 2066 6f72 2074 6865  operties for the
+00034d40: 204e 492d 4469 6769 7461 6c20 5061 7474   NI-Digital Patt
+00034d50: 6572 6e20 4472 6976 6572 2073 6573 7369  ern Driver sessi
+00034d60: 6f6e 2e20 5468 6520 7374 7269 6e67 2063  on. The string c
+00034d70: 616e 2062 6520 656d 7074 792e 2059 6f75  an be empty. You
+00034d80: 2063 616e 2075 7365 2074 6865 2044 7269   can use the Dri
+00034d90: 7665 7253 6574 7570 2066 6c61 6720 746f  verSetup flag to
+00034da0: 2073 696d 756c 6174 6520 6120 6469 6769   simulate a digi
+00034db0: 7461 6c20 7061 7474 6572 6e20 696e 7374  tal pattern inst
+00034dc0: 7275 6d65 6e74 2e20 5768 656e 2073 696d  rument. When sim
+00034dd0: 756c 6174 696e 6720 6120 6469 6769 7461  ulating a digita
+00034de0: 6c20 7061 7474 6572 6e20 696e 7374 7275  l pattern instru
+00034df0: 6d65 6e74 2c20 796f 7520 6d75 7374 2073  ment, you must s
+00034e00: 7065 6369 6679 2074 6865 206d 6f64 656c  pecify the model
+00034e10: 2079 6f75 2077 616e 7420 746f 2073 696d   you want to sim
+00034e20: 756c 6174 652e 2046 6f72 2065 7861 6d70  ulate. For examp
+00034e30: 6c65 2c20 5369 6d75 6c61 7465 203d 2031  le, Simulate = 1
+00034e40: 2c20 4472 6976 6572 5365 7475 7020 3d20  , DriverSetup = 
+00034e50: 4d6f 6465 6c3a 3635 3730 2e0a 0a0a 2020  Model:6570....  
+00034e60: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00034e70: 2020 2020 2020 2020 2020 206e 6577 5f76             new_v
+00034e80: 6920 2869 6e74 293a 2054 6865 2072 6574  i (int): The ret
+00034e90: 7572 6e65 6420 696e 7374 7275 6d65 6e74  urned instrument
+00034ea0: 2073 6573 7369 6f6e 2e0a 0a20 2020 2020   session...     
+00034eb0: 2020 2027 2727 0a20 2020 2020 2020 206f     '''.        o
+00034ec0: 7074 696f 6e5f 7374 7269 6e67 203d 205f  ption_string = _
+00034ed0: 636f 6e76 6572 7465 7273 2e63 6f6e 7665  converters.conve
+00034ee0: 7274 5f69 6e69 745f 7769 7468 5f6f 7074  rt_init_with_opt
+00034ef0: 696f 6e73 5f64 6963 7469 6f6e 6172 7928  ions_dictionary(
+00034f00: 6f70 7469 6f6e 5f73 7472 696e 6729 0a20  option_string). 
+00034f10: 2020 2020 2020 206e 6577 5f76 6920 3d20         new_vi = 
+00034f20: 7365 6c66 2e5f 696e 7465 7270 7265 7465  self._interprete
+00034f30: 722e 696e 6974 5f77 6974 685f 6f70 7469  r.init_with_opti
+00034f40: 6f6e 7328 7265 736f 7572 6365 5f6e 616d  ons(resource_nam
+00034f50: 652c 2069 645f 7175 6572 792c 2072 6573  e, id_query, res
+00034f60: 6574 5f64 6576 6963 652c 206f 7074 696f  et_device, optio
+00034f70: 6e5f 7374 7269 6e67 290a 2020 2020 2020  n_string).      
+00034f80: 2020 7265 7475 726e 206e 6577 5f76 690a    return new_vi.
+00034f90: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
+00034fa0: 6f6e 697a 6564 0a20 2020 2064 6566 205f  onized.    def _
+00034fb0: 696e 6974 6961 7465 2873 656c 6629 3a0a  initiate(self):.
+00034fc0: 2020 2020 2020 2020 7227 2727 5f69 6e69          r'''_ini
+00034fd0: 7469 6174 650a 0a20 2020 2020 2020 2053  tiate..        S
+00034fe0: 7461 7274 7320 6275 7273 7469 6e67 2074  tarts bursting t
+00034ff0: 6865 2070 6174 7465 726e 2063 6f6e 6669  he pattern confi
+00035000: 6775 7265 6420 6279 2073 7461 7274 5f6c  gured by start_l
+00035010: 6162 656c 2c20 6361 7573 696e 6720 7468  abel, causing th
+00035020: 6520 4e49 2d44 6967 6974 616c 2073 6573  e NI-Digital ses
+00035030: 7369 6f6e 2074 6f20 6265 2063 6f6d 6d69  sion to be commi
+00035040: 7474 6564 2e20 546f 2073 746f 7020 7468  tted. To stop th
+00035050: 6520 7061 7474 6572 6e20 6275 7273 742c  e pattern burst,
+00035060: 2063 616c 6c20 6162 6f72 742e 2049 6620   call abort. If 
+00035070: 6b65 6570 2061 6c69 7665 2070 6174 7465  keep alive patte
+00035080: 726e 2069 7320 6275 7273 7469 6e67 2077  rn is bursting w
+00035090: 6865 6e20 6162 6f72 7420 6973 2063 616c  hen abort is cal
+000350a0: 6c65 6420 6f72 2075 706f 6e20 6578 6974  led or upon exit
+000350b0: 696e 6720 7468 6520 636f 6e74 6578 7420  ing the context 
+000350c0: 6d61 6e61 6765 722c 206b 6565 7020 616c  manager, keep al
+000350d0: 6976 6520 7061 7474 6572 6e20 7769 6c6c  ive pattern will
+000350e0: 206e 6f74 2062 6520 7374 6f70 7065 642e   not be stopped.
+000350f0: 2054 6f20 7374 6f70 2074 6865 206b 6565   To stop the kee
+00035100: 7020 616c 6976 6520 7061 7474 6572 6e2c  p alive pattern,
+00035110: 2063 616c 6c20 6162 6f72 745f 6b65 6570   call abort_keep
+00035120: 5f61 6c69 7665 2e0a 2020 2020 2020 2020  _alive..        
+00035130: 2727 270a 2020 2020 2020 2020 7365 6c66  '''.        self
+00035140: 2e5f 696e 7465 7270 7265 7465 722e 696e  ._interpreter.in
+00035150: 6974 6961 7465 2829 0a0a 2020 2020 4069  itiate()..    @i
+00035160: 7669 5f73 796e 6368 726f 6e69 7a65 640a  vi_synchronized.
+00035170: 2020 2020 6465 6620 6973 5f64 6f6e 6528      def is_done(
+00035180: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00035190: 2727 2769 735f 646f 6e65 0a0a 2020 2020  '''is_done..    
+000351a0: 2020 2020 4368 6563 6b73 2074 6865 2068      Checks the h
+000351b0: 6172 6477 6172 6520 746f 2064 6574 6572  ardware to deter
+000351c0: 6d69 6e65 2069 6620 7468 6520 7061 7474  mine if the patt
+000351d0: 6572 6e20 6275 7273 7420 6861 7320 636f  ern burst has co
+000351e0: 6d70 6c65 7465 6420 6f72 2069 6620 616e  mpleted or if an
+000351f0: 7920 6572 726f 7273 2068 6176 6520 6f63  y errors have oc
+00035200: 6375 7272 6564 2e0a 0a20 2020 2020 2020  curred...       
+00035210: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00035220: 2020 2020 2020 646f 6e65 2028 626f 6f6c        done (bool
+00035230: 293a 2041 2042 6f6f 6c65 616e 2074 6861  ): A Boolean tha
+00035240: 7420 696e 6469 6361 7465 7320 7768 6574  t indicates whet
+00035250: 6865 7220 7468 6520 7061 7474 6572 6e20  her the pattern 
+00035260: 6275 7273 7420 636f 6d70 6c65 7465 642e  burst completed.
+00035270: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00035280: 2020 2020 2020 646f 6e65 203d 2073 656c        done = sel
+00035290: 662e 5f69 6e74 6572 7072 6574 6572 2e69  f._interpreter.i
+000352a0: 735f 646f 6e65 2829 0a20 2020 2020 2020  s_done().       
+000352b0: 2072 6574 7572 6e20 646f 6e65 0a0a 2020   return done..  
+000352c0: 2020 4069 7669 5f73 796e 6368 726f 6e69    @ivi_synchroni
+000352d0: 7a65 640a 2020 2020 6465 6620 5f6c 6f61  zed.    def _loa
+000352e0: 645f 6c65 7665 6c73 2873 656c 662c 2066  d_levels(self, f
+000352f0: 696c 655f 7061 7468 293a 0a20 2020 2020  ile_path):.     
+00035300: 2020 2072 2727 275f 6c6f 6164 5f6c 6576     r'''_load_lev
+00035310: 656c 730a 0a20 2020 2020 2020 204c 6f61  els..        Loa
+00035320: 6473 2061 206c 6576 656c 7320 7368 6565  ds a levels shee
+00035330: 7420 6672 6f6d 2061 2073 7065 6369 6669  t from a specifi
+00035340: 6564 2066 696c 652e 0a0a 2020 2020 2020  ed file...      
+00035350: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00035360: 2020 2020 6669 6c65 5f70 6174 6820 2873      file_path (s
+00035370: 7472 293a 2041 6273 6f6c 7574 6520 6669  tr): Absolute fi
+00035380: 6c65 2070 6174 6820 746f 2074 6865 2073  le path to the s
+00035390: 7065 6369 6669 6564 206c 6576 656c 7320  pecified levels 
+000353a0: 7368 6565 7420 6669 6c65 2e0a 0a20 2020  sheet file...   
+000353b0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+000353c0: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
+000353d0: 6572 2e6c 6f61 645f 6c65 7665 6c73 2866  er.load_levels(f
+000353e0: 696c 655f 7061 7468 290a 0a20 2020 2040  ile_path)..    @
+000353f0: 6976 695f 7379 6e63 6872 6f6e 697a 6564  ivi_synchronized
+00035400: 0a20 2020 2064 6566 206c 6f61 645f 7061  .    def load_pa
+00035410: 7474 6572 6e28 7365 6c66 2c20 6669 6c65  ttern(self, file
+00035420: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
+00035430: 7227 2727 6c6f 6164 5f70 6174 7465 726e  r'''load_pattern
+00035440: 0a0a 2020 2020 2020 2020 4c6f 6164 7320  ..        Loads 
+00035450: 7468 6520 7370 6563 6966 6965 6420 7061  the specified pa
+00035460: 7474 6572 6e20 6669 6c65 2e0a 0a20 2020  ttern file...   
+00035470: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00035480: 2020 2020 2020 2066 696c 655f 7061 7468         file_path
+00035490: 2028 7374 7229 3a20 4162 736f 6c75 7465   (str): Absolute
+000354a0: 2066 696c 6520 7061 7468 206f 6620 7468   file path of th
+000354b0: 6520 6269 6e61 7279 202e 6469 6769 7061  e binary .digipa
+000354c0: 7420 7061 7474 6572 6e20 6669 6c65 2074  t pattern file t
+000354d0: 6f20 6c6f 6164 2e20 5370 6563 6966 7920  o load. Specify 
+000354e0: 7468 6520 7061 7474 6572 6e20 746f 2062  the pattern to b
+000354f0: 7572 7374 2075 7369 6e67 2073 7461 7274  urst using start
+00035500: 5f6c 6162 656c 206f 7220 7468 6520 7374  _label or the st
+00035510: 6172 745f 6c61 6265 6c20 7061 7261 6d65  art_label parame
+00035520: 7465 7220 6f66 2074 6865 2062 7572 7374  ter of the burst
+00035530: 5f70 6174 7465 726e 206d 6574 686f 642e  _pattern method.
+00035540: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00035550: 2020 2020 2020 7365 6c66 2e5f 696e 7465        self._inte
+00035560: 7270 7265 7465 722e 6c6f 6164 5f70 6174  rpreter.load_pat
+00035570: 7465 726e 2866 696c 655f 7061 7468 290a  tern(file_path).
+00035580: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
+00035590: 6f6e 697a 6564 0a20 2020 2064 6566 206c  onized.    def l
+000355a0: 6f61 645f 7069 6e5f 6d61 7028 7365 6c66  oad_pin_map(self
+000355b0: 2c20 6669 6c65 5f70 6174 6829 3a0a 2020  , file_path):.  
+000355c0: 2020 2020 2020 7227 2727 6c6f 6164 5f70        r'''load_p
+000355d0: 696e 5f6d 6170 0a0a 2020 2020 2020 2020  in_map..        
+000355e0: 4c6f 6164 7320 6120 7069 6e20 6d61 7020  Loads a pin map 
+000355f0: 6669 6c65 2e20 596f 7520 6361 6e20 6c6f  file. You can lo
+00035600: 6164 206f 6e6c 7920 6120 7369 6e67 6c65  ad only a single
+00035610: 2070 696e 2061 6e64 2063 6861 6e6e 656c   pin and channel
+00035620: 206d 6170 2066 696c 6520 6475 7269 6e67   map file during
+00035630: 2061 6e20 4e49 2d44 6967 6974 616c 2050   an NI-Digital P
+00035640: 6174 7465 726e 2044 7269 7665 7220 7365  attern Driver se
+00035650: 7373 696f 6e2e 2054 6f20 7377 6974 6368  ssion. To switch
+00035660: 2070 696e 206d 6170 732c 2063 7265 6174   pin maps, creat
+00035670: 6520 6120 6e65 7720 7365 7373 696f 6e20  e a new session 
+00035680: 6f72 2063 616c 6c20 7468 6520 7265 7365  or call the rese
+00035690: 7420 6d65 7468 6f64 2e0a 0a20 2020 2020  t method...     
+000356a0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000356b0: 2020 2020 2066 696c 655f 7061 7468 2028       file_path (
+000356c0: 7374 7229 3a20 4162 736f 6c75 7465 2066  str): Absolute f
+000356d0: 696c 6520 7061 7468 2074 6f20 6120 7069  ile path to a pi
+000356e0: 6e20 6d61 7020 6669 6c65 2063 7265 6174  n map file creat
+000356f0: 6564 2077 6974 6820 7468 6520 4469 6769  ed with the Digi
+00035700: 7461 6c20 5061 7474 6572 6e20 4564 6974  tal Pattern Edit
+00035710: 6f72 206f 7220 7468 6520 4e49 2054 6573  or or the NI Tes
+00035720: 7453 7461 6e64 2053 656d 6963 6f6e 6475  tStand Semicondu
+00035730: 6374 6f72 204d 6f64 756c 652e 0a0a 2020  ctor Module...  
+00035740: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00035750: 2020 7365 6c66 2e5f 696e 7465 7270 7265    self._interpre
+00035760: 7465 722e 6c6f 6164 5f70 696e 5f6d 6170  ter.load_pin_map
+00035770: 2866 696c 655f 7061 7468 290a 0a20 2020  (file_path)..   
+00035780: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
+00035790: 6564 0a20 2020 2064 6566 205f 6c6f 6164  ed.    def _load
+000357a0: 5f73 7065 6369 6669 6361 7469 6f6e 7328  _specifications(
+000357b0: 7365 6c66 2c20 6669 6c65 5f70 6174 6829  self, file_path)
+000357c0: 3a0a 2020 2020 2020 2020 7227 2727 5f6c  :.        r'''_l
+000357d0: 6f61 645f 7370 6563 6966 6963 6174 696f  oad_specificatio
+000357e0: 6e73 0a0a 2020 2020 2020 2020 4c6f 6164  ns..        Load
+000357f0: 7320 6120 7370 6563 6966 6963 6174 696f  s a specificatio
+00035800: 6e73 2073 6865 6574 2066 726f 6d20 6120  ns sheet from a 
+00035810: 7370 6563 6966 6965 6420 6669 6c65 2e0a  specified file..
+00035820: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00035830: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+00035840: 7061 7468 2028 7374 7229 3a20 4162 736f  path (str): Abso
+00035850: 6c75 7465 2066 696c 6520 7061 7468 2074  lute file path t
+00035860: 6f20 6120 7370 6563 6966 6963 6174 696f  o a specificatio
+00035870: 6e73 2066 696c 652e 0a0a 2020 2020 2020  ns file...      
+00035880: 2020 2727 270a 2020 2020 2020 2020 7365    '''.        se
+00035890: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
+000358a0: 6c6f 6164 5f73 7065 6369 6669 6361 7469  load_specificati
+000358b0: 6f6e 7328 6669 6c65 5f70 6174 6829 0a0a  ons(file_path)..
+000358c0: 2020 2020 4069 7669 5f73 796e 6368 726f      @ivi_synchro
+000358d0: 6e69 7a65 640a 2020 2020 6465 6620 5f6c  nized.    def _l
+000358e0: 6f61 645f 7469 6d69 6e67 2873 656c 662c  oad_timing(self,
+000358f0: 2066 696c 655f 7061 7468 293a 0a20 2020   file_path):.   
+00035900: 2020 2020 2072 2727 275f 6c6f 6164 5f74       r'''_load_t
+00035910: 696d 696e 670a 0a20 2020 2020 2020 204c  iming..        L
+00035920: 6f61 6473 2061 2074 696d 696e 6720 7368  oads a timing sh
+00035930: 6565 7420 6672 6f6d 2061 2073 7065 6369  eet from a speci
+00035940: 6669 6564 2066 696c 652e 0a0a 2020 2020  fied file...    
+00035950: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00035960: 2020 2020 2020 6669 6c65 5f70 6174 6820        file_path 
+00035970: 2873 7472 293a 2041 6273 6f6c 7574 6520  (str): Absolute 
+00035980: 6669 6c65 2070 6174 6820 746f 2074 6865  file path to the
+00035990: 2073 7065 6369 6669 6564 2074 696d 696e   specified timin
+000359a0: 6720 7368 6565 7420 6669 6c65 2e0a 0a20  g sheet file... 
+000359b0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+000359c0: 2020 2073 656c 662e 5f69 6e74 6572 7072     self._interpr
+000359d0: 6574 6572 2e6c 6f61 645f 7469 6d69 6e67  eter.load_timing
+000359e0: 2866 696c 655f 7061 7468 290a 0a20 2020  (file_path)..   
+000359f0: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
+00035a00: 6564 0a20 2020 2064 6566 2072 6561 645f  ed.    def read_
+00035a10: 7365 7175 656e 6365 725f 666c 6167 2873  sequencer_flag(s
+00035a20: 656c 662c 2066 6c61 6729 3a0a 2020 2020  elf, flag):.    
+00035a30: 2020 2020 7227 2727 7265 6164 5f73 6571      r'''read_seq
+00035a40: 7565 6e63 6572 5f66 6c61 670a 0a20 2020  uencer_flag..   
+00035a50: 2020 2020 2052 6561 6473 2074 6865 2073       Reads the s
+00035a60: 7461 7465 206f 6620 6120 7061 7474 6572  tate of a patter
+00035a70: 6e20 7365 7175 656e 6365 7220 666c 6167  n sequencer flag
+00035a80: 2e20 5573 6520 7061 7474 6572 6e20 7365  . Use pattern se
+00035a90: 7175 656e 6365 7220 666c 6167 7320 746f  quencer flags to
+00035aa0: 2063 6f6f 7264 696e 6174 6520 6578 6563   coordinate exec
+00035ab0: 7574 696f 6e20 6265 7477 6565 6e20 7468  ution between th
+00035ac0: 6520 7061 7474 6572 6e20 7365 7175 656e  e pattern sequen
+00035ad0: 6365 7220 616e 6420 6120 7275 6e74 696d  cer and a runtim
+00035ae0: 6520 7465 7374 2070 726f 6772 616d 2e0a  e test program..
+00035af0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00035b00: 2020 2020 2020 2020 2020 2066 6c61 6720             flag 
+00035b10: 2865 6e75 6d73 2e53 6571 7565 6e63 6572  (enums.Sequencer
+00035b20: 466c 6167 293a 2054 6865 2070 6174 7465  Flag): The patte
+00035b30: 726e 2073 6571 7565 6e63 6572 2066 6c61  rn sequencer fla
+00035b40: 6720 796f 7520 7761 6e74 2074 6f20 7265  g you want to re
+00035b50: 6164 2e0a 0a20 2020 2020 2020 2020 2020  ad...           
+00035b60: 2020 2020 202d 2020 2053 6571 7565 6e63       -   Sequenc
+00035b70: 6572 466c 6167 2e46 4c41 4730 2028 2273  erFlag.FLAG0 ("s
+00035b80: 6571 666c 6167 3022 293a 2052 6561 6473  eqflag0"): Reads
+00035b90: 2070 6174 7465 726e 2073 6571 7565 6e63   pattern sequenc
+00035ba0: 6572 2066 6c61 6720 302e 0a20 2020 2020  er flag 0..     
+00035bb0: 2020 2020 2020 2020 2020 202d 2020 2053             -   S
+00035bc0: 6571 7565 6e63 6572 466c 6167 2e46 4c41  equencerFlag.FLA
+00035bd0: 4731 2028 2273 6571 666c 6167 3122 293a  G1 ("seqflag1"):
+00035be0: 2052 6561 6473 2070 6174 7465 726e 2073   Reads pattern s
+00035bf0: 6571 7565 6e63 6572 2066 6c61 6720 312e  equencer flag 1.
+00035c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00035c10: 202d 2020 2053 6571 7565 6e63 6572 466c   -   SequencerFl
+00035c20: 6167 2e46 4c41 4732 2028 2273 6571 666c  ag.FLAG2 ("seqfl
+00035c30: 6167 3222 293a 2052 6561 6473 2070 6174  ag2"): Reads pat
+00035c40: 7465 726e 2073 6571 7565 6e63 6572 2066  tern sequencer f
+00035c50: 6c61 6720 322e 0a20 2020 2020 2020 2020  lag 2..         
+00035c60: 2020 2020 2020 202d 2020 2053 6571 7565         -   Seque
+00035c70: 6e63 6572 466c 6167 2e46 4c41 4733 2028  ncerFlag.FLAG3 (
+00035c80: 2273 6571 666c 6167 3322 293a 2052 6561  "seqflag3"): Rea
+00035c90: 6473 2070 6174 7465 726e 2073 6571 7565  ds pattern seque
+00035ca0: 6e63 6572 2066 6c61 6720 332e 0a0a 0a20  ncer flag 3.... 
+00035cb0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00035cc0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00035cd0: 6520 2862 6f6f 6c29 3a20 4120 426f 6f6c  e (bool): A Bool
+00035ce0: 6561 6e20 7468 6174 2069 6e64 6963 6174  ean that indicat
+00035cf0: 6573 2074 6865 2073 7461 7465 206f 6620  es the state of 
+00035d00: 7468 6520 7061 7474 6572 6e20 7365 7175  the pattern sequ
+00035d10: 656e 6365 7220 666c 6167 2079 6f75 2073  encer flag you s
+00035d20: 7065 6369 6679 2e0a 0a20 2020 2020 2020  pecify...       
+00035d30: 2027 2727 0a20 2020 2020 2020 2069 6620   '''.        if 
+00035d40: 7479 7065 2866 6c61 6729 2069 7320 6e6f  type(flag) is no
+00035d50: 7420 656e 756d 732e 5365 7175 656e 6365  t enums.Sequence
+00035d60: 7246 6c61 673a 0a20 2020 2020 2020 2020  rFlag:.         
+00035d70: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00035d80: 6f72 2827 5061 7261 6d65 7465 7220 666c  or('Parameter fl
+00035d90: 6167 206d 7573 7420 6265 206f 6620 7479  ag must be of ty
+00035da0: 7065 2027 202b 2073 7472 2865 6e75 6d73  pe ' + str(enums
+00035db0: 2e53 6571 7565 6e63 6572 466c 6167 2929  .SequencerFlag))
+00035dc0: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+00035dd0: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
+00035de0: 6572 2e72 6561 645f 7365 7175 656e 6365  er.read_sequence
+00035df0: 725f 666c 6167 2866 6c61 6729 0a20 2020  r_flag(flag).   
+00035e00: 2020 2020 2072 6574 7572 6e20 7661 6c75       return valu
+00035e10: 650a 0a20 2020 2040 6976 695f 7379 6e63  e..    @ivi_sync
+00035e20: 6872 6f6e 697a 6564 0a20 2020 2064 6566  hronized.    def
+00035e30: 2072 6561 645f 7365 7175 656e 6365 725f   read_sequencer_
+00035e40: 7265 6769 7374 6572 2873 656c 662c 2072  register(self, r
+00035e50: 6567 293a 0a20 2020 2020 2020 2072 2727  eg):.        r''
+00035e60: 2772 6561 645f 7365 7175 656e 6365 725f  'read_sequencer_
+00035e70: 7265 6769 7374 6572 0a0a 2020 2020 2020  register..      
+00035e80: 2020 5265 6164 7320 7468 6520 7661 6c75    Reads the valu
+00035e90: 6520 6f66 2061 2070 6174 7465 726e 2073  e of a pattern s
+00035ea0: 6571 7565 6e63 6572 2072 6567 6973 7465  equencer registe
+00035eb0: 722e 2055 7365 2070 6174 7465 726e 2073  r. Use pattern s
+00035ec0: 6571 7565 6e63 6572 2072 6567 6973 7465  equencer registe
+00035ed0: 7273 2074 6f20 7061 7373 206e 756d 6572  rs to pass numer
+00035ee0: 6963 2076 616c 7565 7320 6265 7477 6565  ic values betwee
+00035ef0: 6e20 7468 6520 7061 7474 6572 6e20 7365  n the pattern se
+00035f00: 7175 656e 6365 7220 616e 6420 6120 7275  quencer and a ru
+00035f10: 6e74 696d 6520 7465 7374 2070 726f 6772  ntime test progr
+00035f20: 616d 2e20 466f 7220 6578 616d 706c 652c  am. For example,
+00035f30: 2079 6f75 2063 616e 2075 7365 2074 6869   you can use thi
+00035f40: 7320 6d65 7468 6f64 2074 6f20 7265 6164  s method to read
+00035f50: 2061 2072 6567 6973 7465 7220 6d6f 6469   a register modi
+00035f60: 6669 6564 2062 7920 7468 6520 7772 6974  fied by the writ
+00035f70: 655f 7265 6720 6f70 636f 6465 2064 7572  e_reg opcode dur
+00035f80: 696e 6720 6120 7061 7474 6572 6e20 6275  ing a pattern bu
+00035f90: 7273 742e 0a0a 2020 2020 2020 2020 4172  rst...        Ar
+00035fa0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00035fb0: 7265 6720 2865 6e75 6d73 2e53 6571 7565  reg (enums.Seque
+00035fc0: 6e63 6572 5265 6769 7374 6572 293a 2054  ncerRegister): T
+00035fd0: 6865 2073 6571 7565 6e63 6572 2072 6567  he sequencer reg
+00035fe0: 6973 7465 7220 746f 2072 6561 6420 6672  ister to read fr
+00035ff0: 6f6d 2e0a 0a20 2020 2020 2020 2020 2020  om...           
+00036000: 2020 2020 202d 2020 2053 6571 7565 6e63       -   Sequenc
+00036010: 6572 5265 6769 7374 6572 2e52 4547 4953  erRegister.REGIS
+00036020: 5445 5230 2028 2272 6567 3022 293a 2052  TER0 ("reg0"): R
+00036030: 6561 6473 2073 6571 7565 6e63 6572 2072  eads sequencer r
+00036040: 6567 6973 7465 7220 302e 0a20 2020 2020  egister 0..     
+00036050: 2020 2020 2020 2020 2020 202d 2020 2053             -   S
+00036060: 6571 7565 6e63 6572 5265 6769 7374 6572  equencerRegister
+00036070: 2e52 4547 4953 5445 5231 2028 2272 6567  .REGISTER1 ("reg
+00036080: 3122 293a 2052 6561 6473 2073 6571 7565  1"): Reads seque
+00036090: 6e63 6572 2072 6567 6973 7465 7220 312e  ncer register 1.
+000360a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000360b0: 202d 2020 2053 6571 7565 6e63 6572 5265   -   SequencerRe
+000360c0: 6769 7374 6572 2e52 4547 4953 5445 5232  gister.REGISTER2
+000360d0: 2028 2272 6567 3222 293a 2052 6561 6473   ("reg2"): Reads
+000360e0: 2073 6571 7565 6e63 6572 2072 6567 6973   sequencer regis
+000360f0: 7465 7220 322e 0a20 2020 2020 2020 2020  ter 2..         
+00036100: 2020 2020 2020 202d 2020 2053 6571 7565         -   Seque
+00036110: 6e63 6572 5265 6769 7374 6572 2e52 4547  ncerRegister.REG
+00036120: 4953 5445 5233 2028 2272 6567 3322 293a  ISTER3 ("reg3"):
+00036130: 2052 6561 6473 2073 6571 7565 6e63 6572   Reads sequencer
+00036140: 2072 6567 6973 7465 7220 332e 0a20 2020   register 3..   
+00036150: 2020 2020 2020 2020 2020 2020 202d 2020               -  
+00036160: 2053 6571 7565 6e63 6572 5265 6769 7374   SequencerRegist
+00036170: 6572 2e52 4547 4953 5445 5234 2028 2272  er.REGISTER4 ("r
+00036180: 6567 3422 293a 2052 6561 6473 2073 6571  eg4"): Reads seq
+00036190: 7565 6e63 6572 2072 6567 6973 7465 7220  uencer register 
+000361a0: 342e 0a20 2020 2020 2020 2020 2020 2020  4..             
+000361b0: 2020 202d 2020 2053 6571 7565 6e63 6572     -   Sequencer
+000361c0: 5265 6769 7374 6572 2e52 4547 4953 5445  Register.REGISTE
+000361d0: 5235 2028 2272 6567 3522 293a 2052 6561  R5 ("reg5"): Rea
+000361e0: 6473 2073 6571 7565 6e63 6572 2072 6567  ds sequencer reg
+000361f0: 6973 7465 7220 352e 0a20 2020 2020 2020  ister 5..       
+00036200: 2020 2020 2020 2020 202d 2020 2053 6571           -   Seq
+00036210: 7565 6e63 6572 5265 6769 7374 6572 2e52  uencerRegister.R
+00036220: 4547 4953 5445 5236 2028 2272 6567 3622  EGISTER6 ("reg6"
+00036230: 293a 2052 6561 6473 2073 6571 7565 6e63  ): Reads sequenc
+00036240: 6572 2072 6567 6973 7465 7220 362e 0a20  er register 6.. 
+00036250: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00036260: 2020 2053 6571 7565 6e63 6572 5265 6769     SequencerRegi
+00036270: 7374 6572 2e52 4547 4953 5445 5237 2028  ster.REGISTER7 (
+00036280: 2272 6567 3722 293a 2052 6561 6473 2073  "reg7"): Reads s
+00036290: 6571 7565 6e63 6572 2072 6567 6973 7465  equencer registe
+000362a0: 7220 372e 0a20 2020 2020 2020 2020 2020  r 7..           
+000362b0: 2020 2020 202d 2020 2053 6571 7565 6e63       -   Sequenc
+000362c0: 6572 5265 6769 7374 6572 2e52 4547 4953  erRegister.REGIS
+000362d0: 5445 5238 2028 2272 6567 3822 293a 2052  TER8 ("reg8"): R
+000362e0: 6561 6473 2073 6571 7565 6e63 6572 2072  eads sequencer r
+000362f0: 6567 6973 7465 7220 382e 0a20 2020 2020  egister 8..     
+00036300: 2020 2020 2020 2020 2020 202d 2020 2053             -   S
+00036310: 6571 7565 6e63 6572 5265 6769 7374 6572  equencerRegister
+00036320: 2e52 4547 4953 5445 5239 2028 2272 6567  .REGISTER9 ("reg
+00036330: 3922 293a 2052 6561 6473 2073 6571 7565  9"): Reads seque
+00036340: 6e63 6572 2072 6567 6973 7465 7220 392e  ncer register 9.
+00036350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00036360: 202d 2020 2053 6571 7565 6e63 6572 5265   -   SequencerRe
+00036370: 6769 7374 6572 2e52 4547 4953 5445 5231  gister.REGISTER1
+00036380: 3020 2822 7265 6731 3022 293a 2052 6561  0 ("reg10"): Rea
+00036390: 6473 2073 6571 7565 6e63 6572 2072 6567  ds sequencer reg
+000363a0: 6973 7465 7220 3130 2e0a 2020 2020 2020  ister 10..      
+000363b0: 2020 2020 2020 2020 2020 2d20 2020 5365            -   Se
+000363c0: 7175 656e 6365 7252 6567 6973 7465 722e  quencerRegister.
+000363d0: 5245 4749 5354 4552 3131 2028 2272 6567  REGISTER11 ("reg
+000363e0: 3131 2229 3a20 5265 6164 7320 7365 7175  11"): Reads sequ
+000363f0: 656e 6365 7220 7265 6769 7374 6572 2031  encer register 1
+00036400: 312e 0a20 2020 2020 2020 2020 2020 2020  1..             
+00036410: 2020 202d 2020 2053 6571 7565 6e63 6572     -   Sequencer
+00036420: 5265 6769 7374 6572 2e52 4547 4953 5445  Register.REGISTE
+00036430: 5231 3220 2822 7265 6731 3222 293a 2052  R12 ("reg12"): R
+00036440: 6561 6473 2073 6571 7565 6e63 6572 2072  eads sequencer r
+00036450: 6567 6973 7465 7220 3132 2e0a 2020 2020  egister 12..    
+00036460: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
+00036470: 5365 7175 656e 6365 7252 6567 6973 7465  SequencerRegiste
+00036480: 722e 5245 4749 5354 4552 3133 2028 2272  r.REGISTER13 ("r
+00036490: 6567 3133 2229 3a20 5265 6164 7320 7365  eg13"): Reads se
+000364a0: 7175 656e 6365 7220 7265 6769 7374 6572  quencer register
+000364b0: 2031 332e 0a20 2020 2020 2020 2020 2020   13..           
+000364c0: 2020 2020 202d 2020 2053 6571 7565 6e63       -   Sequenc
+000364d0: 6572 5265 6769 7374 6572 2e52 4547 4953  erRegister.REGIS
+000364e0: 5445 5231 3420 2822 7265 6731 3422 293a  TER14 ("reg14"):
+000364f0: 2052 6561 6473 2073 6571 7565 6e63 6572   Reads sequencer
+00036500: 2072 6567 6973 7465 7220 3134 2e0a 2020   register 14..  
+00036510: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00036520: 2020 5365 7175 656e 6365 7252 6567 6973    SequencerRegis
+00036530: 7465 722e 5245 4749 5354 4552 3135 2028  ter.REGISTER15 (
+00036540: 2272 6567 3135 2229 3a20 5265 6164 7320  "reg15"): Reads 
+00036550: 7365 7175 656e 6365 7220 7265 6769 7374  sequencer regist
+00036560: 6572 2031 352e 0a0a 0a20 2020 2020 2020  er 15....       
+00036570: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00036580: 2020 2020 2020 7661 6c75 6520 2869 6e74        value (int
+00036590: 293a 2056 616c 7565 2072 6561 6420 6672  ): Value read fr
+000365a0: 6f6d 2074 6865 2073 6571 7565 6e63 6572  om the sequencer
+000365b0: 2072 6567 6973 7465 722e 0a0a 2020 2020   register...    
+000365c0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+000365d0: 6966 2074 7970 6528 7265 6729 2069 7320  if type(reg) is 
+000365e0: 6e6f 7420 656e 756d 732e 5365 7175 656e  not enums.Sequen
+000365f0: 6365 7252 6567 6973 7465 723a 0a20 2020  cerRegister:.   
+00036600: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00036610: 7970 6545 7272 6f72 2827 5061 7261 6d65  ypeError('Parame
+00036620: 7465 7220 7265 6720 6d75 7374 2062 6520  ter reg must be 
+00036630: 6f66 2074 7970 6520 2720 2b20 7374 7228  of type ' + str(
+00036640: 656e 756d 732e 5365 7175 656e 6365 7252  enums.SequencerR
+00036650: 6567 6973 7465 7229 290a 2020 2020 2020  egister)).      
+00036660: 2020 7661 6c75 6520 3d20 7365 6c66 2e5f    value = self._
+00036670: 696e 7465 7270 7265 7465 722e 7265 6164  interpreter.read
+00036680: 5f73 6571 7565 6e63 6572 5f72 6567 6973  _sequencer_regis
+00036690: 7465 7228 7265 6729 0a20 2020 2020 2020  ter(reg).       
+000366a0: 2072 6574 7572 6e20 7661 6c75 650a 0a20   return value.. 
+000366b0: 2020 2040 6976 695f 7379 6e63 6872 6f6e     @ivi_synchron
+000366c0: 697a 6564 0a20 2020 2064 6566 2072 6573  ized.    def res
+000366d0: 6574 5f64 6576 6963 6528 7365 6c66 293a  et_device(self):
+000366e0: 0a20 2020 2020 2020 2072 2727 2772 6573  .        r'''res
+000366f0: 6574 5f64 6576 6963 650a 0a20 2020 2020  et_device..     
+00036700: 2020 2052 6574 7572 6e73 2061 2064 6967     Returns a dig
+00036710: 6974 616c 2070 6174 7465 726e 2069 6e73  ital pattern ins
+00036720: 7472 756d 656e 7420 746f 2061 206b 6e6f  trument to a kno
+00036730: 776e 2073 7461 7465 2e20 5468 6973 206d  wn state. This m
+00036740: 6574 686f 6420 7065 7266 6f72 6d73 2074  ethod performs t
+00036750: 6865 2066 6f6c 6c6f 7769 6e67 2061 6374  he following act
+00036760: 696f 6e73 3a0a 0a20 2020 2020 2020 202d  ions:..        -
+00036770: 2041 626f 7274 7320 7061 7474 6572 6e20   Aborts pattern 
+00036780: 6578 6563 7574 696f 6e2e 0a20 2020 2020  execution..     
+00036790: 2020 202d 2043 6c65 6172 7320 7069 6e20     - Clears pin 
+000367a0: 6d61 7073 2c20 7469 6d65 2073 6574 732c  maps, time sets,
+000367b0: 2073 6f75 7263 6520 616e 6420 6361 7074   source and capt
+000367c0: 7572 6520 7761 7665 666f 726d 732c 2061  ure waveforms, a
+000367d0: 6e64 2070 6174 7465 726e 732e 0a20 2020  nd patterns..   
+000367e0: 2020 2020 202d 2052 6573 6574 7320 616c       - Resets al
+000367f0: 6c20 7072 6f70 6572 7469 6573 2074 6f20  l properties to 
+00036800: 6465 6661 756c 7420 7661 6c75 6573 2c20  default values, 
+00036810: 696e 636c 7564 696e 6720 7468 6520 7365  including the se
+00036820: 6c65 6374 6564 5f66 756e 6374 696f 6e20  lected_function 
+00036830: 7072 6f70 6572 7479 2074 6861 7420 6973  property that is
+00036840: 2073 6574 2074 6f20 5365 6c65 6374 6564   set to Selected
+00036850: 4675 6e63 7469 6f6e 2e44 4953 434f 4e4e  Function.DISCONN
+00036860: 4543 542c 2063 6175 7369 6e67 2074 6865  ECT, causing the
+00036870: 2049 2f4f 2073 7769 7463 6865 7320 746f   I/O switches to
+00036880: 206f 7065 6e2e 0a20 2020 2020 2020 202d   open..        -
+00036890: 2053 746f 7073 2065 7870 6f72 7420 6f66   Stops export of
+000368a0: 2061 6c6c 2065 7874 6572 6e61 6c20 7369   all external si
+000368b0: 676e 616c 7320 616e 6420 6576 656e 7473  gnals and events
+000368c0: 2e0a 2020 2020 2020 2020 2d20 436c 6561  ..        - Clea
+000368d0: 7273 206f 7665 722d 7465 6d70 6572 6174  rs over-temperat
+000368e0: 7572 6520 616e 6420 6f76 6572 2d70 6f77  ure and over-pow
+000368f0: 6572 2063 6f6e 6469 7469 6f6e 732e 0a20  er conditions.. 
+00036900: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00036910: 2020 2073 656c 662e 5f69 6e74 6572 7072     self._interpr
+00036920: 6574 6572 2e72 6573 6574 5f64 6576 6963  eter.reset_devic
+00036930: 6528 290a 0a20 2020 2040 6976 695f 7379  e()..    @ivi_sy
+00036940: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
+00036950: 6566 2073 656c 665f 6361 6c69 6272 6174  ef self_calibrat
+00036960: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00036970: 2072 2727 2773 656c 665f 6361 6c69 6272   r'''self_calibr
+00036980: 6174 650a 0a20 2020 2020 2020 2050 6572  ate..        Per
+00036990: 666f 726d 7320 7365 6c66 2d63 616c 6962  forms self-calib
+000369a0: 7261 7469 6f6e 206f 6e20 6120 6469 6769  ration on a digi
+000369b0: 7461 6c20 7061 7474 6572 6e20 696e 7374  tal pattern inst
+000369c0: 7275 6d65 6e74 2e0a 2020 2020 2020 2020  rument..        
+000369d0: 2727 270a 2020 2020 2020 2020 7365 6c66  '''.        self
+000369e0: 2e5f 696e 7465 7270 7265 7465 722e 7365  ._interpreter.se
+000369f0: 6c66 5f63 616c 6962 7261 7465 2829 0a0a  lf_calibrate()..
+00036a00: 2020 2020 4069 7669 5f73 796e 6368 726f      @ivi_synchro
+00036a10: 6e69 7a65 640a 2020 2020 6465 6620 7365  nized.    def se
+00036a20: 6e64 5f73 6f66 7477 6172 655f 6564 6765  nd_software_edge
+00036a30: 5f74 7269 6767 6572 2873 656c 662c 2074  _trigger(self, t
+00036a40: 7269 6767 6572 2c20 7472 6967 6765 725f  rigger, trigger_
+00036a50: 6964 656e 7469 6669 6572 293a 0a20 2020  identifier):.   
+00036a60: 2020 2020 2072 2727 2773 656e 645f 736f       r'''send_so
+00036a70: 6674 7761 7265 5f65 6467 655f 7472 6967  ftware_edge_trig
+00036a80: 6765 720a 0a20 2020 2020 2020 2046 6f72  ger..        For
+00036a90: 6365 7320 6120 7061 7274 6963 756c 6172  ces a particular
+00036aa0: 2065 6467 652d 6261 7365 6420 7472 6967   edge-based trig
+00036ab0: 6765 7220 746f 206f 6363 7572 2072 6567  ger to occur reg
+00036ac0: 6172 646c 6573 7320 6f66 2068 6f77 2074  ardless of how t
+00036ad0: 6865 2073 7065 6369 6669 6564 2074 7269  he specified tri
+00036ae0: 6767 6572 2069 7320 636f 6e66 6967 7572  gger is configur
+00036af0: 6564 2e20 596f 7520 6361 6e20 7573 6520  ed. You can use 
+00036b00: 7468 6973 206d 6574 686f 6420 6173 2061  this method as a
+00036b10: 2073 6f66 7477 6172 6520 6f76 6572 7269   software overri
+00036b20: 6465 2e0a 0a20 2020 2020 2020 2041 7267  de...        Arg
+00036b30: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+00036b40: 7269 6767 6572 2028 656e 756d 732e 536f  rigger (enums.So
+00036b50: 6674 7761 7265 5472 6967 6765 7229 3a20  ftwareTrigger): 
+00036b60: 5472 6967 6765 7220 7370 6563 6966 6965  Trigger specifie
+00036b70: 7320 7468 6520 7472 6967 6765 7220 796f  s the trigger yo
+00036b80: 7520 7761 6e74 2074 6f20 6f76 6572 7269  u want to overri
+00036b90: 6465 2e0a 0a20 2020 2020 2020 2020 2020  de...           
+00036ba0: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2d2d       +----------
 00036bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00036bc0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00036bc0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
 00036bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00036c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a20 2020  -----------+.   
-00036c50: 2020 2020 2020 2020 2020 2020 207c 2044               | D
-00036c60: 6566 696e 6564 2056 616c 7565 7320 2020  efined Values   
-00036c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036c80: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00036c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  ----------+.    
+00036c50: 2020 2020 2020 2020 2020 2020 7c20 4465              | De
+00036c60: 6669 6e65 6420 5661 6c75 6573 2020 2020  fined Values    
+00036c70: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00036c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00036c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00036ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00036cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00036cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00036cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00036ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00036cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036d00: 2020 7c0a 2020 2020 2020 2020 2020 2020    |.            
-00036d10: 2020 2020 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d      +===========
+00036d00: 207c 0a20 2020 2020 2020 2020 2020 2020   |.             
+00036d10: 2020 202b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d     +============
 00036d20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00036d30: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
+00036d30: 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d  ======+=========
 00036d40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00036d50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00036d60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00036d70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00036d80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00036d90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00036da0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00036db0: 3d3d 3d3d 3d3d 3d3d 3d2b 0a20 2020 2020  =========+.     
-00036dc0: 2020 2020 2020 2020 2020 207c 2053 6f66             | Sof
-00036dd0: 7477 6172 6554 7269 6767 6572 2e53 5441  twareTrigger.STA
-00036de0: 5254 2020 2020 2020 2020 2020 2020 7c20  RT            | 
-00036df0: 4f76 6572 7269 6465 7320 7468 6520 5374  Overrides the St
-00036e00: 6172 7420 7472 6967 6765 722e 2059 6f75  art trigger. You
-00036e10: 206d 7573 7420 7370 6563 6966 7920 616e   must specify an
-00036e20: 2065 6d70 7479 2073 7472 696e 6720 696e   empty string in
-00036e30: 2074 6865 2074 7269 6767 6572 5f69 6465   the trigger_ide
-00036e40: 6e74 6966 6965 7220 7061 7261 6d65 7465  ntifier paramete
-00036e50: 722e 2020 2020 2020 2020 2020 2020 2020  r.              
-00036e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036e70: 7c0a 2020 2020 2020 2020 2020 2020 2020  |.              
-00036e80: 2020 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    +-------------
+00036db0: 3d3d 3d3d 3d3d 3d3d 2b0a 2020 2020 2020  ========+.      
+00036dc0: 2020 2020 2020 2020 2020 7c20 536f 6674            | Soft
+00036dd0: 7761 7265 5472 6967 6765 722e 5354 4152  wareTrigger.STAR
+00036de0: 5420 2020 2020 2020 2020 2020 207c 204f  T            | O
+00036df0: 7665 7272 6964 6573 2074 6865 2053 7461  verrides the Sta
+00036e00: 7274 2074 7269 6767 6572 2e20 596f 7520  rt trigger. You 
+00036e10: 6d75 7374 2073 7065 6369 6679 2061 6e20  must specify an 
+00036e20: 656d 7074 7920 7374 7269 6e67 2069 6e20  empty string in 
+00036e30: 7468 6520 7472 6967 6765 725f 6964 656e  the trigger_iden
+00036e40: 7469 6669 6572 2070 6172 616d 6574 6572  tifier parameter
+00036e50: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00036e60: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00036e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00036e80: 202b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   +--------------
 00036e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00036ea0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00036ea0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
 00036eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00036f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00036f20: 2d2d 2d2d 2d2d 2d2b 0a20 2020 2020 2020  -------+.       
-00036f30: 2020 2020 2020 2020 207c 2053 6f66 7477           | Softw
-00036f40: 6172 6554 7269 6767 6572 2e43 4f4e 4449  areTrigger.CONDI
-00036f50: 5449 4f4e 414c 5f4a 554d 5020 7c20 5370  TIONAL_JUMP | Sp
-00036f60: 6563 6966 6965 7320 746f 2072 6f75 7465  ecifies to route
-00036f70: 2061 2063 6f6e 6469 7469 6f6e 616c 206a   a conditional j
-00036f80: 756d 7020 7472 6967 6765 722e 2059 6f75  ump trigger. You
-00036f90: 206d 7573 7420 7370 6563 6966 7920 6120   must specify a 
-00036fa0: 636f 6e64 6974 696f 6e61 6c20 6a75 6d70  conditional jump
-00036fb0: 2074 7269 6767 6572 2069 6e20 7468 6520   trigger in the 
-00036fc0: 7472 6967 6765 725f 6964 656e 7469 6669  trigger_identifi
-00036fd0: 6572 2070 6172 616d 6574 6572 2e20 7c0a  er parameter. |.
-00036fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00036ff0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00036f20: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
+00036f30: 2020 2020 2020 2020 7c20 536f 6674 7761          | Softwa
+00036f40: 7265 5472 6967 6765 722e 434f 4e44 4954  reTrigger.CONDIT
+00036f50: 494f 4e41 4c5f 4a55 4d50 207c 2053 7065  IONAL_JUMP | Spe
+00036f60: 6369 6669 6573 2074 6f20 726f 7574 6520  cifies to route 
+00036f70: 6120 636f 6e64 6974 696f 6e61 6c20 6a75  a conditional ju
+00036f80: 6d70 2074 7269 6767 6572 2e20 596f 7520  mp trigger. You 
+00036f90: 6d75 7374 2073 7065 6369 6679 2061 2063  must specify a c
+00036fa0: 6f6e 6469 7469 6f6e 616c 206a 756d 7020  onditional jump 
+00036fb0: 7472 6967 6765 7220 696e 2074 6865 2074  trigger in the t
+00036fc0: 7269 6767 6572 5f69 6465 6e74 6966 6965  rigger_identifie
+00036fd0: 7220 7061 7261 6d65 7465 722e 207c 0a20  r parameter. |. 
+00036fe0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00036ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00037000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00037010: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+00037010: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
 00037020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00037030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00037040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00037050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00037060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00037070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00037080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00037090: 2d2d 2d2d 2d2b 0a0a 2020 2020 2020 2020  -----+..        
-000370a0: 2020 2020 2020 2020 4e6f 7465 3a0a 2020          Note:.  
-000370b0: 2020 2020 2020 2020 2020 2020 2020 4f6e                On
-000370c0: 6520 6f72 206d 6f72 6520 6f66 2074 6865  e or more of the
-000370d0: 2072 6566 6572 656e 6365 6420 7661 6c75   referenced valu
-000370e0: 6573 2061 7265 206e 6f74 2069 6e20 7468  es are not in th
-000370f0: 6520 5079 7468 6f6e 2041 5049 2066 6f72  e Python API for
-00037100: 2074 6869 7320 6472 6976 6572 2e20 456e   this driver. En
-00037110: 756d 7320 7468 6174 206f 6e6c 7920 6465  ums that only de
-00037120: 6669 6e65 2076 616c 7565 732c 206f 7220  fine values, or 
-00037130: 7265 7072 6573 656e 7420 5472 7565 2f46  represent True/F
-00037140: 616c 7365 2c20 6861 7665 2062 6565 6e20  alse, have been 
-00037150: 7265 6d6f 7665 642e 0a0a 2020 2020 2020  removed...      
-00037160: 2020 2020 2020 7472 6967 6765 725f 6964        trigger_id
-00037170: 656e 7469 6669 6572 2028 7374 7229 3a20  entifier (str): 
-00037180: 5472 6967 6765 7220 4964 656e 7469 6669  Trigger Identifi
-00037190: 6572 2073 7065 6369 6669 6573 2074 6865  er specifies the
-000371a0: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
-000371b0: 2074 7269 6767 6572 2079 6f75 2077 616e   trigger you wan
-000371c0: 7420 746f 206f 7665 7272 6964 652e 0a20  t to override.. 
-000371d0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-000371e0: 6620 7472 6967 6765 7220 6973 2073 7065  f trigger is spe
-000371f0: 6369 6669 6564 2061 7320 4e49 4449 4749  cified as NIDIGI
-00037200: 5441 4c5f 5641 4c5f 5354 4152 545f 5452  TAL_VAL_START_TR
-00037210: 4947 4745 522c 2074 6869 7320 7061 7261  IGGER, this para
-00037220: 6d65 7465 7220 6d75 7374 2062 6520 616e  meter must be an
-00037230: 2065 6d70 7479 2073 7472 696e 672e 2049   empty string. I
-00037240: 6620 7472 6967 6765 7220 6973 0a20 2020  f trigger is.   
-00037250: 2020 2020 2020 2020 2020 2020 2073 7065               spe
-00037260: 6369 6669 6564 2061 7320 4e49 4449 4749  cified as NIDIGI
-00037270: 5441 4c5f 5641 4c5f 434f 4e44 4954 494f  TAL_VAL_CONDITIO
-00037280: 4e41 4c5f 4a55 4d50 5f54 5249 4747 4552  NAL_JUMP_TRIGGER
-00037290: 2c20 616c 6c6f 7765 6420 7661 6c75 6573  , allowed values
-000372a0: 2061 7265 2063 6f6e 6469 7469 6f6e 616c   are conditional
-000372b0: 4a75 6d70 5472 6967 6765 7230 2c0a 2020  JumpTrigger0,.  
-000372c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000372d0: 6e64 6974 696f 6e61 6c4a 756d 7054 7269  nditionalJumpTri
-000372e0: 6767 6572 312c 2063 6f6e 6469 7469 6f6e  gger1, condition
-000372f0: 616c 4a75 6d70 5472 6967 6765 7232 2c20  alJumpTrigger2, 
-00037300: 616e 6420 636f 6e64 6974 696f 6e61 6c4a  and conditionalJ
-00037310: 756d 7054 7269 6767 6572 332e 0a0a 2020  umpTrigger3...  
-00037320: 2020 2020 2020 2020 2020 2020 2020 4e6f                No
-00037330: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
-00037340: 2020 2020 4f6e 6520 6f72 206d 6f72 6520      One or more 
-00037350: 6f66 2074 6865 2072 6566 6572 656e 6365  of the reference
-00037360: 6420 7661 6c75 6573 2061 7265 206e 6f74  d values are not
-00037370: 2069 6e20 7468 6520 5079 7468 6f6e 2041   in the Python A
-00037380: 5049 2066 6f72 2074 6869 7320 6472 6976  PI for this driv
-00037390: 6572 2e20 456e 756d 7320 7468 6174 206f  er. Enums that o
-000373a0: 6e6c 7920 6465 6669 6e65 2076 616c 7565  nly define value
-000373b0: 732c 206f 7220 7265 7072 6573 656e 7420  s, or represent 
-000373c0: 5472 7565 2f46 616c 7365 2c20 6861 7665  True/False, have
-000373d0: 2062 6565 6e20 7265 6d6f 7665 642e 0a0a   been removed...
-000373e0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000373f0: 2020 2020 6966 2074 7970 6528 7472 6967      if type(trig
-00037400: 6765 7229 2069 7320 6e6f 7420 656e 756d  ger) is not enum
-00037410: 732e 536f 6674 7761 7265 5472 6967 6765  s.SoftwareTrigge
-00037420: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-00037430: 6169 7365 2054 7970 6545 7272 6f72 2827  aise TypeError('
-00037440: 5061 7261 6d65 7465 7220 7472 6967 6765  Parameter trigge
-00037450: 7220 6d75 7374 2062 6520 6f66 2074 7970  r must be of typ
-00037460: 6520 2720 2b20 7374 7228 656e 756d 732e  e ' + str(enums.
-00037470: 536f 6674 7761 7265 5472 6967 6765 7229  SoftwareTrigger)
-00037480: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-00037490: 696e 7465 7270 7265 7465 722e 7365 6e64  interpreter.send
-000374a0: 5f73 6f66 7477 6172 655f 6564 6765 5f74  _software_edge_t
-000374b0: 7269 6767 6572 2874 7269 6767 6572 2c20  rigger(trigger, 
-000374c0: 7472 6967 6765 725f 6964 656e 7469 6669  trigger_identifi
-000374d0: 6572 290a 0a20 2020 2040 6976 695f 7379  er)..    @ivi_sy
-000374e0: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
-000374f0: 6566 2075 6e6c 6f61 645f 616c 6c5f 7061  ef unload_all_pa
-00037500: 7474 6572 6e73 2873 656c 662c 2075 6e6c  tterns(self, unl
-00037510: 6f61 645f 6b65 6570 5f61 6c69 7665 5f70  oad_keep_alive_p
-00037520: 6174 7465 726e 3d46 616c 7365 293a 0a20  attern=False):. 
-00037530: 2020 2020 2020 2072 2727 2775 6e6c 6f61         r'''unloa
-00037540: 645f 616c 6c5f 7061 7474 6572 6e73 0a0a  d_all_patterns..
-00037550: 2020 2020 2020 2020 556e 6c6f 6164 7320          Unloads 
-00037560: 616c 6c20 7061 7474 6572 6e73 2c20 736f  all patterns, so
-00037570: 7572 6365 2077 6176 6566 6f72 6d73 2c20  urce waveforms, 
-00037580: 616e 6420 6361 7074 7572 6520 7761 7665  and capture wave
-00037590: 666f 726d 7320 6672 6f6d 2061 2064 6967  forms from a dig
-000375a0: 6974 616c 2070 6174 7465 726e 2069 6e73  ital pattern ins
-000375b0: 7472 756d 656e 742e 0a0a 2020 2020 2020  trument...      
-000375c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000375d0: 2020 2020 756e 6c6f 6164 5f6b 6565 705f      unload_keep_
-000375e0: 616c 6976 655f 7061 7474 6572 6e20 2862  alive_pattern (b
-000375f0: 6f6f 6c29 3a20 4120 426f 6f6c 6561 6e20  ool): A Boolean 
-00037600: 7468 6174 2073 7065 6369 6669 6573 2077  that specifies w
-00037610: 6865 7468 6572 2074 6f20 6b65 6570 206f  hether to keep o
-00037620: 7220 756e 6c6f 6164 2074 6865 206b 6565  r unload the kee
-00037630: 7020 616c 6976 6520 7061 7474 6572 6e2e  p alive pattern.
-00037640: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00037650: 2020 2020 2020 7365 6c66 2e5f 696e 7465        self._inte
-00037660: 7270 7265 7465 722e 756e 6c6f 6164 5f61  rpreter.unload_a
-00037670: 6c6c 5f70 6174 7465 726e 7328 756e 6c6f  ll_patterns(unlo
-00037680: 6164 5f6b 6565 705f 616c 6976 655f 7061  ad_keep_alive_pa
-00037690: 7474 6572 6e29 0a0a 2020 2020 4069 7669  ttern)..    @ivi
-000376a0: 5f73 796e 6368 726f 6e69 7a65 640a 2020  _synchronized.  
-000376b0: 2020 6465 6620 5f75 6e6c 6f61 645f 7370    def _unload_sp
-000376c0: 6563 6966 6963 6174 696f 6e73 2873 656c  ecifications(sel
-000376d0: 662c 2066 696c 655f 7061 7468 293a 0a20  f, file_path):. 
-000376e0: 2020 2020 2020 2072 2727 275f 756e 6c6f         r'''_unlo
-000376f0: 6164 5f73 7065 6369 6669 6361 7469 6f6e  ad_specification
-00037700: 730a 0a20 2020 2020 2020 2055 6e6c 6f61  s..        Unloa
-00037710: 6473 2074 6865 2067 6976 656e 2073 7065  ds the given spe
-00037720: 6369 6669 6361 7469 6f6e 7320 7368 6565  cifications shee
-00037730: 7420 7072 6573 656e 7420 696e 2074 6865  t present in the
-00037740: 2070 7265 7669 6f75 736c 7920 6c6f 6164   previously load
-00037750: 6564 2073 7065 6369 6669 6361 7469 6f6e  ed specification
-00037760: 7320 6669 6c65 2074 6861 7420 796f 7520  s file that you 
-00037770: 7365 6c65 6374 2e20 596f 7520 6d75 7374  select. You must
-00037780: 2063 616c 6c20 7468 6520 5f6c 6f61 645f   call the _load_
-00037790: 7370 6563 6966 6963 6174 696f 6e73 206d  specifications m
-000377a0: 6574 686f 6420 746f 2072 656c 6f61 6420  ethod to reload 
-000377b0: 7468 6520 6669 6c65 2077 6974 6820 7570  the file with up
-000377c0: 6461 7465 6420 7370 6563 6966 6963 6174  dated specificat
-000377d0: 696f 6e73 2076 616c 7565 732e 2059 6f75  ions values. You
-000377e0: 206d 7573 7420 7468 656e 2063 616c 6c20   must then call 
-000377f0: 7468 6520 6170 706c 795f 6c65 7665 6c73  the apply_levels
-00037800: 5f61 6e64 5f74 696d 696e 6720 6d65 7468  _and_timing meth
-00037810: 6f64 2069 6e20 6f72 6465 7220 746f 2061  od in order to a
-00037820: 7070 6c79 2074 6865 206c 6576 656c 7320  pply the levels 
-00037830: 616e 6420 7469 6d69 6e67 2076 616c 7565  and timing value
-00037840: 7320 7468 6174 2072 6566 6572 656e 6365  s that reference
-00037850: 2074 6865 2075 7064 6174 6564 2073 7065   the updated spe
-00037860: 6369 6669 6361 7469 6f6e 7320 7661 6c75  cifications valu
-00037870: 6573 2e0a 0a20 2020 2020 2020 2041 7267  es...        Arg
-00037880: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00037890: 696c 655f 7061 7468 2028 7374 7229 3a20  ile_path (str): 
-000378a0: 4162 736f 6c75 7465 2066 696c 6520 7061  Absolute file pa
-000378b0: 7468 2074 6f20 6120 6c6f 6164 6564 2073  th to a loaded s
-000378c0: 7065 6369 6669 6361 7469 6f6e 7320 6669  pecifications fi
-000378d0: 6c65 2e0a 0a20 2020 2020 2020 2027 2727  le...        '''
-000378e0: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
-000378f0: 6e74 6572 7072 6574 6572 2e75 6e6c 6f61  nterpreter.unloa
-00037900: 645f 7370 6563 6966 6963 6174 696f 6e73  d_specifications
-00037910: 2866 696c 655f 7061 7468 290a 0a20 2020  (file_path)..   
-00037920: 2040 6976 695f 7379 6e63 6872 6f6e 697a   @ivi_synchroniz
-00037930: 6564 0a20 2020 2064 6566 2077 6169 745f  ed.    def wait_
-00037940: 756e 7469 6c5f 646f 6e65 2873 656c 662c  until_done(self,
-00037950: 2074 696d 656f 7574 3d68 6967 6874 696d   timeout=hightim
-00037960: 652e 7469 6d65 6465 6c74 6128 7365 636f  e.timedelta(seco
-00037970: 6e64 733d 3130 2e30 2929 3a0a 2020 2020  nds=10.0)):.    
-00037980: 2020 2020 7227 2727 7761 6974 5f75 6e74      r'''wait_unt
-00037990: 696c 5f64 6f6e 650a 0a20 2020 2020 2020  il_done..       
-000379a0: 2057 6169 7473 2075 6e74 696c 2074 6865   Waits until the
-000379b0: 2070 6174 7465 726e 2062 7572 7374 2068   pattern burst h
-000379c0: 6173 2063 6f6d 706c 6574 6564 206f 7220  as completed or 
-000379d0: 7468 6520 7469 6d65 6f75 7420 6861 7320  the timeout has 
-000379e0: 6578 7069 7265 642e 0a0a 2020 2020 2020  expired...      
-000379f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00037a00: 2020 2020 7469 6d65 6f75 7420 2868 6967      timeout (hig
-00037a10: 6874 696d 652e 7469 6d65 6465 6c74 612c  htime.timedelta,
-00037a20: 2064 6174 6574 696d 652e 7469 6d65 6465   datetime.timede
-00037a30: 6c74 612c 206f 7220 666c 6f61 7420 696e  lta, or float in
-00037a40: 2073 6563 6f6e 6473 293a 204d 6178 696d   seconds): Maxim
-00037a50: 756d 2074 696d 6520 2869 6e20 7365 636f  um time (in seco
-00037a60: 6e64 7329 2061 6c6c 6f77 6564 2066 6f72  nds) allowed for
-00037a70: 2074 6869 7320 6d65 7468 6f64 2074 6f20   this method to 
-00037a80: 636f 6d70 6c65 7465 2e20 4966 2074 6869  complete. If thi
-00037a90: 7320 6d65 7468 6f64 2064 6f65 7320 6e6f  s method does no
-00037aa0: 7420 636f 6d70 6c65 7465 2077 6974 6869  t complete withi
-00037ab0: 6e20 7468 6973 2074 696d 6520 696e 7465  n this time inte
-00037ac0: 7276 616c 2c20 7468 6973 206d 6574 686f  rval, this metho
-00037ad0: 6420 7265 7475 726e 7320 616e 2065 7272  d returns an err
-00037ae0: 6f72 2e0a 0a20 2020 2020 2020 2027 2727  or...        '''
-00037af0: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
-00037b00: 203d 205f 636f 6e76 6572 7465 7273 2e63   = _converters.c
-00037b10: 6f6e 7665 7274 5f74 696d 6564 656c 7461  onvert_timedelta
-00037b20: 5f74 6f5f 7365 636f 6e64 735f 7265 616c  _to_seconds_real
-00037b30: 3634 2874 696d 656f 7574 290a 2020 2020  64(timeout).    
-00037b40: 2020 2020 7365 6c66 2e5f 696e 7465 7270      self._interp
-00037b50: 7265 7465 722e 7761 6974 5f75 6e74 696c  reter.wait_until
-00037b60: 5f64 6f6e 6528 7469 6d65 6f75 7429 0a0a  _done(timeout)..
-00037b70: 2020 2020 4069 7669 5f73 796e 6368 726f      @ivi_synchro
-00037b80: 6e69 7a65 640a 2020 2020 6465 6620 7772  nized.    def wr
-00037b90: 6974 655f 7365 7175 656e 6365 725f 666c  ite_sequencer_fl
-00037ba0: 6167 2873 656c 662c 2066 6c61 672c 2076  ag(self, flag, v
-00037bb0: 616c 7565 293a 0a20 2020 2020 2020 2072  alue):.        r
-00037bc0: 2727 2777 7269 7465 5f73 6571 7565 6e63  '''write_sequenc
-00037bd0: 6572 5f66 6c61 670a 0a20 2020 2020 2020  er_flag..       
-00037be0: 2057 7269 7465 7320 7468 6520 7374 6174   Writes the stat
-00037bf0: 6520 6f66 2061 2070 6174 7465 726e 2073  e of a pattern s
-00037c00: 6571 7565 6e63 6572 2066 6c61 672e 2055  equencer flag. U
-00037c10: 7365 2070 6174 7465 726e 2073 6571 7565  se pattern seque
-00037c20: 6e63 6572 2066 6c61 6773 2074 6f20 636f  ncer flags to co
-00037c30: 6f72 6469 6e61 7465 2065 7865 6375 7469  ordinate executi
-00037c40: 6f6e 2062 6574 7765 656e 2074 6865 2070  on between the p
-00037c50: 6174 7465 726e 2073 6571 7565 6e63 6572  attern sequencer
-00037c60: 2061 6e64 2061 2072 756e 7469 6d65 2074   and a runtime t
-00037c70: 6573 7420 7072 6f67 7261 6d2e 0a0a 2020  est program...  
-00037c80: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00037c90: 2020 2020 2020 2020 666c 6167 2028 656e          flag (en
-00037ca0: 756d 732e 5365 7175 656e 6365 7246 6c61  ums.SequencerFla
-00037cb0: 6729 3a20 5468 6520 7061 7474 6572 6e20  g): The pattern 
-00037cc0: 7365 7175 656e 6365 7220 666c 6167 2074  sequencer flag t
-00037cd0: 6f20 7772 6974 652e 0a0a 2020 2020 2020  o write...      
-00037ce0: 2020 2020 2020 2020 2020 2d20 2020 5365            -   Se
-00037cf0: 7175 656e 6365 7246 6c61 672e 464c 4147  quencerFlag.FLAG
-00037d00: 3020 2822 7365 7166 6c61 6730 2229 3a20  0 ("seqflag0"): 
-00037d10: 5772 6974 6573 2070 6174 7465 726e 2073  Writes pattern s
-00037d20: 6571 7565 6e63 6572 2066 6c61 6720 302e  equencer flag 0.
-00037d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00037d40: 202d 2020 2053 6571 7565 6e63 6572 466c   -   SequencerFl
-00037d50: 6167 2e46 4c41 4731 2028 2273 6571 666c  ag.FLAG1 ("seqfl
-00037d60: 6167 3122 293a 2057 7269 7465 7320 7061  ag1"): Writes pa
-00037d70: 7474 6572 6e20 7365 7175 656e 6365 7220  ttern sequencer 
-00037d80: 666c 6167 2031 2e0a 2020 2020 2020 2020  flag 1..        
-00037d90: 2020 2020 2020 2020 2d20 2020 5365 7175          -   Sequ
-00037da0: 656e 6365 7246 6c61 672e 464c 4147 3220  encerFlag.FLAG2 
-00037db0: 2822 7365 7166 6c61 6732 2229 3a20 5772  ("seqflag2"): Wr
-00037dc0: 6974 6573 2070 6174 7465 726e 2073 6571  ites pattern seq
-00037dd0: 7565 6e63 6572 2066 6c61 6720 322e 0a20  uencer flag 2.. 
-00037de0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-00037df0: 2020 2053 6571 7565 6e63 6572 466c 6167     SequencerFlag
-00037e00: 2e46 4c41 4733 2028 2273 6571 666c 6167  .FLAG3 ("seqflag
-00037e10: 3322 293a 2057 7269 7465 7320 7061 7474  3"): Writes patt
-00037e20: 6572 6e20 7365 7175 656e 6365 7220 666c  ern sequencer fl
-00037e30: 6167 2033 2e0a 0a20 2020 2020 2020 2020  ag 3...         
-00037e40: 2020 2076 616c 7565 2028 626f 6f6c 293a     value (bool):
-00037e50: 2041 2042 6f6f 6c65 616e 2074 6861 7420   A Boolean that 
-00037e60: 6173 7369 676e 7320 6120 7374 6174 6520  assigns a state 
-00037e70: 746f 2074 6865 2070 6174 7465 726e 2073  to the pattern s
-00037e80: 6571 7565 6e63 6572 2066 6c61 6720 796f  equencer flag yo
-00037e90: 7520 7370 6563 6966 792e 0a0a 2020 2020  u specify...    
-00037ea0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00037eb0: 6966 2074 7970 6528 666c 6167 2920 6973  if type(flag) is
-00037ec0: 206e 6f74 2065 6e75 6d73 2e53 6571 7565   not enums.Seque
-00037ed0: 6e63 6572 466c 6167 3a0a 2020 2020 2020  ncerFlag:.      
-00037ee0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-00037ef0: 4572 726f 7228 2750 6172 616d 6574 6572  Error('Parameter
-00037f00: 2066 6c61 6720 6d75 7374 2062 6520 6f66   flag must be of
-00037f10: 2074 7970 6520 2720 2b20 7374 7228 656e   type ' + str(en
-00037f20: 756d 732e 5365 7175 656e 6365 7246 6c61  ums.SequencerFla
-00037f30: 6729 290a 2020 2020 2020 2020 7365 6c66  g)).        self
-00037f40: 2e5f 696e 7465 7270 7265 7465 722e 7772  ._interpreter.wr
-00037f50: 6974 655f 7365 7175 656e 6365 725f 666c  ite_sequencer_fl
-00037f60: 6167 2866 6c61 672c 2076 616c 7565 290a  ag(flag, value).
-00037f70: 0a20 2020 2040 6976 695f 7379 6e63 6872  .    @ivi_synchr
-00037f80: 6f6e 697a 6564 0a20 2020 2064 6566 2077  onized.    def w
-00037f90: 7269 7465 5f73 6571 7565 6e63 6572 5f72  rite_sequencer_r
-00037fa0: 6567 6973 7465 7228 7365 6c66 2c20 7265  egister(self, re
-00037fb0: 672c 2076 616c 7565 293a 0a20 2020 2020  g, value):.     
-00037fc0: 2020 2072 2727 2777 7269 7465 5f73 6571     r'''write_seq
-00037fd0: 7565 6e63 6572 5f72 6567 6973 7465 720a  uencer_register.
-00037fe0: 0a20 2020 2020 2020 2057 7269 7465 7320  .        Writes 
-00037ff0: 6120 7661 6c75 6520 746f 2061 2070 6174  a value to a pat
-00038000: 7465 726e 2073 6571 7565 6e63 6572 2072  tern sequencer r
-00038010: 6567 6973 7465 722e 2055 7365 2070 6174  egister. Use pat
-00038020: 7465 726e 2073 6571 7565 6e63 6572 2072  tern sequencer r
-00038030: 6567 6973 7465 7273 2074 6f20 7061 7373  egisters to pass
-00038040: 206e 756d 6572 6963 2076 616c 7565 7320   numeric values 
-00038050: 6265 7477 6565 6e20 7468 6520 7061 7474  between the patt
-00038060: 6572 6e20 7365 7175 656e 6365 7220 616e  ern sequencer an
-00038070: 6420 6120 7275 6e74 696d 6520 7465 7374  d a runtime test
-00038080: 2070 726f 6772 616d 2e0a 0a20 2020 2020   program...     
-00038090: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-000380a0: 2020 2020 2072 6567 2028 656e 756d 732e       reg (enums.
-000380b0: 5365 7175 656e 6365 7252 6567 6973 7465  SequencerRegiste
-000380c0: 7229 3a20 5468 6520 7365 7175 656e 6365  r): The sequence
-000380d0: 7220 7265 6769 7374 6572 2079 6f75 2077  r register you w
-000380e0: 616e 7420 746f 2077 7269 7465 2074 6f2e  ant to write to.
-000380f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00038100: 2020 2d20 2020 5365 7175 656e 6365 7252    -   SequencerR
-00038110: 6567 6973 7465 722e 5245 4749 5354 4552  egister.REGISTER
-00038120: 3020 2822 7265 6730 2229 3a20 5772 6974  0 ("reg0"): Writ
-00038130: 6573 2073 6571 7565 6e63 6572 2072 6567  es sequencer reg
-00038140: 6973 7465 7220 302e 0a20 2020 2020 2020  ister 0..       
-00038150: 2020 2020 2020 2020 202d 2020 2053 6571           -   Seq
-00038160: 7565 6e63 6572 5265 6769 7374 6572 2e52  uencerRegister.R
-00038170: 4547 4953 5445 5231 2028 2272 6567 3122  EGISTER1 ("reg1"
-00038180: 293a 2057 7269 7465 7320 7365 7175 656e  ): Writes sequen
-00038190: 6365 7220 7265 6769 7374 6572 2031 2e0a  cer register 1..
-000381a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000381b0: 2d20 2020 5365 7175 656e 6365 7252 6567  -   SequencerReg
-000381c0: 6973 7465 722e 5245 4749 5354 4552 3220  ister.REGISTER2 
-000381d0: 2822 7265 6732 2229 3a20 5772 6974 6573  ("reg2"): Writes
-000381e0: 2073 6571 7565 6e63 6572 2072 6567 6973   sequencer regis
-000381f0: 7465 7220 322e 0a20 2020 2020 2020 2020  ter 2..         
-00038200: 2020 2020 2020 202d 2020 2053 6571 7565         -   Seque
-00038210: 6e63 6572 5265 6769 7374 6572 2e52 4547  ncerRegister.REG
-00038220: 4953 5445 5233 2028 2272 6567 3322 293a  ISTER3 ("reg3"):
-00038230: 2057 7269 7465 7320 7365 7175 656e 6365   Writes sequence
-00038240: 7220 7265 6769 7374 6572 2033 2e0a 2020  r register 3..  
-00038250: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00038260: 2020 5365 7175 656e 6365 7252 6567 6973    SequencerRegis
-00038270: 7465 722e 5245 4749 5354 4552 3420 2822  ter.REGISTER4 ("
-00038280: 7265 6734 2229 3a20 5772 6974 6573 2073  reg4"): Writes s
-00038290: 6571 7565 6e63 6572 2072 6567 6973 7465  equencer registe
-000382a0: 7220 342e 0a20 2020 2020 2020 2020 2020  r 4..           
-000382b0: 2020 2020 202d 2020 2053 6571 7565 6e63       -   Sequenc
-000382c0: 6572 5265 6769 7374 6572 2e52 4547 4953  erRegister.REGIS
-000382d0: 5445 5235 2028 2272 6567 3522 293a 2057  TER5 ("reg5"): W
-000382e0: 7269 7465 7320 7365 7175 656e 6365 7220  rites sequencer 
-000382f0: 7265 6769 7374 6572 2035 2e0a 2020 2020  register 5..    
-00038300: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
-00038310: 5365 7175 656e 6365 7252 6567 6973 7465  SequencerRegiste
-00038320: 722e 5245 4749 5354 4552 3620 2822 7265  r.REGISTER6 ("re
-00038330: 6736 2229 3a20 5772 6974 6573 2073 6571  g6"): Writes seq
-00038340: 7565 6e63 6572 2072 6567 6973 7465 7220  uencer register 
-00038350: 362e 0a20 2020 2020 2020 2020 2020 2020  6..             
-00038360: 2020 202d 2020 2053 6571 7565 6e63 6572     -   Sequencer
-00038370: 5265 6769 7374 6572 2e52 4547 4953 5445  Register.REGISTE
-00038380: 5237 2028 2272 6567 3722 293a 2057 7269  R7 ("reg7"): Wri
-00038390: 7465 7320 7365 7175 656e 6365 7220 7265  tes sequencer re
-000383a0: 6769 7374 6572 2037 2e0a 2020 2020 2020  gister 7..      
-000383b0: 2020 2020 2020 2020 2020 2d20 2020 5365            -   Se
-000383c0: 7175 656e 6365 7252 6567 6973 7465 722e  quencerRegister.
-000383d0: 5245 4749 5354 4552 3820 2822 7265 6738  REGISTER8 ("reg8
-000383e0: 2229 3a20 5772 6974 6573 2073 6571 7565  "): Writes seque
-000383f0: 6e63 6572 2072 6567 6973 7465 7220 382e  ncer register 8.
-00038400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00038410: 202d 2020 2053 6571 7565 6e63 6572 5265   -   SequencerRe
-00038420: 6769 7374 6572 2e52 4547 4953 5445 5239  gister.REGISTER9
-00038430: 2028 2272 6567 3922 293a 2057 7269 7465   ("reg9"): Write
-00038440: 7320 7365 7175 656e 6365 7220 7265 6769  s sequencer regi
-00038450: 7374 6572 2039 2e0a 2020 2020 2020 2020  ster 9..        
-00038460: 2020 2020 2020 2020 2d20 2020 5365 7175          -   Sequ
-00038470: 656e 6365 7252 6567 6973 7465 722e 5245  encerRegister.RE
-00038480: 4749 5354 4552 3130 2028 2272 6567 3130  GISTER10 ("reg10
-00038490: 2229 3a20 5772 6974 6573 2073 6571 7565  "): Writes seque
-000384a0: 6e63 6572 2072 6567 6973 7465 7220 3130  ncer register 10
-000384b0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000384c0: 2020 2d20 2020 5365 7175 656e 6365 7252    -   SequencerR
-000384d0: 6567 6973 7465 722e 5245 4749 5354 4552  egister.REGISTER
-000384e0: 3131 2028 2272 6567 3131 2229 3a20 5772  11 ("reg11"): Wr
-000384f0: 6974 6573 2073 6571 7565 6e63 6572 2072  ites sequencer r
-00038500: 6567 6973 7465 7220 3131 2e0a 2020 2020  egister 11..    
-00038510: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
-00038520: 5365 7175 656e 6365 7252 6567 6973 7465  SequencerRegiste
-00038530: 722e 5245 4749 5354 4552 3132 2028 2272  r.REGISTER12 ("r
-00038540: 6567 3132 2229 3a20 5772 6974 6573 2073  eg12"): Writes s
-00038550: 6571 7565 6e63 6572 2072 6567 6973 7465  equencer registe
-00038560: 7220 3132 2e0a 2020 2020 2020 2020 2020  r 12..          
-00038570: 2020 2020 2020 2d20 2020 5365 7175 656e        -   Sequen
-00038580: 6365 7252 6567 6973 7465 722e 5245 4749  cerRegister.REGI
-00038590: 5354 4552 3133 2028 2272 6567 3133 2229  STER13 ("reg13")
-000385a0: 3a20 5772 6974 6573 2073 6571 7565 6e63  : Writes sequenc
-000385b0: 6572 2072 6567 6973 7465 7220 3133 2e0a  er register 13..
-000385c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000385d0: 2d20 2020 5365 7175 656e 6365 7252 6567  -   SequencerReg
-000385e0: 6973 7465 722e 5245 4749 5354 4552 3134  ister.REGISTER14
-000385f0: 2028 2272 6567 3134 2229 3a20 5772 6974   ("reg14"): Writ
-00038600: 6573 2073 6571 7565 6e63 6572 2072 6567  es sequencer reg
-00038610: 6973 7465 7220 3134 2e0a 2020 2020 2020  ister 14..      
-00038620: 2020 2020 2020 2020 2020 2d20 2020 5365            -   Se
-00038630: 7175 656e 6365 7252 6567 6973 7465 722e  quencerRegister.
-00038640: 5245 4749 5354 4552 3135 2028 2272 6567  REGISTER15 ("reg
-00038650: 3135 2229 3a20 5772 6974 6573 2073 6571  15"): Writes seq
-00038660: 7565 6e63 6572 2072 6567 6973 7465 7220  uencer register 
-00038670: 3135 2e0a 0a20 2020 2020 2020 2020 2020  15...           
-00038680: 2076 616c 7565 2028 696e 7429 3a20 5468   value (int): Th
-00038690: 6520 7661 6c75 6520 796f 7520 7761 6e74  e value you want
-000386a0: 2074 6f20 7772 6974 6520 746f 2074 6865   to write to the
-000386b0: 2072 6567 6973 7465 722e 0a0a 2020 2020   register...    
-000386c0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000386d0: 6966 2074 7970 6528 7265 6729 2069 7320  if type(reg) is 
-000386e0: 6e6f 7420 656e 756d 732e 5365 7175 656e  not enums.Sequen
-000386f0: 6365 7252 6567 6973 7465 723a 0a20 2020  cerRegister:.   
-00038700: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00038710: 7970 6545 7272 6f72 2827 5061 7261 6d65  ypeError('Parame
-00038720: 7465 7220 7265 6720 6d75 7374 2062 6520  ter reg must be 
-00038730: 6f66 2074 7970 6520 2720 2b20 7374 7228  of type ' + str(
-00038740: 656e 756d 732e 5365 7175 656e 6365 7252  enums.SequencerR
-00038750: 6567 6973 7465 7229 290a 2020 2020 2020  egister)).      
-00038760: 2020 7365 6c66 2e5f 696e 7465 7270 7265    self._interpre
-00038770: 7465 722e 7772 6974 655f 7365 7175 656e  ter.write_sequen
-00038780: 6365 725f 7265 6769 7374 6572 2872 6567  cer_register(reg
-00038790: 2c20 7661 6c75 6529 0a0a 2020 2020 4069  , value)..    @i
-000387a0: 7669 5f73 796e 6368 726f 6e69 7a65 640a  vi_synchronized.
-000387b0: 2020 2020 6465 6620 7772 6974 655f 736f      def write_so
-000387c0: 7572 6365 5f77 6176 6566 6f72 6d5f 6272  urce_waveform_br
-000387d0: 6f61 6463 6173 7428 7365 6c66 2c20 7761  oadcast(self, wa
-000387e0: 7665 666f 726d 5f6e 616d 652c 2077 6176  veform_name, wav
-000387f0: 6566 6f72 6d5f 6461 7461 293a 0a20 2020  eform_data):.   
-00038800: 2020 2020 2072 2727 2777 7269 7465 5f73       r'''write_s
-00038810: 6f75 7263 655f 7761 7665 666f 726d 5f62  ource_waveform_b
-00038820: 726f 6164 6361 7374 0a0a 2020 2020 2020  roadcast..      
-00038830: 2020 5772 6974 6573 2074 6865 2073 616d    Writes the sam
-00038840: 6520 7761 7665 666f 726d 2064 6174 6120  e waveform data 
-00038850: 746f 2061 6c6c 2073 6974 6573 2e20 5573  to all sites. Us
-00038860: 6520 7468 6973 2077 7269 7465 206d 6574  e this write met
-00038870: 686f 6420 6966 2079 6f75 2073 6574 2074  hod if you set t
-00038880: 6865 2064 6174 615f 6d61 7070 696e 6720  he data_mapping 
-00038890: 7061 7261 6d65 7465 7220 6f66 2074 6865  parameter of the
-000388a0: 2063 7265 6174 6520 736f 7572 6365 2077   create source w
-000388b0: 6176 6566 6f72 6d20 6d65 7468 6f64 2074  aveform method t
-000388c0: 6f20 536f 7572 6365 4461 7461 4d61 7070  o SourceDataMapp
-000388d0: 696e 672e 4252 4f41 4443 4153 542e 0a0a  ing.BROADCAST...
-000388e0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-000388f0: 2020 2020 2020 2020 2020 7761 7665 666f            wavefo
-00038900: 726d 5f6e 616d 6520 2873 7472 293a 2054  rm_name (str): T
-00038910: 6865 206e 616d 6520 746f 2061 7373 6967  he name to assig
-00038920: 6e20 746f 2074 6865 2077 6176 6566 6f72  n to the wavefor
-00038930: 6d2e 2055 7365 2074 6865 2077 6176 6566  m. Use the wavef
-00038940: 6f72 6d5f 6e61 6d65 2020 7769 7468 2073  orm_name  with s
-00038950: 6f75 7263 655f 7374 6172 7420 6f70 636f  ource_start opco
-00038960: 6465 2069 6e20 796f 7572 2070 6174 7465  de in your patte
-00038970: 726e 2e0a 0a20 2020 2020 2020 2020 2020  rn...           
-00038980: 2077 6176 6566 6f72 6d5f 6461 7461 2028   waveform_data (
-00038990: 6c69 7374 206f 6620 696e 7429 3a20 3144  list of int): 1D
-000389a0: 2061 7272 6179 206f 6620 7361 6d70 6c65   array of sample
-000389b0: 7320 746f 2075 7365 2061 7320 736f 7572  s to use as sour
-000389c0: 6365 2064 6174 6120 746f 2061 7070 6c79  ce data to apply
-000389d0: 2074 6f20 616c 6c20 7369 7465 732e 0a0a   to all sites...
-000389e0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000389f0: 2020 2020 7365 6c66 2e5f 696e 7465 7270      self._interp
-00038a00: 7265 7465 722e 7772 6974 655f 736f 7572  reter.write_sour
-00038a10: 6365 5f77 6176 6566 6f72 6d5f 6272 6f61  ce_waveform_broa
-00038a20: 6463 6173 7428 7761 7665 666f 726d 5f6e  dcast(waveform_n
-00038a30: 616d 652c 2077 6176 6566 6f72 6d5f 6461  ame, waveform_da
-00038a40: 7461 290a 0a20 2020 2040 6976 695f 7379  ta)..    @ivi_sy
-00038a50: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
-00038a60: 6566 2077 7269 7465 5f73 6f75 7263 655f  ef write_source_
-00038a70: 7761 7665 666f 726d 5f64 6174 615f 6672  waveform_data_fr
-00038a80: 6f6d 5f66 696c 655f 7464 6d73 2873 656c  om_file_tdms(sel
-00038a90: 662c 2077 6176 6566 6f72 6d5f 6e61 6d65  f, waveform_name
-00038aa0: 2c20 7761 7665 666f 726d 5f66 696c 655f  , waveform_file_
-00038ab0: 7061 7468 293a 0a20 2020 2020 2020 2072  path):.        r
-00038ac0: 2727 2777 7269 7465 5f73 6f75 7263 655f  '''write_source_
-00038ad0: 7761 7665 666f 726d 5f64 6174 615f 6672  waveform_data_fr
-00038ae0: 6f6d 5f66 696c 655f 7464 6d73 0a0a 2020  om_file_tdms..  
-00038af0: 2020 2020 2020 5772 6974 6573 2061 2073        Writes a s
-00038b00: 6f75 7263 6520 7761 7665 666f 726d 2062  ource waveform b
-00038b10: 6173 6564 206f 6e20 7468 6520 7761 7665  ased on the wave
-00038b20: 666f 726d 2064 6174 6120 616e 6420 636f  form data and co
-00038b30: 6e66 6967 7572 6174 696f 6e20 696e 666f  nfiguration info
-00038b40: 726d 6174 696f 6e20 7468 6520 6669 6c65  rmation the file
-00038b50: 2063 6f6e 7461 696e 732e 0a0a 2020 2020   contains...    
-00038b60: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00038b70: 2020 2020 2020 7761 7665 666f 726d 5f6e        waveform_n
-00038b80: 616d 6520 2873 7472 293a 2054 6865 206e  ame (str): The n
-00038b90: 616d 6520 746f 2061 7373 6967 6e20 746f  ame to assign to
-00038ba0: 2074 6865 2077 6176 6566 6f72 6d2e 2055   the waveform. U
-00038bb0: 7365 2074 6865 2077 6176 6566 6f72 6d5f  se the waveform_
-00038bc0: 6e61 6d65 2020 7769 7468 2073 6f75 7263  name  with sourc
-00038bd0: 655f 7374 6172 7420 6f70 636f 6465 2069  e_start opcode i
-00038be0: 6e20 796f 7572 2070 6174 7465 726e 2e0a  n your pattern..
-00038bf0: 0a20 2020 2020 2020 2020 2020 2077 6176  .            wav
-00038c00: 6566 6f72 6d5f 6669 6c65 5f70 6174 6820  eform_file_path 
-00038c10: 2873 7472 293a 2041 6273 6f6c 7574 6520  (str): Absolute 
-00038c20: 6669 6c65 2070 6174 6820 746f 2074 6865  file path to the
-00038c30: 206c 6f61 6420 736f 7572 6365 2077 6176   load source wav
-00038c40: 6566 6f72 6d20 6669 6c65 2028 2e74 646d  eform file (.tdm
-00038c50: 7329 2e0a 0a20 2020 2020 2020 2027 2727  s)...        '''
-00038c60: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
-00038c70: 6e74 6572 7072 6574 6572 2e77 7269 7465  nterpreter.write
-00038c80: 5f73 6f75 7263 655f 7761 7665 666f 726d  _source_waveform
-00038c90: 5f64 6174 615f 6672 6f6d 5f66 696c 655f  _data_from_file_
-00038ca0: 7464 6d73 2877 6176 6566 6f72 6d5f 6e61  tdms(waveform_na
-00038cb0: 6d65 2c20 7761 7665 666f 726d 5f66 696c  me, waveform_fil
-00038cc0: 655f 7061 7468 290a 0a20 2020 2064 6566  e_path)..    def
-00038cd0: 205f 636c 6f73 6528 7365 6c66 293a 0a20   _close(self):. 
-00038ce0: 2020 2020 2020 2072 2727 275f 636c 6f73         r'''_clos
-00038cf0: 650a 0a20 2020 2020 2020 2043 6c6f 7365  e..        Close
-00038d00: 7320 7468 6520 7370 6563 6966 6965 6420  s the specified 
-00038d10: 696e 7374 7275 6d65 6e74 2073 6573 7369  instrument sessi
-00038d20: 6f6e 2074 6f20 6120 6469 6769 7461 6c20  on to a digital 
-00038d30: 7061 7474 6572 6e20 696e 7374 7275 6d65  pattern instrume
-00038d40: 6e74 2c20 6162 6f72 7473 2070 6174 7465  nt, aborts patte
-00038d50: 726e 2065 7865 6375 7469 6f6e 2c20 616e  rn execution, an
-00038d60: 6420 756e 6c6f 6164 7320 7061 7474 6572  d unloads patter
-00038d70: 6e20 6d65 6d6f 7279 2e20 5468 6520 6368  n memory. The ch
-00038d80: 616e 6e65 6c73 206f 6e20 6120 6469 6769  annels on a digi
-00038d90: 7461 6c20 7061 7474 6572 6e20 696e 7374  tal pattern inst
-00038da0: 7275 6d65 6e74 2072 656d 6169 6e20 696e  rument remain in
-00038db0: 2074 6865 6972 2063 7572 7265 6e74 2073   their current s
-00038dc0: 7461 7465 2e0a 2020 2020 2020 2020 2727  tate..        ''
-00038dd0: 270a 2020 2020 2020 2020 7365 6c66 2e5f  '.        self._
-00038de0: 696e 7465 7270 7265 7465 722e 636c 6f73  interpreter.clos
-00038df0: 6528 290a 0a20 2020 2040 6976 695f 7379  e()..    @ivi_sy
-00038e00: 6e63 6872 6f6e 697a 6564 0a20 2020 2064  nchronized.    d
-00038e10: 6566 2072 6573 6574 2873 656c 6629 3a0a  ef reset(self):.
-00038e20: 2020 2020 2020 2020 7227 2727 7265 7365          r'''rese
-00038e30: 740a 0a20 2020 2020 2020 2052 6574 7572  t..        Retur
-00038e40: 6e73 2061 2064 6967 6974 616c 2070 6174  ns a digital pat
-00038e50: 7465 726e 2069 6e73 7472 756d 656e 7420  tern instrument 
-00038e60: 746f 2061 206b 6e6f 776e 2073 7461 7465  to a known state
-00038e70: 2e20 5468 6973 206d 6574 686f 6420 7065  . This method pe
-00038e80: 7266 6f72 6d73 2074 6865 2066 6f6c 6c6f  rforms the follo
-00038e90: 7769 6e67 2061 6374 696f 6e73 3a0a 0a20  wing actions:.. 
-00038ea0: 2020 2020 2020 202d 2041 626f 7274 7320         - Aborts 
-00038eb0: 7061 7474 6572 6e20 6578 6563 7574 696f  pattern executio
-00038ec0: 6e2e 0a20 2020 2020 2020 202d 2043 6c65  n..        - Cle
-00038ed0: 6172 7320 7069 6e20 6d61 7073 2c20 7469  ars pin maps, ti
-00038ee0: 6d65 2073 6574 732c 2073 6f75 7263 6520  me sets, source 
-00038ef0: 616e 6420 6361 7074 7572 6520 7761 7665  and capture wave
-00038f00: 666f 726d 732c 2061 6e64 2070 6174 7465  forms, and patte
-00038f10: 726e 732e 0a20 2020 2020 2020 202d 2052  rns..        - R
-00038f20: 6573 6574 7320 616c 6c20 7072 6f70 6572  esets all proper
-00038f30: 7469 6573 2074 6f20 6465 6661 756c 7420  ties to default 
-00038f40: 7661 6c75 6573 2c20 696e 636c 7564 696e  values, includin
-00038f50: 6720 7468 6520 7365 6c65 6374 6564 5f66  g the selected_f
-00038f60: 756e 6374 696f 6e20 7072 6f70 6572 7479  unction property
-00038f70: 2074 6861 7420 6973 2073 6574 2074 6f20   that is set to 
-00038f80: 5365 6c65 6374 6564 4675 6e63 7469 6f6e  SelectedFunction
-00038f90: 2e44 4953 434f 4e4e 4543 542c 2063 6175  .DISCONNECT, cau
-00038fa0: 7369 6e67 2074 6865 2049 2f4f 2073 7769  sing the I/O swi
-00038fb0: 7463 6865 7320 746f 206f 7065 6e2e 0a20  tches to open.. 
-00038fc0: 2020 2020 2020 202d 2053 746f 7073 2065         - Stops e
-00038fd0: 7870 6f72 7469 6e67 2061 6c6c 2065 7874  xporting all ext
-00038fe0: 6572 6e61 6c20 7369 676e 616c 7320 616e  ernal signals an
-00038ff0: 6420 6576 656e 7473 2e0a 2020 2020 2020  d events..      
-00039000: 2020 2727 270a 2020 2020 2020 2020 7365    '''.        se
-00039010: 6c66 2e5f 696e 7465 7270 7265 7465 722e  lf._interpreter.
-00039020: 7265 7365 7428 290a 0a20 2020 2040 6976  reset()..    @iv
-00039030: 695f 7379 6e63 6872 6f6e 697a 6564 0a20  i_synchronized. 
-00039040: 2020 2064 6566 205f 7365 6c66 5f74 6573     def _self_tes
-00039050: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-00039060: 2072 2727 275f 7365 6c66 5f74 6573 740a   r'''_self_test.
-00039070: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00039080: 2073 656c 6620 7465 7374 2072 6573 756c   self test resul
-00039090: 7473 2066 726f 6d20 6120 6469 6769 7461  ts from a digita
-000390a0: 6c20 7061 7474 6572 6e20 696e 7374 7275  l pattern instru
-000390b0: 6d65 6e74 2e20 5468 6973 2074 6573 7420  ment. This test 
-000390c0: 7265 7175 6972 6573 2073 6576 6572 616c  requires several
-000390d0: 206d 696e 7574 6573 2074 6f20 6578 6563   minutes to exec
-000390e0: 7574 652e 0a0a 2020 2020 2020 2020 5265  ute...        Re
-000390f0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00039100: 2020 2074 6573 745f 7265 7375 6c74 2028     test_result (
-00039110: 696e 7429 3a20 4120 7061 7261 6d65 7465  int): A paramete
-00039120: 7220 7468 6174 2069 6e64 6963 6174 6573  r that indicates
-00039130: 2069 6620 7468 6520 7365 6c66 2074 6573   if the self tes
-00039140: 7420 7061 7373 6564 2028 3029 206f 7220  t passed (0) or 
-00039150: 6661 696c 6564 2028 213d 3029 2e0a 0a20  failed (!=0)... 
-00039160: 2020 2020 2020 2020 2020 2074 6573 745f             test_
-00039170: 6d65 7373 6167 6520 2873 7472 293a 2054  message (str): T
-00039180: 6865 2072 6574 7572 6e65 6420 7365 6c66  he returned self
-00039190: 2074 6573 7420 7374 6174 7573 206d 6573   test status mes
-000391a0: 7361 6765 2e20 5468 6520 6172 7261 7920  sage. The array 
-000391b0: 6d75 7374 2063 6f6e 7461 696e 2061 7420  must contain at 
-000391c0: 6c65 6173 7420 3235 3620 6368 6172 6163  least 256 charac
-000391d0: 7465 7273 2e0a 0a20 2020 2020 2020 2027  ters...        '
-000391e0: 2727 0a20 2020 2020 2020 2074 6573 745f  ''.        test_
-000391f0: 7265 7375 6c74 2c20 7465 7374 5f6d 6573  result, test_mes
-00039200: 7361 6765 203d 2073 656c 662e 5f69 6e74  sage = self._int
-00039210: 6572 7072 6574 6572 2e73 656c 665f 7465  erpreter.self_te
-00039220: 7374 2829 0a20 2020 2020 2020 2072 6574  st().        ret
-00039230: 7572 6e20 7465 7374 5f72 6573 756c 742c  urn test_result,
-00039240: 2074 6573 745f 6d65 7373 6167 650a        test_message.
+00037090: 2d2d 2d2d 2b0a 0a20 2020 2020 2020 2020  ----+..         
+000370a0: 2020 2020 2020 204e 6f74 653a 0a20 2020         Note:.   
+000370b0: 2020 2020 2020 2020 2020 2020 204f 6e65               One
+000370c0: 206f 7220 6d6f 7265 206f 6620 7468 6520   or more of the 
+000370d0: 7265 6665 7265 6e63 6564 2076 616c 7565  referenced value
+000370e0: 7320 6172 6520 6e6f 7420 696e 2074 6865  s are not in the
+000370f0: 2050 7974 686f 6e20 4150 4920 666f 7220   Python API for 
+00037100: 7468 6973 2064 7269 7665 722e 2045 6e75  this driver. Enu
+00037110: 6d73 2074 6861 7420 6f6e 6c79 2064 6566  ms that only def
+00037120: 696e 6520 7661 6c75 6573 2c20 6f72 2072  ine values, or r
+00037130: 6570 7265 7365 6e74 2054 7275 652f 4661  epresent True/Fa
+00037140: 6c73 652c 2068 6176 6520 6265 656e 2072  lse, have been r
+00037150: 656d 6f76 6564 2e0a 0a20 2020 2020 2020  emoved...       
+00037160: 2020 2020 2074 7269 6767 6572 5f69 6465       trigger_ide
+00037170: 6e74 6966 6965 7220 2873 7472 293a 2054  ntifier (str): T
+00037180: 7269 6767 6572 2049 6465 6e74 6966 6965  rigger Identifie
+00037190: 7220 7370 6563 6966 6965 7320 7468 6520  r specifies the 
+000371a0: 696e 7374 616e 6365 206f 6620 7468 6520  instance of the 
+000371b0: 7472 6967 6765 7220 796f 7520 7761 6e74  trigger you want
+000371c0: 2074 6f20 6f76 6572 7269 6465 2e0a 2020   to override..  
+000371d0: 2020 2020 2020 2020 2020 2020 2020 4966                If
+000371e0: 2074 7269 6767 6572 2069 7320 7370 6563   trigger is spec
+000371f0: 6966 6965 6420 6173 204e 4944 4947 4954  ified as NIDIGIT
+00037200: 414c 5f56 414c 5f53 5441 5254 5f54 5249  AL_VAL_START_TRI
+00037210: 4747 4552 2c20 7468 6973 2070 6172 616d  GGER, this param
+00037220: 6574 6572 206d 7573 7420 6265 2061 6e20  eter must be an 
+00037230: 656d 7074 7920 7374 7269 6e67 2e20 4966  empty string. If
+00037240: 2074 7269 6767 6572 2069 730a 2020 2020   trigger is.    
+00037250: 2020 2020 2020 2020 2020 2020 7370 6563              spec
+00037260: 6966 6965 6420 6173 204e 4944 4947 4954  ified as NIDIGIT
+00037270: 414c 5f56 414c 5f43 4f4e 4449 5449 4f4e  AL_VAL_CONDITION
+00037280: 414c 5f4a 554d 505f 5452 4947 4745 522c  AL_JUMP_TRIGGER,
+00037290: 2061 6c6c 6f77 6564 2076 616c 7565 7320   allowed values 
+000372a0: 6172 6520 636f 6e64 6974 696f 6e61 6c4a  are conditionalJ
+000372b0: 756d 7054 7269 6767 6572 302c 0a20 2020  umpTrigger0,.   
+000372c0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000372d0: 6469 7469 6f6e 616c 4a75 6d70 5472 6967  ditionalJumpTrig
+000372e0: 6765 7231 2c20 636f 6e64 6974 696f 6e61  ger1, conditiona
+000372f0: 6c4a 756d 7054 7269 6767 6572 322c 2061  lJumpTrigger2, a
+00037300: 6e64 2063 6f6e 6469 7469 6f6e 616c 4a75  nd conditionalJu
+00037310: 6d70 5472 6967 6765 7233 2e0a 0a20 2020  mpTrigger3...   
+00037320: 2020 2020 2020 2020 2020 2020 204e 6f74               Not
+00037330: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00037340: 2020 204f 6e65 206f 7220 6d6f 7265 206f     One or more o
+00037350: 6620 7468 6520 7265 6665 7265 6e63 6564  f the referenced
+00037360: 2076 616c 7565 7320 6172 6520 6e6f 7420   values are not 
+00037370: 696e 2074 6865 2050 7974 686f 6e20 4150  in the Python AP
+00037380: 4920 666f 7220 7468 6973 2064 7269 7665  I for this drive
+00037390: 722e 2045 6e75 6d73 2074 6861 7420 6f6e  r. Enums that on
+000373a0: 6c79 2064 6566 696e 6520 7661 6c75 6573  ly define values
+000373b0: 2c20 6f72 2072 6570 7265 7365 6e74 2054  , or represent T
+000373c0: 7275 652f 4661 6c73 652c 2068 6176 6520  rue/False, have 
+000373d0: 6265 656e 2072 656d 6f76 6564 2e0a 0a20  been removed... 
+000373e0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+000373f0: 2020 2069 6620 7479 7065 2874 7269 6767     if type(trigg
+00037400: 6572 2920 6973 206e 6f74 2065 6e75 6d73  er) is not enums
+00037410: 2e53 6f66 7477 6172 6554 7269 6767 6572  .SoftwareTrigger
+00037420: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00037430: 6973 6520 5479 7065 4572 726f 7228 2750  ise TypeError('P
+00037440: 6172 616d 6574 6572 2074 7269 6767 6572  arameter trigger
+00037450: 206d 7573 7420 6265 206f 6620 7479 7065   must be of type
+00037460: 2027 202b 2073 7472 2865 6e75 6d73 2e53   ' + str(enums.S
+00037470: 6f66 7477 6172 6554 7269 6767 6572 2929  oftwareTrigger))
+00037480: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+00037490: 6e74 6572 7072 6574 6572 2e73 656e 645f  nterpreter.send_
+000374a0: 736f 6674 7761 7265 5f65 6467 655f 7472  software_edge_tr
+000374b0: 6967 6765 7228 7472 6967 6765 722c 2074  igger(trigger, t
+000374c0: 7269 6767 6572 5f69 6465 6e74 6966 6965  rigger_identifie
+000374d0: 7229 0a0a 2020 2020 4069 7669 5f73 796e  r)..    @ivi_syn
+000374e0: 6368 726f 6e69 7a65 640a 2020 2020 6465  chronized.    de
+000374f0: 6620 756e 6c6f 6164 5f61 6c6c 5f70 6174  f unload_all_pat
+00037500: 7465 726e 7328 7365 6c66 2c20 756e 6c6f  terns(self, unlo
+00037510: 6164 5f6b 6565 705f 616c 6976 655f 7061  ad_keep_alive_pa
+00037520: 7474 6572 6e3d 4661 6c73 6529 3a0a 2020  ttern=False):.  
+00037530: 2020 2020 2020 7227 2727 756e 6c6f 6164        r'''unload
+00037540: 5f61 6c6c 5f70 6174 7465 726e 730a 0a20  _all_patterns.. 
+00037550: 2020 2020 2020 2055 6e6c 6f61 6473 2061         Unloads a
+00037560: 6c6c 2070 6174 7465 726e 732c 2073 6f75  ll patterns, sou
+00037570: 7263 6520 7761 7665 666f 726d 732c 2061  rce waveforms, a
+00037580: 6e64 2063 6170 7475 7265 2077 6176 6566  nd capture wavef
+00037590: 6f72 6d73 2066 726f 6d20 6120 6469 6769  orms from a digi
+000375a0: 7461 6c20 7061 7474 6572 6e20 696e 7374  tal pattern inst
+000375b0: 7275 6d65 6e74 2e0a 0a20 2020 2020 2020  rument...       
+000375c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+000375d0: 2020 2075 6e6c 6f61 645f 6b65 6570 5f61     unload_keep_a
+000375e0: 6c69 7665 5f70 6174 7465 726e 2028 626f  live_pattern (bo
+000375f0: 6f6c 293a 2041 2042 6f6f 6c65 616e 2074  ol): A Boolean t
+00037600: 6861 7420 7370 6563 6966 6965 7320 7768  hat specifies wh
+00037610: 6574 6865 7220 746f 206b 6565 7020 6f72  ether to keep or
+00037620: 2075 6e6c 6f61 6420 7468 6520 6b65 6570   unload the keep
+00037630: 2061 6c69 7665 2070 6174 7465 726e 2e0a   alive pattern..
+00037640: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00037650: 2020 2020 2073 656c 662e 5f69 6e74 6572       self._inter
+00037660: 7072 6574 6572 2e75 6e6c 6f61 645f 616c  preter.unload_al
+00037670: 6c5f 7061 7474 6572 6e73 2875 6e6c 6f61  l_patterns(unloa
+00037680: 645f 6b65 6570 5f61 6c69 7665 5f70 6174  d_keep_alive_pat
+00037690: 7465 726e 290a 0a20 2020 2040 6976 695f  tern)..    @ivi_
+000376a0: 7379 6e63 6872 6f6e 697a 6564 0a20 2020  synchronized.   
+000376b0: 2064 6566 205f 756e 6c6f 6164 5f73 7065   def _unload_spe
+000376c0: 6369 6669 6361 7469 6f6e 7328 7365 6c66  cifications(self
+000376d0: 2c20 6669 6c65 5f70 6174 6829 3a0a 2020  , file_path):.  
+000376e0: 2020 2020 2020 7227 2727 5f75 6e6c 6f61        r'''_unloa
+000376f0: 645f 7370 6563 6966 6963 6174 696f 6e73  d_specifications
+00037700: 0a0a 2020 2020 2020 2020 556e 6c6f 6164  ..        Unload
+00037710: 7320 7468 6520 6769 7665 6e20 7370 6563  s the given spec
+00037720: 6966 6963 6174 696f 6e73 2073 6865 6574  ifications sheet
+00037730: 2070 7265 7365 6e74 2069 6e20 7468 6520   present in the 
+00037740: 7072 6576 696f 7573 6c79 206c 6f61 6465  previously loade
+00037750: 6420 7370 6563 6966 6963 6174 696f 6e73  d specifications
+00037760: 2066 696c 6520 7468 6174 2079 6f75 2073   file that you s
+00037770: 656c 6563 742e 2059 6f75 206d 7573 7420  elect. You must 
+00037780: 6361 6c6c 2074 6865 205f 6c6f 6164 5f73  call the _load_s
+00037790: 7065 6369 6669 6361 7469 6f6e 7320 6d65  pecifications me
+000377a0: 7468 6f64 2074 6f20 7265 6c6f 6164 2074  thod to reload t
+000377b0: 6865 2066 696c 6520 7769 7468 2075 7064  he file with upd
+000377c0: 6174 6564 2073 7065 6369 6669 6361 7469  ated specificati
+000377d0: 6f6e 7320 7661 6c75 6573 2e20 596f 7520  ons values. You 
+000377e0: 6d75 7374 2074 6865 6e20 6361 6c6c 2074  must then call t
+000377f0: 6865 2061 7070 6c79 5f6c 6576 656c 735f  he apply_levels_
+00037800: 616e 645f 7469 6d69 6e67 206d 6574 686f  and_timing metho
+00037810: 6420 696e 206f 7264 6572 2074 6f20 6170  d in order to ap
+00037820: 706c 7920 7468 6520 6c65 7665 6c73 2061  ply the levels a
+00037830: 6e64 2074 696d 696e 6720 7661 6c75 6573  nd timing values
+00037840: 2074 6861 7420 7265 6665 7265 6e63 6520   that reference 
+00037850: 7468 6520 7570 6461 7465 6420 7370 6563  the updated spec
+00037860: 6966 6963 6174 696f 6e73 2076 616c 7565  ifications value
+00037870: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
+00037880: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+00037890: 6c65 5f70 6174 6820 2873 7472 293a 2041  le_path (str): A
+000378a0: 6273 6f6c 7574 6520 6669 6c65 2070 6174  bsolute file pat
+000378b0: 6820 746f 2061 206c 6f61 6465 6420 7370  h to a loaded sp
+000378c0: 6563 6966 6963 6174 696f 6e73 2066 696c  ecifications fil
+000378d0: 652e 0a0a 2020 2020 2020 2020 2727 270a  e...        '''.
+000378e0: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
+000378f0: 7465 7270 7265 7465 722e 756e 6c6f 6164  terpreter.unload
+00037900: 5f73 7065 6369 6669 6361 7469 6f6e 7328  _specifications(
+00037910: 6669 6c65 5f70 6174 6829 0a0a 2020 2020  file_path)..    
+00037920: 4069 7669 5f73 796e 6368 726f 6e69 7a65  @ivi_synchronize
+00037930: 640a 2020 2020 6465 6620 7761 6974 5f75  d.    def wait_u
+00037940: 6e74 696c 5f64 6f6e 6528 7365 6c66 2c20  ntil_done(self, 
+00037950: 7469 6d65 6f75 743d 6869 6768 7469 6d65  timeout=hightime
+00037960: 2e74 696d 6564 656c 7461 2873 6563 6f6e  .timedelta(secon
+00037970: 6473 3d31 302e 3029 293a 0a20 2020 2020  ds=10.0)):.     
+00037980: 2020 2072 2727 2777 6169 745f 756e 7469     r'''wait_unti
+00037990: 6c5f 646f 6e65 0a0a 2020 2020 2020 2020  l_done..        
+000379a0: 5761 6974 7320 756e 7469 6c20 7468 6520  Waits until the 
+000379b0: 7061 7474 6572 6e20 6275 7273 7420 6861  pattern burst ha
+000379c0: 7320 636f 6d70 6c65 7465 6420 6f72 2074  s completed or t
+000379d0: 6865 2074 696d 656f 7574 2068 6173 2065  he timeout has e
+000379e0: 7870 6972 6564 2e0a 0a20 2020 2020 2020  xpired...       
+000379f0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00037a00: 2020 2074 696d 656f 7574 2028 6869 6768     timeout (high
+00037a10: 7469 6d65 2e74 696d 6564 656c 7461 2c20  time.timedelta, 
+00037a20: 6461 7465 7469 6d65 2e74 696d 6564 656c  datetime.timedel
+00037a30: 7461 2c20 6f72 2066 6c6f 6174 2069 6e20  ta, or float in 
+00037a40: 7365 636f 6e64 7329 3a20 4d61 7869 6d75  seconds): Maximu
+00037a50: 6d20 7469 6d65 2028 696e 2073 6563 6f6e  m time (in secon
+00037a60: 6473 2920 616c 6c6f 7765 6420 666f 7220  ds) allowed for 
+00037a70: 7468 6973 206d 6574 686f 6420 746f 2063  this method to c
+00037a80: 6f6d 706c 6574 652e 2049 6620 7468 6973  omplete. If this
+00037a90: 206d 6574 686f 6420 646f 6573 206e 6f74   method does not
+00037aa0: 2063 6f6d 706c 6574 6520 7769 7468 696e   complete within
+00037ab0: 2074 6869 7320 7469 6d65 2069 6e74 6572   this time inter
+00037ac0: 7661 6c2c 2074 6869 7320 6d65 7468 6f64  val, this method
+00037ad0: 2072 6574 7572 6e73 2061 6e20 6572 726f   returns an erro
+00037ae0: 722e 0a0a 2020 2020 2020 2020 2727 270a  r...        '''.
+00037af0: 2020 2020 2020 2020 7469 6d65 6f75 7420          timeout 
+00037b00: 3d20 5f63 6f6e 7665 7274 6572 732e 636f  = _converters.co
+00037b10: 6e76 6572 745f 7469 6d65 6465 6c74 615f  nvert_timedelta_
+00037b20: 746f 5f73 6563 6f6e 6473 5f72 6561 6c36  to_seconds_real6
+00037b30: 3428 7469 6d65 6f75 7429 0a20 2020 2020  4(timeout).     
+00037b40: 2020 2073 656c 662e 5f69 6e74 6572 7072     self._interpr
+00037b50: 6574 6572 2e77 6169 745f 756e 7469 6c5f  eter.wait_until_
+00037b60: 646f 6e65 2874 696d 656f 7574 290a 0a20  done(timeout).. 
+00037b70: 2020 2040 6976 695f 7379 6e63 6872 6f6e     @ivi_synchron
+00037b80: 697a 6564 0a20 2020 2064 6566 2077 7269  ized.    def wri
+00037b90: 7465 5f73 6571 7565 6e63 6572 5f66 6c61  te_sequencer_fla
+00037ba0: 6728 7365 6c66 2c20 666c 6167 2c20 7661  g(self, flag, va
+00037bb0: 6c75 6529 3a0a 2020 2020 2020 2020 7227  lue):.        r'
+00037bc0: 2727 7772 6974 655f 7365 7175 656e 6365  ''write_sequence
+00037bd0: 725f 666c 6167 0a0a 2020 2020 2020 2020  r_flag..        
+00037be0: 5772 6974 6573 2074 6865 2073 7461 7465  Writes the state
+00037bf0: 206f 6620 6120 7061 7474 6572 6e20 7365   of a pattern se
+00037c00: 7175 656e 6365 7220 666c 6167 2e20 5573  quencer flag. Us
+00037c10: 6520 7061 7474 6572 6e20 7365 7175 656e  e pattern sequen
+00037c20: 6365 7220 666c 6167 7320 746f 2063 6f6f  cer flags to coo
+00037c30: 7264 696e 6174 6520 6578 6563 7574 696f  rdinate executio
+00037c40: 6e20 6265 7477 6565 6e20 7468 6520 7061  n between the pa
+00037c50: 7474 6572 6e20 7365 7175 656e 6365 7220  ttern sequencer 
+00037c60: 616e 6420 6120 7275 6e74 696d 6520 7465  and a runtime te
+00037c70: 7374 2070 726f 6772 616d 2e0a 0a20 2020  st program...   
+00037c80: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00037c90: 2020 2020 2020 2066 6c61 6720 2865 6e75         flag (enu
+00037ca0: 6d73 2e53 6571 7565 6e63 6572 466c 6167  ms.SequencerFlag
+00037cb0: 293a 2054 6865 2070 6174 7465 726e 2073  ): The pattern s
+00037cc0: 6571 7565 6e63 6572 2066 6c61 6720 746f  equencer flag to
+00037cd0: 2077 7269 7465 2e0a 0a20 2020 2020 2020   write...       
+00037ce0: 2020 2020 2020 2020 202d 2020 2053 6571           -   Seq
+00037cf0: 7565 6e63 6572 466c 6167 2e46 4c41 4730  uencerFlag.FLAG0
+00037d00: 2028 2273 6571 666c 6167 3022 293a 2057   ("seqflag0"): W
+00037d10: 7269 7465 7320 7061 7474 6572 6e20 7365  rites pattern se
+00037d20: 7175 656e 6365 7220 666c 6167 2030 2e0a  quencer flag 0..
+00037d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00037d40: 2d20 2020 5365 7175 656e 6365 7246 6c61  -   SequencerFla
+00037d50: 672e 464c 4147 3120 2822 7365 7166 6c61  g.FLAG1 ("seqfla
+00037d60: 6731 2229 3a20 5772 6974 6573 2070 6174  g1"): Writes pat
+00037d70: 7465 726e 2073 6571 7565 6e63 6572 2066  tern sequencer f
+00037d80: 6c61 6720 312e 0a20 2020 2020 2020 2020  lag 1..         
+00037d90: 2020 2020 2020 202d 2020 2053 6571 7565         -   Seque
+00037da0: 6e63 6572 466c 6167 2e46 4c41 4732 2028  ncerFlag.FLAG2 (
+00037db0: 2273 6571 666c 6167 3222 293a 2057 7269  "seqflag2"): Wri
+00037dc0: 7465 7320 7061 7474 6572 6e20 7365 7175  tes pattern sequ
+00037dd0: 656e 6365 7220 666c 6167 2032 2e0a 2020  encer flag 2..  
+00037de0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00037df0: 2020 5365 7175 656e 6365 7246 6c61 672e    SequencerFlag.
+00037e00: 464c 4147 3320 2822 7365 7166 6c61 6733  FLAG3 ("seqflag3
+00037e10: 2229 3a20 5772 6974 6573 2070 6174 7465  "): Writes patte
+00037e20: 726e 2073 6571 7565 6e63 6572 2066 6c61  rn sequencer fla
+00037e30: 6720 332e 0a0a 2020 2020 2020 2020 2020  g 3...          
+00037e40: 2020 7661 6c75 6520 2862 6f6f 6c29 3a20    value (bool): 
+00037e50: 4120 426f 6f6c 6561 6e20 7468 6174 2061  A Boolean that a
+00037e60: 7373 6967 6e73 2061 2073 7461 7465 2074  ssigns a state t
+00037e70: 6f20 7468 6520 7061 7474 6572 6e20 7365  o the pattern se
+00037e80: 7175 656e 6365 7220 666c 6167 2079 6f75  quencer flag you
+00037e90: 2073 7065 6369 6679 2e0a 0a20 2020 2020   specify...     
+00037ea0: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+00037eb0: 6620 7479 7065 2866 6c61 6729 2069 7320  f type(flag) is 
+00037ec0: 6e6f 7420 656e 756d 732e 5365 7175 656e  not enums.Sequen
+00037ed0: 6365 7246 6c61 673a 0a20 2020 2020 2020  cerFlag:.       
+00037ee0: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+00037ef0: 7272 6f72 2827 5061 7261 6d65 7465 7220  rror('Parameter 
+00037f00: 666c 6167 206d 7573 7420 6265 206f 6620  flag must be of 
+00037f10: 7479 7065 2027 202b 2073 7472 2865 6e75  type ' + str(enu
+00037f20: 6d73 2e53 6571 7565 6e63 6572 466c 6167  ms.SequencerFlag
+00037f30: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00037f40: 5f69 6e74 6572 7072 6574 6572 2e77 7269  _interpreter.wri
+00037f50: 7465 5f73 6571 7565 6e63 6572 5f66 6c61  te_sequencer_fla
+00037f60: 6728 666c 6167 2c20 7661 6c75 6529 0a0a  g(flag, value)..
+00037f70: 2020 2020 4069 7669 5f73 796e 6368 726f      @ivi_synchro
+00037f80: 6e69 7a65 640a 2020 2020 6465 6620 7772  nized.    def wr
+00037f90: 6974 655f 7365 7175 656e 6365 725f 7265  ite_sequencer_re
+00037fa0: 6769 7374 6572 2873 656c 662c 2072 6567  gister(self, reg
+00037fb0: 2c20 7661 6c75 6529 3a0a 2020 2020 2020  , value):.      
+00037fc0: 2020 7227 2727 7772 6974 655f 7365 7175    r'''write_sequ
+00037fd0: 656e 6365 725f 7265 6769 7374 6572 0a0a  encer_register..
+00037fe0: 2020 2020 2020 2020 5772 6974 6573 2061          Writes a
+00037ff0: 2076 616c 7565 2074 6f20 6120 7061 7474   value to a patt
+00038000: 6572 6e20 7365 7175 656e 6365 7220 7265  ern sequencer re
+00038010: 6769 7374 6572 2e20 5573 6520 7061 7474  gister. Use patt
+00038020: 6572 6e20 7365 7175 656e 6365 7220 7265  ern sequencer re
+00038030: 6769 7374 6572 7320 746f 2070 6173 7320  gisters to pass 
+00038040: 6e75 6d65 7269 6320 7661 6c75 6573 2062  numeric values b
+00038050: 6574 7765 656e 2074 6865 2070 6174 7465  etween the patte
+00038060: 726e 2073 6571 7565 6e63 6572 2061 6e64  rn sequencer and
+00038070: 2061 2072 756e 7469 6d65 2074 6573 7420   a runtime test 
+00038080: 7072 6f67 7261 6d2e 0a0a 2020 2020 2020  program...      
+00038090: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000380a0: 2020 2020 7265 6720 2865 6e75 6d73 2e53      reg (enums.S
+000380b0: 6571 7565 6e63 6572 5265 6769 7374 6572  equencerRegister
+000380c0: 293a 2054 6865 2073 6571 7565 6e63 6572  ): The sequencer
+000380d0: 2072 6567 6973 7465 7220 796f 7520 7761   register you wa
+000380e0: 6e74 2074 6f20 7772 6974 6520 746f 2e0a  nt to write to..
+000380f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00038100: 202d 2020 2053 6571 7565 6e63 6572 5265   -   SequencerRe
+00038110: 6769 7374 6572 2e52 4547 4953 5445 5230  gister.REGISTER0
+00038120: 2028 2272 6567 3022 293a 2057 7269 7465   ("reg0"): Write
+00038130: 7320 7365 7175 656e 6365 7220 7265 6769  s sequencer regi
+00038140: 7374 6572 2030 2e0a 2020 2020 2020 2020  ster 0..        
+00038150: 2020 2020 2020 2020 2d20 2020 5365 7175          -   Sequ
+00038160: 656e 6365 7252 6567 6973 7465 722e 5245  encerRegister.RE
+00038170: 4749 5354 4552 3120 2822 7265 6731 2229  GISTER1 ("reg1")
+00038180: 3a20 5772 6974 6573 2073 6571 7565 6e63  : Writes sequenc
+00038190: 6572 2072 6567 6973 7465 7220 312e 0a20  er register 1.. 
+000381a0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+000381b0: 2020 2053 6571 7565 6e63 6572 5265 6769     SequencerRegi
+000381c0: 7374 6572 2e52 4547 4953 5445 5232 2028  ster.REGISTER2 (
+000381d0: 2272 6567 3222 293a 2057 7269 7465 7320  "reg2"): Writes 
+000381e0: 7365 7175 656e 6365 7220 7265 6769 7374  sequencer regist
+000381f0: 6572 2032 2e0a 2020 2020 2020 2020 2020  er 2..          
+00038200: 2020 2020 2020 2d20 2020 5365 7175 656e        -   Sequen
+00038210: 6365 7252 6567 6973 7465 722e 5245 4749  cerRegister.REGI
+00038220: 5354 4552 3320 2822 7265 6733 2229 3a20  STER3 ("reg3"): 
+00038230: 5772 6974 6573 2073 6571 7565 6e63 6572  Writes sequencer
+00038240: 2072 6567 6973 7465 7220 332e 0a20 2020   register 3..   
+00038250: 2020 2020 2020 2020 2020 2020 202d 2020               -  
+00038260: 2053 6571 7565 6e63 6572 5265 6769 7374   SequencerRegist
+00038270: 6572 2e52 4547 4953 5445 5234 2028 2272  er.REGISTER4 ("r
+00038280: 6567 3422 293a 2057 7269 7465 7320 7365  eg4"): Writes se
+00038290: 7175 656e 6365 7220 7265 6769 7374 6572  quencer register
+000382a0: 2034 2e0a 2020 2020 2020 2020 2020 2020   4..            
+000382b0: 2020 2020 2d20 2020 5365 7175 656e 6365      -   Sequence
+000382c0: 7252 6567 6973 7465 722e 5245 4749 5354  rRegister.REGIST
+000382d0: 4552 3520 2822 7265 6735 2229 3a20 5772  ER5 ("reg5"): Wr
+000382e0: 6974 6573 2073 6571 7565 6e63 6572 2072  ites sequencer r
+000382f0: 6567 6973 7465 7220 352e 0a20 2020 2020  egister 5..     
+00038300: 2020 2020 2020 2020 2020 202d 2020 2053             -   S
+00038310: 6571 7565 6e63 6572 5265 6769 7374 6572  equencerRegister
+00038320: 2e52 4547 4953 5445 5236 2028 2272 6567  .REGISTER6 ("reg
+00038330: 3622 293a 2057 7269 7465 7320 7365 7175  6"): Writes sequ
+00038340: 656e 6365 7220 7265 6769 7374 6572 2036  encer register 6
+00038350: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00038360: 2020 2d20 2020 5365 7175 656e 6365 7252    -   SequencerR
+00038370: 6567 6973 7465 722e 5245 4749 5354 4552  egister.REGISTER
+00038380: 3720 2822 7265 6737 2229 3a20 5772 6974  7 ("reg7"): Writ
+00038390: 6573 2073 6571 7565 6e63 6572 2072 6567  es sequencer reg
+000383a0: 6973 7465 7220 372e 0a20 2020 2020 2020  ister 7..       
+000383b0: 2020 2020 2020 2020 202d 2020 2053 6571           -   Seq
+000383c0: 7565 6e63 6572 5265 6769 7374 6572 2e52  uencerRegister.R
+000383d0: 4547 4953 5445 5238 2028 2272 6567 3822  EGISTER8 ("reg8"
+000383e0: 293a 2057 7269 7465 7320 7365 7175 656e  ): Writes sequen
+000383f0: 6365 7220 7265 6769 7374 6572 2038 2e0a  cer register 8..
+00038400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00038410: 2d20 2020 5365 7175 656e 6365 7252 6567  -   SequencerReg
+00038420: 6973 7465 722e 5245 4749 5354 4552 3920  ister.REGISTER9 
+00038430: 2822 7265 6739 2229 3a20 5772 6974 6573  ("reg9"): Writes
+00038440: 2073 6571 7565 6e63 6572 2072 6567 6973   sequencer regis
+00038450: 7465 7220 392e 0a20 2020 2020 2020 2020  ter 9..         
+00038460: 2020 2020 2020 202d 2020 2053 6571 7565         -   Seque
+00038470: 6e63 6572 5265 6769 7374 6572 2e52 4547  ncerRegister.REG
+00038480: 4953 5445 5231 3020 2822 7265 6731 3022  ISTER10 ("reg10"
+00038490: 293a 2057 7269 7465 7320 7365 7175 656e  ): Writes sequen
+000384a0: 6365 7220 7265 6769 7374 6572 2031 302e  cer register 10.
+000384b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000384c0: 202d 2020 2053 6571 7565 6e63 6572 5265   -   SequencerRe
+000384d0: 6769 7374 6572 2e52 4547 4953 5445 5231  gister.REGISTER1
+000384e0: 3120 2822 7265 6731 3122 293a 2057 7269  1 ("reg11"): Wri
+000384f0: 7465 7320 7365 7175 656e 6365 7220 7265  tes sequencer re
+00038500: 6769 7374 6572 2031 312e 0a20 2020 2020  gister 11..     
+00038510: 2020 2020 2020 2020 2020 202d 2020 2053             -   S
+00038520: 6571 7565 6e63 6572 5265 6769 7374 6572  equencerRegister
+00038530: 2e52 4547 4953 5445 5231 3220 2822 7265  .REGISTER12 ("re
+00038540: 6731 3222 293a 2057 7269 7465 7320 7365  g12"): Writes se
+00038550: 7175 656e 6365 7220 7265 6769 7374 6572  quencer register
+00038560: 2031 322e 0a20 2020 2020 2020 2020 2020   12..           
+00038570: 2020 2020 202d 2020 2053 6571 7565 6e63       -   Sequenc
+00038580: 6572 5265 6769 7374 6572 2e52 4547 4953  erRegister.REGIS
+00038590: 5445 5231 3320 2822 7265 6731 3322 293a  TER13 ("reg13"):
+000385a0: 2057 7269 7465 7320 7365 7175 656e 6365   Writes sequence
+000385b0: 7220 7265 6769 7374 6572 2031 332e 0a20  r register 13.. 
+000385c0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+000385d0: 2020 2053 6571 7565 6e63 6572 5265 6769     SequencerRegi
+000385e0: 7374 6572 2e52 4547 4953 5445 5231 3420  ster.REGISTER14 
+000385f0: 2822 7265 6731 3422 293a 2057 7269 7465  ("reg14"): Write
+00038600: 7320 7365 7175 656e 6365 7220 7265 6769  s sequencer regi
+00038610: 7374 6572 2031 342e 0a20 2020 2020 2020  ster 14..       
+00038620: 2020 2020 2020 2020 202d 2020 2053 6571           -   Seq
+00038630: 7565 6e63 6572 5265 6769 7374 6572 2e52  uencerRegister.R
+00038640: 4547 4953 5445 5231 3520 2822 7265 6731  EGISTER15 ("reg1
+00038650: 3522 293a 2057 7269 7465 7320 7365 7175  5"): Writes sequ
+00038660: 656e 6365 7220 7265 6769 7374 6572 2031  encer register 1
+00038670: 352e 0a0a 2020 2020 2020 2020 2020 2020  5...            
+00038680: 7661 6c75 6520 2869 6e74 293a 2054 6865  value (int): The
+00038690: 2076 616c 7565 2079 6f75 2077 616e 7420   value you want 
+000386a0: 746f 2077 7269 7465 2074 6f20 7468 6520  to write to the 
+000386b0: 7265 6769 7374 6572 2e0a 0a20 2020 2020  register...     
+000386c0: 2020 2027 2727 0a20 2020 2020 2020 2069     '''.        i
+000386d0: 6620 7479 7065 2872 6567 2920 6973 206e  f type(reg) is n
+000386e0: 6f74 2065 6e75 6d73 2e53 6571 7565 6e63  ot enums.Sequenc
+000386f0: 6572 5265 6769 7374 6572 3a0a 2020 2020  erRegister:.    
+00038700: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+00038710: 7065 4572 726f 7228 2750 6172 616d 6574  peError('Paramet
+00038720: 6572 2072 6567 206d 7573 7420 6265 206f  er reg must be o
+00038730: 6620 7479 7065 2027 202b 2073 7472 2865  f type ' + str(e
+00038740: 6e75 6d73 2e53 6571 7565 6e63 6572 5265  nums.SequencerRe
+00038750: 6769 7374 6572 2929 0a20 2020 2020 2020  gister)).       
+00038760: 2073 656c 662e 5f69 6e74 6572 7072 6574   self._interpret
+00038770: 6572 2e77 7269 7465 5f73 6571 7565 6e63  er.write_sequenc
+00038780: 6572 5f72 6567 6973 7465 7228 7265 672c  er_register(reg,
+00038790: 2076 616c 7565 290a 0a20 2020 2040 6976   value)..    @iv
+000387a0: 695f 7379 6e63 6872 6f6e 697a 6564 0a20  i_synchronized. 
+000387b0: 2020 2064 6566 2077 7269 7465 5f73 6f75     def write_sou
+000387c0: 7263 655f 7761 7665 666f 726d 5f62 726f  rce_waveform_bro
+000387d0: 6164 6361 7374 2873 656c 662c 2077 6176  adcast(self, wav
+000387e0: 6566 6f72 6d5f 6e61 6d65 2c20 7761 7665  eform_name, wave
+000387f0: 666f 726d 5f64 6174 6129 3a0a 2020 2020  form_data):.    
+00038800: 2020 2020 7227 2727 7772 6974 655f 736f      r'''write_so
+00038810: 7572 6365 5f77 6176 6566 6f72 6d5f 6272  urce_waveform_br
+00038820: 6f61 6463 6173 740a 0a20 2020 2020 2020  oadcast..       
+00038830: 2057 7269 7465 7320 7468 6520 7361 6d65   Writes the same
+00038840: 2077 6176 6566 6f72 6d20 6461 7461 2074   waveform data t
+00038850: 6f20 616c 6c20 7369 7465 732e 2055 7365  o all sites. Use
+00038860: 2074 6869 7320 7772 6974 6520 6d65 7468   this write meth
+00038870: 6f64 2069 6620 796f 7520 7365 7420 7468  od if you set th
+00038880: 6520 6461 7461 5f6d 6170 7069 6e67 2070  e data_mapping p
+00038890: 6172 616d 6574 6572 206f 6620 7468 6520  arameter of the 
+000388a0: 6372 6561 7465 2073 6f75 7263 6520 7761  create source wa
+000388b0: 7665 666f 726d 206d 6574 686f 6420 746f  veform method to
+000388c0: 2053 6f75 7263 6544 6174 614d 6170 7069   SourceDataMappi
+000388d0: 6e67 2e42 524f 4144 4341 5354 2e0a 0a20  ng.BROADCAST... 
+000388e0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000388f0: 2020 2020 2020 2020 2077 6176 6566 6f72           wavefor
+00038900: 6d5f 6e61 6d65 2028 7374 7229 3a20 5468  m_name (str): Th
+00038910: 6520 6e61 6d65 2074 6f20 6173 7369 676e  e name to assign
+00038920: 2074 6f20 7468 6520 7761 7665 666f 726d   to the waveform
+00038930: 2e20 5573 6520 7468 6520 7761 7665 666f  . Use the wavefo
+00038940: 726d 5f6e 616d 6520 2077 6974 6820 736f  rm_name  with so
+00038950: 7572 6365 5f73 7461 7274 206f 7063 6f64  urce_start opcod
+00038960: 6520 696e 2079 6f75 7220 7061 7474 6572  e in your patter
+00038970: 6e2e 0a0a 2020 2020 2020 2020 2020 2020  n...            
+00038980: 7761 7665 666f 726d 5f64 6174 6120 286c  waveform_data (l
+00038990: 6973 7420 6f66 2069 6e74 293a 2031 4420  ist of int): 1D 
+000389a0: 6172 7261 7920 6f66 2073 616d 706c 6573  array of samples
+000389b0: 2074 6f20 7573 6520 6173 2073 6f75 7263   to use as sourc
+000389c0: 6520 6461 7461 2074 6f20 6170 706c 7920  e data to apply 
+000389d0: 746f 2061 6c6c 2073 6974 6573 2e0a 0a20  to all sites... 
+000389e0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+000389f0: 2020 2073 656c 662e 5f69 6e74 6572 7072     self._interpr
+00038a00: 6574 6572 2e77 7269 7465 5f73 6f75 7263  eter.write_sourc
+00038a10: 655f 7761 7665 666f 726d 5f62 726f 6164  e_waveform_broad
+00038a20: 6361 7374 2877 6176 6566 6f72 6d5f 6e61  cast(waveform_na
+00038a30: 6d65 2c20 7761 7665 666f 726d 5f64 6174  me, waveform_dat
+00038a40: 6129 0a0a 2020 2020 4069 7669 5f73 796e  a)..    @ivi_syn
+00038a50: 6368 726f 6e69 7a65 640a 2020 2020 6465  chronized.    de
+00038a60: 6620 7772 6974 655f 736f 7572 6365 5f77  f write_source_w
+00038a70: 6176 6566 6f72 6d5f 6461 7461 5f66 726f  aveform_data_fro
+00038a80: 6d5f 6669 6c65 5f74 646d 7328 7365 6c66  m_file_tdms(self
+00038a90: 2c20 7761 7665 666f 726d 5f6e 616d 652c  , waveform_name,
+00038aa0: 2077 6176 6566 6f72 6d5f 6669 6c65 5f70   waveform_file_p
+00038ab0: 6174 6829 3a0a 2020 2020 2020 2020 7227  ath):.        r'
+00038ac0: 2727 7772 6974 655f 736f 7572 6365 5f77  ''write_source_w
+00038ad0: 6176 6566 6f72 6d5f 6461 7461 5f66 726f  aveform_data_fro
+00038ae0: 6d5f 6669 6c65 5f74 646d 730a 0a20 2020  m_file_tdms..   
+00038af0: 2020 2020 2057 7269 7465 7320 6120 736f       Writes a so
+00038b00: 7572 6365 2077 6176 6566 6f72 6d20 6261  urce waveform ba
+00038b10: 7365 6420 6f6e 2074 6865 2077 6176 6566  sed on the wavef
+00038b20: 6f72 6d20 6461 7461 2061 6e64 2063 6f6e  orm data and con
+00038b30: 6669 6775 7261 7469 6f6e 2069 6e66 6f72  figuration infor
+00038b40: 6d61 7469 6f6e 2074 6865 2066 696c 6520  mation the file 
+00038b50: 636f 6e74 6169 6e73 2e0a 0a20 2020 2020  contains...     
+00038b60: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00038b70: 2020 2020 2077 6176 6566 6f72 6d5f 6e61       waveform_na
+00038b80: 6d65 2028 7374 7229 3a20 5468 6520 6e61  me (str): The na
+00038b90: 6d65 2074 6f20 6173 7369 676e 2074 6f20  me to assign to 
+00038ba0: 7468 6520 7761 7665 666f 726d 2e20 5573  the waveform. Us
+00038bb0: 6520 7468 6520 7761 7665 666f 726d 5f6e  e the waveform_n
+00038bc0: 616d 6520 2077 6974 6820 736f 7572 6365  ame  with source
+00038bd0: 5f73 7461 7274 206f 7063 6f64 6520 696e  _start opcode in
+00038be0: 2079 6f75 7220 7061 7474 6572 6e2e 0a0a   your pattern...
+00038bf0: 2020 2020 2020 2020 2020 2020 7761 7665              wave
+00038c00: 666f 726d 5f66 696c 655f 7061 7468 2028  form_file_path (
+00038c10: 7374 7229 3a20 4162 736f 6c75 7465 2066  str): Absolute f
+00038c20: 696c 6520 7061 7468 2074 6f20 7468 6520  ile path to the 
+00038c30: 6c6f 6164 2073 6f75 7263 6520 7761 7665  load source wave
+00038c40: 666f 726d 2066 696c 6520 282e 7464 6d73  form file (.tdms
+00038c50: 292e 0a0a 2020 2020 2020 2020 2727 270a  )...        '''.
+00038c60: 2020 2020 2020 2020 7365 6c66 2e5f 696e          self._in
+00038c70: 7465 7270 7265 7465 722e 7772 6974 655f  terpreter.write_
+00038c80: 736f 7572 6365 5f77 6176 6566 6f72 6d5f  source_waveform_
+00038c90: 6461 7461 5f66 726f 6d5f 6669 6c65 5f74  data_from_file_t
+00038ca0: 646d 7328 7761 7665 666f 726d 5f6e 616d  dms(waveform_nam
+00038cb0: 652c 2077 6176 6566 6f72 6d5f 6669 6c65  e, waveform_file
+00038cc0: 5f70 6174 6829 0a0a 2020 2020 6465 6620  _path)..    def 
+00038cd0: 5f63 6c6f 7365 2873 656c 6629 3a0a 2020  _close(self):.  
+00038ce0: 2020 2020 2020 7227 2727 5f63 6c6f 7365        r'''_close
+00038cf0: 0a0a 2020 2020 2020 2020 436c 6f73 6573  ..        Closes
+00038d00: 2074 6865 2073 7065 6369 6669 6564 2069   the specified i
+00038d10: 6e73 7472 756d 656e 7420 7365 7373 696f  nstrument sessio
+00038d20: 6e20 746f 2061 2064 6967 6974 616c 2070  n to a digital p
+00038d30: 6174 7465 726e 2069 6e73 7472 756d 656e  attern instrumen
+00038d40: 742c 2061 626f 7274 7320 7061 7474 6572  t, aborts patter
+00038d50: 6e20 6578 6563 7574 696f 6e2c 2061 6e64  n execution, and
+00038d60: 2075 6e6c 6f61 6473 2070 6174 7465 726e   unloads pattern
+00038d70: 206d 656d 6f72 792e 2054 6865 2063 6861   memory. The cha
+00038d80: 6e6e 656c 7320 6f6e 2061 2064 6967 6974  nnels on a digit
+00038d90: 616c 2070 6174 7465 726e 2069 6e73 7472  al pattern instr
+00038da0: 756d 656e 7420 7265 6d61 696e 2069 6e20  ument remain in 
+00038db0: 7468 6569 7220 6375 7272 656e 7420 7374  their current st
+00038dc0: 6174 652e 0a20 2020 2020 2020 2027 2727  ate..        '''
+00038dd0: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+00038de0: 6e74 6572 7072 6574 6572 2e63 6c6f 7365  nterpreter.close
+00038df0: 2829 0a0a 2020 2020 4069 7669 5f73 796e  ()..    @ivi_syn
+00038e00: 6368 726f 6e69 7a65 640a 2020 2020 6465  chronized.    de
+00038e10: 6620 7265 7365 7428 7365 6c66 293a 0a20  f reset(self):. 
+00038e20: 2020 2020 2020 2072 2727 2772 6573 6574         r'''reset
+00038e30: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00038e40: 7320 6120 6469 6769 7461 6c20 7061 7474  s a digital patt
+00038e50: 6572 6e20 696e 7374 7275 6d65 6e74 2074  ern instrument t
+00038e60: 6f20 6120 6b6e 6f77 6e20 7374 6174 652e  o a known state.
+00038e70: 2054 6869 7320 6d65 7468 6f64 2070 6572   This method per
+00038e80: 666f 726d 7320 7468 6520 666f 6c6c 6f77  forms the follow
+00038e90: 696e 6720 6163 7469 6f6e 733a 0a0a 2020  ing actions:..  
+00038ea0: 2020 2020 2020 2d20 4162 6f72 7473 2070        - Aborts p
+00038eb0: 6174 7465 726e 2065 7865 6375 7469 6f6e  attern execution
+00038ec0: 2e0a 2020 2020 2020 2020 2d20 436c 6561  ..        - Clea
+00038ed0: 7273 2070 696e 206d 6170 732c 2074 696d  rs pin maps, tim
+00038ee0: 6520 7365 7473 2c20 736f 7572 6365 2061  e sets, source a
+00038ef0: 6e64 2063 6170 7475 7265 2077 6176 6566  nd capture wavef
+00038f00: 6f72 6d73 2c20 616e 6420 7061 7474 6572  orms, and patter
+00038f10: 6e73 2e0a 2020 2020 2020 2020 2d20 5265  ns..        - Re
+00038f20: 7365 7473 2061 6c6c 2070 726f 7065 7274  sets all propert
+00038f30: 6965 7320 746f 2064 6566 6175 6c74 2076  ies to default v
+00038f40: 616c 7565 732c 2069 6e63 6c75 6469 6e67  alues, including
+00038f50: 2074 6865 2073 656c 6563 7465 645f 6675   the selected_fu
+00038f60: 6e63 7469 6f6e 2070 726f 7065 7274 7920  nction property 
+00038f70: 7468 6174 2069 7320 7365 7420 746f 2053  that is set to S
+00038f80: 656c 6563 7465 6446 756e 6374 696f 6e2e  electedFunction.
+00038f90: 4449 5343 4f4e 4e45 4354 2c20 6361 7573  DISCONNECT, caus
+00038fa0: 696e 6720 7468 6520 492f 4f20 7377 6974  ing the I/O swit
+00038fb0: 6368 6573 2074 6f20 6f70 656e 2e0a 2020  ches to open..  
+00038fc0: 2020 2020 2020 2d20 5374 6f70 7320 6578        - Stops ex
+00038fd0: 706f 7274 696e 6720 616c 6c20 6578 7465  porting all exte
+00038fe0: 726e 616c 2073 6967 6e61 6c73 2061 6e64  rnal signals and
+00038ff0: 2065 7665 6e74 732e 0a20 2020 2020 2020   events..       
+00039000: 2027 2727 0a20 2020 2020 2020 2073 656c   '''.        sel
+00039010: 662e 5f69 6e74 6572 7072 6574 6572 2e72  f._interpreter.r
+00039020: 6573 6574 2829 0a0a 2020 2020 4069 7669  eset()..    @ivi
+00039030: 5f73 796e 6368 726f 6e69 7a65 640a 2020  _synchronized.  
+00039040: 2020 6465 6620 5f73 656c 665f 7465 7374    def _self_test
+00039050: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00039060: 7227 2727 5f73 656c 665f 7465 7374 0a0a  r'''_self_test..
+00039070: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
+00039080: 7365 6c66 2074 6573 7420 7265 7375 6c74  self test result
+00039090: 7320 6672 6f6d 2061 2064 6967 6974 616c  s from a digital
+000390a0: 2070 6174 7465 726e 2069 6e73 7472 756d   pattern instrum
+000390b0: 656e 742e 2054 6869 7320 7465 7374 2072  ent. This test r
+000390c0: 6571 7569 7265 7320 7365 7665 7261 6c20  equires several 
+000390d0: 6d69 6e75 7465 7320 746f 2065 7865 6375  minutes to execu
+000390e0: 7465 2e0a 0a20 2020 2020 2020 2052 6574  te...        Ret
+000390f0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00039100: 2020 7465 7374 5f72 6573 756c 7420 2869    test_result (i
+00039110: 6e74 293a 2041 2070 6172 616d 6574 6572  nt): A parameter
+00039120: 2074 6861 7420 696e 6469 6361 7465 7320   that indicates 
+00039130: 6966 2074 6865 2073 656c 6620 7465 7374  if the self test
+00039140: 2070 6173 7365 6420 2830 2920 6f72 2066   passed (0) or f
+00039150: 6169 6c65 6420 2821 3d30 292e 0a0a 2020  ailed (!=0)...  
+00039160: 2020 2020 2020 2020 2020 7465 7374 5f6d            test_m
+00039170: 6573 7361 6765 2028 7374 7229 3a20 5468  essage (str): Th
+00039180: 6520 7265 7475 726e 6564 2073 656c 6620  e returned self 
+00039190: 7465 7374 2073 7461 7475 7320 6d65 7373  test status mess
+000391a0: 6167 652e 2054 6865 2061 7272 6179 206d  age. The array m
+000391b0: 7573 7420 636f 6e74 6169 6e20 6174 206c  ust contain at l
+000391c0: 6561 7374 2032 3536 2063 6861 7261 6374  east 256 charact
+000391d0: 6572 732e 0a0a 2020 2020 2020 2020 2727  ers...        ''
+000391e0: 270a 2020 2020 2020 2020 7465 7374 5f72  '.        test_r
+000391f0: 6573 756c 742c 2074 6573 745f 6d65 7373  esult, test_mess
+00039200: 6167 6520 3d20 7365 6c66 2e5f 696e 7465  age = self._inte
+00039210: 7270 7265 7465 722e 7365 6c66 5f74 6573  rpreter.self_tes
+00039220: 7428 290a 2020 2020 2020 2020 7265 7475  t().        retu
+00039230: 726e 2074 6573 745f 7265 7375 6c74 2c20  rn test_result, 
+00039240: 7465 7374 5f6d 6573 7361 6765 0a         test_message.
```

### Comparing `nidigital-1.4.4/nidigital/session_pb2.py` & `nidigital-1.4.5/nidigital/session_pb2.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital/session_pb2_grpc.py` & `nidigital-1.4.5/nidigital/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/nidigital.egg-info/PKG-INFO` & `nidigital-1.4.5/nidigital.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidigital
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-Digital Pattern Driver Python API
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
 
 As a prerequisite to using the nidigital module, you must install the NI-Digital Pattern Driver runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-Digital Pattern Driver**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidigital~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidigital
+  $ python -m pip install nidigital~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -199,30 +195,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidigital/examples>`_
 
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

### Comparing `nidigital-1.4.4/nidigital.egg-info/SOURCES.txt` & `nidigital-1.4.5/nidigital.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.4/setup.py` & `nidigital-1.4.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.4',
+    version='1.4.5',
     description='NI-Digital Pattern Driver Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -44,15 +44,15 @@
     packages=['nidigital'],
     install_requires=[
         'hightime>=0.2.0',
         'nitclk',
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
@@ -65,13 +65,14 @@
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

