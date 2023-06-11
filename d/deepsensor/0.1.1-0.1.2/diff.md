# Comparing `tmp/deepsensor-0.1.1.tar.gz` & `tmp/deepsensor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsensor-0.1.1.tar", last modified: Sat Jun 10 16:40:27 2023, max compression
+gzip compressed data, was "deepsensor-0.1.2.tar", last modified: Sun Jun 11 22:56:26 2023, max compression
```

## Comparing `deepsensor-0.1.1.tar` & `deepsensor-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.279728 deepsensor-0.1.1/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     1076 2023-05-16 13:27:41.000000 deepsensor-0.1.1/LICENSE
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     4957 2023-06-10 16:40:27.279728 deepsensor-0.1.1/PKG-INFO
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     4560 2023-06-10 16:25:41.000000 deepsensor-0.1.1/README.md
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.275728 deepsensor-0.1.1/deepsensor/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      329 2023-05-24 13:52:11.000000 deepsensor-0.1.1/deepsensor/__init__.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.275728 deepsensor-0.1.1/deepsensor/active_learning/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-19 14:49:00.000000 deepsensor-0.1.1/deepsensor/active_learning/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     8772 2023-05-22 14:39:54.000000 deepsensor-0.1.1/deepsensor/active_learning/acquisition_fns.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      170 2023-06-09 15:07:15.000000 deepsensor-0.1.1/deepsensor/config.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.275728 deepsensor-0.1.1/deepsensor/data/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.1/deepsensor/data/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)    22102 2023-06-07 17:20:41.000000 deepsensor-0.1.1/deepsensor/data/loader.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)    14246 2023-06-09 15:07:15.000000 deepsensor-0.1.1/deepsensor/data/processor.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     3509 2023-05-31 22:34:31.000000 deepsensor-0.1.1/deepsensor/data/task.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     3717 2023-06-07 17:20:41.000000 deepsensor-0.1.1/deepsensor/data/utils.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.275728 deepsensor-0.1.1/deepsensor/model/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.1/deepsensor/model/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     2704 2023-06-07 17:20:41.000000 deepsensor-0.1.1/deepsensor/model/defaults.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)    28006 2023-06-10 13:53:55.000000 deepsensor-0.1.1/deepsensor/model/models.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     8042 2023-06-10 14:54:25.000000 deepsensor-0.1.1/deepsensor/model/nps.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.279728 deepsensor-0.1.1/deepsensor/plot/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.1/deepsensor/plot/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     6091 2023-05-31 22:34:31.000000 deepsensor-0.1.1/deepsensor/plot/utils.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 14:47:21.000000 deepsensor-0.1.1/deepsensor/py.typed
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.279728 deepsensor-0.1.1/deepsensor/tensorflow/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      826 2023-06-09 15:07:15.000000 deepsensor-0.1.1/deepsensor/tensorflow/__init__.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.279728 deepsensor-0.1.1/deepsensor/torch/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      788 2023-06-09 15:03:43.000000 deepsensor-0.1.1/deepsensor/torch/__init__.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.279728 deepsensor-0.1.1/deepsensor/train/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-06 13:04:03.000000 deepsensor-0.1.1/deepsensor/train/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     3770 2023-06-09 17:05:13.000000 deepsensor-0.1.1/deepsensor/train/train.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-17 10:49:11.000000 deepsensor-0.1.1/deepsensor/utils.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.275728 deepsensor-0.1.1/deepsensor.egg-info/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     4957 2023-06-10 16:40:27.000000 deepsensor-0.1.1/deepsensor.egg-info/PKG-INFO
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      942 2023-06-10 16:40:27.000000 deepsensor-0.1.1/deepsensor.egg-info/SOURCES.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-10 16:40:27.000000 deepsensor-0.1.1/deepsensor.egg-info/dependency_links.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-10 14:42:57.000000 deepsensor-0.1.1/deepsensor.egg-info/not-zip-safe
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      127 2023-06-10 16:40:27.000000 deepsensor-0.1.1/deepsensor.egg-info/requires.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)       17 2023-06-10 16:40:27.000000 deepsensor-0.1.1/deepsensor.egg-info/top_level.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      471 2023-06-10 15:57:32.000000 deepsensor-0.1.1/pyproject.toml
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      882 2023-06-10 16:40:27.279728 deepsensor-0.1.1/setup.cfg
--rw-rw-r--   0 tomand    (1001) tomand    (1001)       69 2023-06-10 15:31:16.000000 deepsensor-0.1.1/setup.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-10 16:40:27.279728 deepsensor-0.1.1/tests/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 15:06:33.000000 deepsensor-0.1.1/tests/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     7896 2023-06-09 15:07:18.000000 deepsensor-0.1.1/tests/test_data_processor.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     8740 2023-06-07 17:20:41.000000 deepsensor-0.1.1/tests/test_model.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     5845 2023-06-07 17:20:41.000000 deepsensor-0.1.1/tests/test_task_loader.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     2028 2023-06-08 17:10:45.000000 deepsensor-0.1.1/tests/utils.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.066173 deepsensor-0.1.2/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     1076 2023-05-16 13:27:41.000000 deepsensor-0.1.2/LICENSE
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     4957 2023-06-11 22:56:26.066173 deepsensor-0.1.2/PKG-INFO
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     4560 2023-06-10 16:25:41.000000 deepsensor-0.1.2/README.md
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      329 2023-06-11 17:55:57.000000 deepsensor-0.1.2/deepsensor/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      278 2023-06-11 21:28:07.000000 deepsensor-0.1.2/deepsensor/_version.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/active_learning/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-19 14:49:00.000000 deepsensor-0.1.2/deepsensor/active_learning/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     8772 2023-05-22 14:39:54.000000 deepsensor-0.1.2/deepsensor/active_learning/acquisition_fns.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      170 2023-06-09 15:07:15.000000 deepsensor-0.1.2/deepsensor/config.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/data/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.2/deepsensor/data/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)    22102 2023-06-07 17:20:41.000000 deepsensor-0.1.2/deepsensor/data/loader.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)    14246 2023-06-09 15:07:15.000000 deepsensor-0.1.2/deepsensor/data/processor.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     3509 2023-05-31 22:34:31.000000 deepsensor-0.1.2/deepsensor/data/task.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     3717 2023-06-07 17:20:41.000000 deepsensor-0.1.2/deepsensor/data/utils.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/model/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.2/deepsensor/model/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     2830 2023-06-11 18:38:33.000000 deepsensor-0.1.2/deepsensor/model/defaults.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)    28006 2023-06-10 13:53:55.000000 deepsensor-0.1.2/deepsensor/model/models.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     8042 2023-06-10 14:54:25.000000 deepsensor-0.1.2/deepsensor/model/nps.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     7376 2023-06-11 20:24:15.000000 deepsensor-0.1.2/deepsensor/plot.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 14:47:21.000000 deepsensor-0.1.2/deepsensor/py.typed
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/tensorflow/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      826 2023-06-09 15:07:15.000000 deepsensor-0.1.2/deepsensor/tensorflow/__init__.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/torch/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      788 2023-06-09 15:03:43.000000 deepsensor-0.1.2/deepsensor/torch/__init__.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.066173 deepsensor-0.1.2/deepsensor/train/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-06 13:04:03.000000 deepsensor-0.1.2/deepsensor/train/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     3770 2023-06-09 17:05:13.000000 deepsensor-0.1.2/deepsensor/train/train.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-17 10:49:11.000000 deepsensor-0.1.2/deepsensor/utils.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor.egg-info/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     4957 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/PKG-INFO
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      931 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-10 14:42:57.000000 deepsensor-0.1.2/deepsensor.egg-info/not-zip-safe
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      127 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/requires.txt
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)       17 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/top_level.txt
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      471 2023-06-10 15:57:32.000000 deepsensor-0.1.2/pyproject.toml
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)      882 2023-06-11 22:56:26.066173 deepsensor-0.1.2/setup.cfg
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)       69 2023-06-11 22:18:42.000000 deepsensor-0.1.2/setup.py
+drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.066173 deepsensor-0.1.2/tests/
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 15:06:33.000000 deepsensor-0.1.2/tests/__init__.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     7896 2023-06-09 15:07:18.000000 deepsensor-0.1.2/tests/test_data_processor.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     8740 2023-06-07 17:20:41.000000 deepsensor-0.1.2/tests/test_model.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     5845 2023-06-07 17:20:41.000000 deepsensor-0.1.2/tests/test_task_loader.py
+-rw-rw-r--   0 tomand    (1001) tomand    (1001)     2028 2023-06-08 17:10:45.000000 deepsensor-0.1.2/tests/utils.py
```

### Comparing `deepsensor-0.1.1/LICENSE` & `deepsensor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/PKG-INFO` & `deepsensor-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `deepsensor-0.1.1/README.md` & `deepsensor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/active_learning/acquisition_fns.py` & `deepsensor-0.1.2/deepsensor/active_learning/acquisition_fns.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/data/loader.py` & `deepsensor-0.1.2/deepsensor/data/loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/data/processor.py` & `deepsensor-0.1.2/deepsensor/data/processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/data/task.py` & `deepsensor-0.1.2/deepsensor/data/task.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/data/utils.py` & `deepsensor-0.1.2/deepsensor/data/utils.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/model/defaults.py` & `deepsensor-0.1.2/deepsensor/model/defaults.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,17 @@
             # Gridded variable: use data ppu
             x1_res = np.abs(np.mean(np.diff(var["x1"])))
             x2_res = np.abs(np.mean(np.diff(var["x2"])))
             data_ppu = 1 / np.mean([x1_res, x2_res])
             max_ppu = max(max_ppu, data_ppu * 1.2)  # Add 20% margin
         elif isinstance(var, (pd.DataFrame, pd.Series)):
             # Point-based variable: make ppu as large as possible
-            max_ppu = 300  # TODO: How should we choose this?
+            # TODO: Consider choosing based on shortest distance between points, perhaps with some
+            # check for outliers causing excessively large ppu
+            max_ppu = 300
         else:
             raise ValueError(f"Unknown context input type: {type(var)}")
 
     return int(max_ppu)
 
 
 def gen_encoder_scales(model_ppu: int, task_loader: TaskLoader) -> list:
```

