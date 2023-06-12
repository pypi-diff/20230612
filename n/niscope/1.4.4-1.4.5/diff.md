# Comparing `tmp/niscope-1.4.4.tar.gz` & `tmp/niscope-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niscope-1.4.4.tar", last modified: Fri Apr 14 16:08:51 2023, max compression
+gzip compressed data, was "niscope-1.4.5.tar", last modified: Mon Jun 12 00:40:49 2023, max compression
```

## Comparing `niscope-1.4.4.tar` & `niscope-1.4.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:01.823798 niscope-1.4.4/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13472 2023-04-14 16:09:01.821798 niscope-1.4.4/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12482 2023-04-14 16:06:18.000000 niscope-1.4.4/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:01.638795 niscope-1.4.4/niscope/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:06:05.000000 niscope-1.4.4/niscope/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3243 2023-04-14 16:06:04.000000 niscope-1.4.4/niscope/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5440 2023-04-14 16:05:55.000000 niscope-1.4.4/niscope/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13873 2023-04-14 16:06:04.000000 niscope-1.4.4/niscope/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    20465 2023-04-14 16:06:06.000000 niscope-1.4.4/niscope/_grpc_stub_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    42049 2023-04-14 16:05:57.000000 niscope-1.4.4/niscope/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    46264 2023-04-14 16:05:58.000000 niscope-1.4.4/niscope/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1617 2023-04-14 16:05:59.000000 niscope-1.4.4/niscope/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:06:10.000000 niscope-1.4.4/niscope/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    18294 2023-04-14 16:05:56.000000 niscope-1.4.4/niscope/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4370 2023-04-14 16:06:01.000000 niscope-1.4.4/niscope/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3454 2023-04-14 16:06:07.000000 niscope-1.4.4/niscope/grpc_session_options.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1748 2023-04-14 16:06:10.000000 niscope-1.4.4/niscope/measurement_stats.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-04-14 16:06:09.000000 niscope-1.4.4/niscope/nidevice_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-04-14 16:06:09.000000 niscope-1.4.4/niscope/nidevice_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   111818 2023-04-14 16:06:08.000000 niscope-1.4.4/niscope/niscope_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   148144 2023-04-14 16:06:08.000000 niscope-1.4.4/niscope/niscope_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   252245 2023-04-14 16:06:00.000000 niscope-1.4.4/niscope/session.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-04-14 16:06:10.000000 niscope-1.4.4/niscope/session_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-04-14 16:06:10.000000 niscope-1.4.4/niscope/session_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6425 2023-04-14 16:06:10.000000 niscope-1.4.4/niscope/waveform_info.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:01.806794 niscope-1.4.4/niscope.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13472 2023-04-14 16:09:01.000000 niscope-1.4.4/niscope.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      713 2023-04-14 16:09:01.000000 niscope-1.4.4/niscope.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:01.000000 niscope-1.4.4/niscope.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      161 2023-04-14 16:09:01.000000 niscope-1.4.4/niscope.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        8 2023-04-14 16:09:01.000000 niscope-1.4.4/niscope.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:01.000000 niscope-1.4.4/niscope.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:09:01.824797 niscope-1.4.4/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2214 2023-04-14 16:06:19.000000 niscope-1.4.4/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:40:54.090171 niscope-1.4.5/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13310 2023-06-12 00:40:54.088936 niscope-1.4.5/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12229 2023-06-12 00:38:22.000000 niscope-1.4.5/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:40:53.906710 niscope-1.4.5/niscope/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-06-12 00:38:09.000000 niscope-1.4.5/niscope/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3243 2023-06-12 00:38:08.000000 niscope-1.4.5/niscope/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5440 2023-06-12 00:38:00.000000 niscope-1.4.5/niscope/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13873 2023-06-12 00:38:08.000000 niscope-1.4.5/niscope/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    20927 2023-06-12 00:38:10.000000 niscope-1.4.5/niscope/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    43533 2023-06-12 00:38:02.000000 niscope-1.4.5/niscope/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    48611 2023-06-12 00:38:03.000000 niscope-1.4.5/niscope/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1617 2023-06-12 00:38:04.000000 niscope-1.4.5/niscope/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-06-12 00:38:13.000000 niscope-1.4.5/niscope/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    18294 2023-06-12 00:38:01.000000 niscope-1.4.5/niscope/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4366 2023-06-12 00:38:05.000000 niscope-1.4.5/niscope/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3454 2023-06-12 00:38:11.000000 niscope-1.4.5/niscope/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1748 2023-06-12 00:38:13.000000 niscope-1.4.5/niscope/measurement_stats.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-06-12 00:38:12.000000 niscope-1.4.5/niscope/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-06-12 00:38:12.000000 niscope-1.4.5/niscope/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   111818 2023-06-12 00:38:12.000000 niscope-1.4.5/niscope/niscope_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   148144 2023-06-12 00:38:12.000000 niscope-1.4.5/niscope/niscope_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   254446 2023-06-12 00:38:05.000000 niscope-1.4.5/niscope/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-06-12 00:38:13.000000 niscope-1.4.5/niscope/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-06-12 00:38:13.000000 niscope-1.4.5/niscope/session_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     6425 2023-06-12 00:38:13.000000 niscope-1.4.5/niscope/waveform_info.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:40:54.074931 niscope-1.4.5/niscope.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13310 2023-06-12 00:40:53.000000 niscope-1.4.5/niscope.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      713 2023-06-12 00:40:53.000000 niscope-1.4.5/niscope.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:40:53.000000 niscope-1.4.5/niscope.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      155 2023-06-12 00:40:53.000000 niscope-1.4.5/niscope.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        8 2023-06-12 00:40:53.000000 niscope-1.4.5/niscope.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:40:53.000000 niscope-1.4.5/niscope.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-06-12 00:40:54.091182 niscope-1.4.5/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2268 2023-06-12 00:38:23.000000 niscope-1.4.5/setup.py
```

### Comparing `niscope-1.4.4/PKG-INFO` & `niscope-1.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niscope
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-SCOPE Python API
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
 
 As a prerequisite to using the niscope module, you must install the NI-SCOPE runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SCOPE**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niscope~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install niscope
