# Comparing `tmp/niswitch-1.4.4.tar.gz` & `tmp/niswitch-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niswitch-1.4.4.tar", last modified: Fri Apr 14 16:09:08 2023, max compression
+gzip compressed data, was "niswitch-1.4.5.tar", last modified: Mon Jun 12 00:41:04 2023, max compression
```

## Comparing `niswitch-1.4.4.tar` & `niswitch-1.4.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:18.410721 niswitch-1.4.4/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8761 2023-04-14 16:09:18.408721 niswitch-1.4.4/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7768 2023-04-14 16:06:40.000000 niswitch-1.4.4/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:18.324720 niswitch-1.4.4/niswitch/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:06:29.000000 niswitch-1.4.4/niswitch/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3047 2023-04-14 16:06:27.000000 niswitch-1.4.4/niswitch/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5444 2023-04-14 16:06:20.000000 niswitch-1.4.4/niswitch/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13875 2023-04-14 16:06:28.000000 niswitch-1.4.4/niswitch/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12650 2023-04-14 16:06:30.000000 niswitch-1.4.4/niswitch/_grpc_stub_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    24762 2023-04-14 16:06:22.000000 niswitch-1.4.4/niswitch/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    25339 2023-04-14 16:06:23.000000 niswitch-1.4.4/niswitch/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1623 2023-04-14 16:06:24.000000 niswitch-1.4.4/niswitch/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:06:33.000000 niswitch-1.4.4/niswitch/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13707 2023-04-14 16:06:21.000000 niswitch-1.4.4/niswitch/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4381 2023-04-14 16:06:25.000000 niswitch-1.4.4/niswitch/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3456 2023-04-14 16:06:31.000000 niswitch-1.4.4/niswitch/grpc_session_options.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-04-14 16:06:32.000000 niswitch-1.4.4/niswitch/nidevice_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-04-14 16:06:32.000000 niswitch-1.4.4/niswitch/nidevice_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    55730 2023-04-14 16:06:31.000000 niswitch-1.4.4/niswitch/niswitch_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    96817 2023-04-14 16:06:31.000000 niswitch-1.4.4/niswitch/niswitch_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   114951 2023-04-14 16:06:24.000000 niswitch-1.4.4/niswitch/session.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-04-14 16:06:33.000000 niswitch-1.4.4/niswitch/session_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-04-14 16:06:33.000000 niswitch-1.4.4/niswitch/session_pb2_grpc.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:18.396722 niswitch-1.4.4/niswitch.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8761 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      686 2023-04-14 16:09:18.000000 niswitch-1.4.4/niswitch.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      154 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:09:18.410721 niswitch-1.4.4/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2200 2023-04-14 16:06:40.000000 niswitch-1.4.4/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:08.333868 niswitch-1.4.5/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8598 2023-06-12 00:41:08.331866 niswitch-1.4.5/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7514 2023-06-12 00:38:44.000000 niswitch-1.4.5/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:08.253438 niswitch-1.4.5/niswitch/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-06-12 00:38:33.000000 niswitch-1.4.5/niswitch/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3047 2023-06-12 00:38:32.000000 niswitch-1.4.5/niswitch/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5444 2023-06-12 00:38:26.000000 niswitch-1.4.5/niswitch/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13875 2023-06-12 00:38:32.000000 niswitch-1.4.5/niswitch/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12848 2023-06-12 00:38:34.000000 niswitch-1.4.5/niswitch/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    25549 2023-06-12 00:38:27.000000 niswitch-1.4.5/niswitch/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    26760 2023-06-12 00:38:28.000000 niswitch-1.4.5/niswitch/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1623 2023-06-12 00:38:28.000000 niswitch-1.4.5/niswitch/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-06-12 00:38:37.000000 niswitch-1.4.5/niswitch/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13707 2023-06-12 00:38:26.000000 niswitch-1.4.5/niswitch/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4377 2023-06-12 00:38:30.000000 niswitch-1.4.5/niswitch/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3456 2023-06-12 00:38:34.000000 niswitch-1.4.5/niswitch/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-06-12 00:38:36.000000 niswitch-1.4.5/niswitch/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-06-12 00:38:36.000000 niswitch-1.4.5/niswitch/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    55730 2023-06-12 00:38:35.000000 niswitch-1.4.5/niswitch/niswitch_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    96817 2023-06-12 00:38:35.000000 niswitch-1.4.5/niswitch/niswitch_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   114951 2023-06-12 00:38:29.000000 niswitch-1.4.5/niswitch/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-06-12 00:38:37.000000 niswitch-1.4.5/niswitch/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-06-12 00:38:37.000000 niswitch-1.4.5/niswitch/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:08.319854 niswitch-1.4.5/niswitch.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8598 2023-06-12 00:41:07.000000 niswitch-1.4.5/niswitch.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      686 2023-06-12 00:41:08.000000 niswitch-1.4.5/niswitch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:41:07.000000 niswitch-1.4.5/niswitch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      148 2023-06-12 00:41:07.000000 niswitch-1.4.5/niswitch.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-06-12 00:41:07.000000 niswitch-1.4.5/niswitch.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:41:07.000000 niswitch-1.4.5/niswitch.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-06-12 00:41:08.333868 niswitch-1.4.5/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2254 2023-06-12 00:38:45.000000 niswitch-1.4.5/setup.py
```

### Comparing `niswitch-1.4.4/PKG-INFO` & `niswitch-1.4.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niswitch
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-SWITCH Python API
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
 
 As a prerequisite to using the niswitch module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niswitch~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install niswitch
