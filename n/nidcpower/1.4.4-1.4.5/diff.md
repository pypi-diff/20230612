# Comparing `tmp/nidcpower-1.4.4.tar.gz` & `tmp/nidcpower-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nidcpower-1.4.4.tar", last modified: Fri Apr 14 16:07:48 2023, max compression
+gzip compressed data, was "nidcpower-1.4.5.tar", last modified: Mon Jun 12 00:39:53 2023, max compression
```

## Comparing `nidcpower-1.4.4.tar` & `nidcpower-1.4.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:07:58.313598 nidcpower-1.4.4/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10023 2023-04-14 16:07:58.311597 nidcpower-1.4.4/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9027 2023-04-14 16:04:39.000000 nidcpower-1.4.4/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:07:58.126596 nidcpower-1.4.4/nidcpower/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:04:26.000000 nidcpower-1.4.4/nidcpower/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3385 2023-04-14 16:04:25.000000 nidcpower-1.4.4/nidcpower/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5448 2023-04-14 16:04:16.000000 nidcpower-1.4.4/nidcpower/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14605 2023-04-14 16:04:26.000000 nidcpower-1.4.4/nidcpower/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    23998 2023-04-14 16:04:27.000000 nidcpower-1.4.4/nidcpower/_grpc_stub_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    52552 2023-04-14 16:04:18.000000 nidcpower-1.4.4/nidcpower/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    55036 2023-04-14 16:04:19.000000 nidcpower-1.4.4/nidcpower/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1629 2023-04-14 16:04:20.000000 nidcpower-1.4.4/nidcpower/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:04:31.000000 nidcpower-1.4.4/nidcpower/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    18121 2023-04-14 16:04:17.000000 nidcpower-1.4.4/nidcpower/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4392 2023-04-14 16:04:22.000000 nidcpower-1.4.4/nidcpower/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3458 2023-04-14 16:04:28.000000 nidcpower-1.4.4/nidcpower/grpc_session_options.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4270 2023-04-14 16:04:31.000000 nidcpower-1.4.4/nidcpower/lcr_load_compensation_spot.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12190 2023-04-14 16:04:31.000000 nidcpower-1.4.4/nidcpower/lcr_measurement.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   132948 2023-04-14 16:04:29.000000 nidcpower-1.4.4/nidcpower/nidcpower_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   253396 2023-04-14 16:04:29.000000 nidcpower-1.4.4/nidcpower/nidcpower_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-04-14 16:04:30.000000 nidcpower-1.4.4/nidcpower/nidevice_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-04-14 16:04:30.000000 nidcpower-1.4.4/nidcpower/nidevice_pb2_grpc.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)   477377 2023-04-14 16:04:21.000000 nidcpower-1.4.4/nidcpower/session.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-04-14 16:04:31.000000 nidcpower-1.4.4/nidcpower/session_pb2.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-04-14 16:04:31.000000 nidcpower-1.4.4/nidcpower/session_pb2_grpc.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:07:58.297594 nidcpower-1.4.4/nidcpower.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10023 2023-04-14 16:07:57.000000 nidcpower-1.4.4/nidcpower.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      782 2023-04-14 16:07:57.000000 nidcpower-1.4.4/nidcpower.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:07:57.000000 nidcpower-1.4.4/nidcpower.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      154 2023-04-14 16:07:57.000000 nidcpower-1.4.4/nidcpower.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2023-04-14 16:07:57.000000 nidcpower-1.4.4/nidcpower.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:07:57.000000 nidcpower-1.4.4/nidcpower.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:07:58.313598 nidcpower-1.4.4/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2204 2023-04-14 16:04:40.000000 nidcpower-1.4.4/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:39:57.514364 nidcpower-1.4.5/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9859 2023-06-12 00:39:57.512364 nidcpower-1.4.5/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8772 2023-06-12 00:36:42.000000 nidcpower-1.4.5/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:39:57.331622 nidcpower-1.4.5/nidcpower/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-06-12 00:36:29.000000 nidcpower-1.4.5/nidcpower/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3385 2023-06-12 00:36:27.000000 nidcpower-1.4.5/nidcpower/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5448 2023-06-12 00:36:20.000000 nidcpower-1.4.5/nidcpower/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14605 2023-06-12 00:36:28.000000 nidcpower-1.4.5/nidcpower/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    23998 2023-06-12 00:36:30.000000 nidcpower-1.4.5/nidcpower/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    52552 2023-06-12 00:36:21.000000 nidcpower-1.4.5/nidcpower/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    55036 2023-06-12 00:36:22.000000 nidcpower-1.4.5/nidcpower/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1629 2023-06-12 00:36:23.000000 nidcpower-1.4.5/nidcpower/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-06-12 00:36:32.000000 nidcpower-1.4.5/nidcpower/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    18121 2023-06-12 00:36:20.000000 nidcpower-1.4.5/nidcpower/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4388 2023-06-12 00:36:25.000000 nidcpower-1.4.5/nidcpower/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3458 2023-06-12 00:36:30.000000 nidcpower-1.4.5/nidcpower/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4270 2023-06-12 00:36:32.000000 nidcpower-1.4.5/nidcpower/lcr_load_compensation_spot.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12190 2023-06-12 00:36:33.000000 nidcpower-1.4.5/nidcpower/lcr_measurement.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   132948 2023-06-12 00:36:31.000000 nidcpower-1.4.5/nidcpower/nidcpower_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   253396 2023-06-12 00:36:31.000000 nidcpower-1.4.5/nidcpower/nidcpower_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-06-12 00:36:32.000000 nidcpower-1.4.5/nidcpower/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-06-12 00:36:32.000000 nidcpower-1.4.5/nidcpower/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   477377 2023-06-12 00:36:24.000000 nidcpower-1.4.5/nidcpower/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-06-12 00:36:32.000000 nidcpower-1.4.5/nidcpower/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-06-12 00:36:32.000000 nidcpower-1.4.5/nidcpower/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:39:57.499376 nidcpower-1.4.5/nidcpower.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9859 2023-06-12 00:39:57.000000 nidcpower-1.4.5/nidcpower.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      782 2023-06-12 00:39:57.000000 nidcpower-1.4.5/nidcpower.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:39:57.000000 nidcpower-1.4.5/nidcpower.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      148 2023-06-12 00:39:57.000000 nidcpower-1.4.5/nidcpower.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2023-06-12 00:39:57.000000 nidcpower-1.4.5/nidcpower.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:39:57.000000 nidcpower-1.4.5/nidcpower.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-06-12 00:39:57.515364 nidcpower-1.4.5/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2258 2023-06-12 00:36:42.000000 nidcpower-1.4.5/setup.py
```

### Comparing `nidcpower-1.4.4/PKG-INFO` & `nidcpower-1.4.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidcpower
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-DCPower Python API
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
 
 As a prerequisite to using the nidcpower module, you must install the NI-DCPower runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-DCPower**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidcpower~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidcpower
