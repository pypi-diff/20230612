# Comparing `tmp/pretix-plugin-build-1.0.0.tar.gz` & `tmp/pretix-plugin-build-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-plugin-build-1.0.0.tar", last modified: Thu Apr 27 16:18:08 2023, max compression
+gzip compressed data, was "pretix-plugin-build-1.0.1.tar", last modified: Mon Jun 12 07:37:58 2023, max compression
```

## Comparing `pretix-plugin-build-1.0.0.tar` & `pretix-plugin-build-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-27 16:18:08.587052 pretix-plugin-build-1.0.0/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      511 2023-04-27 16:18:08.587052 pretix-plugin-build-1.0.0/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)       84 2023-04-27 15:40:39.000000 pretix-plugin-build-1.0.0/README.rst
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-27 16:18:08.583718 pretix-plugin-build-1.0.0/pretix_plugin_build/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2023-04-27 15:36:12.000000 pretix-plugin-build-1.0.0/pretix_plugin_build/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      297 2023-04-27 15:40:39.000000 pretix-plugin-build-1.0.0/pretix_plugin_build/build.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-27 16:18:08.587052 pretix-plugin-build-1.0.0/pretix_plugin_build.egg-info/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      511 2023-04-27 16:18:08.000000 pretix-plugin-build-1.0.0/pretix_plugin_build.egg-info/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)      309 2023-04-27 16:18:08.000000 pretix-plugin-build-1.0.0/pretix_plugin_build.egg-info/SOURCES.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-04-27 16:18:08.000000 pretix-plugin-build-1.0.0/pretix_plugin_build.egg-info/dependency_links.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        7 2023-04-27 16:18:08.000000 pretix-plugin-build-1.0.0/pretix_plugin_build.egg-info/requires.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       20 2023-04-27 16:18:08.000000 pretix-plugin-build-1.0.0/pretix_plugin_build.egg-info/top_level.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)      594 2023-04-27 15:40:39.000000 pretix-plugin-build-1.0.0/pyproject.toml
--rw-r--r--   0 raphael   (1000) raphael   (1000)       38 2023-04-27 16:18:08.587052 pretix-plugin-build-1.0.0/setup.cfg
--rw-r--r--   0 raphael   (1000) raphael   (1000)       38 2023-04-27 15:37:14.000000 pretix-plugin-build-1.0.0/setup.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-06-12 07:37:58.960677 pretix-plugin-build-1.0.1/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      511 2023-06-12 07:37:58.960677 pretix-plugin-build-1.0.1/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       84 2023-06-12 07:24:39.000000 pretix-plugin-build-1.0.1/README.rst
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-06-12 07:37:58.960677 pretix-plugin-build-1.0.1/pretix_plugin_build/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2023-06-12 07:24:39.000000 pretix-plugin-build-1.0.1/pretix_plugin_build/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      571 2023-06-12 07:36:08.000000 pretix-plugin-build-1.0.1/pretix_plugin_build/build.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-06-12 07:37:58.960677 pretix-plugin-build-1.0.1/pretix_plugin_build.egg-info/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      511 2023-06-12 07:37:58.000000 pretix-plugin-build-1.0.1/pretix_plugin_build.egg-info/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      309 2023-06-12 07:37:58.000000 pretix-plugin-build-1.0.1/pretix_plugin_build.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-06-12 07:37:58.000000 pretix-plugin-build-1.0.1/pretix_plugin_build.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        7 2023-06-12 07:37:58.000000 pretix-plugin-build-1.0.1/pretix_plugin_build.egg-info/requires.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       20 2023-06-12 07:37:58.000000 pretix-plugin-build-1.0.1/pretix_plugin_build.egg-info/top_level.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      594 2023-06-12 07:37:34.000000 pretix-plugin-build-1.0.1/pyproject.toml
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       38 2023-06-12 07:37:58.960677 pretix-plugin-build-1.0.1/setup.cfg
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       38 2023-06-12 07:24:39.000000 pretix-plugin-build-1.0.1/setup.py
```

### Comparing `pretix-plugin-build-1.0.0/pyproject.toml` & `pretix-plugin-build-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pretix-plugin-build"
-version = "1.0.0"
+version = "1.0.1"
 description = "Build toolchain for pretix plugins"
 readme = "README.rst"
 license = {text = "Apache License"}
 keywords = ["pretix"]
 authors = [
     {name = "pretix team", email = "support@pretix.eu"},
 ]
```

