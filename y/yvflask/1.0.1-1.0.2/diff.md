# Comparing `tmp/yvflask-1.0.1.tar.gz` & `tmp/yvflask-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvflask-1.0.1.tar", last modified: Mon Jun 12 04:53:04 2023, max compression
+gzip compressed data, was "yvflask-1.0.2.tar", last modified: Mon Jun 12 06:37:53 2023, max compression
```

## Comparing `yvflask-1.0.1.tar` & `yvflask-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.706654 yvflask-1.0.1/
--rw-rw-rw-   0        0        0      388 2023-06-12 04:53:04.705655 yvflask-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-12 04:53:04.706654 yvflask-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-06-12 04:49:35.000000 yvflask-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.661811 yvflask-1.0.1/yvflask/
-drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.696679 yvflask-1.0.1/yvflask/FlaskManage/
--rw-rw-rw-   0        0        0       24 2023-06-11 15:20:16.000000 yvflask-1.0.1/yvflask/FlaskManage/__init__.py
--rw-rw-rw-   0        0        0     1329 2023-06-11 18:49:38.000000 yvflask-1.0.1/yvflask/FlaskManage/manager.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.702712 yvflask-1.0.1/yvflask/Yvapp/
--rw-rw-rw-   0        0        0       21 2023-06-11 16:10:59.000000 yvflask-1.0.1/yvflask/Yvapp/__init__.py
--rw-rw-rw-   0        0        0     3086 2023-06-11 18:50:51.000000 yvflask-1.0.1/yvflask/Yvapp/newApp.py
--rw-rw-rw-   0        0        0       46 2023-06-11 16:10:50.000000 yvflask-1.0.1/yvflask/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:53:04.690695 yvflask-1.0.1/yvflask.egg-info/
--rw-rw-rw-   0        0        0      388 2023-06-12 04:53:04.000000 yvflask-1.0.1/yvflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-06-12 04:53:04.000000 yvflask-1.0.1/yvflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 04:53:04.000000 yvflask-1.0.1/yvflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 04:53:04.000000 yvflask-1.0.1/yvflask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 06:37:53.215071 yvflask-1.0.2/
+-rw-rw-rw-   0        0        0      386 2023-06-12 06:37:53.213077 yvflask-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-12 06:37:53.216066 yvflask-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-06-12 06:34:45.000000 yvflask-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:37:53.200109 yvflask-1.0.2/yvflask.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-06-12 06:37:53.000000 yvflask-1.0.2/yvflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-12 06:37:53.000000 yvflask-1.0.2/yvflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:37:53.000000 yvflask-1.0.2/yvflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 06:37:53.000000 yvflask-1.0.2/yvflask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 06:37:53.203110 yvflask-1.0.2/yvtools/
+drwxrwxrwx   0        0        0        0 2023-06-12 06:37:53.207092 yvflask-1.0.2/yvtools/FlaskManage/
+-rw-rw-rw-   0        0        0       30 2023-06-12 06:25:17.000000 yvflask-1.0.2/yvtools/FlaskManage/__init__.py
+-rw-rw-rw-   0        0        0     1329 2023-06-11 18:49:38.000000 yvflask-1.0.2/yvtools/FlaskManage/manager.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:37:53.211082 yvflask-1.0.2/yvtools/Yvapp/
+-rw-rw-rw-   0        0        0       28 2023-06-12 06:26:03.000000 yvflask-1.0.2/yvtools/Yvapp/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-06-12 06:20:52.000000 yvflask-1.0.2/yvtools/Yvapp/newApp.py
+-rw-rw-rw-   0        0        0       48 2023-06-12 06:27:42.000000 yvflask-1.0.2/yvtools/__init__.py
```

### Comparing `yvflask-1.0.1/yvflask/FlaskManage/manager.py` & `yvflask-1.0.2/yvtools/FlaskManage/manager.py`

 * *Files identical despite different names*