+  $ python -m pip install nidcpower~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -189,30 +185,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidcpower/examples>`_
 
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

### Comparing `nidcpower-1.4.4/README.rst` & `nidcpower-1.4.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -98,32 +98,27 @@
 
 
 .. |nidcpowerOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nidcpower.svg
     :alt: Pull Requests for NI-DCPower
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anidcpower
 
 
-
-.. _nidcpower_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nidcpower module, you must install the NI-DCPower runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-DCPower**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nidcpower~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidcpower
-
-
+
+.. _nidcpower_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nidcpower module, you must install the NI-DCPower runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-DCPower**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nidcpower~=1.4.5
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -156,36 +151,34 @@
                     measurements = session.channels[channel_name].fetch_multiple(count=session.fetch_backlog)
                     samples_acquired += len(measurements)
                     for i in range(len(measurements)):
                         print(row_format.format(channel_name, i, measurements[i].voltage, measurements[i].current, measurements[i].in_compliance))
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidcpower/examples>`_
 
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

### Comparing `nidcpower-1.4.4/nidcpower/__init__.py` & `nidcpower-1.4.5/nidcpower/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.4'
+__version__ = '1.4.5'
 
 from nidcpower.enums import *  # noqa: F403,F401,H303
 from nidcpower.errors import DriverWarning  # noqa: F401
 from nidcpower.errors import Error  # noqa: F401
 from nidcpower.grpc_session_options import *  # noqa: F403,F401,H303
 from nidcpower.session import Session  # noqa: F401
 
