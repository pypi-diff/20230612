# Comparing `tmp/nimodinst-1.4.4.tar.gz` & `tmp/nimodinst-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimodinst-1.4.4.tar", last modified: Fri Apr 14 16:09:39 2023, max compression
+gzip compressed data, was "nimodinst-1.4.5.tar", last modified: Mon Jun 12 00:41:31 2023, max compression
```

## Comparing `nimodinst-1.4.4.tar` & `nimodinst-1.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:49.608416 nimodinst-1.4.4/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8905 2023-04-14 16:09:49.607416 nimodinst-1.4.4/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7930 2023-04-14 16:07:07.000000 nimodinst-1.4.4/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:49.526415 nimodinst-1.4.4/nimodinst/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:07:03.000000 nimodinst-1.4.4/nimodinst/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2932 2023-04-14 16:07:01.000000 nimodinst-1.4.4/nimodinst/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13877 2023-04-14 16:07:02.000000 nimodinst-1.4.4/nimodinst/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4561 2023-04-14 16:06:56.000000 nimodinst-1.4.4/nimodinst/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7235 2023-04-14 16:06:57.000000 nimodinst-1.4.4/nimodinst/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1626 2023-04-14 16:06:57.000000 nimodinst-1.4.4/nimodinst/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:07:03.000000 nimodinst-1.4.4/nimodinst/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3314 2023-04-14 16:06:59.000000 nimodinst-1.4.4/nimodinst/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14066 2023-04-14 16:06:58.000000 nimodinst-1.4.4/nimodinst/session.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:49.594416 nimodinst-1.4.4/nimodinst.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8905 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      428 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:09:49.609417 nimodinst-1.4.4/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1963 2023-04-14 16:07:07.000000 nimodinst-1.4.4/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:35.487564 nimodinst-1.4.5/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8741 2023-06-12 00:41:35.485564 nimodinst-1.4.5/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7675 2023-06-12 00:39:12.000000 nimodinst-1.4.5/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:35.406293 nimodinst-1.4.5/nimodinst/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-06-12 00:39:07.000000 nimodinst-1.4.5/nimodinst/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2932 2023-06-12 00:39:06.000000 nimodinst-1.4.5/nimodinst/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13877 2023-06-12 00:39:06.000000 nimodinst-1.4.5/nimodinst/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4561 2023-06-12 00:39:02.000000 nimodinst-1.4.5/nimodinst/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7235 2023-06-12 00:39:02.000000 nimodinst-1.4.5/nimodinst/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1626 2023-06-12 00:39:03.000000 nimodinst-1.4.5/nimodinst/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-06-12 00:39:07.000000 nimodinst-1.4.5/nimodinst/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3310 2023-06-12 00:39:04.000000 nimodinst-1.4.5/nimodinst/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14066 2023-06-12 00:39:03.000000 nimodinst-1.4.5/nimodinst/session.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:35.472564 nimodinst-1.4.5/nimodinst.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8741 2023-06-12 00:41:35.000000 nimodinst-1.4.5/nimodinst.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      428 2023-06-12 00:41:35.000000 nimodinst-1.4.5/nimodinst.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:41:35.000000 nimodinst-1.4.5/nimodinst.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-06-12 00:41:35.000000 nimodinst-1.4.5/nimodinst.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2023-06-12 00:41:35.000000 nimodinst-1.4.5/nimodinst.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:41:35.000000 nimodinst-1.4.5/nimodinst.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-06-12 00:41:35.487564 nimodinst-1.4.5/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2013 2023-06-12 00:39:12.000000 nimodinst-1.4.5/setup.py
```

### Comparing `nimodinst-1.4.4/PKG-INFO` & `nimodinst-1.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimodinst
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-ModInst Python API
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
 
 As a prerequisite to using the nimodinst module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nimodinst~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nimodinst
+  $ python -m pip install nimodinst~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -167,30 +163,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nimodinst/examples>`_
 
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

### Comparing `nimodinst-1.4.4/README.rst` & `nimodinst-1.4.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -98,32 +98,27 @@
 
 
 .. |nimodinstOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nimodinst.svg
     :alt: Pull Requests for NI-ModInst
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Animodinst
 
 
-
-.. _nimodinst_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nimodinst module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nimodinst~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nimodinst
-
-
+
+.. _nimodinst_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nimodinst module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nimodinst~=1.4.5
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -135,36 +130,34 @@
     import nimodinst
     with nimodinst.Session("niscope") as session:
         for device in session:
             print("{: >20} {: >15} {: >10}".format(device.device_name, device.device_model, device.serial_number))
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nimodinst/examples>`_
 
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

### Comparing `nimodinst-1.4.4/nimodinst/__init__.py` & `nimodinst-1.4.5/nimodinst/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.4'
+__version__ = '1.4.5'
 
 from nimodinst.errors import DriverWarning  # noqa: F401
 from nimodinst.errors import Error  # noqa: F401
 from nimodinst.session import Session  # noqa: F401
 
 
 def get_diagnostic_information():
@@ -59,15 +59,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-ModInst"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nimodinst'
-    info['module']['version'] = "1.4.4"
+    info['module']['version'] = "1.4.5"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nimodinst-1.4.4/nimodinst/_converters.py` & `nimodinst-1.4.5/nimodinst/_converters.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.4/nimodinst/_library.py` & `nimodinst-1.4.5/nimodinst/_library.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.4/nimodinst/_library_interpreter.py` & `nimodinst-1.4.5/nimodinst/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.4/nimodinst/_library_singleton.py` & `nimodinst-1.4.5/nimodinst/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.4/nimodinst/_visatype.py` & `nimodinst-1.4.5/nimodinst/_visatype.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.4/nimodinst/errors.py` & `nimodinst-1.4.5/nimodinst/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         super(Error, self).__init__(message)
 
 
 class DriverError(Error):
     '''An error originating from the NI-ModInst driver'''
 
     def __init__(self, code, description):
-        assert (_is_error(code)), "Should not raise Error if code is not fatal."
+        assert _is_error(code), "Should not raise Error if code is not fatal."
         self.code = code
         self.description = description
         super(DriverError, self).__init__(str(self.code) + ": " + self.description)
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-ModInst driver'''
 
     def __init__(self, code, description):
-        assert (_is_warning(code)), "Should not create Warning if code is not positive."
+        assert _is_warning(code), "Should not create Warning if code is not positive."
         super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
 
 
 class UnsupportedConfigurationError(Error):
     '''An error due to using this module in an usupported platform.'''
 
     def __init__(self):
```

### Comparing `nimodinst-1.4.4/nimodinst/session.py` & `nimodinst-1.4.5/nimodinst/session.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.4/nimodinst.egg-info/PKG-INFO` & `nimodinst-1.4.5/nimodinst.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimodinst
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-ModInst Python API
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
 
 As a prerequisite to using the nimodinst module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nimodinst~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nimodinst
+  $ python -m pip install nimodinst~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -167,30 +163,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nimodinst/examples>`_
 
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

### Comparing `nimodinst-1.4.4/setup.py` & `nimodinst-1.4.5/setup.py`

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
     description='NI-ModInst Python API',
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

