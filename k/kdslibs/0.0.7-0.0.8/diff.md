# Comparing `tmp/kdslibs-0.0.7.tar.gz` & `tmp/kdslibs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdslibs-0.0.7.tar", last modified: Sun Jun 11 14:07:25 2023, max compression
+gzip compressed data, was "kdslibs-0.0.8.tar", last modified: Mon Jun 12 16:25:55 2023, max compression
```

## Comparing `kdslibs-0.0.7.tar` & `kdslibs-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-11 14:07:25.052380 kdslibs-0.0.7/
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.7/LICENSE
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-11 14:07:25.052380 kdslibs-0.0.7/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.7/README.md
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-11 14:07:25.042380 kdslibs-0.0.7/kdslibs/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      701 2023-06-10 16:58:59.000000 kdslibs-0.0.7/kdslibs/__init__.py
-drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-11 14:07:25.042380 kdslibs-0.0.7/kdslibs.egg-info/
--rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-11 14:07:25.000000 kdslibs-0.0.7/kdslibs.egg-info/PKG-INFO
--rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-11 14:07:25.000000 kdslibs-0.0.7/kdslibs.egg-info/SOURCES.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-11 14:07:25.000000 kdslibs-0.0.7/kdslibs.egg-info/dependency_links.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-11 14:07:25.000000 kdslibs-0.0.7/kdslibs.egg-info/top_level.txt
--rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-11 14:07:25.052380 kdslibs-0.0.7/setup.cfg
--rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-11 14:07:21.000000 kdslibs-0.0.7/setup.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-12 16:25:55.941564 kdslibs-0.0.8/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:38:45.000000 kdslibs-0.0.8/LICENSE
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-12 16:25:55.941564 kdslibs-0.0.8/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        0 2023-06-10 08:39:00.000000 kdslibs-0.0.8/README.md
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-12 16:25:55.941564 kdslibs-0.0.8/kdslibs/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)     1531 2023-06-12 16:20:05.000000 kdslibs-0.0.8/kdslibs/__init__.py
+drwxr-xr-x   0 diwa      (1000) diwa      (1000)        0 2023-06-12 16:25:55.941564 kdslibs-0.0.8/kdslibs.egg-info/
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      298 2023-06-12 16:25:55.000000 kdslibs-0.0.8/kdslibs.egg-info/PKG-INFO
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      170 2023-06-12 16:25:55.000000 kdslibs-0.0.8/kdslibs.egg-info/SOURCES.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        1 2023-06-12 16:25:55.000000 kdslibs-0.0.8/kdslibs.egg-info/dependency_links.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)        8 2023-06-12 16:25:55.000000 kdslibs-0.0.8/kdslibs.egg-info/top_level.txt
+-rw-r--r--   0 diwa      (1000) diwa      (1000)       38 2023-06-12 16:25:55.941564 kdslibs-0.0.8/setup.cfg
+-rw-r--r--   0 diwa      (1000) diwa      (1000)      432 2023-06-12 16:25:49.000000 kdslibs-0.0.8/setup.py
```

