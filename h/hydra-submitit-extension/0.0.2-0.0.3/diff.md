# Comparing `tmp/hydra_submitit_extension-0.0.2.tar.gz` & `tmp/hydra_submitit_extension-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra_submitit_extension-0.0.2.tar", last modified: Mon Jun 12 13:50:55 2023, max compression
+gzip compressed data, was "hydra_submitit_extension-0.0.3.tar", last modified: Mon Jun 12 20:50:13 2023, max compression
```

## Comparing `hydra_submitit_extension-0.0.2.tar` & `hydra_submitit_extension-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      607 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/.coveragerc
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      566 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/.gitignore
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      530 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/.readthedocs.yml
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       83 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/AUTHORS.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      115 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/CHANGELOG.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13698 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/CONTRIBUTING.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1079 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/LICENSE.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3387 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2923 2023-06-12 13:50:26.000000 hydra_submitit_extension-0.0.2/README.md
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/docs/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1154 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/Makefile
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/docs/_static/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       18 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/_static/.gitignore
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       71 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/authors.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       73 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/changelog.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10109 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/conf.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       76 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/contributing.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      969 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/index.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       66 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/license.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       70 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/readme.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      254 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/docs/requirements.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      346 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/pyproject.toml
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1245 2023-06-12 13:50:55.752874 hydra_submitit_extension-0.0.2/setup.cfg
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      721 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/setup.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.744873 hydra_submitit_extension-0.0.2/src/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.744873 hydra_submitit_extension-0.0.2/src/hydra_plugins/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      577 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      968 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/config.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6593 2023-06-12 12:38:44.000000 hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/submitit_launcher.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/utils/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      612 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/utils/slurm_info.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/src/hydra_submitit_extension.egg-info/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3387 2023-06-12 13:50:55.000000 hydra_submitit_extension-0.0.2/src/hydra_submitit_extension.egg-info/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      982 2023-06-12 13:50:55.000000 hydra_submitit_extension-0.0.2/src/hydra_submitit_extension.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-06-12 13:50:55.000000 hydra_submitit_extension-0.0.2/src/hydra_submitit_extension.egg-info/dependency_links.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-06-12 13:13:11.000000 hydra_submitit_extension-0.0.2/src/hydra_submitit_extension.egg-info/not-zip-safe
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      120 2023-06-12 13:50:55.000000 hydra_submitit_extension-0.0.2/src/hydra_submitit_extension.egg-info/requires.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       14 2023-06-12 13:50:55.000000 hydra_submitit_extension-0.0.2/src/hydra_submitit_extension.egg-info/top_level.txt
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/tests/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/tests/conf/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      288 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.2/tests/conf/config.yaml
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 13:50:55.748874 hydra_submitit_extension-0.0.2/tests/conf/slurm/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      653 2023-06-12 12:38:44.000000 hydra_submitit_extension-0.0.2/tests/conf/slurm/cpu.yaml
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      292 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/tests/conftest.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      601 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/tests/test_skeleton.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      492 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.2/tests/test_submtit_launcher.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2851 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.2/tox.ini
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.014939 hydra_submitit_extension-0.0.3/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      607 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/.coveragerc
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      566 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/.gitignore
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      530 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/.readthedocs.yml
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       83 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/AUTHORS.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      115 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/CHANGELOG.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    13698 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/CONTRIBUTING.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1079 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/LICENSE.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3479 2023-06-12 20:50:13.014939 hydra_submitit_extension-0.0.3/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3015 2023-06-12 19:09:50.000000 hydra_submitit_extension-0.0.3/README.md
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.010939 hydra_submitit_extension-0.0.3/docs/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1154 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/Makefile
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.010939 hydra_submitit_extension-0.0.3/docs/_static/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       18 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/_static/.gitignore
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       71 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/authors.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       73 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/changelog.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    10109 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/conf.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       76 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/contributing.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      969 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/index.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       66 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/license.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       70 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/readme.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      254 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/docs/requirements.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      346 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/pyproject.toml
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1245 2023-06-12 20:50:13.014939 hydra_submitit_extension-0.0.3/setup.cfg
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      721 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/setup.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.002939 hydra_submitit_extension-0.0.3/src/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.002939 hydra_submitit_extension-0.0.3/src/hydra_plugins/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.010939 hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      577 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      968 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/config.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     6848 2023-06-12 20:49:52.000000 hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/submitit_launcher.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.010939 hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/utils/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      612 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/utils/slurm_info.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.010939 hydra_submitit_extension-0.0.3/src/hydra_submitit_extension.egg-info/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3479 2023-06-12 20:50:12.000000 hydra_submitit_extension-0.0.3/src/hydra_submitit_extension.egg-info/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      982 2023-06-12 20:50:12.000000 hydra_submitit_extension-0.0.3/src/hydra_submitit_extension.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-06-12 20:50:12.000000 hydra_submitit_extension-0.0.3/src/hydra_submitit_extension.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-06-12 13:13:11.000000 hydra_submitit_extension-0.0.3/src/hydra_submitit_extension.egg-info/not-zip-safe
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      120 2023-06-12 20:50:12.000000 hydra_submitit_extension-0.0.3/src/hydra_submitit_extension.egg-info/requires.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       14 2023-06-12 20:50:12.000000 hydra_submitit_extension-0.0.3/src/hydra_submitit_extension.egg-info/top_level.txt
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.010939 hydra_submitit_extension-0.0.3/tests/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.010939 hydra_submitit_extension-0.0.3/tests/conf/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      288 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.3/tests/conf/config.yaml
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 20:50:13.014939 hydra_submitit_extension-0.0.3/tests/conf/slurm/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      653 2023-06-12 12:38:44.000000 hydra_submitit_extension-0.0.3/tests/conf/slurm/cpu.yaml
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      292 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/tests/conftest.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      601 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/tests/test_skeleton.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      492 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.3/tests/test_submtit_launcher.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2851 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.3/tox.ini
```

### Comparing `hydra_submitit_extension-0.0.2/.coveragerc` & `hydra_submitit_extension-0.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/.gitignore` & `hydra_submitit_extension-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/.readthedocs.yml` & `hydra_submitit_extension-0.0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/CONTRIBUTING.md` & `hydra_submitit_extension-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/LICENSE.txt` & `hydra_submitit_extension-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/PKG-INFO` & `hydra_submitit_extension-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra_submitit_extension
-Version: 0.0.2
+Version: 0.0.3
 Summary: A more flexible hydra submitit launcher
 Home-page: https://github.com/caplett/hydra_submitit_extension
 Author: Stefan Geyer
 Author-email: git@caplett.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -48,16 +48,20 @@
 
 ``` bash
 pip install hydra-submitit-extension
 ```
 
 ## Quickstart
 
