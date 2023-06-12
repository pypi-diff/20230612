# Comparing `tmp/ansys-api-sherlock-0.1.13.tar.gz` & `tmp/ansys-api-sherlock-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-sherlock-0.1.13.tar", last modified: Thu Apr 20 14:30:26 2023, max compression
+gzip compressed data, was "ansys-api-sherlock-0.1.14.tar", last modified: Mon Jun 12 14:07:28 2023, max compression
```

## Comparing `ansys-api-sherlock-0.1.13.tar` & `ansys-api-sherlock-0.1.14.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:30:26.600176 ansys-api-sherlock-0.1.13/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-20 14:30:26.600176 ansys-api-sherlock-0.1.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:30:26.600176 ansys-api-sherlock-0.1.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:30:26.596176 ansys-api-sherlock-0.1.13/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:30:26.596176 ansys-api-sherlock-0.1.13/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:30:26.596176 ansys-api-sherlock-0.1.13/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:30:26.596176 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:30:26.600176 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockCommonService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockLayerService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockModelService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockPartsService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockProjectService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-04-20 14:30:02.000000 ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockStackupService.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:30:26.600176 ansys-api-sherlock-0.1.13/src/ansys_api_sherlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-20 14:30:26.000000 ansys-api-sherlock-0.1.13/src/ansys_api_sherlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 14:30:26.000000 ansys-api-sherlock-0.1.13/src/ansys_api_sherlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:30:26.000000 ansys-api-sherlock-0.1.13/src/ansys_api_sherlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 14:30:26.000000 ansys-api-sherlock-0.1.13/src/ansys_api_sherlock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 14:30:26.000000 ansys-api-sherlock-0.1.13/src/ansys_api_sherlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 14:30:26.000000 ansys-api-sherlock-0.1.13/src/ansys_api_sherlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockCommonService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockLayerService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockModelService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockPartsService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockProjectService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockStackupService.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/top_level.txt
```

### Comparing `ansys-api-sherlock-0.1.13/LICENSE` & `ansys-api-sherlock-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.13/PKG-INFO` & `ansys-api-sherlock-0.1.14/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,64 @@
-Metadata-Version: 2.1
-Name: ansys-api-sherlock
-Version: 0.1.13
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:30:26 on 20 April 2023
-Home-page: https://github.com/ansys/ansys-api-sherlock
-Author: ANSYS, Inc.
-Author-email: support@ansys.com
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### ansys-api-sherlock gRPC Interface Package
 
 This Python package contains the auto-generated gRPC Python interface files for
 Sherlock.
 
 
 #### Installation
 
-Provided that these wheels have been published to public PyPI, they can be
-installed with:
+Provided that wheels have been published to public PyPI, you can install the latest package
+with this command:
 
 ```
 pip install ansys-api-sherlock
 ```
 
-Otherwise, see the
+Otherwise, in the PySherlock documentation, see the instructions for downloading and installing
+this package in`Install packages <https://sherlock.docs.pyansys.com/version/dev/getting_started/installation.html>`_.
 
 
-#### Build
+#### Build packages
 
-To build the gRPC packages, run:
+To build the gRPC packages, run these commands:
 
 ```
 pip install build
 python -m build
 ```
 
-This will create both the source distribution containing just the protofiles
-along with the wheel containing the protofiles and build Python interface
-files.
+The preceding commands create both the source distribution containing only the PROTO files
+and the wheel containing the PROTO files and build Python interface files.
 
 Note that the interface files are identical regardless of the version of Python
 used to generate them, but the last pre-built wheel for ``grpcio~=1.17`` was
-Python 3.7, so to improve your build time, use Python 3.7 when building the
+Python 3.7. To improve your build time, use Python 3.7 when building the
 wheel.
 
 
-#### Manual Deployment
+#### Manual deployment
 
-After building the packages, manually deploy them with:
+After building the packages, manually deploy them with these commands:
 
 ```
 pip install twine
 twine upload dist/*
 ```
 
 Note that this is automatically done through CI/CD.
 
 
