# Comparing `tmp/sb-arch-opt-1.1.0.tar.gz` & `tmp/sb-arch-opt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sb-arch-opt-1.1.0.tar", last modified: Wed May 31 14:04:46 2023, max compression
+gzip compressed data, was "sb-arch-opt-1.1.1.tar", last modified: Mon Jun 12 13:48:21 2023, max compression
```

## Comparing `sb-arch-opt-1.1.0.tar` & `sb-arch-opt-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/sb_arch_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/design_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/design_space_explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/pareto_front.py
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22217 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/sb_arch_opt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 14:04:46.000000 sb-arch-opt-1.1.0/sb_arch_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:04:46.180679 sb-arch-opt-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-31 14:04:33.000000 sb-arch-opt-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:21.855454 sb-arch-opt-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-12 13:48:21.855454 sb-arch-opt-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:21.851454 sb-arch-opt-1.1.1/sb_arch_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/design_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/design_space_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-06-12 13:48:07.000000 sb-arch-opt-1.1.1/sb_arch_opt/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22217 2023-06-12 13:48:08.000000 sb-arch-opt-1.1.1/sb_arch_opt/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-12 13:48:08.000000 sb-arch-opt-1.1.1/sb_arch_opt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:48:21.855454 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 13:48:21.000000 sb-arch-opt-1.1.1/sb_arch_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:48:21.855454 sb-arch-opt-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-12 13:48:08.000000 sb-arch-opt-1.1.1/setup.py
```

### Comparing `sb-arch-opt-1.1.0/LICENSE` & `sb-arch-opt-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.0/sb_arch_opt/design_space.py` & `sb-arch-opt-1.1.1/sb_arch_opt/design_space.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.0/sb_arch_opt/design_space_explicit.py` & `sb-arch-opt-1.1.1/sb_arch_opt/design_space_explicit.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.0/sb_arch_opt/pareto_front.py` & `sb-arch-opt-1.1.1/sb_arch_opt/pareto_front.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.0/sb_arch_opt/problem.py` & `sb-arch-opt-1.1.1/sb_arch_opt/problem.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.0/sb_arch_opt/sampling.py` & `sb-arch-opt-1.1.1/sb_arch_opt/sampling.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.0/sb_arch_opt/util.py` & `sb-arch-opt-1.1.1/sb_arch_opt/util.py`

 * *Files identical despite different names*

### Comparing `sb-arch-opt-1.1.0/setup.py` & `sb-arch-opt-1.1.1/setup.py`

 * *Files identical despite different names*

