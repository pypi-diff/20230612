# Comparing `tmp/pyqt5-utils-1.0.2.tar.gz` & `tmp/pyqt5-utils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt5-utils-1.0.2.tar", last modified: Mon Jun 12 10:48:15 2023, max compression
+gzip compressed data, was "pyqt5-utils-1.0.3.tar", last modified: Mon Jun 12 10:52:42 2023, max compression
```

## Comparing `pyqt5-utils-1.0.2.tar` & `pyqt5-utils-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 10:48:15.634709 pyqt5-utils-1.0.2/
--rw-rw-rw-   0        0        0      740 2023-06-12 10:39:09.000000 pyqt5-utils-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      242 2023-06-12 10:48:15.633709 pyqt5-utils-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-12 10:33:40.000000 pyqt5-utils-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 10:48:15.628710 pyqt5-utils-1.0.2/pyqt5_utils/
--rw-rw-rw-   0        0        0      437 2023-06-12 10:46:26.000000 pyqt5-utils-1.0.2/pyqt5_utils/Utils.py
--rw-rw-rw-   0        0        0       24 2023-06-12 10:24:06.000000 pyqt5-utils-1.0.2/pyqt5_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:48:15.632709 pyqt5-utils-1.0.2/pyqt5_utils.egg-info/
--rw-rw-rw-   0        0        0      242 2023-06-12 10:48:15.000000 pyqt5-utils-1.0.2/pyqt5_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-12 10:48:15.000000 pyqt5-utils-1.0.2/pyqt5_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 10:48:15.000000 pyqt5-utils-1.0.2/pyqt5_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-12 10:48:15.000000 pyqt5-utils-1.0.2/pyqt5_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 10:48:15.634709 pyqt5-utils-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-06-12 10:46:39.000000 pyqt5-utils-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:52:42.883953 pyqt5-utils-1.0.3/
+-rw-rw-rw-   0        0        0      740 2023-06-12 10:39:09.000000 pyqt5-utils-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      684 2023-06-12 10:52:42.882953 pyqt5-utils-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-12 10:33:40.000000 pyqt5-utils-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 10:52:42.877954 pyqt5-utils-1.0.3/pyqt5_utils/
+-rw-rw-rw-   0        0        0      437 2023-06-12 10:46:26.000000 pyqt5-utils-1.0.3/pyqt5_utils/Utils.py
+-rw-rw-rw-   0        0        0       24 2023-06-12 10:24:06.000000 pyqt5-utils-1.0.3/pyqt5_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:52:42.881953 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/
+-rw-rw-rw-   0        0        0      684 2023-06-12 10:52:42.000000 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-12 10:52:42.000000 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:52:42.000000 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-12 10:52:42.000000 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:52:42.883953 pyqt5-utils-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      443 2023-06-12 10:52:40.000000 pyqt5-utils-1.0.3/setup.py
```

### Comparing `pyqt5-utils-1.0.2/LICENSE` & `pyqt5-utils-1.0.3/LICENSE`

 * *Files identical despite different names*

