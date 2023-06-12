# Comparing `tmp/clenv-0.0.6.tar.gz` & `tmp/clenv-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clenv-0.0.6.tar", last modified: Fri Jun  9 20:16:03 2023, max compression
+gzip compressed data, was "clenv-0.0.7.tar", last modified: Mon Jun 12 16:12:39 2023, max compression
```

## Comparing `clenv-0.0.6.tar` & `clenv-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.788407 clenv-0.0.6/
--rw-r--r--   0 brainco    (501) staff       (20)     1067 2023-04-26 09:03:52.000000 clenv-0.0.6/LICENSE
--rw-r--r--   0 brainco    (501) staff       (20)     4138 2023-06-09 20:16:03.787797 clenv-0.0.6/PKG-INFO
--rw-r--r--   0 brainco    (501) staff       (20)     3455 2023-06-09 19:54:28.000000 clenv-0.0.6/README.md
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.776973 clenv-0.0.6/clenv/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 09:54:11.000000 clenv-0.0.6/clenv/__init__.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.780617 clenv-0.0.6/clenv/cli/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:03:58.000000 clenv-0.0.6/clenv/cli/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)      390 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/__main__.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.783058 clenv-0.0.6/clenv/cli/config/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:04:34.000000 clenv-0.0.6/clenv/cli/config/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)      828 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/config/config_loader.py
--rw-r--r--   0 brainco    (501) staff       (20)    14187 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/config/config_manager.py
--rw-r--r--   0 brainco    (501) staff       (20)     5650 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/config/config_subcommand.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.784275 clenv-0.0.6/clenv/cli/queue/
--rw-r--r--   0 brainco    (501) staff       (20)       13 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/queue/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)     2182 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/queue/queue_manager.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.785563 clenv-0.0.6/clenv/cli/task/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/task/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)     8320 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/task/task_subcommand.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.786888 clenv-0.0.6/clenv/cli/user/
--rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:05:30.000000 clenv-0.0.6/clenv/cli/user/__init__.py
--rw-r--r--   0 brainco    (501) staff       (20)     2724 2023-06-09 19:36:56.000000 clenv-0.0.6/clenv/cli/user/user_subcommand.py
-drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-09 20:16:03.779948 clenv-0.0.6/clenv.egg-info/
--rw-r--r--   0 brainco    (501) staff       (20)     4138 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/PKG-INFO
--rw-r--r--   0 brainco    (501) staff       (20)      583 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/SOURCES.txt
--rw-r--r--   0 brainco    (501) staff       (20)        1 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/dependency_links.txt
--rw-r--r--   0 brainco    (501) staff       (20)       50 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/entry_points.txt
--rw-r--r--   0 brainco    (501) staff       (20)       59 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/requires.txt
--rw-r--r--   0 brainco    (501) staff       (20)        6 2023-06-09 20:16:03.000000 clenv-0.0.6/clenv.egg-info/top_level.txt
--rw-r--r--   0 brainco    (501) staff       (20)       38 2023-06-09 20:16:03.788598 clenv-0.0.6/setup.cfg
--rw-r--r--   0 brainco    (501) staff       (20)     1147 2023-06-09 19:36:56.000000 clenv-0.0.6/setup.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-12 16:12:39.082896 clenv-0.0.7/
+-rw-r--r--   0 brainco    (501) staff       (20)     1067 2023-04-26 09:03:52.000000 clenv-0.0.7/LICENSE
+-rw-r--r--   0 brainco    (501) staff       (20)     4138 2023-06-12 16:12:39.082575 clenv-0.0.7/PKG-INFO
+-rw-r--r--   0 brainco    (501) staff       (20)     3455 2023-06-09 19:54:28.000000 clenv-0.0.7/README.md
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-12 16:12:39.073183 clenv-0.0.7/clenv/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 09:54:11.000000 clenv-0.0.7/clenv/__init__.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-12 16:12:39.076593 clenv-0.0.7/clenv/cli/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:03:58.000000 clenv-0.0.7/clenv/cli/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)      390 2023-06-09 19:36:56.000000 clenv-0.0.7/clenv/cli/__main__.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-12 16:12:39.079343 clenv-0.0.7/clenv/cli/config/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:04:34.000000 clenv-0.0.7/clenv/cli/config/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)      828 2023-06-09 19:36:56.000000 clenv-0.0.7/clenv/cli/config/config_loader.py
+-rw-r--r--   0 brainco    (501) staff       (20)    14187 2023-06-09 19:36:56.000000 clenv-0.0.7/clenv/cli/config/config_manager.py
+-rw-r--r--   0 brainco    (501) staff       (20)     5650 2023-06-09 19:36:56.000000 clenv-0.0.7/clenv/cli/config/config_subcommand.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-12 16:12:39.080265 clenv-0.0.7/clenv/cli/queue/
+-rw-r--r--   0 brainco    (501) staff       (20)       13 2023-06-09 19:36:56.000000 clenv-0.0.7/clenv/cli/queue/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)     2182 2023-06-09 19:36:56.000000 clenv-0.0.7/clenv/cli/queue/queue_manager.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-12 16:12:39.081155 clenv-0.0.7/clenv/cli/task/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-06-09 19:36:56.000000 clenv-0.0.7/clenv/cli/task/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)     8320 2023-06-09 19:36:56.000000 clenv-0.0.7/clenv/cli/task/task_subcommand.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-12 16:12:39.082031 clenv-0.0.7/clenv/cli/user/
+-rw-r--r--   0 brainco    (501) staff       (20)        0 2023-04-26 10:05:30.000000 clenv-0.0.7/clenv/cli/user/__init__.py
+-rw-r--r--   0 brainco    (501) staff       (20)     2724 2023-06-09 19:36:56.000000 clenv-0.0.7/clenv/cli/user/user_subcommand.py
+drwxr-xr-x   0 brainco    (501) staff       (20)        0 2023-06-12 16:12:39.075935 clenv-0.0.7/clenv.egg-info/
+-rw-r--r--   0 brainco    (501) staff       (20)     4138 2023-06-12 16:12:39.000000 clenv-0.0.7/clenv.egg-info/PKG-INFO
+-rw-r--r--   0 brainco    (501) staff       (20)      583 2023-06-12 16:12:39.000000 clenv-0.0.7/clenv.egg-info/SOURCES.txt
+-rw-r--r--   0 brainco    (501) staff       (20)        1 2023-06-12 16:12:39.000000 clenv-0.0.7/clenv.egg-info/dependency_links.txt
+-rw-r--r--   0 brainco    (501) staff       (20)       50 2023-06-12 16:12:39.000000 clenv-0.0.7/clenv.egg-info/entry_points.txt
+-rw-r--r--   0 brainco    (501) staff       (20)       77 2023-06-12 16:12:39.000000 clenv-0.0.7/clenv.egg-info/requires.txt
+-rw-r--r--   0 brainco    (501) staff       (20)        6 2023-06-12 16:12:39.000000 clenv-0.0.7/clenv.egg-info/top_level.txt
+-rw-r--r--   0 brainco    (501) staff       (20)       38 2023-06-12 16:12:39.083006 clenv-0.0.7/setup.cfg
+-rw-r--r--   0 brainco    (501) staff       (20)     1176 2023-06-12 16:08:00.000000 clenv-0.0.7/setup.py
```

### Comparing `clenv-0.0.6/LICENSE` & `clenv-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clenv-0.0.6/PKG-INFO` & `clenv-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clenv
-Version: 0.0.6
+Version: 0.0.7
 Summary: ClearML config profile manager
 Home-page: https://github.com/DavidSonoda/clenv
 Author: Juewei Dong
 Author-email: juewei.dong@brainco.tech
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `clenv-0.0.6/README.md` & `clenv-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `clenv-0.0.6/clenv/cli/config/config_loader.py` & `clenv-0.0.7/clenv/cli/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `clenv-0.0.6/clenv/cli/config/config_manager.py` & `clenv-0.0.7/clenv/cli/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `clenv-0.0.6/clenv/cli/config/config_subcommand.py` & `clenv-0.0.7/clenv/cli/config/config_subcommand.py`

 * *Files identical despite different names*

### Comparing `clenv-0.0.6/clenv/cli/queue/queue_manager.py` & `clenv-0.0.7/clenv/cli/queue/queue_manager.py`

 * *Files identical despite different names*

### Comparing `clenv-0.0.6/clenv/cli/task/task_subcommand.py` & `clenv-0.0.7/clenv/cli/task/task_subcommand.py`

 * *Files identical despite different names*

### Comparing `clenv-0.0.6/clenv/cli/user/user_subcommand.py` & `clenv-0.0.7/clenv/cli/user/user_subcommand.py`

 * *Files identical despite different names*

### Comparing `clenv-0.0.6/clenv.egg-info/PKG-INFO` & `clenv-0.0.7/clenv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clenv
-Version: 0.0.6
+Version: 0.0.7
 Summary: ClearML config profile manager
 Home-page: https://github.com/DavidSonoda/clenv
 Author: Juewei Dong
 Author-email: juewei.dong@brainco.tech
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `clenv-0.0.6/clenv.egg-info/SOURCES.txt` & `clenv-0.0.7/clenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clenv-0.0.6/setup.py` & `clenv-0.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="clenv",
-    version="0.0.6",
+    version="0.0.7",
     description="ClearML config profile manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Juewei Dong",
     author_email="juewei.dong@brainco.tech",
     url="https://github.com/DavidSonoda/clenv",
     license="MIT",
@@ -31,9 +31,10 @@
         ],
     },
     install_requires=[
         "clearml>=1.10.0",
         "click>=8.1.0",
         "pyhocon==0.3.35",
         "bcrypt>=4.0.0",
+        "GitPython==3.1.31",
     ],
 )
```