@@ -69,15 +69,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-DCPower"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nidcpower'
-    info['module']['version'] = "1.4.4"
+    info['module']['version'] = "1.4.5"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nidcpower-1.4.4/nidcpower/_attributes.py` & `nidcpower-1.4.5/nidcpower/_attributes.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/_converters.py` & `nidcpower-1.4.5/nidcpower/_converters.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/_grpc_stub_interpreter.py` & `nidcpower-1.4.5/nidcpower/_grpc_stub_interpreter.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/_library.py` & `nidcpower-1.4.5/nidcpower/_library.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/_library_interpreter.py` & `nidcpower-1.4.5/nidcpower/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/_library_singleton.py` & `nidcpower-1.4.5/nidcpower/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/_visatype.py` & `nidcpower-1.4.5/nidcpower/_visatype.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/enums.py` & `nidcpower-1.4.5/nidcpower/enums.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/errors.py` & `nidcpower-1.4.5/nidcpower/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         super(Error, self).__init__(message)
 
 
 class DriverError(Error):
     '''An error originating from the NI-DCPower driver'''
 
     def __init__(self, code, description):
-        assert (_is_error(code)), "Should not raise Error if code is not fatal."
+        assert _is_error(code), "Should not raise Error if code is not fatal."
         self.code = code
         self.description = description
         super(DriverError, self).__init__(str(self.code) + ": " + self.description)
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-DCPower driver'''
 
     def __init__(self, code, description):
-        assert (_is_warning(code)), "Should not create Warning if code is not positive."
+        assert _is_warning(code), "Should not create Warning if code is not positive."
         super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
 
 
 class RpcError(Error):
     '''An error specific to sessions to the NI gRPC Device Server'''
 
     def __init__(self, rpc_code, description):
```

### Comparing `nidcpower-1.4.4/nidcpower/grpc_session_options.py` & `nidcpower-1.4.5/nidcpower/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/lcr_load_compensation_spot.py` & `nidcpower-1.4.5/nidcpower/lcr_load_compensation_spot.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/lcr_measurement.py` & `nidcpower-1.4.5/nidcpower/lcr_measurement.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/nidcpower_pb2.py` & `nidcpower-1.4.5/nidcpower/nidcpower_pb2.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/nidcpower_pb2_grpc.py` & `nidcpower-1.4.5/nidcpower/nidcpower_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/nidevice_pb2.py` & `nidcpower-1.4.5/nidcpower/nidevice_pb2.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/session.py` & `nidcpower-1.4.5/nidcpower/session.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/session_pb2.py` & `nidcpower-1.4.5/nidcpower/session_pb2.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower/session_pb2_grpc.py` & `nidcpower-1.4.5/nidcpower/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/nidcpower.egg-info/PKG-INFO` & `nidcpower-1.4.5/nidcpower.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidcpower
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-DCPower Python API
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
 
 As a prerequisite to using the nidcpower module, you must install the NI-DCPower runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-DCPower**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidcpower~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidcpower
+  $ python -m pip install nidcpower~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -189,30 +185,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidcpower/examples>`_
 
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

### Comparing `nidcpower-1.4.4/nidcpower.egg-info/SOURCES.txt` & `nidcpower-1.4.5/nidcpower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nidcpower-1.4.4/setup.py` & `nidcpower-1.4.5/setup.py`

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
     description='NI-DCPower Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -43,15 +43,15 @@
     include_package_data=True,
     packages=['nidcpower'],
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

