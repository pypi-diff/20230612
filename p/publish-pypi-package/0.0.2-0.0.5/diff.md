# Comparing `tmp/publish_pypi_package-0.0.2.tar.gz` & `tmp/publish_pypi_package-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "publish_pypi_package-0.0.2.tar", last modified: Tue May 23 19:54:27 2023, max compression
+gzip compressed data, was "publish_pypi_package-0.0.5.tar", last modified: Mon Jun 12 12:56:01 2023, max compression
```

## Comparing `publish_pypi_package-0.0.2.tar` & `publish_pypi_package-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:54:27.946866 publish_pypi_package-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-23 19:54:16.000000 publish_pypi_package-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-23 19:54:27.946866 publish_pypi_package-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-23 19:54:16.000000 publish_pypi_package-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:54:27.946866 publish_pypi_package-0.0.2/publish_pypi_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-23 19:54:27.000000 publish_pypi_package-0.0.2/publish_pypi_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-23 19:54:27.000000 publish_pypi_package-0.0.2/publish_pypi_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:54:27.000000 publish_pypi_package-0.0.2/publish_pypi_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 19:54:27.000000 publish_pypi_package-0.0.2/publish_pypi_package.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:54:27.946866 publish_pypi_package-0.0.2/py_package/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 19:54:16.000000 publish_pypi_package-0.0.2/py_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 19:54:16.000000 publish_pypi_package-0.0.2/py_package/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-23 19:54:16.000000 publish_pypi_package-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 19:54:27.946866 publish_pypi_package-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-23 19:54:16.000000 publish_pypi_package-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:01.144092 publish_pypi_package-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-12 12:56:01.144092 publish_pypi_package-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:01.140092 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-12 12:56:01.000000 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 12:56:01.000000 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:56:01.000000 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 12:56:01.000000 publish_pypi_package-0.0.5/publish_pypi_package.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:01.140092 publish_pypi_package-0.0.5/py_package/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/py_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/py_package/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:56:01.144092 publish_pypi_package-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:56:01.140092 publish_pypi_package-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 12:55:49.000000 publish_pypi_package-0.0.5/tests/test_tempertaure.py
```

### Comparing `publish_pypi_package-0.0.2/LICENSE` & `publish_pypi_package-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `publish_pypi_package-0.0.2/PKG-INFO` & `publish_pypi_package-0.0.5/publish_pypi_package.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: publish_pypi_package
-Version: 0.0.2
+Name: publish-pypi-package
+Version: 0.0.5
 Summary: Publish the Python package in PyPI
 Author: Refael
 Author-email: Refael Beker <beker.refael@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/RefaelBeker7/publish-python-package
 Project-URL: Bug Tracker, https://github.com/RefaelBeker7/publish-python-package/issues
 Keywords: conversion
@@ -14,36 +14,53 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # publish-python-package
 
 > Publish the Python package in PyPI
 
-### Building the package files
+### Building the package files in local
 ------------------------
 
 We need to build our python package:
 > Before we begin this step, I should mention that I’m using Python3.
 
-* In your terminal (at the root of the project) run:
+1. In your terminal (at the root of the project) run:
 
 ``` 
 python -m pip install --upgrade build
 
 python -m build
 
 python -m pip install --upgrade pip setuptools wheel
 
 python setup.py sdist bdist_wheel
 
 ### This commands creates a source distribution and a shareable wheel that can be published on pypi.org.
 ```
 
-* To test this, create a virtual Python environment.
-* Then, install the convsn package using the wheel distribution. Depending on your Python installation. ```(you may need to use pip3)```
+2. To test this, create a virtual Python environment.
+3. Then, install the convsn package using the wheel distribution. Depending on your Python installation. ```(you may need to use pip3)```
 > Run: pip install <relative-path>python -m pip install .\publish-python-package\dist\package_pypi-0.0.2-py3-none-any.whl
 
 > If need update then run: python -m pip install --upgrade py_package
 
-* Use the python script file named test.py,
+4. Use the python script named `tests/test_tempertaure.py`,
 run the script while still in the virtual Python environment.
 
+## Using the publish Python package
+https://pypi.org/project/publish-pypi-package/
+
+> pip searches for the package files in the official Python Package Index, on pypi.org.
+
+> Installing Python pip on your system allows you to manage PyPI packages easily.
+
+- There are two installation options, via test pypi or via pypi. </br>Both work and have been tested successfully. </br>
+The way to use:
+```
+## Test PyPi - test.pypi.org
+python -m pip install --upgrade --index-url https://test.pypi.org/simple publish_pypi_package
+
+## PyPi - pypi.org
+python -m pip install publish_pypi_package
+```
+- Run the tests/test_tempertaure.py script
```

### Comparing `publish_pypi_package-0.0.2/README.md` & `publish_pypi_package-0.0.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 # publish-python-package
 
 > Publish the Python package in PyPI
 
-### Building the package files
+### Building the package files in local
 ------------------------
 
 We need to build our python package:
 > Before we begin this step, I should mention that I’m using Python3.
 
