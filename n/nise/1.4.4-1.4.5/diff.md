# Comparing `tmp/nise-1.4.4.tar.gz` & `tmp/nise-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nise-1.4.4.tar", last modified: Fri Apr 14 16:09:23 2023, max compression
+gzip compressed data, was "nise-1.4.5.tar", last modified: Mon Jun 12 00:41:17 2023, max compression
```

## Comparing `nise-1.4.4.tar` & `nise-1.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:34.087863 nise-1.4.4/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8719 2023-04-14 16:09:34.085863 nise-1.4.4/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7745 2023-04-14 16:06:54.000000 nise-1.4.4/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:34.004862 nise-1.4.4/nise/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:06:49.000000 nise-1.4.4/nise/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2976 2023-04-14 16:06:48.000000 nise-1.4.4/nise/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13867 2023-04-14 16:06:49.000000 nise-1.4.4/nise/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8599 2023-04-14 16:06:43.000000 nise-1.4.4/nise/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10784 2023-04-14 16:06:44.000000 nise-1.4.4/nise/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1593 2023-04-14 16:06:44.000000 nise-1.4.4/nise/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:06:49.000000 nise-1.4.4/nise/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1160 2023-04-14 16:06:42.000000 nise-1.4.4/nise/enums.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3729 2023-04-14 16:06:46.000000 nise-1.4.4/nise/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    36136 2023-04-14 16:06:45.000000 nise-1.4.4/nise/session.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:34.072863 nise-1.4.4/nise.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8719 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      367 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        5 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:09:34.088863 nise-1.4.4/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1957 2023-04-14 16:06:54.000000 nise-1.4.4/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:21.752550 nise-1.4.5/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8560 2023-06-12 00:41:21.750550 nise-1.4.5/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7495 2023-06-12 00:38:59.000000 nise-1.4.5/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:21.671548 nise-1.4.5/nise/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-06-12 00:38:53.000000 nise-1.4.5/nise/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2976 2023-06-12 00:38:52.000000 nise-1.4.5/nise/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13867 2023-06-12 00:38:53.000000 nise-1.4.5/nise/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8599 2023-06-12 00:38:48.000000 nise-1.4.5/nise/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10784 2023-06-12 00:38:49.000000 nise-1.4.5/nise/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1593 2023-06-12 00:38:49.000000 nise-1.4.5/nise/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-06-12 00:38:53.000000 nise-1.4.5/nise/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1160 2023-06-12 00:38:47.000000 nise-1.4.5/nise/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3725 2023-06-12 00:38:50.000000 nise-1.4.5/nise/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    36136 2023-06-12 00:38:50.000000 nise-1.4.5/nise/session.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:21.738549 nise-1.4.5/nise.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8560 2023-06-12 00:41:21.000000 nise-1.4.5/nise.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      367 2023-06-12 00:41:21.000000 nise-1.4.5/nise.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:41:21.000000 nise-1.4.5/nise.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-06-12 00:41:21.000000 nise-1.4.5/nise.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        5 2023-06-12 00:41:21.000000 nise-1.4.5/nise.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:41:21.000000 nise-1.4.5/nise.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-06-12 00:41:21.753550 nise-1.4.5/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2007 2023-06-12 00:38:59.000000 nise-1.4.5/setup.py
```

### Comparing `nise-1.4.4/PKG-INFO` & `nise-1.4.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nise
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI Switch Executive Python API
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
 
 Overall Status
 --------------
 
@@ -135,20 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nise module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nise~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nise
+  $ python -m pip install nise~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -166,30 +162,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nise/examples>`_
 
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

### Comparing `nise-1.4.4/README.rst` & `nise-1.4.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -98,32 +98,27 @@
 
 
 .. |niseOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nise.svg
     :alt: Pull Requests for NI Switch Executive
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anise
 
 
-
-.. _nise_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nise module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nise~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nise
-
-
+
+.. _nise_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nise module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nise~=1.4.5
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -134,36 +129,34 @@
 
     import nise
     with nise.Session('SwitchExecutiveExample') as session:
         session.connect('DIOToUUT')
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nise/examples>`_
 
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

### Comparing `nise-1.4.4/nise/__init__.py` & `nise-1.4.5/nise/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.4'
+__version__ = '1.4.5'
 
 from nise.enums import *  # noqa: F403,F401,H303
 from nise.errors import DriverWarning  # noqa: F401
 from nise.errors import Error  # noqa: F401
 from nise.session import Session  # noqa: F401
 
 
@@ -60,15 +60,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI Switch Executive"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nise'
-    info['module']['version'] = "1.4.4"
+    info['module']['version'] = "1.4.5"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nise-1.4.4/nise/_converters.py` & `nise-1.4.5/nise/_converters.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.4/nise/_library.py` & `nise-1.4.5/nise/_library.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.4/nise/_library_interpreter.py` & `nise-1.4.5/nise/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.4/nise/_library_singleton.py` & `nise-1.4.5/nise/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.4/nise/_visatype.py` & `nise-1.4.5/nise/_visatype.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.4/nise/enums.py` & `nise-1.4.5/nise/enums.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.4/nise/errors.py` & `nise-1.4.5/nise/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         super(Error, self).__init__(message)
 
 
 class DriverError(Error):
     '''An error originating from the NI Switch Executive driver'''
 
     def __init__(self, code, description):
-        assert (_is_error(code)), "Should not raise Error if code is not fatal."
+        assert _is_error(code), "Should not raise Error if code is not fatal."
         self.code = code
         self.description = description
         super(DriverError, self).__init__(str(self.code) + ": " + self.description)
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI Switch Executive driver'''
 
     def __init__(self, code, description):
-        assert (_is_warning(code)), "Should not create Warning if code is not positive."
+        assert _is_warning(code), "Should not create Warning if code is not positive."
         super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
 
 
 class UnsupportedConfigurationError(Error):
     '''An error due to using this module in an usupported platform.'''
 
     def __init__(self):
```

### Comparing `nise-1.4.4/nise/session.py` & `nise-1.4.5/nise/session.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.4/nise.egg-info/PKG-INFO` & `nise-1.4.5/nise.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nise
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI Switch Executive Python API
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
 
 Overall Status
 --------------
 
@@ -135,20 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nise module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nise~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nise
+  $ python -m pip install nise~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -166,30 +162,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nise/examples>`_
 
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

### Comparing `nise-1.4.4/setup.py` & `nise-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.4',
+    version='1.4.5',
     description='NI Switch Executive Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
@@ -57,13 +57,14 @@
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