+  $ python -m pip install niscope~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -257,30 +253,28 @@
 
 
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

### Comparing `niscope-1.4.4/README.rst` & `niscope-1.4.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -98,32 +98,27 @@
 
 
 .. |niscopeOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/niscope.svg
     :alt: Pull Requests for NI-SCOPE
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Aniscope
 
 
-
-.. _niscope_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the niscope module, you must install the NI-SCOPE runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-SCOPE**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install niscope~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install niscope
-
-
+
+.. _niscope_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the niscope module, you must install the NI-SCOPE runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-SCOPE**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install niscope~=1.4.5
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -224,36 +219,34 @@
         - index 3 = record 1, channel 1
         - etc.
 
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/niscope/examples>`_
 
 
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

### Comparing `niscope-1.4.4/niscope/__init__.py` & `niscope-1.4.5/niscope/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.4'
+__version__ = '1.4.5'
 
 from niscope.enums import *  # noqa: F403,F401,H303
 from niscope.errors import DriverWarning  # noqa: F401
 from niscope.errors import Error  # noqa: F401
 from niscope.grpc_session_options import *  # noqa: F403,F401,H303
 from niscope.session import Session  # noqa: F401
 
@@ -67,15 +67,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-SCOPE"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'niscope'
-    info['module']['version'] = "1.4.4"
+    info['module']['version'] = "1.4.5"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `niscope-1.4.4/niscope/_attributes.py` & `niscope-1.4.5/niscope/_attributes.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/_converters.py` & `niscope-1.4.5/niscope/_converters.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/_grpc_stub_interpreter.py` & `niscope-1.4.5/niscope/_grpc_stub_interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,21 @@
     def get_attribute_vi_string(self, channel_list, attribute_id):  # noqa: N802
         response = self._invoke(
             self._client.GetAttributeViString,
             grpc_types.GetAttributeViStringRequest(vi=self._vi, channel_list=channel_list, attribute_id=attribute_id),
         )
         return response.value
 
+    def get_channel_names(self, indices):  # noqa: N802
+        response = self._invoke(
+            self._client.GetChannelNameFromString,
+            grpc_types.GetChannelNameFromStringRequest(vi=self._vi, index=indices),
+        )
+        return response.name
+
     def get_equalization_filter_coefficients(self, channel, number_of_coefficients):  # noqa: N802
         response = self._invoke(
             self._client.GetEqualizationFilterCoefficients,
             grpc_types.GetEqualizationFilterCoefficientsRequest(vi=self._vi, channel=channel, number_of_coefficients=number_of_coefficients),
         )
         return response.coefficients
 
@@ -414,14 +421,17 @@
 
     def set_attribute_vi_string(self, channel_list, attribute_id, value):  # noqa: N802
         self._invoke(
             self._client.SetAttributeViString,
             grpc_types.SetAttributeViStringRequest(vi=self._vi, channel_list=channel_list, attribute_id=attribute_id, value_raw=value),
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

### Comparing `niscope-1.4.4/niscope/_library.py` & `niscope-1.4.5/niscope/_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         self.niScope_FetchBinary8_cfunc = None
         self.niScope_FetchMeasurementStats_cfunc = None
         self.niScope_GetAttributeViBoolean_cfunc = None
         self.niScope_GetAttributeViInt32_cfunc = None
         self.niScope_GetAttributeViInt64_cfunc = None
         self.niScope_GetAttributeViReal64_cfunc = None
         self.niScope_GetAttributeViString_cfunc = None
