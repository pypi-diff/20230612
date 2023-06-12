# Comparing `tmp/controlnet_v11_utils-0.0.5.tar.gz` & `tmp/controlnet_v11_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ivan.rodkin/lab/ControlNet-v1-1-nightly/dist/.tmp-bjo7znqx/controlnet_v11_utils-0.0.5.tar", last modified: Mon Jun 12 19:00:14 2023, max compression
+gzip compressed data, was "/home/ivan.rodkin/lab/ControlNet-v1-1-nightly/dist/.tmp-sxlhrxtc/controlnet_v11_utils-0.0.6.tar", last modified: Mon Jun 12 19:12:40 2023, max compression
```

## Comparing `controlnet_v11_utils-0.0.5.tar` & `controlnet_v11_utils-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,16 @@
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:00:14.323769 controlnet_v11_utils-0.0.5/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 19:00:14.323769 controlnet_v11_utils-0.0.5/PKG-INFO
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:00:14.313769 controlnet_v11_utils-0.0.5/controlnet/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 18:59:21.000000 controlnet_v11_utils-0.0.5/controlnet/__init__.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       20 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.5/controlnet/config.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    13462 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_annotator.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5599 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_canny.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5466 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_depth.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     6022 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_inpaint.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4710 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_ip2p.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5335 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_lineart.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5364 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_lineart_anime.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5647 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_mlsd.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5311 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_normalbae.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5348 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_openpose.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5720 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_scribble.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5313 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_scribble_interactive.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5722 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_seg.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     4696 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_shuffle.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5617 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_softedge.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)     5249 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/gradio_tile.py
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      155 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.5/controlnet/share.py
-drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:00:14.323769 controlnet_v11_utils-0.0.5/controlnet_v11_utils.egg-info/
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 19:00:14.000000 controlnet_v11_utils-0.0.5/controlnet_v11_utils.egg-info/PKG-INFO
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      721 2023-06-12 19:00:14.000000 controlnet_v11_utils-0.0.5/controlnet_v11_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 19:00:14.000000 controlnet_v11_utils-0.0.5/controlnet_v11_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       11 2023-06-12 19:00:14.000000 controlnet_v11_utils-0.0.5/controlnet_v11_utils.egg-info/top_level.txt
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       38 2023-06-12 19:00:14.323769 controlnet_v11_utils-0.0.5/setup.cfg
--rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      174 2023-06-12 19:00:04.000000 controlnet_v11_utils-0.0.5/setup.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:12:40.888288 controlnet_v11_utils-0.0.6/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 19:12:40.888288 controlnet_v11_utils-0.0.6/PKG-INFO
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)    31985 2023-06-12 10:51:30.000000 controlnet_v11_utils-0.0.6/README.md
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:12:40.888288 controlnet_v11_utils-0.0.6/config/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       20 2023-06-12 19:10:48.000000 controlnet_v11_utils-0.0.6/config/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       20 2023-06-12 10:51:31.000000 controlnet_v11_utils-0.0.6/config/config.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:12:40.888288 controlnet_v11_utils-0.0.6/controlnet_v11_utils.egg-info/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       64 2023-06-12 19:12:40.000000 controlnet_v11_utils-0.0.6/controlnet_v11_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      263 2023-06-12 19:12:40.000000 controlnet_v11_utils-0.0.6/controlnet_v11_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)        1 2023-06-12 19:12:40.000000 controlnet_v11_utils-0.0.6/controlnet_v11_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       13 2023-06-12 19:12:40.000000 controlnet_v11_utils-0.0.6/controlnet_v11_utils.egg-info/top_level.txt
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       38 2023-06-12 19:12:40.888288 controlnet_v11_utils-0.0.6/setup.cfg
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      149 2023-06-12 19:12:01.000000 controlnet_v11_utils-0.0.6/setup.py
+drwxr-xr-x   0 ivan.rodkin  (2075) students  (2002)        0 2023-06-12 19:12:40.888288 controlnet_v11_utils-0.0.6/share/
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)       18 2023-06-12 19:10:32.000000 controlnet_v11_utils-0.0.6/share/__init__.py
+-rw-r--r--   0 ivan.rodkin  (2075) students  (2002)      155 2023-06-12 10:51:32.000000 controlnet_v11_utils-0.0.6/share/share.py
```

