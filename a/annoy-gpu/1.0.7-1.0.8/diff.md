# Comparing `tmp/annoy_gpu-1.0.7.tar.gz` & `tmp/annoy_gpu-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/annoy_gpu-1.0.7.tar", last modified: Mon Jun 12 15:59:39 2023, max compression
+gzip compressed data, was "dist/annoy_gpu-1.0.8.tar", last modified: Mon Jun 12 17:36:08 2023, max compression
```

## Comparing `annoy_gpu-1.0.7.tar` & `annoy_gpu-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/annoy_gpu/
--rw-r--r--   0 root         (0) root         (0)      684 2023-05-11 13:47:29.000000 annoy_gpu-1.0.7/annoy_gpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-12 15:29:01.000000 annoy_gpu-1.0.7/annoy_gpu/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 13:47:29.000000 annoy_gpu-1.0.7/annoy_gpu/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/annoy_gpu.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1315 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/annoy_gpu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/annoy_gpu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/annoy_gpu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/annoy_gpu.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/src/
--rw-r--r--   0 root         (0) root         (0)    61356 2023-06-12 15:25:35.000000 annoy_gpu-1.0.7/src/annoylib.h
--rw-r--r--   0 root         (0) root         (0)    23272 2023-06-12 15:17:34.000000 annoy_gpu-1.0.7/src/annoymodule.cu
--rw-r--r--   0 root         (0) root         (0)     2753 2023-06-10 13:41:00.000000 annoy_gpu-1.0.7/src/kissrandom.h
--rw-r--r--   0 root         (0) root         (0)     5791 2023-06-09 14:33:59.000000 annoy_gpu-1.0.7/src/mman.h
--rw-r--r--   0 root         (0) root         (0)    11362 2023-05-11 13:47:29.000000 annoy_gpu-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-11 13:47:29.000000 annoy_gpu-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-12 14:14:47.000000 annoy_gpu-1.0.7/README.rst
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-12 09:59:58.000000 annoy_gpu-1.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8608 2023-06-12 15:37:15.000000 annoy_gpu-1.0.7/setup.py
--rw-r--r--   0 root         (0) root         (0)     1315 2023-06-12 15:49:13.000000 annoy_gpu-1.0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/annoy_gpu/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-05-11 13:47:29.000000 annoy_gpu-1.0.8/annoy_gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-12 15:29:01.000000 annoy_gpu-1.0.8/annoy_gpu/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 13:47:29.000000 annoy_gpu-1.0.8/annoy_gpu/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/annoy_gpu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/annoy_gpu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/annoy_gpu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/annoy_gpu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/annoy_gpu.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/src/
+-rw-r--r--   0 root         (0) root         (0)    61358 2023-06-12 17:25:04.000000 annoy_gpu-1.0.8/src/annoylib.h
+-rw-r--r--   0 root         (0) root         (0)    23479 2023-06-12 17:06:02.000000 annoy_gpu-1.0.8/src/annoymodule.cu
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-06-10 13:41:00.000000 annoy_gpu-1.0.8/src/kissrandom.h
+-rw-r--r--   0 root         (0) root         (0)     5791 2023-06-09 14:33:59.000000 annoy_gpu-1.0.8/src/mman.h
+-rw-r--r--   0 root         (0) root         (0)    11362 2023-05-11 13:47:29.000000 annoy_gpu-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-11 13:47:29.000000 annoy_gpu-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2006 2023-06-12 16:39:46.000000 annoy_gpu-1.0.8/README.rst
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-12 09:59:58.000000 annoy_gpu-1.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8608 2023-06-12 17:25:26.000000 annoy_gpu-1.0.8/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2023-06-12 17:25:42.000000 annoy_gpu-1.0.8/PKG-INFO
```

### Comparing `annoy_gpu-1.0.7/annoy_gpu/__init__.py` & `annoy_gpu-1.0.8/annoy_gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `annoy_gpu-1.0.7/annoy_gpu/__init__.pyi` & `annoy_gpu-1.0.8/annoy_gpu/__init__.pyi`

 * *Files identical despite different names*

### Comparing `annoy_gpu-1.0.7/annoy_gpu.egg-info/PKG-INFO` & `annoy_gpu-1.0.8/annoy_gpu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annoy-gpu
-Version: 1.0.7
+Version: 1.0.8
 Summary: Approximate Nearest Neighbors in C++/Python optimized for memory usage and loading/saving to disk. Can run with GPU speedup.
 Home-page: https://github.com/Ri-chard-Wu/annoy-gpu
 Author: Erik Bernhardsson, Ri-chard-Wu
 Author-email: mail@erikbern.com, glotigorgeous@gmail.com
 License: Apache License 2.0
 Keywords: nns,approximate nearest neighbor search
 Platform: UNKNOWN