+        self.niScope_GetChannelNameFromString_cfunc = None
         self.niScope_GetEqualizationFilterCoefficients_cfunc = None
         self.niScope_GetError_cfunc = None
         self.niScope_ImportAttributeConfigurationBuffer_cfunc = None
         self.niScope_ImportAttributeConfigurationFile_cfunc = None
         self.niScope_InitWithOptions_cfunc = None
         self.niScope_InitiateAcquisition_cfunc = None
         self.niScope_LockSession_cfunc = None
@@ -75,14 +76,15 @@
         self.niScope_ResetWithDefaults_cfunc = None
         self.niScope_SendSoftwareTriggerEdge_cfunc = None
         self.niScope_SetAttributeViBoolean_cfunc = None
         self.niScope_SetAttributeViInt32_cfunc = None
         self.niScope_SetAttributeViInt64_cfunc = None
         self.niScope_SetAttributeViReal64_cfunc = None
         self.niScope_SetAttributeViString_cfunc = None
+        self.niScope_SetRuntimeEnvironment_cfunc = None
         self.niScope_UnlockSession_cfunc = None
         self.niScope_close_cfunc = None
         self.niScope_error_message_cfunc = None
         self.niScope_reset_cfunc = None
         self.niScope_self_test_cfunc = None
 
     def _get_library_function(self, name):
@@ -392,14 +394,22 @@
         with self._func_lock:
             if self.niScope_GetAttributeViString_cfunc is None:
                 self.niScope_GetAttributeViString_cfunc = self._get_library_function('niScope_GetAttributeViString')
                 self.niScope_GetAttributeViString_cfunc.argtypes = [ViSession, ctypes.POINTER(ViChar), ViAttr, ViInt32, ctypes.POINTER(ViChar)]  # noqa: F405
                 self.niScope_GetAttributeViString_cfunc.restype = ViStatus  # noqa: F405
         return self.niScope_GetAttributeViString_cfunc(vi, channel_list, attribute_id, buf_size, value)
 