-#### Automatic Deployment
+#### Automatic deployment
 
-This repository contains GitHub CI/CD that enables the automatic building of
+This repository contains a ``.github`` directory with the ``ci.yml`` workflow
+file. This file uses GitHub Actions to automatically build the
 source and wheel packages for these gRPC Python interface files. By default,
 these are built on PRs, the main branch, and on tags when pushing. Artifacts
 are uploaded for each PR.
 
-To publicly release wheels to PyPI, ensure your branch is up-to-date and then
-push tags. For example, for the version ``v0.5.0``.
+To publicly release wheels to PyPI, ensure that your branch is up to date and then
+push tags. For example, to push tags for version ``v0.5.0``, you would use these commands:
 
 ```bash
 git tag v0.5.0
 git push --tags
 ```
```

### Comparing `ansys-api-sherlock-0.1.13/setup.py` & `ansys-api-sherlock-0.1.14/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockCommonService.proto` & `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockCommonService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockLayerService.proto` & `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockLayerService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto` & `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockModelService.proto` & `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockModelService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockPartsService.proto` & `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockPartsService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockProjectService.proto` & `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockProjectService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.13/src/ansys/api/sherlock/v0/SherlockStackupService.proto` & `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockStackupService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.13/src/ansys_api_sherlock.egg-info/PKG-INFO` & `ansys-api-sherlock-0.1.14/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.13
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:30:26 on 20 April 2023
+Version: 0.1.14
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:07:28 on 12 June 2023
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,62 +14,63 @@
 
 This Python package contains the auto-generated gRPC Python interface files for
 Sherlock.
 
 
 #### Installation
 
-Provided that these wheels have been published to public PyPI, they can be
-installed with:
+Provided that wheels have been published to public PyPI, you can install the latest package
+with this command:
 
 ```
 pip install ansys-api-sherlock
 ```
 
-Otherwise, see the
+Otherwise, in the PySherlock documentation, see the instructions for downloading and installing
+this package in`Install packages <https://sherlock.docs.pyansys.com/version/dev/getting_started/installation.html>`_.
 
 
-#### Build
+#### Build packages
 
-To build the gRPC packages, run:
+To build the gRPC packages, run these commands:
 
 ```
 pip install build
 python -m build
 ```
 
-This will create both the source distribution containing just the protofiles
-along with the wheel containing the protofiles and build Python interface
-files.
+The preceding commands create both the source distribution containing only the PROTO files
+and the wheel containing the PROTO files and build Python interface files.
 
 Note that the interface files are identical regardless of the version of Python
 used to generate them, but the last pre-built wheel for ``grpcio~=1.17`` was
-Python 3.7, so to improve your build time, use Python 3.7 when building the
+Python 3.7. To improve your build time, use Python 3.7 when building the
 wheel.
 
 
-#### Manual Deployment
+#### Manual deployment
 
-After building the packages, manually deploy them with:
+After building the packages, manually deploy them with these commands:
 
 ```
 pip install twine
 twine upload dist/*
 ```
 
 Note that this is automatically done through CI/CD.
 
 
-#### Automatic Deployment
+#### Automatic deployment
 
-This repository contains GitHub CI/CD that enables the automatic building of
+This repository contains a ``.github`` directory with the ``ci.yml`` workflow
+file. This file uses GitHub Actions to automatically build the
 source and wheel packages for these gRPC Python interface files. By default,
 these are built on PRs, the main branch, and on tags when pushing. Artifacts
 are uploaded for each PR.
 
-To publicly release wheels to PyPI, ensure your branch is up-to-date and then
-push tags. For example, for the version ``v0.5.0``.
+To publicly release wheels to PyPI, ensure that your branch is up to date and then
+push tags. For example, to push tags for version ``v0.5.0``, you would use these commands:
 
 ```bash
 git tag v0.5.0
 git push --tags
 ```
```

### Comparing `ansys-api-sherlock-0.1.13/src/ansys_api_sherlock.egg-info/SOURCES.txt` & `ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

