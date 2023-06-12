# Comparing `tmp/colorpie-0.0.1.tar.gz` & `tmp/colorpie-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorpie-0.0.1.tar", last modified: Sun Oct 23 18:20:27 2022, max compression
+gzip compressed data, was "colorpie-1.0.0.tar", last modified: Mon Jun 12 20:20:52 2023, max compression
```

## Comparing `colorpie-0.0.1.tar` & `colorpie-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-10-23 18:20:27.503653 colorpie-0.0.1/
--rw-rw-rw-   0        0        0     1090 2022-10-20 09:59:32.000000 colorpie-0.0.1/LICENSE
--rw-rw-rw-   0        0        0        0 2022-08-01 15:43:54.000000 colorpie-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1820 2022-10-23 18:20:27.503653 colorpie-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2022-10-23 18:13:29.000000 colorpie-0.0.1/README.md
--rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 colorpie-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      966 2022-10-23 18:20:27.513630 colorpie-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-23 18:20:27.473326 colorpie-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2022-10-23 18:20:27.492738 colorpie-0.0.1/src/colorpie/
--rw-rw-rw-   0        0        0      111 2022-10-23 18:10:00.000000 colorpie-0.0.1/src/colorpie/__init__.py
--rw-rw-rw-   0        0        0     1132 2022-10-21 10:39:24.000000 colorpie-0.0.1/src/colorpie/constants.py
--rw-rw-rw-   0        0        0     3707 2022-10-20 19:59:05.000000 colorpie-0.0.1/src/colorpie/core.py
--rw-rw-rw-   0        0        0     6901 2022-10-23 18:10:00.000000 colorpie-0.0.1/src/colorpie/handlers.py
--rw-rw-rw-   0        0        0    33851 2022-10-23 18:16:23.000000 colorpie-0.0.1/src/colorpie/mapping.py
--rw-rw-rw-   0        0        0      509 2022-10-20 18:31:10.000000 colorpie-0.0.1/src/colorpie/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-23 18:20:27.503653 colorpie-0.0.1/src/colorpie.egg-info/
--rw-rw-rw-   0        0        0     1820 2022-10-23 18:20:27.000000 colorpie-0.0.1/src/colorpie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2022-10-23 18:20:27.000000 colorpie-0.0.1/src/colorpie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-23 18:20:27.000000 colorpie-0.0.1/src/colorpie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-23 18:20:27.000000 colorpie-0.0.1/src/colorpie.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2022-10-23 18:20:27.000000 colorpie-0.0.1/src/colorpie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 20:20:52.843631 colorpie-1.0.0/
+-rw-rw-rw-   0        0        0     1090 2022-10-20 09:59:32.000000 colorpie-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-04 21:46:54.000000 colorpie-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1254 2023-06-12 20:20:52.843631 colorpie-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-06-12 19:57:30.000000 colorpie-1.0.0/README.md
+-rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 colorpie-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      966 2023-06-12 20:20:52.844563 colorpie-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 20:20:52.829340 colorpie-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 20:20:52.838844 colorpie-1.0.0/src/colorpie/
+-rw-rw-rw-   0        0        0      248 2023-06-12 19:35:36.000000 colorpie-1.0.0/src/colorpie/__init__.py
+-rw-rw-rw-   0        0        0     1337 2023-06-12 19:35:36.000000 colorpie-1.0.0/src/colorpie/constants.py
+-rw-rw-rw-   0        0        0     4414 2023-06-12 20:09:01.000000 colorpie-1.0.0/src/colorpie/handlers.py
+-rw-rw-rw-   0        0        0      918 2023-06-12 17:08:54.000000 colorpie-1.0.0/src/colorpie/mapping.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:20:52.842809 colorpie-1.0.0/src/colorpie.egg-info/
+-rw-rw-rw-   0        0        0     1254 2023-06-12 20:20:52.000000 colorpie-1.0.0/src/colorpie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-06-12 20:20:52.000000 colorpie-1.0.0/src/colorpie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 20:20:52.000000 colorpie-1.0.0/src/colorpie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-23 18:20:27.000000 colorpie-1.0.0/src/colorpie.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-12 20:20:52.000000 colorpie-1.0.0/src/colorpie.egg-info/top_level.txt
```

### Comparing `colorpie-0.0.1/LICENSE` & `colorpie-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `colorpie-0.0.1/setup.cfg` & `colorpie-1.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6c 6f72 7069 650d 0a76 6572   = colorpie..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e31 0d0a 6175  sion = 0.0.1..au
+00000020: 7369 6f6e 203d 2031 2e30 2e30 0d0a 6175  sion = 1.0.0..au
 00000030: 7468 6f72 203d 2043 6c61 7564 6975 2044  thor = Claudiu D
 00000040: 5255 470d 0a61 7574 686f 725f 656d 6169  RUG..author_emai
 00000050: 6c20 3d20 636c 6175 6469 752e 6472 7567  l = claudiu.drug
 00000060: 406f 7574 6c6f 6f6b 2e63 6f6d 0d0a 6c69  @outlook.com..li
 00000070: 6365 6e73 6520 3d20 4d49 5420 4c69 6365  cense = MIT Lice
 00000080: 6e73 650d 0a64 6573 6372 6970 7469 6f6e  nse..description
 00000090: 203d 2054 6572 6d69 6e61 6c20 636f 6c6f   = Terminal colo
```

