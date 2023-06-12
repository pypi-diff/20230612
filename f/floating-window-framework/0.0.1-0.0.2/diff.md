# Comparing `tmp/floating-window-framework-0.0.1.tar.gz` & `tmp/floating-window-framework-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floating-window-framework-0.0.1.tar", last modified: Mon Jun 12 10:41:15 2023, max compression
+gzip compressed data, was "floating-window-framework-0.0.2.tar", last modified: Mon Jun 12 10:44:27 2023, max compression
```

## Comparing `floating-window-framework-0.0.1.tar` & `floating-window-framework-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 10:41:15.946248 floating-window-framework-0.0.1/
--rw-r--r--   0 attai     (1000) attai     (1000)     1070 2023-06-12 10:09:18.000000 floating-window-framework-0.0.1/LICENSE
--rw-r--r--   0 attai     (1000) attai     (1000)      493 2023-06-12 10:41:15.946248 floating-window-framework-0.0.1/PKG-INFO
--rw-r--r--   0 attai     (1000) attai     (1000)     2648 2023-06-12 10:07:53.000000 floating-window-framework-0.0.1/README.md
-drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 10:41:15.946248 floating-window-framework-0.0.1/floating_window_framework.egg-info/
--rw-r--r--   0 attai     (1000) attai     (1000)      493 2023-06-12 10:41:15.000000 floating-window-framework-0.0.1/floating_window_framework.egg-info/PKG-INFO
--rw-r--r--   0 attai     (1000) attai     (1000)      348 2023-06-12 10:41:15.000000 floating-window-framework-0.0.1/floating_window_framework.egg-info/SOURCES.txt
--rw-r--r--   0 attai     (1000) attai     (1000)        1 2023-06-12 10:41:15.000000 floating-window-framework-0.0.1/floating_window_framework.egg-info/dependency_links.txt
--rw-r--r--   0 attai     (1000) attai     (1000)        8 2023-06-12 10:41:15.000000 floating-window-framework-0.0.1/floating_window_framework.egg-info/requires.txt
--rw-r--r--   0 attai     (1000) attai     (1000)        4 2023-06-12 10:41:15.000000 floating-window-framework-0.0.1/floating_window_framework.egg-info/top_level.txt
-drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 10:41:15.946248 floating-window-framework-0.0.1/fwf/
--rw-r--r--   0 attai     (1000) attai     (1000)      115 2023-06-12 10:35:10.000000 floating-window-framework-0.0.1/fwf/__init__.py
--rw-r--r--   0 attai     (1000) attai     (1000)     1787 2023-06-12 10:36:50.000000 floating-window-framework-0.0.1/fwf/base_app.py
--rw-r--r--   0 attai     (1000) attai     (1000)     2407 2023-06-12 10:34:21.000000 floating-window-framework-0.0.1/fwf/component.py
--rw-r--r--   0 attai     (1000) attai     (1000)      527 2023-06-12 10:34:19.000000 floating-window-framework-0.0.1/fwf/keybindings.py
--rw-r--r--   0 attai     (1000) attai     (1000)       79 2023-06-12 10:41:15.946248 floating-window-framework-0.0.1/setup.cfg
--rw-r--r--   0 attai     (1000) attai     (1000)      698 2023-06-12 10:41:00.000000 floating-window-framework-0.0.1/setup.py
+drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 10:44:27.314749 floating-window-framework-0.0.2/
+-rw-r--r--   0 attai     (1000) attai     (1000)     1070 2023-06-12 10:09:18.000000 floating-window-framework-0.0.2/LICENSE
+-rw-r--r--   0 attai     (1000) attai     (1000)      493 2023-06-12 10:44:27.314749 floating-window-framework-0.0.2/PKG-INFO
+-rw-r--r--   0 attai     (1000) attai     (1000)     2648 2023-06-12 10:07:53.000000 floating-window-framework-0.0.2/README.md
+drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 10:44:27.314749 floating-window-framework-0.0.2/floating_window_framework.egg-info/
+-rw-r--r--   0 attai     (1000) attai     (1000)      493 2023-06-12 10:44:27.000000 floating-window-framework-0.0.2/floating_window_framework.egg-info/PKG-INFO
+-rw-r--r--   0 attai     (1000) attai     (1000)      348 2023-06-12 10:44:27.000000 floating-window-framework-0.0.2/floating_window_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 attai     (1000) attai     (1000)        1 2023-06-12 10:44:27.000000 floating-window-framework-0.0.2/floating_window_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 attai     (1000) attai     (1000)        8 2023-06-12 10:44:27.000000 floating-window-framework-0.0.2/floating_window_framework.egg-info/requires.txt
+-rw-r--r--   0 attai     (1000) attai     (1000)        4 2023-06-12 10:44:27.000000 floating-window-framework-0.0.2/floating_window_framework.egg-info/top_level.txt
+drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 10:44:27.314749 floating-window-framework-0.0.2/fwf/
+-rw-r--r--   0 attai     (1000) attai     (1000)      115 2023-06-12 10:35:10.000000 floating-window-framework-0.0.2/fwf/__init__.py
+-rw-r--r--   0 attai     (1000) attai     (1000)     1787 2023-06-12 10:36:50.000000 floating-window-framework-0.0.2/fwf/base_app.py
+-rw-r--r--   0 attai     (1000) attai     (1000)     2407 2023-06-12 10:34:21.000000 floating-window-framework-0.0.2/fwf/component.py
+-rw-r--r--   0 attai     (1000) attai     (1000)      527 2023-06-12 10:34:19.000000 floating-window-framework-0.0.2/fwf/keybindings.py
+-rw-r--r--   0 attai     (1000) attai     (1000)       79 2023-06-12 10:44:27.314749 floating-window-framework-0.0.2/setup.cfg
+-rw-r--r--   0 attai     (1000) attai     (1000)      698 2023-06-12 10:43:03.000000 floating-window-framework-0.0.2/setup.py
```

### Comparing `floating-window-framework-0.0.1/LICENSE` & `floating-window-framework-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.1/README.md` & `floating-window-framework-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.1/fwf/base_app.py` & `floating-window-framework-0.0.2/fwf/base_app.py`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.1/fwf/component.py` & `floating-window-framework-0.0.2/fwf/component.py`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.1/fwf/keybindings.py` & `floating-window-framework-0.0.2/fwf/keybindings.py`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.1/setup.py` & `floating-window-framework-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='floating-window-framework',
-    version='0.0.1',
+    version='0.0.2',
     description='Floating Window Framework',
     long_description='A framework for building floating window applications.',
     author='Youssef Attai',
     author_email='youssefgalalnazem@gmail.com',
     url='https://github.com/youssef-attai/fwf',
     packages=['fwf'],
     classifiers=[
```

