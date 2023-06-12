# Comparing `tmp/torchbricks-0.0.4.tar.gz` & `tmp/torchbricks-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbricks-0.0.4.tar", last modified: Tue Jun  6 23:00:59 2023, max compression
+gzip compressed data, was "torchbricks-0.0.5.tar", last modified: Mon Jun 12 20:14:19 2023, max compression
```

## Comparing `torchbricks-0.0.4.tar` & `torchbricks-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.260885 torchbricks-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-06 23:00:40.000000 torchbricks-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-06 23:00:40.000000 torchbricks-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-06 23:00:59.260885 torchbricks-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-06 23:00:40.000000 torchbricks-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-06 23:00:40.000000 torchbricks-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:00:59.260885 torchbricks-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.256885 torchbricks-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.260885 torchbricks-0.0.4/src/torchbricks/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 23:00:40.000000 torchbricks-0.0.4/src/torchbricks/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 23:00:40.000000 torchbricks-0.0.4/src/torchbricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-06-06 23:00:40.000000 torchbricks-0.0.4/src/torchbricks/bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 23:00:40.000000 torchbricks-0.0.4/src/torchbricks/custom_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.260885 torchbricks-0.0.4/src/torchbricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 23:00:59.000000 torchbricks-0.0.4/src/torchbricks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:00:59.260885 torchbricks-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-06 23:00:40.000000 torchbricks-0.0.4/tests/test_bricks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:14:19.032652 torchbricks-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 20:14:04.000000 torchbricks-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-12 20:14:04.000000 torchbricks-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-06-12 20:14:19.032652 torchbricks-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-12 20:14:04.000000 torchbricks-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-12 20:14:04.000000 torchbricks-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:14:19.032652 torchbricks-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:14:19.032652 torchbricks-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:14:19.032652 torchbricks-0.0.5/src/torchbricks/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 20:14:04.000000 torchbricks-0.0.5/src/torchbricks/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 20:14:04.000000 torchbricks-0.0.5/src/torchbricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-06-12 20:14:04.000000 torchbricks-0.0.5/src/torchbricks/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 20:14:04.000000 torchbricks-0.0.5/src/torchbricks/custom_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:14:19.032652 torchbricks-0.0.5/src/torchbricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-06-12 20:14:19.000000 torchbricks-0.0.5/src/torchbricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-12 20:14:19.000000 torchbricks-0.0.5/src/torchbricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:14:19.000000 torchbricks-0.0.5/src/torchbricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 20:14:19.000000 torchbricks-0.0.5/src/torchbricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 20:14:19.000000 torchbricks-0.0.5/src/torchbricks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:14:19.032652 torchbricks-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-12 20:14:04.000000 torchbricks-0.0.5/tests/test_bricks.py
```

### Comparing `torchbricks-0.0.4/LICENSE` & `torchbricks-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.4/pyproject.toml` & `torchbricks-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.ruff]
 line-length = 140
 
 [project]
 name = "torchbricks"
-version = "0.0.4"
+version = "0.0.5"
 description = "Decoupled and modular approach to building multi-task ML models"
 readme = "README.md"
 authors = [{ name = "Peter Hviid Christianse", email = "PeterHviidChristiansen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,15 +23,15 @@
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/PeteHeine/torchbricks"
 
 # bumpver update --patch | --minor | --major --dry
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.0.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]  # Specify all files containging version-numbers
```

### Comparing `torchbricks-0.0.4/src/torchbricks/bricks.py` & `torchbricks-0.0.5/src/torchbricks/bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.4/src/torchbricks/custom_metrics.py` & `torchbricks-0.0.5/src/torchbricks/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.4/tests/test_bricks.py` & `torchbricks-0.0.5/tests/test_bricks.py`

 * *Files identical despite different names*

