# Comparing `tmp/usellm-0.0.5.tar.gz` & `tmp/usellm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usellm-0.0.5.tar", last modified: Tue May 30 06:23:43 2023, max compression
+gzip compressed data, was "usellm-0.0.6.tar", last modified: Mon Jun 12 12:31:30 2023, max compression
```

## Comparing `usellm-0.0.5.tar` & `usellm-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-30 06:23:43.995170 usellm-0.0.5/
--rw-r--r--   0 jovian     (501) staff       (20)     1063 2023-05-10 15:34:43.000000 usellm-0.0.5/LICENSE
--rw-r--r--   0 jovian     (501) staff       (20)     3736 2023-05-30 06:23:43.995042 usellm-0.0.5/PKG-INFO
--rw-r--r--   0 jovian     (501) staff       (20)     3476 2023-05-27 19:44:21.000000 usellm-0.0.5/README.md
--rw-r--r--   0 jovian     (501) staff       (20)       38 2023-05-30 06:23:43.995209 usellm-0.0.5/setup.cfg
--rw-r--r--   0 jovian     (501) staff       (20)      523 2023-05-30 06:13:33.000000 usellm-0.0.5/setup.py
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-30 06:23:43.994260 usellm-0.0.5/usellm/
--rw-r--r--   0 jovian     (501) staff       (20)       90 2023-05-27 17:31:49.000000 usellm-0.0.5/usellm/__init__.py
--rw-r--r--   0 jovian     (501) staff       (20)     3633 2023-05-28 06:16:38.000000 usellm-0.0.5/usellm/use_llm.py
--rw-r--r--   0 jovian     (501) staff       (20)       72 2023-05-27 17:32:05.000000 usellm-0.0.5/usellm/utils.py
-drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-05-30 06:23:43.994886 usellm-0.0.5/usellm.egg-info/
--rw-r--r--   0 jovian     (501) staff       (20)     3736 2023-05-30 06:23:43.000000 usellm-0.0.5/usellm.egg-info/PKG-INFO
--rw-r--r--   0 jovian     (501) staff       (20)      228 2023-05-30 06:23:43.000000 usellm-0.0.5/usellm.egg-info/SOURCES.txt
--rw-r--r--   0 jovian     (501) staff       (20)        1 2023-05-30 06:23:43.000000 usellm-0.0.5/usellm.egg-info/dependency_links.txt
--rw-r--r--   0 jovian     (501) staff       (20)       17 2023-05-30 06:23:43.000000 usellm-0.0.5/usellm.egg-info/requires.txt
--rw-r--r--   0 jovian     (501) staff       (20)        7 2023-05-30 06:23:43.000000 usellm-0.0.5/usellm.egg-info/top_level.txt
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-06-12 12:31:30.434120 usellm-0.0.6/
+-rw-r--r--   0 jovian     (501) staff       (20)     1063 2023-05-10 15:34:43.000000 usellm-0.0.6/LICENSE
+-rw-r--r--   0 jovian     (501) staff       (20)     3736 2023-06-12 12:31:30.433895 usellm-0.0.6/PKG-INFO
+-rw-r--r--   0 jovian     (501) staff       (20)     3476 2023-05-27 19:44:21.000000 usellm-0.0.6/README.md
+-rw-r--r--   0 jovian     (501) staff       (20)       38 2023-06-12 12:31:30.434210 usellm-0.0.6/setup.cfg
+-rw-r--r--   0 jovian     (501) staff       (20)      583 2023-06-12 12:30:45.000000 usellm-0.0.6/setup.py
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-06-12 12:31:30.432275 usellm-0.0.6/usellm/
+-rw-r--r--   0 jovian     (501) staff       (20)       90 2023-05-27 17:31:49.000000 usellm-0.0.6/usellm/__init__.py
+-rw-r--r--   0 jovian     (501) staff       (20)     7470 2023-06-12 12:30:45.000000 usellm-0.0.6/usellm/use_llm.py
+-rw-r--r--   0 jovian     (501) staff       (20)       72 2023-05-27 17:32:05.000000 usellm-0.0.6/usellm/utils.py
+drwxr-xr-x   0 jovian     (501) staff       (20)        0 2023-06-12 12:31:30.433185 usellm-0.0.6/usellm.egg-info/
+-rw-r--r--   0 jovian     (501) staff       (20)     3736 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/PKG-INFO
+-rw-r--r--   0 jovian     (501) staff       (20)      228 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/SOURCES.txt
+-rw-r--r--   0 jovian     (501) staff       (20)        1 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/dependency_links.txt
+-rw-r--r--   0 jovian     (501) staff       (20)       17 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/requires.txt
+-rw-r--r--   0 jovian     (501) staff       (20)        7 2023-06-12 12:31:30.000000 usellm-0.0.6/usellm.egg-info/top_level.txt
```

### Comparing `usellm-0.0.5/LICENSE` & `usellm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `usellm-0.0.5/PKG-INFO` & `usellm-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usellm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Use Large Language Models in Python App
 Home-page: https://github.com/usellm/usellm-py
 Author: Siddhant
 Author-email: siddhant@jovian.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `usellm-0.0.5/README.md` & `usellm-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `usellm-0.0.5/usellm.egg-info/PKG-INFO` & `usellm-0.0.6/usellm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usellm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Use Large Language Models in Python App
 Home-page: https://github.com/usellm/usellm-py
 Author: Siddhant
 Author-email: siddhant@jovian.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

