# Comparing `tmp/dysweep-0.0.7.tar.gz` & `tmp/dysweep-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.0.7.tar", last modified: Mon Jun  5 19:42:42 2023, max compression
+gzip compressed data, was "dysweep-0.0.8.tar", last modified: Mon Jun 12 16:57:04 2023, max compression
```

## Comparing `dysweep-0.0.7.tar` & `dysweep-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:42:42.111350 dysweep-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 19:40:29.000000 dysweep-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-05 19:42:42.111350 dysweep-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-05 19:40:29.000000 dysweep-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:42:42.111350 dysweep-0.0.7/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 19:40:29.000000 dysweep-0.0.7/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-06-05 19:40:29.000000 dysweep-0.0.7/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21659 2023-06-05 19:40:29.000000 dysweep-0.0.7/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-05 19:40:29.000000 dysweep-0.0.7/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:42:42.111350 dysweep-0.0.7/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-05 19:42:42.000000 dysweep-0.0.7/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-05 19:42:42.000000 dysweep-0.0.7/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:42:42.000000 dysweep-0.0.7/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 19:42:42.000000 dysweep-0.0.7/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 19:42:42.111350 dysweep-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-05 19:40:29.000000 dysweep-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:57:04.072711 dysweep-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 16:54:49.000000 dysweep-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 16:57:04.072711 dysweep-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 16:54:49.000000 dysweep-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:57:04.068711 dysweep-0.0.8/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 16:54:49.000000 dysweep-0.0.8/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-12 16:54:49.000000 dysweep-0.0.8/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-06-12 16:54:49.000000 dysweep-0.0.8/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-12 16:54:49.000000 dysweep-0.0.8/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:57:04.068711 dysweep-0.0.8/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 16:57:04.000000 dysweep-0.0.8/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 16:57:04.000000 dysweep-0.0.8/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:57:04.000000 dysweep-0.0.8/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 16:57:04.000000 dysweep-0.0.8/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:57:04.072711 dysweep-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-12 16:54:49.000000 dysweep-0.0.8/setup.py
```

### Comparing `dysweep-0.0.7/LICENSE` & `dysweep-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.7/PKG-INFO` & `dysweep-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.7
+Version: 0.0.8
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.7/dysweep/parallel.py` & `dysweep-0.0.8/dysweep/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import functools
 from random_word import RandomWords
 import json
 import shutil
 import os
 import traceback
 import inspect
+import threading
 
 SPLIT = '-'
 
 
 @dataclass
 class ResumableSweepConfig:
     default_root_dir: th.Union[Path, str]
@@ -147,15 +148,15 @@
 
                     os.makedirs(checkpoint_dir / new_dir_name)
 
                     # dump a json in checkpoint_dir/run_id containing the sweep config
                     with open(checkpoint_dir / new_dir_name / "sweep_config.json", "w") as f:
                         json.dump(sweep_config, f, indent=4, sort_keys=True)
 
-                new_checkpoint_dir = checkpoint_dir / new_dir_name
+                    new_checkpoint_dir = checkpoint_dir / new_dir_name
             except Exception as e:
                 print(traceback.format_exc())
                 raise e
 
             if conf.use_lightning_logger:
                 # check the function signature matches
                 # the one we expect.
@@ -200,22 +201,32 @@
                     raise e
 
             # remove the entire new_checkpoint_dir if the function has finished
             # running.
             shutil.copyfile(new_checkpoint_dir / "sweep_config.json",
                             checkpoint_dir / f"{experiment_id}-config.json")
             shutil.rmtree(new_checkpoint_dir)
-
+            # finish the wandb run so that later .init calls can resume different ones
+            wandb.finish()
+            
             return ret
         
         
         if conf.resume:
             for _ in range(conf.count):
                 if check_non_empty(checkpoint_dir):
-                    modified_function()
+                    # run modified_function in a separate thread and wait for it to finish
+                    # before running the agent.
+                    # this is to ensure that the function is running before the agent
+                    # starts.
+                    modified_function_thread = threading.Thread(
+                        target=modified_function)
+                    modified_function_thread.start()
+                    modified_function_thread.join()
+                    
                 else:
                     break
         else:
             agent(conf.sweep_id, function=modified_function,
                   entity=conf.entity, project=conf.project, count=conf.count)
     else:
         try:
```

### Comparing `dysweep-0.0.7/dysweep/utils.py` & `dysweep-0.0.8/dysweep/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,20 +207,14 @@
                   root_args: th.Optional[th.Union[th.Dict, th.List]] = None):
     # try and catch an exception and add "line" to the exception and then re-raise it
     if current_path is None:
         current_path = []
     if root_args is None:
         root_args = args
 
-    # print("000000000000000-------000000000000000")
-    # print("args")
-    # pprint(args)
-    # print("sweep_config")
-    # pprint(sweep_config)
-
     try:
         if isinstance(args, list):
             if isinstance(sweep_config, dict):
                 if DY_LIST_OPERATIONS in sweep_config:
                     ops = sweep_config.pop(DY_LIST_OPERATIONS)
 
                     # Convert operations from dictionary to a list
```

### Comparing `dysweep-0.0.7/dysweep/wandbX.py` & `dysweep-0.0.8/dysweep/wandbX.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.7/dysweep.egg-info/PKG-INFO` & `dysweep-0.0.8/dysweep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.7
+Version: 0.0.8
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.7/setup.py` & `dysweep-0.0.8/setup.py`

 * *Files identical despite different names*

