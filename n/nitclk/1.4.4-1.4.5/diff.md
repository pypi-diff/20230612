# Comparing `tmp/nitclk-1.4.4.tar.gz` & `tmp/nitclk-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitclk-1.4.4.tar", last modified: Fri Apr 14 16:09:53 2023, max compression
+gzip compressed data, was "nitclk-1.4.5.tar", last modified: Mon Jun 12 00:41:45 2023, max compression
```

## Comparing `nitclk-1.4.4.tar` & `nitclk-1.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:10:04.067100 nitclk-1.4.4/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8502 2023-04-14 16:10:04.065103 nitclk-1.4.4/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7536 2023-04-14 16:07:20.000000 nitclk-1.4.4/README.rst
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:10:03.982102 nitclk-1.4.4/nitclk/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:07:16.000000 nitclk-1.4.4/nitclk/VERSION
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3461 2023-04-14 16:07:14.000000 nitclk-1.4.4/nitclk/__init__.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5436 2023-04-14 16:07:09.000000 nitclk-1.4.4/nitclk/_attributes.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14604 2023-04-14 16:07:15.000000 nitclk-1.4.4/nitclk/_converters.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10861 2023-04-14 16:07:09.000000 nitclk-1.4.4/nitclk/_library.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12538 2023-04-14 16:07:10.000000 nitclk-1.4.4/nitclk/_library_interpreter.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1608 2023-04-14 16:07:11.000000 nitclk-1.4.4/nitclk/_library_singleton.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:07:16.000000 nitclk-1.4.4/nitclk/_visatype.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3281 2023-04-14 16:07:12.000000 nitclk-1.4.4/nitclk/errors.py
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)    45940 2023-04-14 16:07:12.000000 nitclk-1.4.4/nitclk/session.py
-drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:10:04.052101 nitclk-1.4.4/nitclk.egg-info/
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8502 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/PKG-INFO
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)      405 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/SOURCES.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/dependency_links.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/requires.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        7 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/top_level.txt
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/zip-safe
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:10:04.068101 nitclk-1.4.4/setup.cfg
--rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1951 2023-04-14 16:07:20.000000 nitclk-1.4.4/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:49.383299 nitclk-1.4.5/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8341 2023-06-12 00:41:49.381299 nitclk-1.4.5/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7284 2023-06-12 00:39:25.000000 nitclk-1.4.5/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:49.302297 nitclk-1.4.5/nitclk/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-06-12 00:39:21.000000 nitclk-1.4.5/nitclk/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3461 2023-06-12 00:39:19.000000 nitclk-1.4.5/nitclk/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5436 2023-06-12 00:39:15.000000 nitclk-1.4.5/nitclk/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14604 2023-06-12 00:39:20.000000 nitclk-1.4.5/nitclk/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10861 2023-06-12 00:39:15.000000 nitclk-1.4.5/nitclk/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12538 2023-06-12 00:39:16.000000 nitclk-1.4.5/nitclk/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1608 2023-06-12 00:39:16.000000 nitclk-1.4.5/nitclk/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-06-12 00:39:21.000000 nitclk-1.4.5/nitclk/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3277 2023-06-12 00:39:18.000000 nitclk-1.4.5/nitclk/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    45940 2023-06-12 00:39:17.000000 nitclk-1.4.5/nitclk/session.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-06-12 00:41:49.368300 nitclk-1.4.5/nitclk.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8341 2023-06-12 00:41:49.000000 nitclk-1.4.5/nitclk.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      405 2023-06-12 00:41:49.000000 nitclk-1.4.5/nitclk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:41:49.000000 nitclk-1.4.5/nitclk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-06-12 00:41:49.000000 nitclk-1.4.5/nitclk.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        7 2023-06-12 00:41:49.000000 nitclk-1.4.5/nitclk.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-06-12 00:41:49.000000 nitclk-1.4.5/nitclk.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-06-12 00:41:49.383299 nitclk-1.4.5/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2001 2023-06-12 00:39:26.000000 nitclk-1.4.5/setup.py
```

### Comparing `nitclk-1.4.4/PKG-INFO` & `nitclk-1.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitclk
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-TClk Python API
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
 
 As a prerequisite to using the nitclk module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nitclk~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nitclk