+    def niScope_GetChannelNameFromString(self, vi, indices, buffer_size, names):  # noqa: N802
+        with self._func_lock:
+            if self.niScope_GetChannelNameFromString_cfunc is None:
+                self.niScope_GetChannelNameFromString_cfunc = self._get_library_function('niScope_GetChannelNameFromString')
+                self.niScope_GetChannelNameFromString_cfunc.argtypes = [ViSession, ctypes.POINTER(ViChar), ViInt32, ctypes.POINTER(ViChar)]  # noqa: F405
+                self.niScope_GetChannelNameFromString_cfunc.restype = ViStatus  # noqa: F405
+        return self.niScope_GetChannelNameFromString_cfunc(vi, indices, buffer_size, names)
+
     def niScope_GetEqualizationFilterCoefficients(self, vi, channel, number_of_coefficients, coefficients):  # noqa: N802
         with self._func_lock:
             if self.niScope_GetEqualizationFilterCoefficients_cfunc is None:
                 self.niScope_GetEqualizationFilterCoefficients_cfunc = self._get_library_function('niScope_GetEqualizationFilterCoefficients')
                 self.niScope_GetEqualizationFilterCoefficients_cfunc.argtypes = [ViSession, ctypes.POINTER(ViChar), ViInt32, ctypes.POINTER(ViReal64)]  # noqa: F405
                 self.niScope_GetEqualizationFilterCoefficients_cfunc.restype = ViStatus  # noqa: F405
         return self.niScope_GetEqualizationFilterCoefficients_cfunc(vi, channel, number_of_coefficients, coefficients)
@@ -536,14 +546,22 @@
         with self._func_lock:
             if self.niScope_SetAttributeViString_cfunc is None:
                 self.niScope_SetAttributeViString_cfunc = self._get_library_function('niScope_SetAttributeViString')
                 self.niScope_SetAttributeViString_cfunc.argtypes = [ViSession, ctypes.POINTER(ViChar), ViAttr, ctypes.POINTER(ViChar)]  # noqa: F405
                 self.niScope_SetAttributeViString_cfunc.restype = ViStatus  # noqa: F405
         return self.niScope_SetAttributeViString_cfunc(vi, channel_list, attribute_id, value)
 
+    def niScope_SetRuntimeEnvironment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        with self._func_lock:
+            if self.niScope_SetRuntimeEnvironment_cfunc is None:
+                self.niScope_SetRuntimeEnvironment_cfunc = self._get_library_function('niScope_SetRuntimeEnvironment')
+                self.niScope_SetRuntimeEnvironment_cfunc.argtypes = [ctypes.POINTER(ViChar), ctypes.POINTER(ViChar), ctypes.POINTER(ViChar), ctypes.POINTER(ViChar)]  # noqa: F405
+                self.niScope_SetRuntimeEnvironment_cfunc.restype = ViStatus  # noqa: F405
+        return self.niScope_SetRuntimeEnvironment_cfunc(environment, environment_version, reserved1, reserved2)
+
     def niScope_UnlockSession(self, vi, caller_has_lock):  # noqa: N802
         with self._func_lock:
             if self.niScope_UnlockSession_cfunc is None:
                 self.niScope_UnlockSession_cfunc = self._get_library_function('niScope_UnlockSession')
                 self.niScope_UnlockSession_cfunc.argtypes = [ViSession, ctypes.POINTER(ViBoolean)]  # noqa: F405
                 self.niScope_UnlockSession_cfunc.restype = ViStatus  # noqa: F405
         return self.niScope_UnlockSession_cfunc(vi, caller_has_lock)
```

### Comparing `niscope-1.4.4/niscope/_library_interpreter.py` & `niscope-1.4.5/niscope/_library_interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 import array
 import ctypes
 import hightime  # noqa: F401