-* In your terminal (at the root of the project) run:
+1. In your terminal (at the root of the project) run:
 
 ``` 
 python -m pip install --upgrade build
 
 python -m build
 
 python -m pip install --upgrade pip setuptools wheel
 
 python setup.py sdist bdist_wheel
 
 ### This commands creates a source distribution and a shareable wheel that can be published on pypi.org.
 ```
 
-* To test this, create a virtual Python environment.
-* Then, install the convsn package using the wheel distribution. Depending on your Python installation. ```(you may need to use pip3)```
+2. To test this, create a virtual Python environment.
+3. Then, install the convsn package using the wheel distribution. Depending on your Python installation. ```(you may need to use pip3)```
 > Run: pip install <relative-path>python -m pip install .\publish-python-package\dist\package_pypi-0.0.2-py3-none-any.whl
 
 > If need update then run: python -m pip install --upgrade py_package
 
-* Use the python script file named test.py,
+4. Use the python script named `tests/test_tempertaure.py`,
 run the script while still in the virtual Python environment.
 
+## Using the publish Python package
+https://pypi.org/project/publish-pypi-package/
+
+> pip searches for the package files in the official Python Package Index, on pypi.org.
+
+> Installing Python pip on your system allows you to manage PyPI packages easily.
+
+- There are two installation options, via test pypi or via pypi. </br>Both work and have been tested successfully. </br>
+The way to use:
+```
+## Test PyPi - test.pypi.org
+python -m pip install --upgrade --index-url https://test.pypi.org/simple publish_pypi_package
+
+## PyPi - pypi.org
+python -m pip install publish_pypi_package
+```
+- Run the tests/test_tempertaure.py script
```

### Comparing `publish_pypi_package-0.0.2/publish_pypi_package.egg-info/PKG-INFO` & `publish_pypi_package-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: publish-pypi-package
-Version: 0.0.2
+Name: publish_pypi_package
+Version: 0.0.5
 Summary: Publish the Python package in PyPI
 Author: Refael
 Author-email: Refael Beker <beker.refael@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/RefaelBeker7/publish-python-package
 Project-URL: Bug Tracker, https://github.com/RefaelBeker7/publish-python-package/issues
 Keywords: conversion
@@ -14,36 +14,53 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # publish-python-package
 
 > Publish the Python package in PyPI
 
-### Building the package files
+### Building the package files in local
 ------------------------
 
 We need to build our python package:
 > Before we begin this step, I should mention that I’m using Python3.
 
-* In your terminal (at the root of the project) run:
+1. In your terminal (at the root of the project) run:
 
 ``` 
 python -m pip install --upgrade build
 
 python -m build
 
 python -m pip install --upgrade pip setuptools wheel
 
 python setup.py sdist bdist_wheel
 
 ### This commands creates a source distribution and a shareable wheel that can be published on pypi.org.
 ```
 
-* To test this, create a virtual Python environment.
-* Then, install the convsn package using the wheel distribution. Depending on your Python installation. ```(you may need to use pip3)```
+2. To test this, create a virtual Python environment.
+3. Then, install the convsn package using the wheel distribution. Depending on your Python installation. ```(you may need to use pip3)```
 > Run: pip install <relative-path>python -m pip install .\publish-python-package\dist\package_pypi-0.0.2-py3-none-any.whl
 
 > If need update then run: python -m pip install --upgrade py_package
 
-* Use the python script file named test.py,
+4. Use the python script named `tests/test_tempertaure.py`,
 run the script while still in the virtual Python environment.
 
+## Using the publish Python package
+https://pypi.org/project/publish-pypi-package/
+
+> pip searches for the package files in the official Python Package Index, on pypi.org.
+
+> Installing Python pip on your system allows you to manage PyPI packages easily.
+
+- There are two installation options, via test pypi or via pypi. </br>Both work and have been tested successfully. </br>
+The way to use:
+```
+## Test PyPi - test.pypi.org
+python -m pip install --upgrade --index-url https://test.pypi.org/simple publish_pypi_package
+
+## PyPi - pypi.org
+python -m pip install publish_pypi_package
+```
+- Run the tests/test_tempertaure.py script
```

### Comparing `publish_pypi_package-0.0.2/pyproject.toml` & `publish_pypi_package-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "publish_pypi_package"
-version = "0.0.2"
+version = "0.0.5"
 authors = [
     {name = "Refael Beker", email = "beker.refael@gmail.com"},
 ]
 description = "Publish the Python package in PyPI"
 readme = "README.md"
 license = {text = "BSD 3-Clause License"}
 requires-python = ">=3.7"
```

### Comparing `publish_pypi_package-0.0.2/setup.py` & `publish_pypi_package-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.5'
 DESCRIPTION = 'A conversion package'
 LONG_DESCRIPTION = 'A package that makes it easy to convert values between several units of measurement'
 
 setup(
     name="publish_pypi_package",
     version=VERSION,
     description=DESCRIPTION,
```

