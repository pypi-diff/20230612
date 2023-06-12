# Comparing `tmp/advancedselector-2.1.0.tar.gz` & `tmp/advancedselector-2.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advancedselector-2.1.0.tar", last modified: Mon Jun 12 20:14:52 2023, max compression
+gzip compressed data, was "advancedselector-2.1.0.1.tar", last modified: Mon Jun 12 20:39:07 2023, max compression
```

## Comparing `advancedselector-2.1.0.tar` & `advancedselector-2.1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 20:14:52.693434 advancedselector-2.1.0/
--rw-rw-rw-   0        0        0     1092 2023-06-12 14:16:20.000000 advancedselector-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     1787 2023-06-12 20:14:52.693434 advancedselector-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-06-12 14:16:20.000000 advancedselector-2.1.0/README.md
--rw-rw-rw-   0        0        0       82 2023-06-12 20:11:41.000000 advancedselector-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      989 2023-06-12 20:14:52.694433 advancedselector-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 20:14:52.673298 advancedselector-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 20:14:52.691426 advancedselector-2.1.0/src/advancedselector.egg-info/
--rw-rw-rw-   0        0        0     1787 2023-06-12 20:14:52.000000 advancedselector-2.1.0/src/advancedselector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-06-12 20:14:52.000000 advancedselector-2.1.0/src/advancedselector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 20:14:52.000000 advancedselector-2.1.0/src/advancedselector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-12 20:14:52.000000 advancedselector-2.1.0/src/advancedselector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-06-12 20:14:52.000000 advancedselector-2.1.0/src/advancedselector.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 20:14:52.000000 advancedselector-2.1.0/src/advancedselector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-12 20:14:03.000000 advancedselector-2.1.0/src/advancedselector.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-06-12 20:14:52.692434 advancedselector-2.1.0/tests/
--rw-rw-rw-   0        0        0      179 2023-06-12 14:46:12.000000 advancedselector-2.1.0/tests/test_colors.py
--rw-rw-rw-   0        0        0      193 2023-06-12 14:43:59.000000 advancedselector-2.1.0/tests/test_picker.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:39:07.880250 advancedselector-2.1.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-06-12 14:16:20.000000 advancedselector-2.1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      632 2023-06-12 20:39:07.879637 advancedselector-2.1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-06-12 14:16:20.000000 advancedselector-2.1.0.1/README.md
+-rw-rw-rw-   0        0        0      719 2023-06-12 20:38:53.000000 advancedselector-2.1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 20:39:07.880250 advancedselector-2.1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 20:39:07.861637 advancedselector-2.1.0.1/src/
+-rw-rw-rw-   0        0        0      532 2023-06-12 20:31:07.000000 advancedselector-2.1.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:39:07.876634 advancedselector-2.1.0.1/src/advancedselector.egg-info/
+-rw-rw-rw-   0        0        0      632 2023-06-12 20:39:07.000000 advancedselector-2.1.0.1/src/advancedselector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-06-12 20:39:07.000000 advancedselector-2.1.0.1/src/advancedselector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 20:39:07.000000 advancedselector-2.1.0.1/src/advancedselector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-12 20:39:07.000000 advancedselector-2.1.0.1/src/advancedselector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-12 20:39:07.000000 advancedselector-2.1.0.1/src/advancedselector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      902 2023-06-12 14:41:03.000000 advancedselector-2.1.0.1/src/colors.py
+-rw-rw-rw-   0        0        0     6026 2023-06-12 20:30:17.000000 advancedselector-2.1.0.1/src/picker.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:39:07.878639 advancedselector-2.1.0.1/tests/
+-rw-rw-rw-   0        0        0      179 2023-06-12 14:46:12.000000 advancedselector-2.1.0.1/tests/test_colors.py
+-rw-rw-rw-   0        0        0      193 2023-06-12 14:43:59.000000 advancedselector-2.1.0.1/tests/test_picker.py
```

### Comparing `advancedselector-2.1.0/LICENSE` & `advancedselector-2.1.0.1/LICENSE`

 * *Files identical despite different names*

