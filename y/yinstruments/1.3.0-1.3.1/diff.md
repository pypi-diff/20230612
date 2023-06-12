# Comparing `tmp/yinstruments-1.3.0.tar.gz` & `tmp/yinstruments-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yinstruments-1.3.0.tar", last modified: Fri Jun  9 19:52:27 2023, max compression
+gzip compressed data, was "yinstruments-1.3.1.tar", last modified: Mon Jun 12 19:01:14 2023, max compression
```

## Comparing `yinstruments-1.3.0.tar` & `yinstruments-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-09 19:52:27.097223 yinstruments-1.3.0/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-09 19:52:27.087223 yinstruments-1.3.0/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-06-09 19:52:27.097223 yinstruments-1.3.0/setup.cfg
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      432 2023-06-09 19:50:33.000000 yinstruments-1.3.0/setup.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-09 19:52:27.087223 yinstruments-1.3.0/yinstruments/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3633 2023-06-06 14:51:33.000000 yinstruments-1.3.0/yinstruments/async_reader.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     5828 2023-06-09 19:36:07.000000 yinstruments-1.3.0/yinstruments/powersupply.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     4131 2023-06-09 19:32:01.000000 yinstruments-1.3.0/yinstruments/usb_finder.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3564 2023-06-09 19:39:39.000000 yinstruments-1.3.0/yinstruments/usb_power.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-09 19:52:27.087223 yinstruments-1.3.0/yinstruments.egg-info/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      297 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/SOURCES.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/dependency_links.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       45 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/requires.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       13 2023-06-09 19:52:27.000000 yinstruments-1.3.0/yinstruments.egg-info/top_level.txt
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-12 19:01:14.706849 yinstruments-1.3.1/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-06-12 19:01:14.706849 yinstruments-1.3.1/setup.cfg
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      446 2023-06-12 19:00:57.000000 yinstruments-1.3.1/setup.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/test/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      268 2023-06-12 18:57:50.000000 yinstruments-1.3.1/test/test_packaging.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/yinstruments/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 18:59:11.000000 yinstruments-1.3.1/yinstruments/__init__.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3633 2023-06-06 14:51:33.000000 yinstruments-1.3.1/yinstruments/async_reader.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/yinstruments/pdu/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 18:59:19.000000 yinstruments-1.3.1/yinstruments/pdu/__init__.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1780 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/pdu/cli.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2880 2023-06-12 18:57:50.000000 yinstruments-1.3.1/yinstruments/pdu/lindy.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1982 2023-06-12 18:57:50.000000 yinstruments-1.3.1/yinstruments/pdu/netbooter.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      650 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/pdu/pdu.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     5828 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/powersupply.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     4131 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/usb_finder.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3564 2023-06-12 18:37:25.000000 yinstruments-1.3.1/yinstruments/usb_power.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-06-12 19:01:14.706849 yinstruments-1.3.1/yinstruments.egg-info/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      312 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      478 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/SOURCES.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/dependency_links.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       45 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/requires.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       13 2023-06-12 19:01:14.000000 yinstruments-1.3.1/yinstruments.egg-info/top_level.txt
```

### Comparing `yinstruments-1.3.0/yinstruments/async_reader.py` & `yinstruments-1.3.1/yinstruments/async_reader.py`

 * *Files identical despite different names*

### Comparing `yinstruments-1.3.0/yinstruments/powersupply.py` & `yinstruments-1.3.1/yinstruments/powersupply.py`

 * *Files identical despite different names*

### Comparing `yinstruments-1.3.0/yinstruments/usb_finder.py` & `yinstruments-1.3.1/yinstruments/usb_finder.py`

 * *Files identical despite different names*

### Comparing `yinstruments-1.3.0/yinstruments/usb_power.py` & `yinstruments-1.3.1/yinstruments/usb_power.py`

 * *Files identical despite different names*