+  $ python -m pip install niswitch~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -167,30 +163,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/niswitch/examples>`_
 
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

### Comparing `niswitch-1.4.4/README.rst` & `niswitch-1.4.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -98,32 +98,27 @@
 
 
 .. |niswitchOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/niswitch.svg
     :alt: Pull Requests for NI-SWITCH
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Aniswitch
 
 
-
-.. _niswitch_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the niswitch module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install niswitch~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install niswitch
-
-
+
+.. _niswitch_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the niswitch module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install niswitch~=1.4.5
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -134,36 +129,34 @@
 
     import niswitch
     with niswitch.Session("Dev1") as session:
         session.connect(channel1='r0', channel2='c0')
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/niswitch/examples>`_
 
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

### Comparing `niswitch-1.4.4/niswitch/__init__.py` & `niswitch-1.4.5/niswitch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.4'
+__version__ = '1.4.5'
 
 from niswitch.enums import *  # noqa: F403,F401,H303
 from niswitch.errors import DriverWarning  # noqa: F401
 from niswitch.errors import Error  # noqa: F401
 from niswitch.grpc_session_options import *  # noqa: F403,F401,H303
 from niswitch.session import Session  # noqa: F401
 
@@ -61,15 +61,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-SWITCH"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'niswitch'
-    info['module']['version'] = "1.4.4"
+    info['module']['version'] = "1.4.5"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `niswitch-1.4.4/niswitch/_attributes.py` & `niswitch-1.4.5/niswitch/_attributes.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/_converters.py` & `niswitch-1.4.5/niswitch/_converters.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/_grpc_stub_interpreter.py` & `niswitch-1.4.5/niswitch/_grpc_stub_interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,17 @@
 
     def set_path(self, path_list):  # noqa: N802
         self._invoke(
             self._client.SetPath,
             grpc_types.SetPathRequest(vi=self._vi, path_list=path_list),
         )
 
+    def set_runtime_environment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        raise NotImplementedError('set_runtime_environment is not supported over gRPC')
+
     def unlock(self):  # noqa: N802
         self._lock.release()
 
     def wait_for_debounce(self, maximum_time_ms):  # noqa: N802
         self._invoke(
             self._client.WaitForDebounce,
             grpc_types.WaitForDebounceRequest(vi=self._vi, maximum_time_ms=maximum_time_ms),
```

### Comparing `niswitch-1.4.4/niswitch/_library.py` & `niswitch-1.4.5/niswitch/_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         self.niSwitch_RouteTriggerInput_cfunc = None
         self.niSwitch_SendSoftwareTrigger_cfunc = None
         self.niSwitch_SetAttributeViBoolean_cfunc = None
         self.niSwitch_SetAttributeViInt32_cfunc = None
         self.niSwitch_SetAttributeViReal64_cfunc = None
         self.niSwitch_SetAttributeViString_cfunc = None
         self.niSwitch_SetPath_cfunc = None
+        self.niSwitch_SetRuntimeEnvironment_cfunc = None
         self.niSwitch_UnlockSession_cfunc = None
         self.niSwitch_WaitForDebounce_cfunc = None
         self.niSwitch_WaitForScanComplete_cfunc = None
         self.niSwitch_close_cfunc = None
         self.niSwitch_error_message_cfunc = None
         self.niSwitch_reset_cfunc = None
         self.niSwitch_self_test_cfunc = None
@@ -174,21 +175,21 @@
         with self._func_lock:
             if self.niSwitch_GetChannelName_cfunc is None:
                 self.niSwitch_GetChannelName_cfunc = self._get_library_function('niSwitch_GetChannelName')
                 self.niSwitch_GetChannelName_cfunc.argtypes = [ViSession, ViInt32, ViInt32, ctypes.POINTER(ViChar)]  # noqa: F405
                 self.niSwitch_GetChannelName_cfunc.restype = ViStatus  # noqa: F405
         return self.niSwitch_GetChannelName_cfunc(vi, index, buffer_size, channel_name_buffer)
 
