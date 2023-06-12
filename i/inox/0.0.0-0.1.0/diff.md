# Comparing `tmp/inox-0.0.0.tar.gz` & `tmp/inox-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inox-0.0.0.tar", last modified: Fri May 26 15:40:11 2023, max compression
+gzip compressed data, was "inox-0.1.0.tar", last modified: Mon Jun 12 11:45:27 2023, max compression
```

## Comparing `inox-0.0.0.tar` & `inox-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-05-26 15:40:11.682954 inox-0.0.0/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2023-05-26 14:59:48.000000 inox-0.0.0/LICENSE
--rw-rw-r--   0 francois  (1001) francois  (1001)      599 2023-05-26 15:40:11.682954 inox-0.0.0/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)       35 2023-05-26 14:23:59.000000 inox-0.0.0/README.md
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-05-26 15:40:11.682954 inox-0.0.0/inox/
--rw-rw-r--   0 francois  (1001) francois  (1001)      105 2023-05-26 14:59:48.000000 inox-0.0.0/inox/__init__.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-05-26 15:40:11.682954 inox-0.0.0/inox/nn/
--rw-rw-r--   0 francois  (1001) francois  (1001)       86 2023-05-26 14:59:48.000000 inox-0.0.0/inox/nn/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     3780 2023-05-26 14:33:16.000000 inox-0.0.0/inox/nn/base.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     1421 2023-05-26 14:59:48.000000 inox-0.0.0/inox/nn/layers.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     1565 2023-05-26 14:28:18.000000 inox-0.0.0/inox/tree_util.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-05-26 15:40:11.682954 inox-0.0.0/inox.egg-info/
--rw-rw-r--   0 francois  (1001) francois  (1001)      599 2023-05-26 15:40:11.000000 inox-0.0.0/inox.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)      264 2023-05-26 15:40:11.000000 inox-0.0.0/inox.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-05-26 15:40:11.000000 inox-0.0.0/inox.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)       12 2023-05-26 15:40:11.000000 inox-0.0.0/inox.egg-info/requires.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-05-26 15:40:11.000000 inox-0.0.0/inox.egg-info/top_level.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)      666 2023-05-26 15:40:11.686955 inox-0.0.0/setup.cfg
--rw-rw-r--   0 francois  (1001) francois  (1001)       72 2023-05-26 14:59:48.000000 inox-0.0.0/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-12 11:45:27.110046 inox-0.1.0/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2023-06-12 11:10:49.000000 inox-0.1.0/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2915 2023-06-12 11:45:27.110046 inox-0.1.0/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2351 2023-06-12 11:10:49.000000 inox-0.1.0/README.md
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-12 11:45:27.110046 inox-0.1.0/inox/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      126 2023-06-12 11:43:51.000000 inox-0.1.0/inox/__init__.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-12 11:45:27.110046 inox-0.1.0/inox/nn/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      236 2023-06-12 11:10:49.000000 inox-0.1.0/inox/nn/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5541 2023-06-07 15:59:20.000000 inox-0.1.0/inox/nn/activation.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)      981 2023-06-07 15:59:20.000000 inox-0.1.0/inox/nn/container.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1526 2023-06-12 11:10:49.000000 inox-0.1.0/inox/nn/dropout.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1677 2023-06-12 11:10:49.000000 inox-0.1.0/inox/nn/einops.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     8467 2023-06-07 15:59:20.000000 inox-0.1.0/inox/nn/linear.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     6479 2023-06-12 11:10:49.000000 inox-0.1.0/inox/nn/module.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3331 2023-06-12 11:10:49.000000 inox-0.1.0/inox/nn/normalization.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3504 2023-06-12 11:10:49.000000 inox-0.1.0/inox/nn/pooling.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1943 2023-06-12 11:10:49.000000 inox-0.1.0/inox/random.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     8013 2023-06-12 11:10:49.000000 inox-0.1.0/inox/tree_util.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-12 11:45:27.110046 inox-0.1.0/inox.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2915 2023-06-12 11:45:27.000000 inox-0.1.0/inox.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)      422 2023-06-12 11:45:27.000000 inox-0.1.0/inox.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-06-12 11:45:27.000000 inox-0.1.0/inox.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       26 2023-06-12 11:45:27.000000 inox-0.1.0/inox.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-06-12 11:45:27.000000 inox-0.1.0/inox.egg-info/top_level.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       26 2023-06-12 11:10:49.000000 inox-0.1.0/requirements.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)      666 2023-06-12 11:45:27.110046 inox-0.1.0/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1001)       72 2023-05-26 14:59:48.000000 inox-0.1.0/setup.py
```

### Comparing `inox-0.0.0/LICENSE` & `inox-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inox-0.0.0/setup.cfg` & `inox-0.1.0/setup.cfg`

 * *Files identical despite different names*

