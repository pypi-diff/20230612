# Comparing `tmp/torchbones-1.2.2.tar.gz` & `tmp/torchbones-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.2.2.tar", last modified: Fri Jun  9 16:50:44 2023, max compression
+gzip compressed data, was "torchbones-1.2.3.tar", last modified: Mon Jun 12 20:55:02 2023, max compression
```

## Comparing `torchbones-1.2.2.tar` & `torchbones-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-09 16:50:44.754741 torchbones-1.2.2/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-09 16:50:44.754741 torchbones-1.2.2/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-09 16:50:44.754741 torchbones-1.2.2/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-09 16:50:01.000000 torchbones-1.2.2/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-09 16:50:44.754741 torchbones-1.2.2/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.2/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    17154 2023-06-09 16:49:56.000000 torchbones-1.2.2/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-09 16:50:44.754741 torchbones-1.2.2/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-09 16:50:44.000000 torchbones-1.2.2/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-09 16:50:44.000000 torchbones-1.2.2/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-09 16:50:44.000000 torchbones-1.2.2/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-09 16:50:44.000000 torchbones-1.2.2/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-09 16:50:44.000000 torchbones-1.2.2/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:55:02.024489 torchbones-1.2.3/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-12 20:55:02.024489 torchbones-1.2.3/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-12 20:55:02.024489 torchbones-1.2.3/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-12 20:54:38.000000 torchbones-1.2.3/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:55:02.014489 torchbones-1.2.3/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.3/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    17154 2023-06-09 16:49:56.000000 torchbones-1.2.3/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:55:02.024489 torchbones-1.2.3/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-12 20:55:01.000000 torchbones-1.2.3/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.2.2/torchbones/main.py` & `torchbones-1.2.3/torchbones/main.py`

 * *Files identical despite different names*

