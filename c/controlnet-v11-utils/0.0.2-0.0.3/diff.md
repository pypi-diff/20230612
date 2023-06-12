# Comparing `tmp/controlnet-v11-utils-0.0.2.tar.gz` & `tmp/controlnet_v11_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ivan.rodkin/lab/ControlNet-v1-1-nightly/dist/.tmp-cksnp7mp/controlnet-v11-utils-0.0.2.tar", last modified: Mon Jun 12 18:45:42 2023, max compression
+gzip compressed data, was "/home/ivan.rodkin/lab/ControlNet-v1-1-nightly/dist/.tmp-ewygglpz/controlnet_v11_utils-0.0.3.tar", last modified: Mon Jun 12 18:50:34 2023, max compression
```

## Comparing `controlnet-v11-utils-0.0.2.tar` & `controlnet_v11_utils-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 18:45:42.758493 controlnet-v11-utils-0.0.2/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 18:45:42.758493 controlnet-v11-utils-0.0.2/PKG-INFO
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    31985 2023-06-12 10:51:30.000000 controlnet-v11-utils-0.0.2/README.md
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 18:45:42.758493 controlnet-v11-utils-0.0.2/controlnet_v11_utils.egg-info/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 18:45:42.000000 controlnet-v11-utils-0.0.2/controlnet_v11_utils.egg-info/PKG-INFO
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      194 2023-06-12 18:45:42.000000 controlnet-v11-utils-0.0.2/controlnet_v11_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 18:45:42.000000 controlnet-v11-utils-0.0.2/controlnet_v11_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 18:45:42.000000 controlnet-v11-utils-0.0.2/controlnet_v11_utils.egg-info/top_level.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       38 2023-06-12 18:45:42.758493 controlnet-v11-utils-0.0.2/setup.cfg
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      149 2023-06-12 18:45:31.000000 controlnet-v11-utils-0.0.2/setup.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 18:50:34.510259 controlnet_v11_utils-0.0.3/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 18:50:34.510259 controlnet_v11_utils-0.0.3/PKG-INFO
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    31985 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.3/README.md
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 18:50:34.510259 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 18:50:34.000000 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      194 2023-06-12 18:50:34.000000 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 18:50:34.000000 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 18:50:34.000000 controlnet_v11_utils-0.0.3/controlnet_v11_utils.egg-info/top_level.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       38 2023-06-12 18:50:34.510259 controlnet_v11_utils-0.0.3/setup.cfg
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      149 2023-06-12 18:50:16.000000 controlnet_v11_utils-0.0.3/setup.py
```

### Comparing `controlnet-v11-utils-0.0.2/README.md` & `controlnet_v11_utils-0.0.3/README.md`

 * *Files identical despite different names*

