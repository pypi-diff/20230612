# Comparing `tmp/pylibx-0.1.1.tar.gz` & `tmp/pylibx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\John\Develop\workspace\pypkt\pylibx\dist\tmp2qi66wjr\pylibx-0.1.1.tar", last modified: Thu Jun 16 06:35:43 2022, max compression
+gzip compressed data, was "D:\John\Develop\workspace\pypkt\pylibx\dist\.tmp-ckggjc3g\pylibx-0.2.0.tar", last modified: Mon Jun 12 02:14:28 2023, max compression
```

## Comparing `pylibx-0.1.1.tar` & `pylibx-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-06-16 06:35:43.629943 pylibx-0.1.1/
--rw-rw-rw-   0        0        0      155 2022-06-16 06:35:43.628946 pylibx-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-06-16 06:35:43.608001 pylibx-0.1.1/pylibx/
--rw-rw-rw-   0        0        0       83 2020-12-07 11:21:47.000000 pylibx-0.1.1/pylibx/__init__.py
--rw-rw-rw-   0        0        0     2065 2022-06-16 06:31:15.000000 pylibx-0.1.1/pylibx/pidfile.py
-drwxrwxrwx   0        0        0        0 2022-06-16 06:35:43.626986 pylibx-0.1.1/pylibx.egg-info/
--rw-rw-rw-   0        0        0      155 2022-06-16 06:35:43.000000 pylibx-0.1.1/pylibx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2022-06-16 06:35:43.000000 pylibx-0.1.1/pylibx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-16 06:35:43.000000 pylibx-0.1.1/pylibx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-06-16 06:35:43.000000 pylibx-0.1.1/pylibx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-16 06:35:43.629943 pylibx-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      297 2022-06-16 06:34:07.000000 pylibx-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:14:28.362614 pylibx-0.2.0/
+-rw-rw-rw-   0        0        0     7816 2023-06-12 01:45:38.000000 pylibx-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      178 2023-06-12 02:14:28.362113 pylibx-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 02:14:28.342096 pylibx-0.2.0/pylibx/
+-rw-rw-rw-   0        0        0       83 2023-06-12 01:45:38.000000 pylibx-0.2.0/pylibx/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-06-12 01:57:03.000000 pylibx-0.2.0/pylibx/cksum.py
+-rw-rw-rw-   0        0        0      900 2023-06-12 01:54:55.000000 pylibx-0.2.0/pylibx/kv.py
+-rw-rw-rw-   0        0        0     2065 2023-06-12 01:45:38.000000 pylibx-0.2.0/pylibx/pidfile.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:14:28.360112 pylibx-0.2.0/pylibx.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-12 02:14:28.000000 pylibx-0.2.0/pylibx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-12 02:14:28.000000 pylibx-0.2.0/pylibx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 02:14:28.000000 pylibx-0.2.0/pylibx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 02:14:28.000000 pylibx-0.2.0/pylibx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 02:14:28.363114 pylibx-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      297 2023-06-12 02:00:08.000000 pylibx-0.2.0/setup.py
```

### Comparing `pylibx-0.1.1/pylibx/pidfile.py` & `pylibx-0.2.0/pylibx/pidfile.py`

 * *Files identical despite different names*