+  $ python -m pip install nitclk~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -164,30 +160,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nitclk/examples>`_
 
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

### Comparing `nitclk-1.4.4/README.rst` & `nitclk-1.4.5/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -98,32 +98,27 @@
 
 
 .. |nitclkOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nitclk.svg
     :alt: Pull Requests for NI-TClk
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anitclk
 
 
-
-.. _nitclk_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nitclk module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nitclk~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nitclk
-
-
+
+.. _nitclk_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nitclk module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nitclk~=1.4.5
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -132,36 +127,34 @@
 
 .. code-block:: python
 
     import nitclk
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nitclk/examples>`_
 
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

### Comparing `nitclk-1.4.4/nitclk/__init__.py` & `nitclk-1.4.5/nitclk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.4'
+__version__ = '1.4.5'
 
 from nitclk.errors import DriverWarning  # noqa: F401
 from nitclk.errors import Error  # noqa: F401
 from nitclk.session import SessionReference  # noqa: F401
 
 # Function imports
 from nitclk.session import configure_for_homogeneous_triggers  # noqa: F401
@@ -69,15 +69,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-TClk"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nitclk'
-    info['module']['version'] = "1.4.4"
+    info['module']['version'] = "1.4.5"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nitclk-1.4.4/nitclk/_attributes.py` & `nitclk-1.4.5/nitclk/_attributes.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.4/nitclk/_converters.py` & `nitclk-1.4.5/nitclk/_converters.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.4/nitclk/_library.py` & `nitclk-1.4.5/nitclk/_library.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.4/nitclk/_library_interpreter.py` & `nitclk-1.4.5/nitclk/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.4/nitclk/_library_singleton.py` & `nitclk-1.4.5/nitclk/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.4/nitclk/_visatype.py` & `nitclk-1.4.5/nitclk/_visatype.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.4/nitclk/errors.py` & `nitclk-1.4.5/nitclk/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         super(Error, self).__init__(message)
 
 
 class DriverError(Error):
     '''An error originating from the NI-TClk driver'''
 
     def __init__(self, code, description):
-        assert (_is_error(code)), "Should not raise Error if code is not fatal."
+        assert _is_error(code), "Should not raise Error if code is not fatal."
         self.code = code
         self.description = description
         super(DriverError, self).__init__(str(self.code) + ": " + self.description)
 
 
 class DriverWarning(Warning):
     '''A warning originating from the NI-TClk driver'''
 
     def __init__(self, code, description):
-        assert (_is_warning(code)), "Should not create Warning if code is not positive."
+        assert _is_warning(code), "Should not create Warning if code is not positive."
         super(DriverWarning, self).__init__('Warning {0} occurred.\n\n{1}'.format(code, description))
 
 
 class UnsupportedConfigurationError(Error):
     '''An error due to using this module in an usupported platform.'''
 
     def __init__(self):
```

### Comparing `nitclk-1.4.4/nitclk/session.py` & `nitclk-1.4.5/nitclk/session.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.4/nitclk.egg-info/PKG-INFO` & `nitclk-1.4.5/nitclk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitclk
-Version: 1.4.4
+Version: 1.4.5
 Summary: NI-TClk Python API
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
 
 As a prerequisite to using the nitclk module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nitclk~=1.4.4
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nitclk
+  $ python -m pip install nitclk~=1.4.5
 
 
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
@@ -164,30 +160,28 @@
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nitclk/examples>`_
 
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

### Comparing `nitclk-1.4.4/setup.py` & `nitclk-1.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.4',
+    version='1.4.5',
     description='NI-TClk Python API',
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

