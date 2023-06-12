# Comparing `tmp/sentio-prober-control-23.1.2.tar.gz` & `tmp/sentio-prober-control-23.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentio-prober-control-23.1.2.tar", last modified: Mon Mar 20 15:22:11 2023, max compression
+gzip compressed data, was "sentio-prober-control-23.1.3.tar", last modified: Mon Jun 12 14:01:42 2023, max compression
```

## Comparing `sentio-prober-control-23.1.2.tar` & `sentio-prober-control-23.1.3.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:22:11.313490 sentio-prober-control-23.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-20 15:22:11.309490 sentio-prober-control-23.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:22:11.305490 sentio-prober-control-23.1.2/sentio_prober_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:22:11.309490 sentio-prober-control-23.1.2/sentio_prober_control/Communication/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Communication/CommunicatorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Communication/CommunicatorGpib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Communication/CommunicatorTcpIp.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Communication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:22:11.309490 sentio-prober-control-23.1.2/sentio_prober_control/Devices/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Devices/Enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Devices/GpibAdlinkDriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Devices/GpibNiDriver.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:22:11.309490 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:22:11.309490 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/AuxCleaningGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/AuxCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/CommandGroupBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/CompensationCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/LoaderCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/ModuleCommandGroupBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/ProbeCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/ServiceCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/SiPHCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/StatusCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/VisionCameraCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/VisionCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/VisionCompensationGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/VisionIMagProCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapBinsCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapPathCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapPoiCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapSubsiteCommandGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/Enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/ProberBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    14397 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/ProberSentio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/Response.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/Sentio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-20 15:21:59.000000 sentio-prober-control-23.1.2/sentio_prober_control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:22:11.305490 sentio-prober-control-23.1.2/sentio_prober_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-20 15:22:11.000000 sentio-prober-control-23.1.2/sentio_prober_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-20 15:22:11.000000 sentio-prober-control-23.1.2/sentio_prober_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 15:22:11.000000 sentio-prober-control-23.1.2/sentio_prober_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-20 15:22:11.000000 sentio-prober-control-23.1.2/sentio_prober_control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 15:22:11.313490 sentio-prober-control-23.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:42.337060 sentio-prober-control-23.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-12 14:01:42.337060 sentio-prober-control-23.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:42.333060 sentio-prober-control-23.1.3/sentio_prober_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:42.333060 sentio-prober-control-23.1.3/sentio_prober_control/Communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Communication/CommunicatorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Communication/CommunicatorGpib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Communication/CommunicatorTcpIp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Communication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:42.333060 sentio-prober-control-23.1.3/sentio_prober_control/Devices/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Devices/Enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Devices/GpibAdlinkDriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Devices/GpibNiDriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:42.337060 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:42.337060 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/AuxCleaningGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/AuxCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/CommandGroupBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/CompensationCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/LoaderCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/ModuleCommandGroupBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/ProbeCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/ServiceCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/SiPHCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/StatusCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/VisionCameraCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/VisionCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/VisionCompensationGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/VisionIMagProCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapBinsCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapCompensationCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapDieCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapPathCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapPoiCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapSubsiteCommandGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/Enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/ProberBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14364 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/ProberSentio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/Sentio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 14:01:32.000000 sentio-prober-control-23.1.3/sentio_prober_control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:42.333060 sentio-prober-control-23.1.3/sentio_prober_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-12 14:01:42.000000 sentio-prober-control-23.1.3/sentio_prober_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-12 14:01:42.000000 sentio-prober-control-23.1.3/sentio_prober_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:01:42.000000 sentio-prober-control-23.1.3/sentio_prober_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 14:01:42.000000 sentio-prober-control-23.1.3/sentio_prober_control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:01:42.337060 sentio-prober-control-23.1.3/setup.cfg
```

### Comparing `sentio-prober-control-23.1.2/LICENSE` & `sentio-prober-control-23.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/PKG-INFO` & `sentio-prober-control-23.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentio-prober-control
-Version: 23.1.2
+Version: 23.1.3
 Summary: MPI Sentio Prober Control - Python Bindings
 Author-email: Ingo Berg <ingo.berg@atv-systems.de>
 Project-URL: Homepage, https://www.mpi-corporation.com/ast/engineering-probe-systems/mpi-sentio-software-suite/
 Project-URL: Bug Tracker, https://github.com/SentioProberDev/SentioProberControl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,30 +26,26 @@
 ## Instructions for installing the SENTIO® prober control Python package
 
 The package for controlling MPI probe stations running the MPI SENTIO Software suite is now available via [pythons package index](https://pypi.org/project/sentio-prober-control/). To install the
 package simply type:
 
 ```python -m pip install sentio-prober-control```
 
-You no longer need to download the package by yourself, just use pip.
+You no longer need to download the package by yourself, just use pip. If you cannot access the internet from your machine you can still download the archives from [the release section of this project](https://github.com/SentioProberDev/SentioProberControl/releases/).
 
 ## Example-Scripts
 
 A set of example scripts for python is maintained in a seperate archive at GitHub. 
 
 https://github.com/SentioProberDev/Examples-Python
 
 ## Troubleshooting
 
-If you have problems getting the package to work. Check wether an old version of the sentio-prober-control is still installed. To do so type
+Most problems arise from having multiple python environments on the local machine and installing the sentio-prober-control package into the wrong python environment. You can list all installed packages with the command:
 
 ```python -m pip list```
 
-if an older version is listed uninstall it first by using the command. 
-
-```python -m pip uninstall sentio-prober-control```
-
-After the uninstallation you can proceed with the installation as explained in the section above.
+Make sure that the sentio-prober-control package in the latest version is in that list.
 
 ## Instructions for Package maintainer
 
-[Manually Building a Package](PackageUpdate.md)
+[Manually Building a Package](https://github.com/SentioProberDev/SentioProberControl/blob/master/PackageUpdate.md)
```

### Comparing `sentio-prober-control-23.1.2/README.md` & `sentio-prober-control-23.1.3/sentio_prober_control.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,51 @@
+Metadata-Version: 2.1
+Name: sentio-prober-control
+Version: 23.1.3
+Summary: MPI Sentio Prober Control - Python Bindings
+Author-email: Ingo Berg <ingo.berg@atv-systems.de>
+Project-URL: Homepage, https://www.mpi-corporation.com/ast/engineering-probe-systems/mpi-sentio-software-suite/
+Project-URL: Bug Tracker, https://github.com/SentioProberDev/SentioProberControl/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![GitHub issues](https://img.shields.io/github/issues/SentioProberDev/SentioProberControl.svg?maxAge=360)](https://github.com/SentioProberDev/SentioProberControl/issues)
 [![Version](https://img.shields.io/github/release/SentioProberDev/SentioProberControl.svg?maxAge=360)](https://github.com/SentioProberDev/SentioProberControl/releases/)
 # SENTIO® Prober Control - Python Bindings
 This archive contains a package with python bindings to control a [MPI SENTIO® probe station](https://www.mpi-corporation.com/ast/engineering-probe-systems/mpi-sentio-software-suite/).
 
 ![AST_Back_2A fw_](https://user-images.githubusercontent.com/2202567/204108957-0c7a864a-a526-4d32-a1ca-51985a0b01c6.png)
 
 ## Instructions for installing the SENTIO® prober control Python package
 
 The package for controlling MPI probe stations running the MPI SENTIO Software suite is now available via [pythons package index](https://pypi.org/project/sentio-prober-control/). To install the
 package simply type:
 
 ```python -m pip install sentio-prober-control```
 
-You no longer need to download the package by yourself, just use pip.
+You no longer need to download the package by yourself, just use pip. If you cannot access the internet from your machine you can still download the archives from [the release section of this project](https://github.com/SentioProberDev/SentioProberControl/releases/).
 
 ## Example-Scripts
 
 A set of example scripts for python is maintained in a seperate archive at GitHub. 
 
 https://github.com/SentioProberDev/Examples-Python
 
 ## Troubleshooting
 
-If you have problems getting the package to work. Check wether an old version of the sentio-prober-control is still installed. To do so type
+Most problems arise from having multiple python environments on the local machine and installing the sentio-prober-control package into the wrong python environment. You can list all installed packages with the command:
 
 ```python -m pip list```
 
-if an older version is listed uninstall it first by using the command. 
-
-```python -m pip uninstall sentio-prober-control```
-
-After the uninstallation you can proceed with the installation as explained in the section above.
+Make sure that the sentio-prober-control package in the latest version is in that list.
 
 ## Instructions for Package maintainer
 
-[Manually Building a Package](PackageUpdate.md)
+[Manually Building a Package](https://github.com/SentioProberDev/SentioProberControl/blob/master/PackageUpdate.md)
```

### Comparing `sentio-prober-control-23.1.2/pyproject.toml` & `sentio-prober-control-23.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sentio-prober-control"
-version = "23.1.2"
+version = "23.1.3"
 authors = [
   { name="Ingo Berg", email="ingo.berg@atv-systems.de" },
 ]
 description = "MPI Sentio Prober Control - Python Bindings"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Communication/CommunicatorGpib.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Communication/CommunicatorGpib.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Communication/CommunicatorTcpIp.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Communication/CommunicatorTcpIp.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Devices/GpibAdlinkDriver.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Devices/GpibAdlinkDriver.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Devices/GpibNiDriver.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Devices/GpibNiDriver.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/AuxCleaningGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/AuxCleaningGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/AuxCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/AuxCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/CompensationCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/CompensationCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/LoaderCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/LoaderCommandGroup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,11 +41,11 @@
         return resp.message()
 
     def switch_work_area(self, area:str):
         self._comm.send("move_chuck_work_area {0}".format(area))
         resp = Response.check_resp(self._comm.read_line())
         return resp.message()
 
-    def unlaod_wafer(self):
+    def unload_wafer(self):
         self._comm.send("loader:unload_wafer")
         resp = Response.check_resp(self._comm.read_line())
         return resp.message()
```

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/ModuleCommandGroupBase.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/ModuleCommandGroupBase.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/ProbeCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/ProbeCommandGroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,19 +55,14 @@
         return resp.message()
 
     def move_probe_contact(self, probe: ProbeSentio) -> float:
         self.__comm.send("move_positioner_contact {0}".format(probe.toSentioAbbr()))
         resp = Response.check_resp(self.__comm.read_line())
         return float(resp.message())
 
-    def add_probe_site(self, probe: ProbeSentio, x: float = 0, y: float = 0, id: str = None ) -> int:
-        self.__comm.send("add_positioner_site {0},{1},{2},{3}".format(probe.toSentioAbbr(), x, y, id))
-        resp = Response.check_resp(self.__comm.read_line())
-        return int(resp.message())
-
     def get_probe_site(self, probe: ProbeSentio, idx: int ) -> int:
         self.__comm.send("get_positioner_site {0},{1}".format(probe.toSentioAbbr(), idx))
         resp = Response.check_resp(self.__comm.read_line())
         tok = resp.message().split(",")
 
         return int(tok[0]), str(tok[1]), float(tok[2]), float(tok[3])
 
@@ -76,30 +71,54 @@
         resp = Response.check_resp(self.__comm.read_line())
         return int(resp.message())
 
     def step_probe_site(self, probe: ProbeSentio, idx: int )  -> float:
         self.__comm.send("step_positioner_site {0},{1}".format(probe.toSentioAbbr(), idx))
         resp = Response.check_resp(self.__comm.read_line())
         tok = resp.message().split(",")
-        return float(tok[0]), float(tok[1])
+        return tok[0], float(tok[1]), float(tok[2])
 
     def step_probe_site_first(self, probe: ProbeSentio)  -> float:
         self.__comm.send("step_positioner_site_first {0}".format(probe.toSentioAbbr()))
         resp = Response.check_resp(self.__comm.read_line())
         tok = resp.message().split(",")
-        return float(tok[0]), float(tok[1])
+        return tok[0], float(tok[1]), float(tok[2])
 
     def step_probe_site_next(self, probe: ProbeSentio)  -> float:
         self.__comm.send("step_positioner_site_next {0}".format(probe.toSentioAbbr()))
         resp = Response.check_resp(self.__comm.read_line())
         tok = resp.message().split(",")
-        return float(tok[0]), float(tok[1])
+        return tok[0], float(tok[1]), float(tok[2])
 
     def remove_probe_site(self, probe: ProbeSentio, idx: int )  -> float:
         self.__comm.send("remove_positioner_site {0},{1}".format(probe.toSentioAbbr(), idx))
         resp = Response.check_resp(self.__comm.read_line())
         return resp.message()
 
     def reset_probe_site(self, probe: ProbeSentio)  -> float:
         self.__comm.send("reset_positioner_sites {0}".format(probe.toSentioAbbr()))
         resp = Response.check_resp(self.__comm.read_line())
-        return resp.message()
+        return resp.message()
+
+    def async_step_probe_site(self, probe: ProbeSentio, idx: int )  -> float:
+        self.__comm.send("start_step_positioner_site {0},{1}".format(probe.toSentioAbbr(), idx))
+        resp = Response.check_resp(self.__comm.read_line())
+        if not resp.ok():
+            raise ProberException(resp.message())
+
+        return resp.cmd_id()
+
+    def async_step_probe_site_next(self, probe: ProbeSentio)  -> float:
+        self.__comm.send("start_step_positioner_site_next {0}".format(probe.toSentioAbbr()))
+        resp = Response.check_resp(self.__comm.read_line())
+        if not resp.ok():
+            raise ProberException(resp.message())
+
+        return resp.cmd_id()
+
+    def async_step_probe_site_first(self, probe: ProbeSentio)  -> float:
+        self.__comm.send("start_step_positioner_site_first {0}".format(probe.toSentioAbbr()))
+        resp = Response.check_resp(self.__comm.read_line())
+        if not resp.ok():
+            raise ProberException(resp.message())
+
+        return resp.cmd_id()
```

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/ServiceCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/ServiceCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/SiPHCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/SiPHCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/StatusCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/StatusCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/VisionCameraCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/VisionCameraCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/VisionCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/VisionCommandGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,21 +169,21 @@
 
     def ptpa_find_pads(self, row: int = 0, column: int = 0):
         self._comm.send("vis:execute_ptpa_find_pads {0},{1}".format(row, column))
         resp = Response.check_resp(self._comm.read_line())
         tok = resp.message().split(",")
         return float(tok[0]), float(tok[1]), float(tok[2])
 
-    def ptpa_find_tips(self, ptpa_mode: PTPA_Find_Tips_Mode):
+    def ptpa_find_tips(self, ptpa_mode: PtpaFindTipsMode):
         self._comm.send("vis:ptpa_find_tips {0}".format(ptpa_mode.toSentioAbbr()))
         resp = Response.check_resp(self._comm.read_line())
         tok = resp.message().split(",")
         return float(tok[0]), float(tok[1]), float(tok[2])
 
-    def start_execute_compensation(self, comp_type: Die_Compensation_Type, comp_mode: Die_Compensation_Mode):
+    def start_execute_compensation(self, comp_type: DieCompensationType, comp_mode: DieCompensationMode):
         self._comm.send("vis:compensation:start_execute {0},{1}".format(comp_type.toSentioAbbr(), comp_mode.toSentioAbbr()))
         resp = Response.check_resp(self._comm.read_line())
 
         if not resp.ok():
             raise ProberException(resp.message())
 
         return resp.cmd_id()
```

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/VisionCompensationGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/VisionCompensationGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/VisionIMagProCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/VisionIMagProCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapBinsCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapBinsCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapCommandGroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,32 @@
 from sentio_prober_control.Sentio.Response import Response
 from sentio_prober_control.Sentio.ProberBase import ProberException
 from sentio_prober_control.Sentio.CommandGroups.CommandGroupBase import CommandGroupBase
 from sentio_prober_control.Sentio.CommandGroups.WafermapBinsCommandGroup import  WafermapBinsCommandGroup
 from sentio_prober_control.Sentio.CommandGroups.WafermapPathCommandGroup import  WafermapPathCommandGroup
 from sentio_prober_control.Sentio.CommandGroups.WafermapPoiCommandGroup import  WafermapPoiCommandGroup
 from sentio_prober_control.Sentio.CommandGroups.WafermapSubsiteCommandGroup import  WafermapSubsiteGroup
+from sentio_prober_control.Sentio.CommandGroups.WafermapCompensationCommandGroup import  WafermapCompensationCommandGroup
+from sentio_prober_control.Sentio.CommandGroups.WafermapDieCommandGroup import  WafermapDieCommandGroup
 from sentio_prober_control.Sentio.Enumerations import *
 
 from typing import Tuple
 
 
-class WafermapDieGroup(CommandGroupBase):
-    def remove(self, x: int, y: int):
-        self._comm.send("map:die:remove {0}, {1}".format(x, y))
-        Response.check_resp(self._comm.read_line())
-
-
 class WafermapCommandGroup(ModuleCommandGroupBase):
     def __init__(self, comm):
         super().__init__(comm, 'map')
         self.__end_of_route: bool = False
 
         self.subsites = WafermapSubsiteGroup(comm, self)
         self.path = WafermapPathCommandGroup(comm)
         self.bins = WafermapBinsCommandGroup(comm)
-        self.die = WafermapDieGroup(comm)
+        self.die = WafermapDieCommandGroup(comm)
         self.poi = WafermapPoiCommandGroup(comm)
+        self.compensation = WafermapCompensationCommandGroup(comm)
 
     def create(self, diameter: float):
         self._comm.send("map:create {0}".format(diameter))
         Response.check_resp(self._comm.read_line())
 
     def create_rect(self, cols: int, rows: int):
         self._comm.send("map:create_rect {0}, {1}".format(cols, rows))
@@ -233,17 +230,8 @@
         # i.e. Stepping while at the end of the route
         if not resp.ok():
             raise ProberException(resp.message())
 
         return int(tok[0]), int(tok[1]), int(tok[2])
 
     def end_of_route(self):
-        return self.__end_of_routeecute
-
-    def execute_topogrphy(self, execute:ExecuteAction):
-        self._comm.send("map:compensation:topography {}".format(execute.toSentioAbbr()))
-        resp = Response.check_resp(self._comm.read_line())
-        # i.e. Stepping while at the end of the route
-        if not resp.ok():
-            raise ProberException(resp.message())
-
-        return resp.cmd_id()
+        return self.__end_of_route
```

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapPathCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapPathCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapPoiCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapPoiCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/CommandGroups/WafermapSubsiteCommandGroup.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/CommandGroups/WafermapSubsiteCommandGroup.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/Enumerations.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/Enumerations.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,28 +175,31 @@
 class Module(Enum):
     Wafermap = 0,
     Vision = 1,
     Setup = 2,
     Service = 3,
     Qalibria = 4,
     AuxSites = 5,
-    Loader = 6
+    Loader = 6,
+    Dashboard = 7
 
     def toSentioAbbr(self):
         switcher = {
             Module.Wafermap: "Wafermap",
             Module.Vision: "Vision",
             Module.Setup: "Setup",
             Module.Service: "Service",
             Module.Qalibria: "Qalibria",
             Module.AuxSites: "AuxSites",
-            Module.Loader: "Loader"
+            Module.Loader: "Loader",
+            Module.Dashboard: "Dashboard",
         }
         return switcher.get(self, "Invalid Module Name")
 
+
 class AxisOrient(Enum):
     DownRight = 0,
     DownLeft = 1,
     UpRight = 2,
     UpLeft = 3
 
     def toSentioAbbr(self):
@@ -249,21 +252,23 @@
             AutoFocusCmd.GoTo: "G"
         }
         return switcher.get(self, "Invalid auto focus function")
 
 class AutoAlignCmd(Enum):
     AutoDieSize = 0,
     UpdateDieSize = 1,
-    TwoPt = 2
+    TwoPt = 2,
+    CurrentDieSize = 3,
 
     def toSentioAbbr(self):
         switcher = {
             AutoAlignCmd.AutoDieSize: "auto",
             AutoAlignCmd.UpdateDieSize: "update",
-            AutoAlignCmd.TwoPt: "2pt"
+            AutoAlignCmd.TwoPt: "2pt",
+            AutoAlignCmd.CurrentDieSize: ""
         }
         return switcher.get(self, "Invalid Auto Align function")
 
 class ScopeXYReference(Enum):
     Zero = 0,
     Home = 1,
     Relative = 2
@@ -643,24 +648,24 @@
             ProbeXYReference.Current: "Current",
         }
         return switcher.get(self, "Invalid probe xy reference")
 
 
 class ProbeZReference(Enum):
     Zero = 0,
-    Relative = 1,
+    Current = 1,
     Contact = 2,
     Separation = 3
 
     def toSentioAbbr(self):
         switcher = {
-            ProbeZReference.Zero: "Z",
-            ProbeZReference.Relative: "R",
-            ProbeZReference.Contact: "C",
-            ProbeZReference.Separation: "S"
+            ProbeZReference.Zero: "Zero",
+            ProbeZReference.Current: "Current",
+            ProbeZReference.Contact: "Contact",
+            ProbeZReference.Separation: "Separation"
         }
         return switcher.get(self, "Invalid probe z reference")
 
 
 class ProbeSentio(Enum):
     East = 0,
     West = 1,
@@ -731,51 +736,51 @@
 class ExecuteAction(Enum):
     Execute = 0,
     Abort = 1,
 
     def toSentioAbbr(self):
         switcher = {
             ExecuteAction.Execute: "execute",
-            ExecuteAction.Abort: "aboru",
+            ExecuteAction.Abort: "abort",
         }
         return switcher.get(self, "Invalid ExecuteAction function")
 
-class PTPA_Find_Tips_Mode(Enum):
+class PtpaFindTipsMode(Enum):
     OnAxis = 0,
     OffAxis = 1,
 
     def toSentioAbbr(self):
         switcher = {
-            PTPA_Find_Tips_Mode.OnAxis: "OnAxis",
-            PTPA_Find_Tips_Mode.OffAxis: "OffAxis",
+            PtpaFindTipsMode.OnAxis: "OnAxis",
+            PtpaFindTipsMode.OffAxis: "OffAxis",
         }
         return switcher.get(self, "Invalid PTPA_Find_Tips_Mode function")
 
-class Die_Compensation_Type(Enum):
-    DiaAlign = 0,
+class DieCompensationType(Enum):
+    DieAlign = 0,
     MapScan = 1,
     Topography = 2,
 
     def toSentioAbbr(self):
         switcher = {
-            Die_Compensation_Type.DiaAlign: "DiaAlign",
-            Die_Compensation_Type.MapScan: "MapScan",
-            Die_Compensation_Type.MapScan: "Topography",
+            DieCompensationType.DieAlign: "DieAlign",
+            DieCompensationType.MapScan: "MapScan",
+            DieCompensationType.Topography: "Topography",
         }
         return switcher.get(self, "Invalid Compensation_Type function")
 
-class Die_Compensation_Mode(Enum):
+class DieCompensationMode(Enum):
     Lateral = 0,
     Vertical = 1,
     Both = 2,
     ProbeCard = 3,
     SkateDetection = 4,
 
     def toSentioAbbr(self):
         switcher = {
-            Die_Compensation_Mode.Lateral: "Lateral",
-            Die_Compensation_Mode.Vertical: "Vertical",
-            Die_Compensation_Mode.Both: "Both",
-            Die_Compensation_Mode.ProbeCard: "ProbeCard",
-            Die_Compensation_Mode.SkateDetection: "SkateDetection",
+            DieCompensationMode.Lateral: "Lateral",
+            DieCompensationMode.Vertical: "Vertical",
+            DieCompensationMode.Both: "Both",
+            DieCompensationMode.ProbeCard: "ProbeCard",
+            DieCompensationMode.SkateDetection: "SkateDetection",
         }
-        return switcher.get(self, "Invalid Die_Compensation_Mode function")
+        return switcher.get(self, "Invalid DieCompensationMode function")
```

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/ProberBase.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/ProberBase.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/ProberSentio.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/ProberSentio.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,14 +249,18 @@
         return float(tok[0]), float(tok[1])
 
     def move_scope_z(self, ref: ScopeZReference, z: float) -> float:
         self.comm.send("move_scope_z {0}, {1}".format(ref.toSentioAbbr(), z))
         resp = Response.check_resp(self.comm.read_line())
         return float(resp.message())
 
+    def move_scope_lift(self, state: bool) -> float:
+        self.comm.send(f"move_scope_lift {state}")
+        Response.check_resp(self.comm.read_line())
+
     def get_scope_xy(self) -> Tuple[float, float]:
         self.comm.send("get_scope_xy")
         resp = Response.check_resp(self.comm.read_line())
         tok = resp.message().split(",")
         return float(tok[0]), float(tok[1])
 
     def get_scope_z(self) -> float:
@@ -334,12 +338,7 @@
         self.comm.send('status:show_hint \"{0}\", \"{1}\"'.format(msg, subtext))
         resp = Response.check_resp(self.comm.read_line())
 
     def get_project(self, pfi: ProjectFileInfo = ProjectFileInfo.FullPath) -> str:
         self.comm.send(f'get_project {pfi.toSentioAbbr()}')
         resp = Response.check_resp(self.comm.read_line())
         return resp.message()
-
-    def step_scope_site(self, site: str):
-        self.comm.send('step_scope_site {}'.format(site))
-        resp = Response.check_resp(self.comm.read_line())
-        return resp.message()
```

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control/Sentio/Response.py` & `sentio-prober-control-23.1.3/sentio_prober_control/Sentio/Response.py`

 * *Files identical despite different names*

### Comparing `sentio-prober-control-23.1.2/sentio_prober_control.egg-info/SOURCES.txt` & `sentio-prober-control-23.1.3/sentio_prober_control.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -31,11 +31,13 @@
 sentio_prober_control/Sentio/CommandGroups/StatusCommandGroup.py
 sentio_prober_control/Sentio/CommandGroups/VisionCameraCommandGroup.py
 sentio_prober_control/Sentio/CommandGroups/VisionCommandGroup.py
 sentio_prober_control/Sentio/CommandGroups/VisionCompensationGroup.py
 sentio_prober_control/Sentio/CommandGroups/VisionIMagProCommandGroup.py
 sentio_prober_control/Sentio/CommandGroups/WafermapBinsCommandGroup.py
 sentio_prober_control/Sentio/CommandGroups/WafermapCommandGroup.py
+sentio_prober_control/Sentio/CommandGroups/WafermapCompensationCommandGroup.py
+sentio_prober_control/Sentio/CommandGroups/WafermapDieCommandGroup.py
 sentio_prober_control/Sentio/CommandGroups/WafermapPathCommandGroup.py
 sentio_prober_control/Sentio/CommandGroups/WafermapPoiCommandGroup.py
 sentio_prober_control/Sentio/CommandGroups/WafermapSubsiteCommandGroup.py
 sentio_prober_control/Sentio/CommandGroups/__init__.py
```

