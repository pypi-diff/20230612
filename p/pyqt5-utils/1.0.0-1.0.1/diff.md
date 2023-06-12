# Comparing `tmp/pyqt5-utils-1.0.0.tar.gz` & `tmp/pyqt5-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt5-utils-1.0.0.tar", last modified: Mon Jun 12 10:24:58 2023, max compression
+gzip compressed data, was "pyqt5-utils-1.0.1.tar", last modified: Mon Jun 12 10:39:25 2023, max compression
```

## Comparing `pyqt5-utils-1.0.0.tar` & `pyqt5-utils-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 10:24:58.295295 pyqt5-utils-1.0.0/
--rw-rw-rw-   0        0        0      219 2023-06-12 10:24:58.294296 pyqt5-utils-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 10:24:58.289296 pyqt5-utils-1.0.0/pyqt5_utils/
--rw-rw-rw-   0        0        0      426 2023-06-12 10:23:39.000000 pyqt5-utils-1.0.0/pyqt5_utils/Utils.py
--rw-rw-rw-   0        0        0       24 2023-06-12 10:24:06.000000 pyqt5-utils-1.0.0/pyqt5_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:24:58.293289 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/
--rw-rw-rw-   0        0        0      219 2023-06-12 10:24:58.000000 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-06-12 10:24:58.000000 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 10:24:58.000000 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-12 10:24:58.000000 pyqt5-utils-1.0.0/pyqt5_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 10:24:58.295295 pyqt5-utils-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-06-12 10:24:56.000000 pyqt5-utils-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:39:25.162613 pyqt5-utils-1.0.1/
+-rw-rw-rw-   0        0        0      740 2023-06-12 10:39:09.000000 pyqt5-utils-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      242 2023-06-12 10:39:25.162613 pyqt5-utils-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-12 10:33:40.000000 pyqt5-utils-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 10:39:25.156612 pyqt5-utils-1.0.1/pyqt5_utils/
+-rw-rw-rw-   0        0        0      424 2023-06-12 10:39:09.000000 pyqt5-utils-1.0.1/pyqt5_utils/Utils.py
+-rw-rw-rw-   0        0        0       24 2023-06-12 10:24:06.000000 pyqt5-utils-1.0.1/pyqt5_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:39:25.161614 pyqt5-utils-1.0.1/pyqt5_utils.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-06-12 10:39:25.000000 pyqt5-utils-1.0.1/pyqt5_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-12 10:39:25.000000 pyqt5-utils-1.0.1/pyqt5_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:39:25.000000 pyqt5-utils-1.0.1/pyqt5_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-12 10:39:25.000000 pyqt5-utils-1.0.1/pyqt5_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:39:25.163613 pyqt5-utils-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      234 2023-06-12 10:39:20.000000 pyqt5-utils-1.0.1/setup.py
```

