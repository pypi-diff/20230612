# Comparing `tmp/decoratory-0.0.1.tar.gz` & `tmp/decoratory-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.0.1.tar", last modified: Thu Jun  8 06:40:57 2023, max compression
+gzip compressed data, was "decoratory-0.1.0.1.tar", last modified: Mon Jun 12 12:50:24 2023, max compression
```

## Comparing `decoratory-0.0.1.tar` & `decoratory-0.1.0.1.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 06:40:57.481399 decoratory-0.0.1/
--rw-rw-rw-   0        0        0     1095 2023-06-07 09:14:23.000000 decoratory-0.0.1/License.txt
--rw-rw-rw-   0        0        0     1497 2023-06-08 06:40:57.481399 decoratory-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-06-07 16:58:08.000000 decoratory-0.0.1/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-07 14:24:45.000000 decoratory-0.0.1/Requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 06:40:57.485396 decoratory-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3502 2023-06-08 06:40:19.000000 decoratory-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 06:40:57.449422 decoratory-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 06:40:57.465400 decoratory-0.0.1/src/decoratory/
--rw-rw-rw-   0        0        0        0 2023-06-07 09:04:14.000000 decoratory-0.0.1/src/decoratory/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-07 09:05:05.000000 decoratory-0.0.1/src/decoratory/example.py
-drwxrwxrwx   0        0        0        0 2023-06-08 06:40:57.481399 decoratory-0.0.1/src/decoratory.egg-info/
--rw-rw-rw-   0        0        0     1497 2023-06-08 06:40:57.000000 decoratory-0.0.1/src/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-06-08 06:40:57.000000 decoratory-0.0.1/src/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 06:40:57.000000 decoratory-0.0.1/src/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 06:40:57.000000 decoratory-0.0.1/src/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 12:50:24.058247 decoratory-0.1.0.1/
+-rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.0.1/License.txt
+-rw-rw-rw-   0        0        0    16170 2023-06-12 12:50:24.058247 decoratory-0.1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14568 2023-06-12 11:38:10.000000 decoratory-0.1.0.1/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.0.1/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 12:50:23.757437 decoratory-0.1.0.1/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-12 12:50:24.011380 decoratory-0.1.0.1/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.0.1/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     5084 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     4938 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14035 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    20586 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    38553 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     7107 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    12164 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:50:24.058247 decoratory-0.1.0.1/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    16170 2023-06-12 12:50:23.000000 decoratory-0.1.0.1/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-06-12 12:50:23.000000 decoratory-0.1.0.1/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:50:23.000000 decoratory-0.1.0.1/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 12:50:23.000000 decoratory-0.1.0.1/Sources/decoratory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:50:24.058247 decoratory-0.1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3929 2023-06-12 12:49:52.000000 decoratory-0.1.0.1/setup.py
```