```

### Comparing `annoy_gpu-1.0.7/src/annoylib.h` & `annoy_gpu-1.0.8/src/annoylib.h`

 * *Files 0% similar despite different names*

```diff
@@ -1071,18 +1071,17 @@
       }
 
       thread_roots.push_back(_make_tree_gup_build(indices, true, _random, bp));
       // printf("n trees built: %d / %d\n", thread_roots.size(), n_tree);    
 
       annoylib_showUpdate("n trees built: %d / %d\n", thread_roots.size(), n_tree);
 
-      char buf[100];
-      sprintf(buf, "n trees built: %d / %d\n", thread_roots.size(), n_tree);
-      
-      pyPrint(buf);
+      // char buf[100];
+      // sprintf(buf, "n trees built: %d / %d\n", thread_roots.size(), n_tree);
+      // pyPrint(buf);
     }
 
     _roots.insert(_roots.end(), thread_roots.begin(), thread_roots.end());
   }
```

### Comparing `annoy_gpu-1.0.7/src/annoymodule.cu` & `annoy_gpu-1.0.8/src/annoymodule.cu`

 * *Files 2% similar despite different names*

```diff
@@ -229,18 +229,25 @@
 
 
 
 static PyObject *
 py_an_set_print_redirection(py_annoy *self, PyObject *args) {
 
   PyObject *file = NULL;
+
   
   if (!PyArg_ParseTuple(args, "O", &file))
       return NULL;
+  Py_INCREF(file);
 
+  // char buf[100];
+  // sprintf(buf, "[test] n trees built: %d / %d\n", 1, 6);
+  // PyObject *pystr = PyUnicode_FromString(buf);
+  // PyFile_WriteObject(pystr, file, Py_PRINT_RAW);
+    
   self->ptr->set_print_redirection(file);
 
   Py_RETURN_NONE;      
 }
```

### Comparing `annoy_gpu-1.0.7/src/kissrandom.h` & `annoy_gpu-1.0.8/src/kissrandom.h`

 * *Files identical despite different names*

### Comparing `annoy_gpu-1.0.7/src/mman.h` & `annoy_gpu-1.0.8/src/mman.h`

 * *Files identical despite different names*

### Comparing `annoy_gpu-1.0.7/LICENSE` & `annoy_gpu-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `annoy_gpu-1.0.7/README.rst` & `annoy_gpu-1.0.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 -----
 
 This project is derived from `Annoy <https://github.com/spotify/annoy/tree/main>`_. The original project can use multi-thread to accelerate build process. In this project GPU is used to accelerate the build process. This project is still under development. Currently it only support the 'angular' metrics.
 
 Install
 -------
 
-First set the environment variable "CUDAHOME" to CUDA installation location, e.g. ``export CUDAHOME=/usr/local/cuda-10.2``, then run ``pip install annoy_gpu`` to pull down the latest version from `PyPI <https://test.pypi.org/project/annoy-gpu>`_.
+First set the environment variable "CUDAHOME" to CUDA installation location, e.g. ``export CUDAHOME=/usr/local/cuda-10.2``, then run ``pip install annoy_gpu`` to pull down the latest version from `PyPI <https://pypi.org/project/annoy-gpu/>`_.
 
 Python code example
 -------------------
 
 Add items and then save at 'test-1e5.tree'.
 
 .. code-block:: python
```

### Comparing `annoy_gpu-1.0.7/setup.py` & `annoy_gpu-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools_cuda import CudaExtension
 import codecs
 import os
 import platform
 import sys
 
 
-version='1.0.7'
+version='1.0.8'
 
 readme_note = """\
 .. note::
 
     This project is derived from `Annoy <https://github.com/spotify/annoy/tree/main>`_. The original project can use multi-thread to accelerate build process. In this project GPU is used to accelerate the build process. This project is still under developing. Currently it only support the Angular metrics.
 
 """
```

### Comparing `annoy_gpu-1.0.7/PKG-INFO` & `annoy_gpu-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annoy_gpu
-Version: 1.0.7
+Version: 1.0.8
 Summary: Approximate Nearest Neighbors in C++/Python optimized for memory usage and loading/saving to disk. Can run with GPU speedup.
 Home-page: https://github.com/Ri-chard-Wu/annoy-gpu
 Author: Erik Bernhardsson, Ri-chard-Wu
 Author-email: mail@erikbern.com, glotigorgeous@gmail.com
 License: Apache License 2.0
 Keywords: nns,approximate nearest neighbor search
 Platform: UNKNOWN
```

