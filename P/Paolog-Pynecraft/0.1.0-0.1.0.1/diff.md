# Comparing `tmp/Paolog_Pynecraft-0.1.0.tar.gz` & `tmp/Paolog_Pynecraft-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Paolog_Pynecraft-0.1.0.tar", last modified: Mon Jun 12 17:57:28 2023, max compression
+gzip compressed data, was "Paolog_Pynecraft-0.1.0.1.tar", last modified: Mon Jun 12 18:15:40 2023, max compression
```

## Comparing `Paolog_Pynecraft-0.1.0.tar` & `Paolog_Pynecraft-0.1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 17:57:28.834905 Paolog_Pynecraft-0.1.0/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:55:45.000000 Paolog_Pynecraft-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      133 2023-06-12 17:57:28.834905 Paolog_Pynecraft-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 17:57:28.824258 Paolog_Pynecraft-0.1.0/Paolog_Pynecraft/
--rw-rw-rw-   0        0        0    12040 2023-04-16 13:49:22.000000 Paolog_Pynecraft-0.1.0/Paolog_Pynecraft/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:57:28.831713 Paolog_Pynecraft-0.1.0/Paolog_Pynecraft.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-12 17:57:28.000000 Paolog_Pynecraft-0.1.0/Paolog_Pynecraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-06-12 17:57:28.000000 Paolog_Pynecraft-0.1.0/Paolog_Pynecraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 17:57:28.000000 Paolog_Pynecraft-0.1.0/Paolog_Pynecraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 17:57:28.000000 Paolog_Pynecraft-0.1.0/Paolog_Pynecraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2023-06-12 17:57:03.000000 Paolog_Pynecraft-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 17:57:28.834905 Paolog_Pynecraft-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      172 2023-06-12 17:46:10.000000 Paolog_Pynecraft-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:15:40.454843 Paolog_Pynecraft-0.1.0.1/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:55:45.000000 Paolog_Pynecraft-0.1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      135 2023-06-12 18:15:40.453745 Paolog_Pynecraft-0.1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 18:15:40.445609 Paolog_Pynecraft-0.1.0.1/Paolog_Pynecraft/
+-rw-rw-rw-   0        0        0    12040 2023-04-16 13:49:22.000000 Paolog_Pynecraft-0.1.0.1/Paolog_Pynecraft/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:15:40.451562 Paolog_Pynecraft-0.1.0.1/Paolog_Pynecraft.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-06-12 18:15:40.000000 Paolog_Pynecraft-0.1.0.1/Paolog_Pynecraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-06-12 18:15:40.000000 Paolog_Pynecraft-0.1.0.1/Paolog_Pynecraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:15:40.000000 Paolog_Pynecraft-0.1.0.1/Paolog_Pynecraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-12 18:15:40.000000 Paolog_Pynecraft-0.1.0.1/Paolog_Pynecraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       87 2023-06-12 17:57:03.000000 Paolog_Pynecraft-0.1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 18:15:40.454843 Paolog_Pynecraft-0.1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      174 2023-06-12 18:15:36.000000 Paolog_Pynecraft-0.1.0.1/setup.py
```

### Comparing `Paolog_Pynecraft-0.1.0/Paolog_Pynecraft/__init__.py` & `Paolog_Pynecraft-0.1.0.1/Paolog_Pynecraft/__init__.py`

 * *Files identical despite different names*