+```
+python main.py hydra/launcher=submitit_slurm_extended -m
+```
 
-``` yaml
+All Parameter:
+``` yaml config.yaml
 # @package hydra.launcher
 
 # No changes to Submitit Launcher plugin
 submitit_folder: ${hydra.sweep.dir}/.submitit/%j
 timeout_min: 30
 cpus_per_task: 1
 gpus_per_node: null
```

### Comparing `hydra_submitit_extension-0.0.2/README.md` & `hydra_submitit_extension-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -33,16 +33,20 @@
 
 ``` bash
 pip install hydra-submitit-extension
 ```
 
 ## Quickstart
 
+```
+python main.py hydra/launcher=submitit_slurm_extended -m
+```
 
-``` yaml
+All Parameter:
+``` yaml config.yaml
 # @package hydra.launcher
 
 # No changes to Submitit Launcher plugin
 submitit_folder: ${hydra.sweep.dir}/.submitit/%j
 timeout_min: 30
 cpus_per_task: 1
 gpus_per_node: null
```

### Comparing `hydra_submitit_extension-0.0.2/docs/Makefile` & `hydra_submitit_extension-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/docs/conf.py` & `hydra_submitit_extension-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/docs/index.md` & `hydra_submitit_extension-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/setup.cfg` & `hydra_submitit_extension-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/setup.py` & `hydra_submitit_extension-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/__init__.py` & `hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/config.py` & `hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/config.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/submitit_launcher.py` & `hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/submitit_launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved
 import logging
 import os
 import time
+import sys
 from pathlib import Path
 from typing import Any, Dict, List, Set, Optional, Sequence
 
 from hydra.core.singleton import Singleton
-from hydra.core.utils import JobReturn, filter_overrides, run_job, setup_globals
+from hydra.core.utils import JobReturn, filter_overrides, run_job, setup_globals, JobStatus
 from hydra.types import HydraContext, TaskFunction
 from omegaconf import DictConfig, OmegaConf, open_dict
 
 from hydra_plugins.hydra_submitit_launcher.submitit_launcher import SlurmLauncher
 from submitit.core.core import Job
 from hydra_plugins.hydra_submitit_extension.config import ExtendedSlurmQueueConf
 from hydra_plugins.hydra_submitit_extension.utils.slurm_info import QueueInfo
@@ -173,15 +174,18 @@
                             all_jobs.append(executor.submit(self, *jp))
                             log.info(f"\t#{jp[2]} : Scheduled")
                 else:
                     break
 
             for i in set(all_jobs) - finished_jobs: 
                 if i.state not in self.ACTIVE_JOB_STATES:
-                    i.results()
+                    result = i.result()
+                    if result.status != JobStatus.COMPLETED:
+                        sys.stderr.write(f"Error executing job with overrides: {result.overrides}" + os.linesep)
+                        raise result._return_value
                     finished_jobs.add(i)
 
             time.sleep(params["reschedule_interval"])
 
         return [j.results()[0] for j in all_jobs]
```

### Comparing `hydra_submitit_extension-0.0.2/src/hydra_plugins/hydra_submitit_extension/utils/slurm_info.py` & `hydra_submitit_extension-0.0.3/src/hydra_plugins/hydra_submitit_extension/utils/slurm_info.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/src/hydra_submitit_extension.egg-info/PKG-INFO` & `hydra_submitit_extension-0.0.3/src/hydra_submitit_extension.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-submitit-extension
-Version: 0.0.2
+Version: 0.0.3
 Summary: A more flexible hydra submitit launcher
 Home-page: https://github.com/caplett/hydra_submitit_extension
 Author: Stefan Geyer
 Author-email: git@caplett.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
@@ -48,16 +48,20 @@
 
 ``` bash
 pip install hydra-submitit-extension
 ```
 
 ## Quickstart
 
+```
+python main.py hydra/launcher=submitit_slurm_extended -m
+```
 
-``` yaml
+All Parameter:
+``` yaml config.yaml
 # @package hydra.launcher
 
 # No changes to Submitit Launcher plugin
 submitit_folder: ${hydra.sweep.dir}/.submitit/%j
 timeout_min: 30
 cpus_per_task: 1
 gpus_per_node: null
```

### Comparing `hydra_submitit_extension-0.0.2/src/hydra_submitit_extension.egg-info/SOURCES.txt` & `hydra_submitit_extension-0.0.3/src/hydra_submitit_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/tests/conf/slurm/cpu.yaml` & `hydra_submitit_extension-0.0.3/tests/conf/slurm/cpu.yaml`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/tests/test_skeleton.py` & `hydra_submitit_extension-0.0.3/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.2/tox.ini` & `hydra_submitit_extension-0.0.3/tox.ini`

 * *Files identical despite different names*