### Comparing `deepsensor-0.1.1/deepsensor/model/models.py` & `deepsensor-0.1.2/deepsensor/model/models.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/model/nps.py` & `deepsensor-0.1.2/deepsensor/model/nps.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/plot/utils.py` & `deepsensor-0.1.2/deepsensor/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import numpy as np
 
-import matplotlib as mpl
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1 import make_axes_locatable
+import matplotlib.patches as mpatches
 
-from deepsensor.model.nps import compute_encoding_tensor
 
-
-def plot_context_encoding(
+def context_encoding(
     model,
     task,
     task_loader,
     batch_idx=0,
     context_set_idxs=None,
     land_idx=None,
     cbar=True,
@@ -23,15 +21,15 @@
     return_axes=False,
 ):
     """Plot the encoding of a context set in a task
 
     Parameters
     ----------
     model : DeepSensor model
-    task : dict
+    task : Task
         Task containing context set to plot encoding of
     task_loader : deepsensor.data.loader.TaskLoader
         DataLoader used to load the data, containing context set metadata used for plotting
     batch_idx : int, optional
         Batch index in encoding to plot, by default 0
     context_set_idxs : list or int, optional
         Indices of context sets to plot, by default None (plots all context sets)
@@ -44,14 +42,16 @@
         List of titles to override for each subplot, by default None.
         If None, titles are generated from context set metadata
     size : int, optional
         Size of the figure in inches, by default 20
     return_axes : bool, optional
         Whether to return the axes of the figure, by default False
     """
+    from .model.nps import compute_encoding_tensor
+
     encoding_tensor = compute_encoding_tensor(model, task)
     encoding_tensor = encoding_tensor[batch_idx]
 
     if isinstance(context_set_idxs, int):
         context_set_idxs = [context_set_idxs]
     if context_set_idxs is None:
         context_set_idxs = np.array(range(len(task_loader.context)))
@@ -116,15 +116,15 @@
     plt.tight_layout()
     if not return_axes:
         return fig
     elif return_axes:
         return fig, axes
 
 
-def plot_offgrid_context(
+def offgrid_context(
     axes,
     task,
     data_processor=None,
     task_loader=None,
     plot_target=False,
     add_legend=True,
     **scatter_kwargs,
@@ -176,7 +176,50 @@
                 **scatter_kwargs,
                 facecolors=None if markers[set_i] == "x" else "none",
                 label=label,
             )
 
     if add_legend:
         axes[0].legend(loc="best")
+
+
+def receptive_field(receptive_field, data_processor, crs, extent="global"):
+    fig, ax = plt.subplots(subplot_kw=dict(projection=crs))
+
+    if extent == "global":
+        ax.set_global()
+    else:
+        ax.set_extent(extent, crs=crs)
+
+    x11, x12 = data_processor.norm_params["coords"]["x1"]["map"]
+    x21, x22 = data_processor.norm_params["coords"]["x2"]["map"]
+
+    x1_rf_raw = receptive_field * (x12 - x11)
+    x2_rf_raw = receptive_field * (x22 - x21)
+
+    x1_midpoint_raw = (x12 + x11) / 2
+    x2_midpoint_raw = (x22 + x21) / 2
+
+    # Compute bottom left corner of receptive field
+    x1_corner = x1_midpoint_raw - x1_rf_raw / 2
+    x2_corner = x2_midpoint_raw - x2_rf_raw / 2
+
+    ax.add_patch(
+        mpatches.Rectangle(
+            xy=[x2_corner, x1_corner],  # Cartesian fmt: x2, x1
+            width=x2_rf_raw,
+            height=x1_rf_raw,
+            facecolor="black",
+            alpha=0.3,
+            transform=crs,
+        )
+    )
+    ax.coastlines()
+    ax.gridlines(draw_labels=True, alpha=0.2)
+
+    x1_name = data_processor.norm_params["coords"]["x1"]["name"]
+    x2_name = data_processor.norm_params["coords"]["x2"]["name"]
+    ax.set_title(
+        f"Receptive field in raw coords: {x1_name}={x1_rf_raw:.2f}, {x2_name}={x2_rf_raw:.2f}"
+    )
+
+    return fig
```

### Comparing `deepsensor-0.1.1/deepsensor/tensorflow/__init__.py` & `deepsensor-0.1.2/deepsensor/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/torch/__init__.py` & `deepsensor-0.1.2/deepsensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor/train/train.py` & `deepsensor-0.1.2/deepsensor/train/train.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/deepsensor.egg-info/PKG-INFO` & `deepsensor-0.1.2/deepsensor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `deepsensor-0.1.1/deepsensor.egg-info/SOURCES.txt` & `deepsensor-0.1.2/deepsensor.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 deepsensor/__init__.py
+deepsensor/_version.py
 deepsensor/config.py
+deepsensor/plot.py
 deepsensor/py.typed
 deepsensor/utils.py
 deepsensor.egg-info/PKG-INFO
 deepsensor.egg-info/SOURCES.txt
 deepsensor.egg-info/dependency_links.txt
 deepsensor.egg-info/not-zip-safe
 deepsensor.egg-info/requires.txt
@@ -20,16 +22,14 @@
 deepsensor/data/processor.py
 deepsensor/data/task.py
 deepsensor/data/utils.py
 deepsensor/model/__init__.py
 deepsensor/model/defaults.py
 deepsensor/model/models.py
 deepsensor/model/nps.py
-deepsensor/plot/__init__.py
-deepsensor/plot/utils.py
 deepsensor/tensorflow/__init__.py
 deepsensor/torch/__init__.py
 deepsensor/train/__init__.py
 deepsensor/train/train.py
 tests/__init__.py
 tests/test_data_processor.py
 tests/test_model.py
```

### Comparing `deepsensor-0.1.1/setup.cfg` & `deepsensor-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepsensor
-version = 0.1.1
+version = 0.1.2
 author = Tom R. Andersson
 author_email = tomand@bas.ac.uk
 description = A Python package for modelling xarray and pandas data with neural processes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tom-andersson/deepsensor
 license = MIT
```

### Comparing `deepsensor-0.1.1/tests/test_data_processor.py` & `deepsensor-0.1.2/tests/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/tests/test_model.py` & `deepsensor-0.1.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/tests/test_task_loader.py` & `deepsensor-0.1.2/tests/test_task_loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.1/tests/utils.py` & `deepsensor-0.1.2/tests/utils.py`

 * *Files identical despite different names*

