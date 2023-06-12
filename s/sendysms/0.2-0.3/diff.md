# Comparing `tmp/sendysms-0.2.tar.gz` & `tmp/sendysms-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sendysms-0.2.tar", last modified: Mon Jun 12 20:35:08 2023, max compression
+gzip compressed data, was "sendysms-0.3.tar", last modified: Mon Jun 12 20:53:46 2023, max compression
```

## Comparing `sendysms-0.2.tar` & `sendysms-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 20:35:08.750067 sendysms-0.2/
--rw-rw-rw-   0        0        0      236 2023-06-12 20:35:08.745100 sendysms-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 20:35:08.668085 sendysms-0.2/sendysms/
--rw-rw-rw-   0        0        0      496 2023-06-12 20:29:27.000000 sendysms-0.2/sendysms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 20:35:08.740132 sendysms-0.2/sendysms.egg-info/
--rw-rw-rw-   0        0        0      236 2023-06-12 20:35:08.000000 sendysms-0.2/sendysms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-12 20:35:08.000000 sendysms-0.2/sendysms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 20:35:08.000000 sendysms-0.2/sendysms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 20:35:08.000000 sendysms-0.2/sendysms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 20:35:08.000000 sendysms-0.2/sendysms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 20:35:08.750067 sendysms-0.2/setup.cfg
--rw-rw-rw-   0        0        0      360 2023-06-12 20:34:52.000000 sendysms-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:53:46.339523 sendysms-0.3/
+-rw-rw-rw-   0        0        0      236 2023-06-12 20:53:46.334557 sendysms-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 20:53:46.250587 sendysms-0.3/sendysms/
+-rw-rw-rw-   0        0        0      482 2023-06-12 20:53:27.000000 sendysms-0.3/sendysms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:53:46.328596 sendysms-0.3/sendysms.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-06-12 20:53:45.000000 sendysms-0.3/sendysms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-12 20:53:45.000000 sendysms-0.3/sendysms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 20:53:45.000000 sendysms-0.3/sendysms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 20:53:45.000000 sendysms-0.3/sendysms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 20:53:45.000000 sendysms-0.3/sendysms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 20:53:46.339523 sendysms-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      360 2023-06-12 20:53:32.000000 sendysms-0.3/setup.py
```

