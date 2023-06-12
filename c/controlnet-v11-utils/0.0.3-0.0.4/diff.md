# Comparing `tmp/controlnet_v11_utils-0.0.3.tar.gz` & `tmp/controlnet_v11_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ivan.rodkin/lab/ControlNet-v1-1-nightly/dist/.tmp-ewygglpz/controlnet_v11_utils-0.0.3.tar", last modified: Mon Jun 12 18:50:34 2023, max compression
+gzip compressed data, was "/home/ivan.rodkin/lab/ControlNet-v1-1-nightly/dist/.tmp-dqh3_r67/controlnet_v11_utils-0.0.4.tar", last modified: Mon Jun 12 18:54:15 2023, max compression
```

## Comparing `controlnet_v11_utils-0.0.3.tar` & `controlnet_v11_utils-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,9 @@
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 18:50:34.510259 controlnet_v11_utils-0.0.3/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 18:50:34.510259 controlnet_v11_utils-0.0.3/PKG-INFO
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    31985 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.3/README.md
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 18:50:34.510259 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 18:50:34.000000 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/PKG-INFO
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      194 2023-06-12 18:50:34.000000 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 18:50:34.000000 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 18:50:34.000000 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/top_level.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       38 2023-06-12 18:50:34.510259 controlnet_v11_utils-0.0.3/setup.cfg
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      149 2023-06-12 18:50:16.000000 controlnet_v11_utils-0.0.3/setup.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 18:54:15.291596 controlnet_v11_utils-0.0.4/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 18:54:15.291596 controlnet_v11_utils-0.0.4/PKG-INFO
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 18:54:15.291596 controlnet_v11_utils-0.0.4/controlnet_v11_utils.egg-info/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 18:54:15.000000 controlnet_v11_utils-0.0.4/controlnet_v11_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      184 2023-06-12 18:54:15.000000 controlnet_v11_utils-0.0.4/controlnet_v11_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 18:54:15.000000 controlnet_v11_utils-0.0.4/controlnet_v11_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 18:54:15.000000 controlnet_v11_utils-0.0.4/controlnet_v11_utils.egg-info/top_level.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       38 2023-06-12 18:54:15.291596 controlnet_v11_utils-0.0.4/setup.cfg
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      174 2023-06-12 18:53:48.000000 controlnet_v11_utils-0.0.4/setup.py
```