-    def niSwitch_GetError(self, vi, code, buffer_size, description):  # noqa: N802
+    def niSwitch_GetError(self, vi, error_code, buffer_size, description):  # noqa: N802
         with self._func_lock:
             if self.niSwitch_GetError_cfunc is None:
                 self.niSwitch_GetError_cfunc = self._get_library_function('niSwitch_GetError')
                 self.niSwitch_GetError_cfunc.argtypes = [ViSession, ctypes.POINTER(ViStatus), ViInt32, ctypes.POINTER(ViChar)]  # noqa: F405
                 self.niSwitch_GetError_cfunc.restype = ViStatus  # noqa: F405
-        return self.niSwitch_GetError_cfunc(vi, code, buffer_size, description)
+        return self.niSwitch_GetError_cfunc(vi, error_code, buffer_size, description)
 
     def niSwitch_GetPath(self, vi, channel1, channel2, buffer_size, path):  # noqa: N802
         with self._func_lock:
             if self.niSwitch_GetPath_cfunc is None:
                 self.niSwitch_GetPath_cfunc = self._get_library_function('niSwitch_GetPath')
                 self.niSwitch_GetPath_cfunc.argtypes = [ViSession, ctypes.POINTER(ViChar), ctypes.POINTER(ViChar), ViInt32, ctypes.POINTER(ViChar)]  # noqa: F405
                 self.niSwitch_GetPath_cfunc.restype = ViStatus  # noqa: F405
@@ -318,14 +319,22 @@
         with self._func_lock:
             if self.niSwitch_SetPath_cfunc is None:
                 self.niSwitch_SetPath_cfunc = self._get_library_function('niSwitch_SetPath')
                 self.niSwitch_SetPath_cfunc.argtypes = [ViSession, ctypes.POINTER(ViChar)]  # noqa: F405
                 self.niSwitch_SetPath_cfunc.restype = ViStatus  # noqa: F405
         return self.niSwitch_SetPath_cfunc(vi, path_list)
 
+    def niSwitch_SetRuntimeEnvironment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        with self._func_lock:
+            if self.niSwitch_SetRuntimeEnvironment_cfunc is None:
+                self.niSwitch_SetRuntimeEnvironment_cfunc = self._get_library_function('niSwitch_SetRuntimeEnvironment')
+                self.niSwitch_SetRuntimeEnvironment_cfunc.argtypes = [ctypes.POINTER(ViChar), ctypes.POINTER(ViChar), ctypes.POINTER(ViChar), ctypes.POINTER(ViChar)]  # noqa: F405
+                self.niSwitch_SetRuntimeEnvironment_cfunc.restype = ViStatus  # noqa: F405
+        return self.niSwitch_SetRuntimeEnvironment_cfunc(environment, environment_version, reserved1, reserved2)
+
     def niSwitch_UnlockSession(self, vi, caller_has_lock):  # noqa: N802
         with self._func_lock:
             if self.niSwitch_UnlockSession_cfunc is None:
                 self.niSwitch_UnlockSession_cfunc = self._get_library_function('niSwitch_UnlockSession')
                 self.niSwitch_UnlockSession_cfunc.argtypes = [ViSession, ctypes.POINTER(ViBoolean)]  # noqa: F405
                 self.niSwitch_UnlockSession_cfunc.restype = ViStatus  # noqa: F405
         return self.niSwitch_UnlockSession_cfunc(vi, caller_has_lock)
```

### Comparing `niswitch-1.4.4/niswitch/_library_interpreter.py` & `niswitch-1.4.5/niswitch/_library_interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 import array
 import ctypes
 import hightime  # noqa: F401
