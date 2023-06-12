# Comparing `tmp/pyqt5-utils-0.1.tar.gz` & `tmp/pyqt5-utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt5-utils-0.1.tar", last modified: Mon Jun 12 10:10:55 2023, max compression
+gzip compressed data, was "pyqt5-utils-1.0.0.tar", last modified: Mon Jun 12 10:24:58 2023, max compression
```

## Comparing `pyqt5-utils-0.1.tar` & `pyqt5-utils-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 10:10:55.856195 pyqt5-utils-0.1/
--rw-rw-rw-   0        0        0      217 2023-06-12 10:10:55.856195 pyqt5-utils-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 10:10:55.850202 pyqt5-utils-0.1/pyqt5_utils/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:59:26.000000 pyqt5-utils-0.1/pyqt5_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:10:55.854201 pyqt5-utils-0.1/pyqt5_utils.egg-info/
--rw-rw-rw-   0        0        0      217 2023-06-12 10:10:55.000000 pyqt5-utils-0.1/pyqt5_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-06-12 10:10:55.000000 pyqt5-utils-0.1/pyqt5_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 10:10:55.000000 pyqt5-utils-0.1/pyqt5_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-12 10:10:55.000000 pyqt5-utils-0.1/pyqt5_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 10:10:55.857194 pyqt5-utils-0.1/setup.cfg
--rw-rw-rw-   0        0        0      232 2023-06-12 10:09:08.000000 pyqt5-utils-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:24:58.295295 pyqt5-utils-1.0.0/
+-rw-rw-rw-   0        0        0      219 2023-06-12 10:24:58.294296 pyqt5-utils-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 10:24:58.289296 pyqt5-utils-1.0.0/pyqt5_utils/
+-rw-rw-rw-   0        0        0      426 2023-06-12 10:23:39.000000 pyqt5-utils-1.0.0/pyqt5_utils/Utils.py
+-rw-rw-rw-   0        0        0       24 2023-06-12 10:24:06.000000 pyqt5-utils-1.0.0/pyqt5_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:24:58.293289 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-06-12 10:24:58.000000 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-06-12 10:24:58.000000 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:24:58.000000 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-12 10:24:58.000000 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:24:58.295295 pyqt5-utils-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      234 2023-06-12 10:24:56.000000 pyqt5-utils-1.0.0/setup.py
```

