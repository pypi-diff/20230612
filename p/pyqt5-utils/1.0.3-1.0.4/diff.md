# Comparing `tmp/pyqt5-utils-1.0.3.tar.gz` & `tmp/pyqt5-utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt5-utils-1.0.3.tar", last modified: Mon Jun 12 10:52:42 2023, max compression
+gzip compressed data, was "pyqt5-utils-1.0.4.tar", last modified: Mon Jun 12 10:54:56 2023, max compression
```

## Comparing `pyqt5-utils-1.0.3.tar` & `pyqt5-utils-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 10:52:42.883953 pyqt5-utils-1.0.3/
--rw-rw-rw-   0        0        0      740 2023-06-12 10:39:09.000000 pyqt5-utils-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      684 2023-06-12 10:52:42.882953 pyqt5-utils-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-12 10:33:40.000000 pyqt5-utils-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 10:52:42.877954 pyqt5-utils-1.0.3/pyqt5_utils/
--rw-rw-rw-   0        0        0      437 2023-06-12 10:46:26.000000 pyqt5-utils-1.0.3/pyqt5_utils/Utils.py
--rw-rw-rw-   0        0        0       24 2023-06-12 10:24:06.000000 pyqt5-utils-1.0.3/pyqt5_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:52:42.881953 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/
--rw-rw-rw-   0        0        0      684 2023-06-12 10:52:42.000000 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-12 10:52:42.000000 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 10:52:42.000000 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-12 10:52:42.000000 pyqt5-utils-1.0.3/pyqt5_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 10:52:42.883953 pyqt5-utils-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      443 2023-06-12 10:52:40.000000 pyqt5-utils-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:54:56.338691 pyqt5-utils-1.0.4/
+-rw-rw-rw-   0        0        0      740 2023-06-12 10:39:09.000000 pyqt5-utils-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      649 2023-06-12 10:54:56.337691 pyqt5-utils-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-06-12 10:54:39.000000 pyqt5-utils-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 10:54:56.332700 pyqt5-utils-1.0.4/pyqt5_utils/
+-rw-rw-rw-   0        0        0      437 2023-06-12 10:46:26.000000 pyqt5-utils-1.0.4/pyqt5_utils/Utils.py
+-rw-rw-rw-   0        0        0       24 2023-06-12 10:24:06.000000 pyqt5-utils-1.0.4/pyqt5_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:54:56.336691 pyqt5-utils-1.0.4/pyqt5_utils.egg-info/
+-rw-rw-rw-   0        0        0      649 2023-06-12 10:54:56.000000 pyqt5-utils-1.0.4/pyqt5_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-12 10:54:56.000000 pyqt5-utils-1.0.4/pyqt5_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:54:56.000000 pyqt5-utils-1.0.4/pyqt5_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-12 10:54:56.000000 pyqt5-utils-1.0.4/pyqt5_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:54:56.338691 pyqt5-utils-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      443 2023-06-12 10:54:52.000000 pyqt5-utils-1.0.4/setup.py
```

### Comparing `pyqt5-utils-1.0.3/LICENSE` & `pyqt5-utils-1.0.4/LICENSE`

 * *Files identical despite different names*