+import platform
+
 import niscope._library_singleton as _library_singleton
 import niscope._visatype as _visatype
 import niscope.enums as enums  # noqa: F401
 import niscope.errors as errors
 
 import niscope.waveform_info as waveform_info  # noqa: F401
 
 import niscope.measurement_stats as measurement_stats  # noqa: F401
 
 
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
@@ -56,14 +61,29 @@
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
@@ -482,14 +502,27 @@
         errors.handle_error(self, error_code, ignore_warnings=True, is_error_handling=False)
         buf_size_ctype = _visatype.ViInt32(error_code)  # case S180
         value_ctype = (_visatype.ViChar * buf_size_ctype.value)()  # case C060
         error_code = self._library.niScope_GetAttributeViString(vi_ctype, channel_list_ctype, attribute_id_ctype, buf_size_ctype, value_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return value_ctype.value.decode(self._encoding)
 
+    def get_channel_names(self, indices):  # noqa: N802
+        vi_ctype = _visatype.ViSession(self._vi)  # case S110
+        indices_ctype = ctypes.create_string_buffer(indices.encode(self._encoding))  # case C020
+        buffer_size_ctype = _visatype.ViInt32()  # case S170
+        names_ctype = None  # case C050
+        error_code = self._library.niScope_GetChannelNameFromString(vi_ctype, indices_ctype, buffer_size_ctype, names_ctype)
+        errors.handle_error(self, error_code, ignore_warnings=True, is_error_handling=False)
+        buffer_size_ctype = _visatype.ViInt32(error_code)  # case S180
+        names_ctype = (_visatype.ViChar * buffer_size_ctype.value)()  # case C060
+        error_code = self._library.niScope_GetChannelNameFromString(vi_ctype, indices_ctype, buffer_size_ctype, names_ctype)
+        errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
+        return names_ctype.value.decode(self._encoding)
+
     def get_equalization_filter_coefficients(self, channel, number_of_coefficients):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         channel_ctype = ctypes.create_string_buffer(channel.encode(self._encoding))  # case C010
         number_of_coefficients_ctype = _visatype.ViInt32(number_of_coefficients)  # case S210
         coefficients_size = number_of_coefficients  # case B600
         coefficients_ctype = _get_ctypes_pointer_for_buffer(library_type=_visatype.ViReal64, size=coefficients_size)  # case B600
         error_code = self._library.niScope_GetEqualizationFilterCoefficients(vi_ctype, channel_ctype, number_of_coefficients_ctype, coefficients_ctype)
@@ -633,14 +666,23 @@
         channel_list_ctype = ctypes.create_string_buffer(channel_list.encode(self._encoding))  # case C010
         attribute_id_ctype = _visatype.ViAttr(attribute_id)  # case S150
         value_ctype = ctypes.create_string_buffer(value.encode(self._encoding))  # case C020
         error_code = self._library.niScope_SetAttributeViString(vi_ctype, channel_list_ctype, attribute_id_ctype, value_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
+    def set_runtime_environment(self, environment, environment_version, reserved1, reserved2):  # noqa: N802
+        environment_ctype = ctypes.create_string_buffer(environment.encode(self._encoding))  # case C020
+        environment_version_ctype = ctypes.create_string_buffer(environment_version.encode(self._encoding))  # case C020
+        reserved1_ctype = ctypes.create_string_buffer(reserved1.encode(self._encoding))  # case C020
+        reserved2_ctype = ctypes.create_string_buffer(reserved2.encode(self._encoding))  # case C020
+        error_code = self._library.niScope_SetRuntimeEnvironment(environment_ctype, environment_version_ctype, reserved1_ctype, reserved2_ctype)
+        errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
+        return
+
     def unlock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         error_code = self._library.niScope_UnlockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def close(self):  # noqa: N802
```

### Comparing `niscope-1.4.4/niscope/_library_singleton.py` & `niscope-1.4.5/niscope/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/_visatype.py` & `niscope-1.4.5/niscope/_visatype.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/enums.py` & `niscope-1.4.5/niscope/enums.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/errors.py` & `niscope-1.4.5/niscope/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         super(Error, self).__init__(message)
 
 
 class DriverError(Error):
     '''An error originating from the NI-SCOPE driver'''
 
     def __init__(self, code, description):
-        assert (_is_error(code)), "Should not raise Error if code is not fatal."
+        assert _is_error(code), "Should not raise Error if code is not fatal."
         self.code = code
         self.description = description
         super(DriverError, self).__init__(str(self.code) + ": " + self.description)
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-SCOPE driver'''
 
     def __init__(self, code, description):
-        assert (_is_warning(code)), "Should not create Warning if code is not positive."
+        assert _is_warning(code), "Should not create Warning if code is not positive."
         super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
 
 
 class RpcError(Error):
     '''An error specific to sessions to the NI gRPC Device Server'''
 
     def __init__(self, rpc_code, description):
```

### Comparing `niscope-1.4.4/niscope/grpc_session_options.py` & `niscope-1.4.5/niscope/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/measurement_stats.py` & `niscope-1.4.5/niscope/measurement_stats.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/nidevice_pb2.py` & `niscope-1.4.5/niscope/nidevice_pb2.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/niscope_pb2.py` & `niscope-1.4.5/niscope/niscope_pb2.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/niscope_pb2_grpc.py` & `niscope-1.4.5/niscope/niscope_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/session.py` & `niscope-1.4.5/niscope/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -2128,20 +2128,25 @@
         if isinstance(wfm, array.ArrayType):
             mv = memoryview(wfm)
         else:
             mv = wfm
 
         waveform_info._populate_samples_info(wfm_info, mv, num_samples)
 
-        lwfm_i = len(wfm_info)
-        lrcl = len(self._repeated_capability_list)
+        channel_names = _converters.expand_channel_string(
+            self._repeated_capability,
+            self._all_channels_in_session
+        )
+
+        wfm_info_count = len(wfm_info)
+        channel_count = len(channel_names)
         # Should this raise instead? If this asserts, is it the users fault?
-        assert lwfm_i % lrcl == 0, 'Number of waveforms should be evenly divisible by the number of channels: len(wfm_info) == {0}, len(self._repeated_capability_list) == {1}'.format(lwfm_i, lrcl)
-        actual_num_records = int(lwfm_i / lrcl)
-        waveform_info._populate_channel_and_record_info(wfm_info, self._repeated_capability_list, range(record_number, record_number + actual_num_records))
+        assert wfm_info_count % channel_count == 0, 'Number of waveforms should be evenly divisible by the number of channels: len(wfm_info) == {0}, len(channel_names) == {1}'.format(wfm_info_count, channel_count)
+        actual_num_records = int(wfm_info_count / channel_count)
+        waveform_info._populate_channel_and_record_info(wfm_info, channel_names, range(record_number, record_number + actual_num_records))
 
         return wfm_info
 
     @ivi_synchronized
     def fetch_array_measurement(self, array_meas_function, meas_wfm_size=None, relative_to=enums.FetchRelativeTo.PRETRIGGER, offset=0, record_number=0, num_records=None, meas_num_samples=None, timeout=hightime.timedelta(seconds=5.0)):
         r'''fetch_array_measurement
 
@@ -2227,19 +2232,25 @@
                 meas_wfm_size = self._actual_meas_wfm_size(array_meas_function)
 
         meas_wfm, wfm_info = self._fetch_array_measurement(array_meas_function, meas_wfm_size, timeout)
 
         record_length = int(len(meas_wfm) / len(wfm_info))
         waveform_info._populate_samples_info(wfm_info, meas_wfm, record_length)
 
+        channel_names = _converters.expand_channel_string(
+            self._repeated_capability,
+            self._all_channels_in_session
+        )
+
         wfm_info_count = len(wfm_info)
-        channel_count = len(self._repeated_capability_list)
-        assert wfm_info_count % channel_count == 0, 'Number of waveforms should be evenly divisible by the number of channels: len(wfm_info) == {0}, len(self._repeated_capability_list) == {1}'.format(wfm_info_count, channel_count)
+        channel_count = len(channel_names)
+        # Should this raise instead? If this asserts, is it the users fault?
+        assert wfm_info_count % channel_count == 0, 'Number of waveforms should be evenly divisible by the number of channels: len(wfm_info) == {0}, len(channel_names) == {1}'.format(wfm_info_count, channel_count)
         actual_num_records = int(wfm_info_count / channel_count)
-        waveform_info._populate_channel_and_record_info(wfm_info, self._repeated_capability_list, range(record_number, record_number + actual_num_records))
+        waveform_info._populate_channel_and_record_info(wfm_info, channel_names, range(record_number, record_number + actual_num_records))
 
         return wfm_info
 
     @ivi_synchronized
     def fetch_measurement_stats(self, scalar_meas_function, relative_to=enums.FetchRelativeTo.PRETRIGGER, offset=0, record_number=0, num_records=None, timeout=hightime.timedelta(seconds=5.0)):
         r'''fetch_measurement_stats
 
@@ -2321,19 +2332,25 @@
         results, means, stdevs, min_vals, max_vals, nums_in_stats = self._fetch_measurement_stats(scalar_meas_function, timeout)
 
         output = []
         for result, mean, stdev, min_val, max_val, num_in_stats in zip(results, means, stdevs, min_vals, max_vals, nums_in_stats):
             measurement_stat = measurement_stats.MeasurementStats(result, mean, stdev, min_val, max_val, num_in_stats)
             output.append(measurement_stat)
 
+        channel_names = _converters.expand_channel_string(
+            self._repeated_capability,
+            self._all_channels_in_session
+        )
+
         results_count = len(results)
-        channel_count = len(self._repeated_capability_list)
-        assert results_count % channel_count == 0, 'Number of results should be evenly divisible by the number of channels: len(results) == {0}, len(self._repeated_capability_list) == {1}'.format(results_count, channel_count)
+        channel_count = len(channel_names)
+        # Should this raise instead? If this asserts, is it the users fault?
+        assert results_count % channel_count == 0, 'Number of results should be evenly divisible by the number of channels: len(results) == {0}, len(channel_names) == {1}'.format(results_count, channel_count)
         actual_num_records = int(results_count / channel_count)
-        waveform_info._populate_channel_and_record_info(output, self._repeated_capability_list, range(record_number, record_number + actual_num_records))
+        waveform_info._populate_channel_and_record_info(output, channel_names, range(record_number, record_number + actual_num_records))
 
         return output
 
     @ivi_synchronized
     def get_equalization_filter_coefficients(self):
         '''get_equalization_filter_coefficients
 
@@ -2430,20 +2447,25 @@
         if isinstance(wfm, array.ArrayType):
             mv = memoryview(wfm)
         else:
             mv = wfm
 
         waveform_info._populate_samples_info(wfm_info, mv, num_samples)
 
-        lwfm_i = len(wfm_info)
-        lrcl = len(self._repeated_capability_list)
+        channel_names = _converters.expand_channel_string(
+            self._repeated_capability,
+            self._all_channels_in_session
+        )
+
+        wfm_info_count = len(wfm_info)
+        channel_count = len(channel_names)
         # Should this raise instead? If this asserts, is it the users fault?
-        assert lwfm_i % lrcl == 0, 'Number of waveforms should be evenly divisible by the number of channels: len(wfm_info) == {0}, len(self._repeated_capability_list) == {1}'.format(lwfm_i, lrcl)
-        actual_num_records = int(lwfm_i / lrcl)
-        waveform_info._populate_channel_and_record_info(wfm_info, self._repeated_capability_list, range(record_number, record_number + actual_num_records))
+        assert wfm_info_count % channel_count == 0, 'Number of waveforms should be evenly divisible by the number of channels: len(wfm_info) == {0}, len(channel_names) == {1}'.format(wfm_info_count, channel_count)
+        actual_num_records = int(wfm_info_count / channel_count)
+        waveform_info._populate_channel_and_record_info(wfm_info, channel_names, range(record_number, record_number + actual_num_records))
 
         return wfm_info
 
     @ivi_synchronized
     def _fetch(self, num_samples, timeout=hightime.timedelta(seconds=5.0)):
         r'''_fetch
 
@@ -3143,19 +3165,25 @@
         else:
             raise TypeError("Unsupported dtype. Is {0}, expected {1}, {2}, {3}, or {4}".format(waveform.dtype, numpy.float64, numpy.int8, numpy.int16, numpy.int32))
 
         mv = memoryview(waveform)
 
         waveform_info._populate_samples_info(wfm_info, mv, num_samples)
 
-        lwfm_i = len(wfm_info)
-        lrcl = len(self._repeated_capability_list)
-        assert lwfm_i % lrcl == 0, 'Number of waveforms should be evenly divisible by the number of channels: len(wfm_info) == {0}, len(self._repeated_capability_list) == {1}'.format(lwfm_i, lrcl)
-        actual_num_records = int(lwfm_i / lrcl)
-        waveform_info._populate_channel_and_record_info(wfm_info, self._repeated_capability_list, range(record_number, record_number + actual_num_records))
+        channel_names = _converters.expand_channel_string(
+            self._repeated_capability,
+            self._all_channels_in_session
+        )
+
+        wfm_info_count = len(wfm_info)
+        channel_count = len(channel_names)
+        # Should this raise instead? If this asserts, is it the users fault?
+        assert wfm_info_count % channel_count == 0, 'Number of waveforms should be evenly divisible by the number of channels: len(wfm_info) == {0}, len(channel_names) == {1}'.format(wfm_info_count, channel_count)
+        actual_num_records = int(wfm_info_count / channel_count)
+        waveform_info._populate_channel_and_record_info(wfm_info, channel_names, range(record_number, record_number + actual_num_records))
 
         return wfm_info
 
     @ivi_synchronized
     def _fetch_measurement_stats(self, scalar_meas_function, timeout=hightime.timedelta(seconds=5.0)):
         r'''_fetch_measurement_stats
 
@@ -4819,14 +4847,38 @@
             temperature (float): Returns the **temperature** in degrees Celsius during the last calibration.
 
         '''
 
         return self._cal_fetch_temperature(enums._CalibrationTypes.SELF.value)
 
     @ivi_synchronized
+    def get_channel_names(self, indices):
+        r'''get_channel_names
+
+        Returns a list of channel names for given channel indices.
+
+        Args:
+            indices (basic sequence types, str, or int): Index list for the channels in the session. Valid values are from zero to the total number of channels in the session minus one. The index string can be one of the following formats:
+
+                -   A comma-separated list—for example, "0,2,3,1"
+                -   A range using a hyphen—for example, "0-3"
+                -   A range using a colon—for example, "0:3 "
+
+                You can combine comma-separated lists and ranges that use a hyphen or colon. Both out-of-order and repeated indices are supported ("2,3,0", "1,2,2,3"). White space characters, including spaces, tabs, feeds, and carriage returns, are allowed between characters. Ranges can be incrementing or decrementing.
+
+
+        Returns:
+            names (list of str): The channel name(s) at the specified indices.
+
+        '''
+        indices = _converters.convert_repeated_capabilities_without_prefix(indices)
+        names = self._interpreter.get_channel_names(indices)
+        return _converters.convert_comma_separated_string_to_list(names)
+
+    @ivi_synchronized
     def import_attribute_configuration_buffer(self, configuration):
         r'''import_attribute_configuration_buffer
 
         Imports a property configuration to the session from the specified
         configuration buffer.
 
         You can export and import session property configurations only between
```

### Comparing `niscope-1.4.4/niscope/session_pb2.py` & `niscope-1.4.5/niscope/session_pb2.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/session_pb2_grpc.py` & `niscope-1.4.5/niscope/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope/waveform_info.py` & `niscope-1.4.5/niscope/waveform_info.py`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/niscope.egg-info/PKG-INFO` & `niscope-1.4.5/niscope.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niscope
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-SCOPE Python API
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
 
 As a prerequisite to using the niscope module, you must install the NI-SCOPE runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SCOPE**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niscope~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install niscope
+  $ python -m pip install niscope~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -257,30 +253,28 @@
 
 
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

### Comparing `niscope-1.4.4/niscope.egg-info/SOURCES.txt` & `niscope-1.4.5/niscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niscope-1.4.4/setup.py` & `niscope-1.4.5/setup.py`

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
     description='NI-SCOPE Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -44,15 +44,15 @@
     packages=['niscope'],
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

