# Comparing `tmp/gh_subdir-0.1.1.tar.gz` & `tmp/gh_subdir-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_subdir-0.1.1.tar", last modified: Mon Jun 12 06:25:16 2023, max compression
+gzip compressed data, was "gh_subdir-0.1.2.tar", last modified: Mon Jun 12 06:28:02 2023, max compression
```

## Comparing `gh_subdir-0.1.1.tar` & `gh_subdir-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.961028 gh_subdir-0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-06-12 04:39:33.000000 gh_subdir-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      264 2023-06-12 06:25:16.961028 gh_subdir-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      887 2023-06-12 06:08:12.000000 gh_subdir-0.1.1/README.md
--rw-rw-rw-   0        0        0      111 2023-06-12 06:25:16.963032 gh_subdir-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      453 2023-06-12 06:25:06.000000 gh_subdir-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.917416 gh_subdir-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.959037 gh_subdir-0.1.1/src/gh_subdir.egg-info/
--rw-rw-rw-   0        0        0      264 2023-06-12 06:25:16.000000 gh_subdir-0.1.1/src/gh_subdir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-06-12 06:25:16.000000 gh_subdir-0.1.1/src/gh_subdir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:25:16.000000 gh_subdir-0.1.1/src/gh_subdir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-12 06:25:16.000000 gh_subdir-0.1.1/src/gh_subdir.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:25:16.000000 gh_subdir-0.1.1/src/gh_subdir.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 06:28:02.219103 gh_subdir-0.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-12 04:39:33.000000 gh_subdir-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      264 2023-06-12 06:28:02.219103 gh_subdir-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2023-06-12 06:08:12.000000 gh_subdir-0.1.2/README.md
+-rw-rw-rw-   0        0        0      111 2023-06-12 06:28:02.222104 gh_subdir-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      412 2023-06-12 06:27:44.000000 gh_subdir-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:28:02.184580 gh_subdir-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 06:28:02.217259 gh_subdir-0.1.2/src/gh_subdir.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-06-12 06:28:02.000000 gh_subdir-0.1.2/src/gh_subdir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-06-12 06:28:02.000000 gh_subdir-0.1.2/src/gh_subdir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:28:02.000000 gh_subdir-0.1.2/src/gh_subdir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:28:02.000000 gh_subdir-0.1.2/src/gh_subdir.egg-info/top_level.txt
```

### Comparing `gh_subdir-0.1.1/LICENSE` & `gh_subdir-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_subdir-0.1.1/README.md` & `gh_subdir-0.1.2/README.md`

 * *Files identical despite different names*