+import platform
+
 import niswitch._library_singleton as _library_singleton
 import niswitch._visatype as _visatype
 import niswitch.enums as enums  # noqa: F401
 import niswitch.errors as errors
 
 
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
@@ -206,24 +226,24 @@
         channel_name_buffer_ctype = (_visatype.ViChar * buffer_size_ctype.value)()  # case C060
         error_code = self._library.niSwitch_GetChannelName(vi_ctype, index_ctype, buffer_size_ctype, channel_name_buffer_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return channel_name_buffer_ctype.value.decode(self._encoding)
 
     def get_error(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
-        code_ctype = _visatype.ViStatus()  # case S220
+        error_code_ctype = _visatype.ViStatus()  # case S220
         buffer_size_ctype = _visatype.ViInt32()  # case S170
         description_ctype = None  # case C050
-        error_code = self._library.niSwitch_GetError(vi_ctype, None if code_ctype is None else (ctypes.pointer(code_ctype)), buffer_size_ctype, description_ctype)
+        error_code = self._library.niSwitch_GetError(vi_ctype, None if error_code_ctype is None else (ctypes.pointer(error_code_ctype)), buffer_size_ctype, description_ctype)
         errors.handle_error(self, error_code, ignore_warnings=True, is_error_handling=True)
         buffer_size_ctype = _visatype.ViInt32(error_code)  # case S180
         description_ctype = (_visatype.ViChar * buffer_size_ctype.value)()  # case C060
-        error_code = self._library.niSwitch_GetError(vi_ctype, None if code_ctype is None else (ctypes.pointer(code_ctype)), buffer_size_ctype, description_ctype)
+        error_code = self._library.niSwitch_GetError(vi_ctype, None if error_code_ctype is None else (ctypes.pointer(error_code_ctype)), buffer_size_ctype, description_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=True)
-        return int(code_ctype.value), description_ctype.value.decode(self._encoding)
+        return int(error_code_ctype.value), description_ctype.value.decode(self._encoding)
 
     def get_path(self, channel1, channel2):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         channel1_ctype = ctypes.create_string_buffer(channel1.encode(self._encoding))  # case C020
         channel2_ctype = ctypes.create_string_buffer(channel2.encode(self._encoding))  # case C020
         buffer_size_ctype = _visatype.ViInt32()  # case S170
         path_ctype = None  # case C050
@@ -364,14 +384,23 @@
     def set_path(self, path_list):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         path_list_ctype = ctypes.create_string_buffer(path_list.encode(self._encoding))  # case C020
         error_code = self._library.niSwitch_SetPath(vi_ctype, path_list_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
+    def set_runtime_environment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        environment_ctype = ctypes.create_string_buffer(environment.encode(self._encoding))  # case C020
+        environment_version_ctype = ctypes.create_string_buffer(environment_version.encode(self._encoding))  # case C020
+        reserved1_ctype = ctypes.create_string_buffer(reserved1.encode(self._encoding))  # case C020
+        reserved2_ctype = ctypes.create_string_buffer(reserved2.encode(self._encoding))  # case C020
+        error_code = self._library.niSwitch_SetRuntimeEnvironment(environment_ctype, environment_version_ctype, reserved1_ctype, reserved2_ctype)
+        errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
+        return
+
     def unlock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         error_code = self._library.niSwitch_UnlockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def wait_for_debounce(self, maximum_time_ms):  # noqa: N802
```

### Comparing `niswitch-1.4.4/niswitch/_library_singleton.py` & `niswitch-1.4.5/niswitch/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/_visatype.py` & `niswitch-1.4.5/niswitch/_visatype.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/enums.py` & `niswitch-1.4.5/niswitch/enums.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/errors.py` & `niswitch-1.4.5/niswitch/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         super(Error, self).__init__(message)
 
 
 class DriverError(Error):
     '''An error originating from the NI-SWITCH driver'''
 
     def __init__(self, code, description):
-        assert (_is_error(code)), "Should not raise Error if code is not fatal."
+        assert _is_error(code), "Should not raise Error if code is not fatal."
         self.code = code
         self.description = description
         super(DriverError, self).__init__(str(self.code) + ": " + self.description)
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-SWITCH driver'''
 
     def __init__(self, code, description):
-        assert (_is_warning(code)), "Should not create Warning if code is not positive."
+        assert _is_warning(code), "Should not create Warning if code is not positive."
         super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
 
 
 class RpcError(Error):
     '''An error specific to sessions to the NI gRPC Device Server'''
 
     def __init__(self, rpc_code, description):
```

### Comparing `niswitch-1.4.4/niswitch/grpc_session_options.py` & `niswitch-1.4.5/niswitch/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/nidevice_pb2.py` & `niswitch-1.4.5/niswitch/nidevice_pb2.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/niswitch_pb2.py` & `niswitch-1.4.5/niswitch/niswitch_pb2.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/niswitch_pb2_grpc.py` & `niswitch-1.4.5/niswitch/niswitch_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/session.py` & `niswitch-1.4.5/niswitch/session.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/session_pb2.py` & `niswitch-1.4.5/niswitch/session_pb2.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch/session_pb2_grpc.py` & `niswitch-1.4.5/niswitch/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/niswitch.egg-info/PKG-INFO` & `niswitch-1.4.5/niswitch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niswitch
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-SWITCH Python API
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
 
 As a prerequisite to using the niswitch module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niswitch~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install niswitch
+  $ python -m pip install niswitch~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -167,30 +163,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/niswitch/examples>`_
 
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

### Comparing `niswitch-1.4.4/niswitch.egg-info/SOURCES.txt` & `niswitch-1.4.5/niswitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.4/setup.py` & `niswitch-1.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.4',
+    version='1.4.5',
     description='NI-SWITCH Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -43,15 +43,15 @@
     include_package_data=True,
     packages=['niswitch'],
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

