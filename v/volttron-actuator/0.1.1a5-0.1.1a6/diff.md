# Comparing `tmp/volttron_actuator-0.1.1a5.tar.gz` & `tmp/volttron_actuator-0.1.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_actuator-0.1.1a5.tar", max compression
+gzip compressed data, was "volttron_actuator-0.1.1a6.tar", max compression
```

## Comparing `volttron_actuator-0.1.1a5.tar` & `volttron_actuator-0.1.1a6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11927 2023-05-08 19:50:39.203936 volttron_actuator-0.1.1a5/LICENSE
--rw-r--r--   0        0        0     2666 2023-05-08 19:50:39.203936 volttron_actuator-0.1.1a5/README.md
--rw-r--r--   0        0        0     1910 2023-05-08 19:52:00.688713 volttron_actuator-0.1.1a5/pyproject.toml
--rw-r--r--   0        0        0     1570 2023-05-08 19:50:39.203936 volttron_actuator-0.1.1a5/src/actuator/__init__.py
--rw-r--r--   0        0        0    52552 2023-05-08 19:50:39.203936 volttron_actuator-0.1.1a5/src/actuator/agent.py
--rw-r--r--   0        0        0    16122 2023-05-08 19:50:39.203936 volttron_actuator-0.1.1a5/src/actuator/scheduler.py
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a5/setup.py
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a5/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/LICENSE
+-rw-r--r--   0        0        0     1830 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/README.md
+-rw-r--r--   0        0        0     1910 2023-06-12 17:05:50.085291 volttron_actuator-0.1.1a6/pyproject.toml
+-rw-r--r--   0        0        0     1570 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/src/actuator/__init__.py
+-rw-r--r--   0        0        0    52552 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/src/actuator/agent.py
+-rw-r--r--   0        0        0    16122 2023-06-12 17:03:42.499354 volttron_actuator-0.1.1a6/src/actuator/scheduler.py
+-rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a6/setup.py
+-rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a6/PKG-INFO
```

### Comparing `volttron_actuator-0.1.1a5/LICENSE` & `volttron_actuator-0.1.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a5/pyproject.toml` & `volttron_actuator-0.1.1a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 exclude = ['docs/']
 
 [tool.poetry]
 name = "volttron-actuator"
-version = "0.1.1a5"
+version = "0.1.1a6"
 description = "The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices."
 authors = ["Mark Bonicillo <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/VOLTTRON/volttron-actuator"
 homepage = "https://github.com/VOLTTRON/volttron-actuator"
 keywords = []
```

### Comparing `volttron_actuator-0.1.1a5/src/actuator/__init__.py` & `volttron_actuator-0.1.1a6/src/actuator/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a5/src/actuator/agent.py` & `volttron_actuator-0.1.1a6/src/actuator/agent.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a5/src/actuator/scheduler.py` & `volttron_actuator-0.1.1a6/src/actuator/scheduler.py`

 * *Files identical despite different names*

