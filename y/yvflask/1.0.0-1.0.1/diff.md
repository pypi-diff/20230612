# Comparing `tmp/yvflask-1.0.0.tar.gz` & `tmp/yvflask-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvflask-1.0.0.tar", last modified: Sun Jun 11 18:57:25 2023, max compression
+gzip compressed data, was "yvflask-1.0.1.tar", last modified: Mon Jun 12 04:53:04 2023, max compression
```

## Comparing `yvflask-1.0.0.tar` & `yvflask-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 18:57:25.479885 yvflask-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-11 18:57:25.441625 yvflask-1.0.0/FlaskManage/
--rw-rw-rw-   0        0        0       24 2023-06-11 15:20:16.000000 yvflask-1.0.0/FlaskManage/__init__.py
--rw-rw-rw-   0        0        0     1329 2023-06-11 18:49:38.000000 yvflask-1.0.0/FlaskManage/manager.py
--rw-rw-rw-   0        0        0      388 2023-06-11 18:57:25.477928 yvflask-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 18:57:25.447608 yvflask-1.0.0/Yvapp/
--rw-rw-rw-   0        0        0       21 2023-06-11 16:10:59.000000 yvflask-1.0.0/Yvapp/__init__.py
--rw-rw-rw-   0        0        0     3086 2023-06-11 18:50:51.000000 yvflask-1.0.0/Yvapp/newApp.py
--rw-rw-rw-   0        0        0       42 2023-06-11 18:57:25.479885 yvflask-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-06-11 18:54:06.000000 yvflask-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 18:57:25.475933 yvflask-1.0.0/yvflask.egg-info/
--rw-rw-rw-   0        0        0      388 2023-06-11 18:57:25.000000 yvflask-1.0.0/yvflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-11 18:57:25.000000 yvflask-1.0.0/yvflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 18:57:25.000000 yvflask-1.0.0/yvflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-11 18:57:25.000000 yvflask-1.0.0/yvflask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.706654 yvflask-1.0.1/
+-rw-rw-rw-   0        0        0      388 2023-06-12 04:53:04.705655 yvflask-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-12 04:53:04.706654 yvflask-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      510 2023-06-12 04:49:35.000000 yvflask-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.661811 yvflask-1.0.1/yvflask/
+drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.696679 yvflask-1.0.1/yvflask/FlaskManage/
+-rw-rw-rw-   0        0        0       24 2023-06-11 15:20:16.000000 yvflask-1.0.1/yvflask/FlaskManage/__init__.py
+-rw-rw-rw-   0        0        0     1329 2023-06-11 18:49:38.000000 yvflask-1.0.1/yvflask/FlaskManage/manager.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.702712 yvflask-1.0.1/yvflask/Yvapp/
+-rw-rw-rw-   0        0        0       21 2023-06-11 16:10:59.000000 yvflask-1.0.1/yvflask/Yvapp/__init__.py
+-rw-rw-rw-   0        0        0     3086 2023-06-11 18:50:51.000000 yvflask-1.0.1/yvflask/Yvapp/newApp.py
+-rw-rw-rw-   0        0        0       46 2023-06-11 16:10:50.000000 yvflask-1.0.1/yvflask/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.690695 yvflask-1.0.1/yvflask.egg-info/
+-rw-rw-rw-   0        0        0      388 2023-06-12 04:53:04.000000 yvflask-1.0.1/yvflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-12 04:53:04.000000 yvflask-1.0.1/yvflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 04:53:04.000000 yvflask-1.0.1/yvflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 04:53:04.000000 yvflask-1.0.1/yvflask.egg-info/top_level.txt
```

### Comparing `yvflask-1.0.0/FlaskManage/manager.py` & `yvflask-1.0.1/yvflask/FlaskManage/manager.py`

 * *Files identical despite different names*

### Comparing `yvflask-1.0.0/Yvapp/newApp.py` & `yvflask-1.0.1/yvflask/Yvapp/newApp.py`

 * *Files identical despite different names*

