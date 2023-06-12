# Comparing `tmp/easydags-0.0.7.tar.gz` & `tmp/easydags-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydags-0.0.7.tar", last modified: Fri Jun  9 14:30:28 2023, max compression
+gzip compressed data, was "easydags-0.1.0.tar", last modified: Mon Jun 12 08:01:26 2023, max compression
```

## Comparing `easydags-0.0.7.tar` & `easydags-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-09 14:30:28.705435 easydags-0.0.7/
--rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.7/LICENSE
--rw-r--r--   0 mateograciano   (501) staff       (20)    16755 2023-06-09 14:30:28.705155 easydags-0.0.7/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)    16560 2023-06-09 14:28:29.000000 easydags-0.0.7/README.md
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-09 14:30:28.703967 easydags-0.0.7/easydags/
--rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.7/easydags/__init__.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.7/easydags/config.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    22827 2023-06-09 14:25:30.000000 easydags-0.0.7/easydags/dag.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.7/easydags/errors.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    11304 2023-06-06 21:34:44.000000 easydags-0.0.7/easydags/node.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.7/easydags/ops.py
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-09 14:30:28.704879 easydags-0.0.7/easydags.egg-info/
--rw-r--r--   0 mateograciano   (501) staff       (20)    16755 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/SOURCES.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/dependency_links.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/requires.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-09 14:30:28.000000 easydags-0.0.7/easydags.egg-info/top_level.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.0.7/pyproject.toml
--rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-09 14:30:28.705492 easydags-0.0.7/setup.cfg
--rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-09 14:29:32.000000 easydags-0.0.7/setup.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-12 08:01:26.263112 easydags-0.1.0/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.1.0/LICENSE
+-rw-r--r--   0 mateograciano   (501) staff       (20)    20483 2023-06-12 08:01:26.262859 easydags-0.1.0/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)    20288 2023-06-12 07:57:01.000000 easydags-0.1.0/README.md
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-12 08:01:26.261669 easydags-0.1.0/easydags/
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.1.0/easydags/__init__.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.1.0/easydags/config.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    23016 2023-06-12 07:48:19.000000 easydags-0.1.0/easydags/dag.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.1.0/easydags/errors.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    12266 2023-06-12 07:39:41.000000 easydags-0.1.0/easydags/node.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)     3829 2023-06-12 07:21:06.000000 easydags-0.1.0/easydags/ops.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-12 08:01:26.262596 easydags-0.1.0/easydags.egg-info/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    20483 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/SOURCES.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/dependency_links.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/requires.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/top_level.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.1.0/pyproject.toml
+-rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-12 08:01:26.263170 easydags-0.1.0/setup.cfg
+-rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-12 07:57:43.000000 easydags-0.1.0/setup.py
```

### Comparing `easydags-0.0.7/LICENSE` & `easydags-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easydags-0.0.7/PKG-INFO` & `easydags-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydags
-Version: 0.0.7
+Version: 0.1.0
 Summary: Dags made easy
 Author: Mateo Graciano
 Author-email: magralo@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easydags: DAGs made easy
@@ -173,14 +173,110 @@
 dag = DAG(nodes,max_concurrency=2) #Create the DAG as the list of nodes
 
 dag.execute() # execute the dag
 
 ```
 
 
+#### Another way to define hard and soft dependencies
+
+Following the idea from airflow we can do the following
+
+- A>B B depends on A (soft)
+- A>>B B depends on A (hard)
+
+For example we can define the ensemble as
+
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def prepro():
+    #print('beginning pre pro')
+    time.sleep(3)
+    #print('end pre pro')
+    return 'df with cool features'
+
+
+
+node0 = ExecNode(id_= 'pre_process',
+              exec_function = prepro,
+              output_name = 'my_cool_df'
+              ) 
+
+
+def model1(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 1')
+    time.sleep(3)
+    print('finish training model1')
+    
+    return 'model 1 37803'
+
+node1 = ExecNode(id_= 'model1',
+              exec_function = model1 ,
+              output_name = 'model1'
+              )   
+
+
+
+def model2(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 2')
+    time.sleep(3)
+    print('finished training model2')
+    
+    return 'model 2 5678'
+
+node2 = ExecNode(id_= 'model2',
+              exec_function = model2 ,
+              output_name = 'model2'
+              ) 
+
+
+
+def ensemble(**kwargs):
+    model1 = kwargs['model1']
+    model2 = kwargs['model2']
+    
+    result = f'{model1} and {model2}'
+    
+    print(result)
+    
+    return result 
+
+node3= ExecNode(id_= 'ensemble',
+              exec_function = ensemble ,
+              depends_on_hard= ['model1','model2'],
+              output_name = 'ensemble'
+              ) 
+
+node0>>node1
+node0>>node2
+
+node1>>node3
+node2>>node3
+
+nodes = [node0, node1, node3, node2]
+
+
+
+
+dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
+
+dag.execute()
+```
+
+
 #### Defining the simple ensemble
 
 ``` python
 from easydags import  ExecNode, DAG
 import time
 
 nodes = []
@@ -315,14 +411,18 @@
               ) )   
 
 dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
 
 dag.execute()
 ```
 
+
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
+
+
 You can also only draw your DAG without executing (maybe if you only want to show the structure of your dag to someone or to paste it on your documentation)
 
 ```python
 #See draw_ensemble.py
 from easydags import  ExecNode, DAG
 import time
 
@@ -400,16 +500,14 @@
 dag.only_draw(name = 'green dag')
 
 dag.only_draw(name = 'yellow dag', color = 'yellow')
 
 ```
 
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
-
 
 #### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
 
 ```python
 
@@ -431,14 +529,104 @@
               max_concurrency=3, 
               debug = False,
               error_type_fatal= False)
 
 dag.execute() # if there is an error we wont raise an exception because error_type_fatal= False 
 ```
 
+#### Running your dag since your last checkpoint
+
+This is a very important feature of this library, the dag object stores the states of the nodes after one execution... if you run/execute your dag for a second time we will only run the nodes that failed or that did not run in the previous execution. As an example you can execute the following code (Please note that when a node wont run you will see the follwing message: "{self.id} already in finished state, wont run")
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def prepro():
+    #print('beginning pre pro')
+    time.sleep(3)
+    #print('end pre pro')
+    return 'df with cool features'
+
+
+
+node0 = ExecNode(id_= 'pre_process',
+              exec_function = prepro,
+              output_name = 'my_cool_df'
+              ) 
+
+
+def model1(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 1')
+    time.sleep(3)
+    print('finish training model1')
+    
+    return 'model 1 37803'
+
+node1 = ExecNode(id_= 'model1',
+              exec_function = model1 ,
+              output_name = 'model1'
+              )   
+
+
+
+def model2(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 2')
+    time.sleep(3)
+    print('finished training model2')
+    
+    return 'model 2 5678'
+
+node2 = ExecNode(id_= 'model2',
+              exec_function = model2 ,
+              output_name = 'model2'
+              ) 
+
+
+
+def ensemble(**kwargs):
+    model1 = kwargs['model1']
+    model2 = kwargs['model2']
+    
+    result = f'{model1} and {model2}'
+    
+    print(result)
+    
+    return result 
+
+node3= ExecNode(id_= 'ensemble',
+              exec_function = ensemble ,
+              depends_on_hard= ['model1','model2'],
+              output_name = 'ensemble'
+              ) 
+
+node0>>node1
+node0>>node2
+
+node1>>node3
+node2>>node3
+
+nodes = [node0, node1, node3, node2]
+
+
+dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
+
+dag.execute()
+    
+
+```
+
+
 
 
 ## Deploying your DAGs
 
 #### Deploying on serverless (GCP example)
 
 Basically the idea is that you can run one API where each endpoint is a different dag... as an example you can have the following api_example.py
```

### Comparing `easydags-0.0.7/README.md` & `easydags-0.1.0/easydags.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: easydags
+Version: 0.1.0
+Summary: Dags made easy
+Author: Mateo Graciano
+Author-email: magralo@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Easydags: DAGs made easy
 
 This library heavily inspired this package: https://github.com/mindee/tawazi, and a little bit by Airflow.
 
 
 ## Easy install using pypi
 You can easily install this in a separate conda envioronment with the following:
@@ -164,14 +173,110 @@
 dag = DAG(nodes,max_concurrency=2) #Create the DAG as the list of nodes
 
 dag.execute() # execute the dag
 
 ```
 
 
+#### Another way to define hard and soft dependencies
+
+Following the idea from airflow we can do the following
+
+- A>B B depends on A (soft)
+- A>>B B depends on A (hard)
+
+For example we can define the ensemble as
+
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def prepro():
+    #print('beginning pre pro')
+    time.sleep(3)
+    #print('end pre pro')
+    return 'df with cool features'
+
+
+
+node0 = ExecNode(id_= 'pre_process',
+              exec_function = prepro,
+              output_name = 'my_cool_df'
+              ) 
+
+
+def model1(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 1')
+    time.sleep(3)
+    print('finish training model1')
+    
+    return 'model 1 37803'
+
+node1 = ExecNode(id_= 'model1',
+              exec_function = model1 ,
+              output_name = 'model1'
+              )   
+
+
+
+def model2(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 2')
+    time.sleep(3)
+    print('finished training model2')
+    
+    return 'model 2 5678'
+
+node2 = ExecNode(id_= 'model2',
+              exec_function = model2 ,
+              output_name = 'model2'
+              ) 
+
+
+
+def ensemble(**kwargs):
+    model1 = kwargs['model1']
+    model2 = kwargs['model2']
+    
+    result = f'{model1} and {model2}'
+    
+    print(result)
+    
+    return result 
+
+node3= ExecNode(id_= 'ensemble',
+              exec_function = ensemble ,
+              depends_on_hard= ['model1','model2'],
+              output_name = 'ensemble'
+              ) 
+
+node0>>node1
+node0>>node2
+
+node1>>node3
+node2>>node3
+
+nodes = [node0, node1, node3, node2]
+
+
+
+
+dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
+
+dag.execute()
+```
+
+
 #### Defining the simple ensemble
 
 ``` python
 from easydags import  ExecNode, DAG
 import time
 
 nodes = []
@@ -306,14 +411,18 @@
               ) )   
 
 dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
 
 dag.execute()
 ```
 
+
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
+
+
 You can also only draw your DAG without executing (maybe if you only want to show the structure of your dag to someone or to paste it on your documentation)
 
 ```python
 #See draw_ensemble.py
 from easydags import  ExecNode, DAG
 import time
 
@@ -391,16 +500,14 @@
 dag.only_draw(name = 'green dag')
 
 dag.only_draw(name = 'yellow dag', color = 'yellow')
 
 ```
 
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
-
 
 #### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
 
 ```python
 
@@ -422,14 +529,104 @@
               max_concurrency=3, 
               debug = False,
               error_type_fatal= False)
 
 dag.execute() # if there is an error we wont raise an exception because error_type_fatal= False 
 ```
 
+#### Running your dag since your last checkpoint
+
+This is a very important feature of this library, the dag object stores the states of the nodes after one execution... if you run/execute your dag for a second time we will only run the nodes that failed or that did not run in the previous execution. As an example you can execute the following code (Please note that when a node wont run you will see the follwing message: "{self.id} already in finished state, wont run")
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def prepro():
+    #print('beginning pre pro')
+    time.sleep(3)
+    #print('end pre pro')
+    return 'df with cool features'
+
+
+
+node0 = ExecNode(id_= 'pre_process',
+              exec_function = prepro,
+              output_name = 'my_cool_df'
+              ) 
+
+
+def model1(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 1')
+    time.sleep(3)
+    print('finish training model1')
+    
+    return 'model 1 37803'
+
+node1 = ExecNode(id_= 'model1',
+              exec_function = model1 ,
+              output_name = 'model1'
+              )   
+
+
+
+def model2(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 2')
+    time.sleep(3)
+    print('finished training model2')
+    
+    return 'model 2 5678'
+
+node2 = ExecNode(id_= 'model2',
+              exec_function = model2 ,
+              output_name = 'model2'
+              ) 
+
+
+
+def ensemble(**kwargs):
+    model1 = kwargs['model1']
+    model2 = kwargs['model2']
+    
+    result = f'{model1} and {model2}'
+    
+    print(result)
+    
+    return result 
+
+node3= ExecNode(id_= 'ensemble',
+              exec_function = ensemble ,
+              depends_on_hard= ['model1','model2'],
+              output_name = 'ensemble'
+              ) 
+
+node0>>node1
+node0>>node2
+
+node1>>node3
+node2>>node3
+
+nodes = [node0, node1, node3, node2]
+
+
+dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
+
+dag.execute()
+    
+
+```
+
+
 
 
 ## Deploying your DAGs
 
 #### Deploying on serverless (GCP example)
 
 Basically the idea is that you can run one API where each endpoint is a different dag... as an example you can have the following api_example.py
@@ -579,8 +776,8 @@
 Basically the idea here is that you can create a different conda envioronment for each dag (or just one... do what you need here) and create bash script that:
 
 1. Activate the conda envioronment
 2. Run a python script with your dag
 
 After that you can use cronjobs to schedule your dags (please read how to use crontab -e on linux)
 
-You will need to to make the bash and python script executables with chmod +x {file}
+You will need to to make the bash and python script executables with chmod +x {file}
```

### Comparing `easydags-0.0.7/easydags/dag.py` & `easydags-0.1.0/easydags/dag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import time
-from concurrent.futures import ALL_COMPLETED, FIRST_COMPLETED, Future, ThreadPoolExecutor, wait
+from concurrent.futures import (
+    ALL_COMPLETED,
+    FIRST_COMPLETED,
+    Future,
+    ThreadPoolExecutor,
+    wait,
+)
 from copy import deepcopy
 from typing import Any, Dict, Hashable, List, Optional, Set, Tuple, Union
 
 import networkx as nx
 from loguru import logger
 from networkx import find_cycle
 from networkx.exception import NetworkXNoCycle, NetworkXUnfeasible
 
 import traceback
 
 from .errors import ErrorStrategy
 from .node import ExecNode
 from datetime import datetime
 
+
 # todo remove dependency on DiGraph!
 class DiGraphEx(nx.DiGraph):
     """
     Extends the DiGraph with some methods
     """
 
     def root_nodes(self) -> List[Hashable]:
@@ -125,15 +132,17 @@
         """
         Makes the simple topological sort of the graph nodes
         """
         return list(nx.topological_sort(self))
 
 
 # TODO: move into a separate module (Helper functions)
-def subgraph(graph: DiGraphEx, leaves_ids: Optional[List[Union[Hashable, ExecNode]]]) -> DiGraphEx:
+def subgraph(
+    graph: DiGraphEx, leaves_ids: Optional[List[Union[Hashable, ExecNode]]]
+) -> DiGraphEx:
     """returns a deep copy of the same graph if leaves_ids is None,
     otherwise returns a new graph by applying `graph.subgraph_leaves`
 
     Args:
         graph (DiGraphEx): graph describing the DAG
         leaves_ids (List[Union[Hashable, ExecNode]]): The leaves that must be executed
 
@@ -145,15 +154,16 @@
     graph = deepcopy(graph)
 
     # TODO: make the creation of subgraph possible directly from initialization
     # 1. create the subgraph
     if leaves_ids is not None:
         # Extract the ids from the provided leaves/leaves_ids
         leaves_ids = [
-            node_id.id if isinstance(node_id, ExecNode) else node_id for node_id in leaves_ids
+            node_id.id if isinstance(node_id, ExecNode) else node_id
+            for node_id in leaves_ids
         ]
 
         graph.subgraph_leaves(leaves_ids)
 
     return graph
 
 
@@ -164,43 +174,45 @@
         * Limited number of threads.
         * Parallelization constraint of each ExecNode (is_sequential attribute)
     """
 
     def __init__(
         self,
         exec_nodes: List[ExecNode],
-        name: str = 'DAG',
+        name: str = "DAG",
         max_concurrency: int = 1,
         debug: bool = True,
         error_type_fatal: bool = True,
-        draw: bool = True
+        draw: bool = True,
     ):
         """
         Args:
             exec_nodes: all the ExecNodes
             max_concurrency: the maximal number of threads running in parallel
             name: Name of the dag, will be usefull for creating the html output
             degub: weather or not you want degub messages
             error_type_fatal: weather or not you want the whole process to fail if at least one node fails
             draw: Set false if you do not want the html output
 
         """
         self.graph_ids = DiGraphEx()
-    
+
         self.name = name
 
         self.debug = debug
         self.draw = draw
 
         self.error_type_fatal = error_type_fatal
         # since ExecNodes are modified they must be copied
         self.exec_nodes = exec_nodes
 
         self.max_concurrency = int(max_concurrency)
-        assert max_concurrency >= 1, "Invalid maximum number of threads! Must be a positive integer"
+        assert (
+            max_concurrency >= 1
+        ), "Invalid maximum number of threads! Must be a positive integer"
 
         # variables necessary for DAG construction
         self.backwards_hierarchy: Dict[Hashable, List[Hashable]] = {
             exec_node.id: exec_node.depends_on for exec_node in self.exec_nodes
         }
         self.node_dict: Dict[Hashable, ExecNode] = {
             exec_node.id: exec_node for exec_node in self.exec_nodes
@@ -254,15 +266,17 @@
 
         # set sequence order
         topological_order = self.graph_ids.topological_sort()
 
         # calculate the sum of priorities of all recursive children
         self.assign_recursive_children_compound_priority()
 
-        self.exec_node_sequence = [self.node_dict[node_name] for node_name in topological_order]
+        self.exec_node_sequence = [
+            self.node_dict[node_name] for node_name in topological_order
+        ]
 
     def assign_recursive_children_compound_priority(self) -> None:
         """
         Assigns a compound priority to all nodes in the graph.
         The compound priority is the sum of the priorities of all children recursively.
         """
         # Note: if there was a forward dependency recorded, this would have been much easier
@@ -272,267 +286,234 @@
 
         # 2. assign the compound priority for all the remaining nodes in the graph:
         # Priority assignment happens by epochs:
         # 2.1. during every epoch, we assign the compound priority for the parents of the current leaf nodes
         # 2.2. at the end of every epoch, we trim the graph from its leaf nodes;
         #       hence the previous parents become the new leaf nodes
         while len(graph_ids) > 0:
-
             # Epoch level
             for leaf_id in leaf_ids:
                 leaf_node = self.node_dict[leaf_id]
 
                 for parent_id in self.backwards_hierarchy[leaf_id]:
                     # increment the compound_priority of the parent node by the leaf priority
                     parent_node = self.node_dict[parent_id]
                     parent_node.compound_priority += leaf_node.compound_priority
 
                 # trim the graph from its leaf nodes
                 graph_ids.remove_node(leaf_id)
 
             # assign the new leaf nodes
             leaf_ids = graph_ids.leaf_nodes()
-    
-    def only_draw(self, name = None, color = 'green') -> None:
+
+    def only_draw(self, name=None, color="green") -> None:
         """
         Draws the Networkx directed graph.
         Args:
             k: parameter for the layout of the graph, the higher, the further the nodes apart
             display: display the layout created
             t: time to display in seconds
         """
 
         if name is None:
             name = self.name
 
-
         for layer, nodes in enumerate(nx.topological_generations(self.graph_ids)):
             # `multipartite_layout` expects the layer as a node attribute, so add the
             # numeric layer value as a node attribute
             for node in nodes:
                 self.graph_ids.nodes[node]["layer"] = layer
 
         # Compute the multipartite_layout using the "layer" node attribute
         pos = nx.multipartite_layout(self.graph_ids, subset_key="layer")
-        
 
         from pyvis.network import Network
 
-        
-
         head_title = f"{self.name} structure"
 
-        g = Network(layout=True,directed =True,heading=head_title)
-
+        g = Network(layout=True, directed=True, heading=head_title)
 
         titles = []
-        color_map = [] 
-        
-        for f in  list(pos.keys()):
-            title = f'''id: {f}'''
+        color_map = []
+
+        for f in list(pos.keys()):
+            title = f"""id: {f}"""
             titles.append(title)
             color_map.append(color)
 
-
-
-        aux = [x[0]   for x in pos.values()]
+        aux = [x[0] for x in pos.values()]
 
         pos_holder = list(set(aux))
 
         pos_holder.sort()
 
-        
-
         level = [pos_holder.index(i) for i in aux]
 
-
         for i in range(len(pos.keys())):
-            g.add_node(list(pos.keys())[i],
-                         label= list(pos.keys())[i],
-                         level = level[i],
-                         title = titles[i],
-                         color= color_map[i])
-            
-
-        #g = Network('500px', '500px')
-
-
+            g.add_node(
+                list(pos.keys())[i],
+                label=list(pos.keys())[i],
+                level=level[i],
+                title=titles[i],
+                color=color_map[i],
+            )
 
+        # g = Network('500px', '500px')
 
-        for e in self.graph_ids.edges :
-            
-            g.add_edge(e[0],e[1])
-            
+        for e in self.graph_ids.edges:
+            g.add_edge(e[0], e[1])
 
-        g.set_options('''
+        g.set_options(
+            """
         var options = {
             "layout": {
                 "hierarchical": {
                     "enabled": true,
                     "direction": "LR",  
                     "sortMethod": "directed"
                 }
             },
             "physics": {
                 "enabled": false
             }
         }
-        ''')
+        """
+        )
 
+        html_file_name = f"{name}_structure.html"
+        g.show(html_file_name)
 
-        
+        import re
 
-        html_file_name = f'{name}_structure.html'
-        g.show( html_file_name)
-        
-
-        import re 
-        html_str = re.sub(r'<center>.+?<\/h1>\s+<\/center>', '', g.html, 1, re.DOTALL)
-        h = open( html_file_name,'w')
+        html_str = re.sub(r"<center>.+?<\/h1>\s+<\/center>", "", g.html, 1, re.DOTALL)
+        h = open(html_file_name, "w")
         h.write(html_str)
         h.close()
-        
 
     def _draw(self) -> None:
         """
         Draws the Networkx directed graph.
         Args:
             k: parameter for the layout of the graph, the higher, the further the nodes apart
             display: display the layout created
             t: time to display in seconds
         """
 
-
         for layer, nodes in enumerate(nx.topological_generations(self.graph_ids)):
             # `multipartite_layout` expects the layer as a node attribute, so add the
             # numeric layer value as a node attribute
             for node in nodes:
                 self.graph_ids.nodes[node]["layer"] = layer
 
         # Compute the multipartite_layout using the "layer" node attribute
         pos = nx.multipartite_layout(self.graph_ids, subset_key="layer")
-        
 
-
-        print('drawing')
+        print("drawing")
 
         aux = self.node_dict
 
-
         from pyvis.network import Network
 
-        
-
         # datetime object containing current date and time
-        
 
         head_title = f"{self.name} execution states after run at {self.dt_string}"
 
-        g = Network(layout=True,directed =True,heading=head_title)
-
+        g = Network(layout=True, directed=True, heading=head_title)
 
         titles = []
-        color_map = [] 
-        
-        for f in  list(pos.keys()):
-            state = aux[f].result['state']
-            m = aux[f].result['message']
-            initial = aux[f].result['initial_time']
-            final = aux[f].result['final_time']
-            duration = aux[f].result['duration']
-            title = f'''id: {f}
+        color_map = []
+
+        for f in list(pos.keys()):
+            state = aux[f].result["state"]
+            m = aux[f].result["message"]
+            initial = aux[f].result["initial_time"]
+            final = aux[f].result["final_time"]
+            duration = aux[f].result["duration"]
+            title = f"""id: {f}
                         started at: {initial} and finished at {final}
                         exec_time: {duration}
                         state: {state}
-                        message: {m}'''
+                        message: {m}"""
             titles.append(title)
-            
-            if state == 0  :
-                color_map.append('grey')
-            if state == 1  :
-                color_map.append('green')
-            if state == -1  :
-                color_map.append('red')
 
+            if state == 0:
+                color_map.append("grey")
+            if state == 1:
+                color_map.append("green")
+            if state == -1:
+                color_map.append("red")
 
-        aux = [x[0]   for x in pos.values()]
+        aux = [x[0] for x in pos.values()]
 
         pos_holder = list(set(aux))
 
         pos_holder.sort()
 
-        
-
         level = [pos_holder.index(i) for i in aux]
 
-
         for i in range(len(pos.keys())):
-            g.add_node(list(pos.keys())[i],
-                         label= list(pos.keys())[i],
-                         level = level[i],
-                         title = titles[i],
-                         color= color_map[i])
-            
+            g.add_node(
+                list(pos.keys())[i],
+                label=list(pos.keys())[i],
+                level=level[i],
+                title=titles[i],
+                color=color_map[i],
+            )
 
-        #g = Network('500px', '500px')
+        # g = Network('500px', '500px')
 
         for key in pos.keys():
             x = pos[key][0]
-            y = pos[key][1] 
-            
-
-
-
+            y = pos[key][1]
 
-        for e in self.graph_ids.edges :
-            
-            g.add_edge(e[0],e[1])
-            
+        for e in self.graph_ids.edges:
+            g.add_edge(e[0], e[1])
 
-        g.set_options('''
+        g.set_options(
+            """
         var options = {
             "layout": {
                 "hierarchical": {
                     "enabled": true,
                     "direction": "LR",  
                     "sortMethod": "directed"
                 }
             },
             "physics": {
                 "enabled": false
             }
         }
-        ''')
+        """
+        )
 
-        html_file_name = f'{self.name}_states_run.html'
-        g.show( html_file_name)
-        
+        html_file_name = f"{self.name}_states_run.html"
+        g.show(html_file_name)
+
+        import re
 
-        import re 
-        html_str = re.sub(r'<center>.+?<\/h1>\s+<\/center>', '', g.html, 1, re.DOTALL)
-        h = open( html_file_name,'w')
+        html_str = re.sub(r"<center>.+?<\/h1>\s+<\/center>", "", g.html, 1, re.DOTALL)
+        h = open(html_file_name, "w")
         h.write(html_str)
         h.close()
 
-        
-
     def execute(
         self, leaves_ids: Optional[List[Union[Hashable, ExecNode]]] = None
     ) -> Dict[Hashable, Any]:
         """
         Thread safe execution of the DAG.
         Args:
             leaves_ids: The nodes (or the ids of the nodes) to be executed
         Returns:
             node_dict: dictionary with keys the name of the function and value the result after the execution
         """
 
         from datetime import datetime
+
         now = datetime.now()
-        
+
         self.dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
         # 0.1 create a subgraph of the graph if necessary
         graph = subgraph(self.graph_ids, leaves_ids)
 
         # 0.2 deepcopy the node_dict in order to modify the results inside every node
         node_dict = deepcopy(self.node_dict)
 
@@ -563,15 +544,18 @@
                 #    this can occur in two cases:
                 #       1. if maximum concurrency is reached
                 #       2. if no runnable node exists (i.e. all root nodes are being executed)
                 #    in both cases: block until a node finishes
                 #       => a new root node will be available
                 num_running_threads = get_num_running_threads(futures)
                 num_runnable_nodes_ids = len(runnable_nodes_ids)
-                if num_running_threads == self.max_concurrency or num_runnable_nodes_ids == 0:
+                if (
+                    num_running_threads == self.max_concurrency
+                    or num_runnable_nodes_ids == 0
+                ):
                     # must wait and not submit any workers before a worker ends
                     # (that might create a new more prioritized node) to be executed
                     if self.debug:
                         logger.debug(
                             f"Waiting for ExecNodes {running} to finish. Finished running {done}"
                         )
                     done_, running = wait(running, return_when=FIRST_COMPLETED)
@@ -601,19 +585,19 @@
                 # 4.1 get the most prioritized node to run
                 # 4.1.1 get all the nodes that have the highest priority
                 runnable_nodes = [node_dict[node_id] for node_id in runnable_nodes_ids]
                 highest_priority_nodes = get_highest_priority_nodes(runnable_nodes)
 
                 # 4.1.2 get the node with the highest compound priority
                 # (randomly selected if multiple are suggested)
-                exec_node = sorted(highest_priority_nodes, key=lambda node: node.compound_priority)[
-                    -1
-                ]
+                exec_node = sorted(
+                    highest_priority_nodes, key=lambda node: node.compound_priority
+                )[-1]
 
-                logger.info(f"{exec_node.id} will run!")
+                # logger.info(f"{exec_node.id} will run!")
 
                 # 4.2 if the current node must be run sequentially, wait for a running node to finish.
                 # in that case we must prune the graph to re-check whether a new root node
                 # (maybe with a higher priority) has been created => continue the loop
                 # Note: This step might run a number of times in the while loop
                 #       before the exec_node gets submitted
                 num_running_threads = get_num_running_threads(futures)
@@ -624,42 +608,50 @@
                             f"Wait for the end of a node in {running}"
                         )
                     done_, running = wait(running, return_when=FIRST_COMPLETED)
                     # go to step 6
                     continue
 
                 # 5.1 submit the exec node to the executor
-                exec_future = executor.submit(exec_node.execute, 
-                                              node_dict=node_dict, 
-                                              debug = self.debug,
-                                              initial_time = datetime.now().strftime("%Y-%m-%d, %H:%M:%S"))
+                if exec_node.state !=1:
+                    exec_future = executor.submit(
+                        exec_node.execute,
+                        node_dict=node_dict,
+                        debug=self.debug,
+                        initial_time=datetime.now().strftime("%Y-%m-%d, %H:%M:%S"),
+                    )
+                    
+                else:
+                    
+                    logger.info(f"{exec_node.id} already in finished state, wont run")
+                    exec_future = executor.submit(
+                        lambda : print('')
+                    )
+
                 running.add(exec_future)
                 futures[exec_node.id] = exec_future
 
                 # 5.2 wait for the sequential node to finish
                 # TODO: not sure this code ever runs
                 if exec_node.is_sequential:
                     wait(futures.values(), return_when=ALL_COMPLETED)
         self.node_dict = node_dict
-        
+
         if self.draw:
             self._draw()
 
-        states = [node_dict[x].result['state'] for x in node_dict]
-
-        if (min(states)!=1) and (self.error_type_fatal):
-            raise ValueError('DAG did not finished as expected')
+        states = [node_dict[x].result["state"] for x in node_dict]
+        
+        if (min(states) != 1) and (self.error_type_fatal):
+            raise ValueError("DAG did not finished as expected")
 
         return self
 
-
-
-    def handle_exception(self, graph: DiGraphEx, fut: "Future[Any]", id_: Hashable) -> None:
+    def handle_exception(
+        self, graph: DiGraphEx, fut: "Future[Any]", id_: Hashable
+    ) -> None:
         """
         This simply raise an error if any
 
         """
 
-
         _res = fut.result()  # noqa: F841
-
-
```

### Comparing `easydags-0.0.7/easydags/node.py` & `easydags-0.1.0/easydags/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 
 # TODO: replace exec_nodes with dict
 # a temporary variable used to pass in exec_nodes to the DAG during building
 exec_nodes: List["ExecNode"] = []
 exec_nodes_lock = Lock()
 from datetime import datetime
 
+
 class ExecNode:
     """
     This class is the base executable node of the Directed Acyclic Execution Graph
     """
+
     def __init__(
         self,
         id_: Hashable,
         exec_function: Callable[..., Any] = lambda **kwargs: None,
         depends_on_hard: Optional[List[Hashable]] = [],
         depends_on_soft: Optional[List[Hashable]] = [],
         output_name: Optional[str] = None,
@@ -40,148 +42,184 @@
             priority (int, optional): priority compared to other ExecNodes;
                 the higher the number the higher the priority.
             is_sequential (bool, optional): whether to execute this ExecNode in sequential order with respect to others.
              When this ExecNode must be executed, all other nodes are waited to finish before starting execution.
              Defaults to False.
         """
 
-
-
         self.id = id_
         self.exec_function = exec_function
 
         depends_on = depends_on_hard.copy()
         depends_on.extend(depends_on_soft)
-        self.depends_on = depends_on 
+        self.depends_on = depends_on
         self.depends_on_hard = depends_on_hard
         self.priority: int = priority
         self.compound_priority: int = priority
         self.n_trials: int = n_trials
         self.is_sequential = is_sequential
+        self.state = 0
 
         # a string that identifies the ExecNode.
         # It is either the name of the identifying function or the identifying string id_
         self.__name__ = self.exec_function.__name__ if not isinstance(id_, str) else id_
 
         # Attempt to automatically assign a good enough argument name
         if isinstance(output_name, str) and output_name != "":
             self.argument_name = output_name
         else:
-            #self.argument_name = (
+            # self.argument_name = (
             #    self.id.__name__ if isinstance(self.id, FunctionType) else str(self.id)
-            #)
-            self.argument_name = f'{str(self.id)}_result' 
+            # )
+            self.argument_name = f"{str(self.id)}_result"
 
         # todo remove and make ExecNode immutable
         self.result: Optional[Dict[str, Any]] = None
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__} {self.id} ~ | <{hex(id(self))}>"
 
     @property
     def computed_dependencies(self) -> bool:
         return isinstance(self.depends_on, list)
 
+    def _add_soft_dependency(self, other):
+        depends_on = other.depends_on.copy()
+
+        depends_on.insert(0, self.id)
+
+        other.depends_on = depends_on
+
+        return self
+
+    def __gt__(self, other):
+        # soft dependency
+
+        aux = self._add_soft_dependency(other)
+
+        return aux
+
+    def _add_hard_dependency(self, other):
+        depends_on = other.depends_on.copy()
+        depends_on_hard = other.depends_on_hard.copy()
+
+        depends_on.insert(0, self.id)
+        depends_on_hard.insert(0, self.id)
+
+        other.depends_on = depends_on
+        other.depends_on_hard = depends_on_hard
+
+        return other
+
+    def __rshift__(self, other):
+        # hard dependency
+        aux = self._add_hard_dependency(other)
+
+        return aux
+
     # this is breaking change however
-    def execute(self, 
-                node_dict: Dict[Hashable, "ExecNode"], 
-                debug: bool = True,
-                initial_time: str = datetime.now().strftime("%Y-%m-%d, %H:%M:%S")) -> Optional[Dict[str, Any]]:
+    def execute(
+        self,
+        node_dict: Dict[Hashable, "ExecNode"],
+        debug: bool = True,
+        initial_time: str = datetime.now().strftime("%Y-%m-%d, %H:%M:%S"),
+    ) -> Optional[Dict[str, Any]]:
         """
         Execute the ExecNode directly or according to an execution graph.
         Args:
             node_dict (Dict[Hashable, ExecNode]): A shared dictionary containing the other ExecNodes in the DAG;
                                                 the key is the id of the ExecNode.
 
         Returns: the result of the execution of the current ExecNode
         """
         logger.info(f"Start executing {self.id} at {initial_time}")
         # 1. fabricate the arguments for this ExecNode
         if debug:
             logger.debug(f"Start executing {self.id} with task {self.exec_function}")
 
         kwargs = {
-            node_dict[dep_hash].argument_name: node_dict[dep_hash].result['result']
+            node_dict[dep_hash].argument_name: node_dict[dep_hash].result["result"]
             for dep_hash in self.depends_on_hard
         }
 
         prev_states = {
-            node_dict[dep_hash].argument_name: node_dict[dep_hash].result['state']
+            node_dict[dep_hash].argument_name: node_dict[dep_hash].result["state"]
             for dep_hash in self.depends_on
         }
 
         prev_states = [x[1] for x in list(prev_states.items())]
-        
-        result = {}
 
-        error = ''
+        result = {}
 
-        if len(prev_states)>0:
-            
-            
-            if (min(prev_states)==1): #all prev nodes are ok
+        error = ""
 
-                i = 0 
+        if len(prev_states) > 0:
+            if min(prev_states) == 1:  # all prev nodes are ok
+                i = 0
 
                 while i < self.n_trials:
                     try:
-                        result['result'] = self.exec_function(**kwargs)
-                        result['state'] = 1
-                        result['message'] = 'Executed as expected' 
-                        break # no need for re-trials
+                        result["result"] = self.exec_function(**kwargs)
+                        result["state"] = 1
+                        result["message"] = "Executed as expected"
+                        self.state = 1
+                        break  # no need for re-trials
                     except:
-                        result['result'] = None
-                        result['state'] = -1
-                        
+                        result["result"] = None
+                        result["state"] = -1
+
                         error = traceback.format_exc()
                         msg = f"The error when executing {self.id} on trial {i+1} : {error}"
-                        result['message'] = msg
+                        result["message"] = msg
+                        self.state = -1
                         logger.info(msg)
-                    i+=1
+                    i += 1
             else:
-                result['result'] = None
-                result['state'] = 0
-                result['message'] = 'Did not run'
+                result["result"] = None
+                result["state"] = 0
+                result["message"] = "Did not run"
+                self.state = 0
 
         else:
-            i = 0 
+            i = 0
 
             while i < self.n_trials:
                 try:
-                    result['result'] = self.exec_function(**kwargs)
-                    result['state'] = 1
-                    result['message'] = 'Executed as expected' 
-                    break # no need for re-trials
+                    result["result"] = self.exec_function(**kwargs)
+                    result["state"] = 1
+                    result["message"] = "Executed as expected"
+                    self.state = 1
+                    break  # no need for re-trials
                 except:
-                    result['result'] = None
-                    result['state'] = -1     
+                    result["result"] = None
+                    result["state"] = -1
                     error = traceback.format_exc()
                     msg = f"The error when executing {self.id} on trial {i+1} : {error}"
-                    result['message'] = msg
+                    result["message"] = msg
+                    self.state = -1
                     logger.info(msg)
-                i+=1
-
-        
-            
+                i += 1
 
-        result['initial_time'] = initial_time
+        result["initial_time"] = initial_time
         final = datetime.now().strftime("%Y-%m-%d, %H:%M:%S")
-        result['final_time'] = final
-        result['duration'] = (datetime.strptime(initial_time,"%Y-%m-%d, %H:%M:%S")-datetime.strptime(final,"%Y-%m-%d, %H:%M:%S")).total_seconds()
-        result['duration'] = str(-int(result['duration']))+ ' sec'
+        result["final_time"] = final
+        result["duration"] = (
+            datetime.strptime(initial_time, "%Y-%m-%d, %H:%M:%S")
+            - datetime.strptime(final, "%Y-%m-%d, %H:%M:%S")
+        ).total_seconds()
+        result["duration"] = str(-int(result["duration"])) + " sec"
 
         self.result = result
 
         # 3. useless return value
         if debug:
             logger.debug(f"Finished executing {self.id} with task {self.exec_function}")
         return result
 
 
-
 class PreComputedExecNode(ExecNode):
     # todo must change this because two functions in the same DAG can use the same argument name for two constants!
     def __init__(self, func: Callable[..., Any], argument_name: str, value: Any):
         super().__init__(
             id_=f"{hash(func)}_{argument_name}",
             exec_function=lambda: value,
             depends_on=[],
@@ -260,15 +298,17 @@
             provided_arguments_names.add(function_arguments_names[i])
 
         for argument_name, arg in kwargs.items():
             if isinstance(arg, LazyExecNode):
                 dependencies.append(arg.id)
             else:
                 # if the argument is a custom or constant
-                pre_c_exec_node = PreComputedExecNode(self.exec_function, argument_name, arg)
+                pre_c_exec_node = PreComputedExecNode(
+                    self.exec_function, argument_name, arg
+                )
                 exec_nodes.append(pre_c_exec_node)
                 dependencies.append(pre_c_exec_node.id)
 
             provided_arguments_names.add(argument_name)
 
         # Fill default valued parameters with default values if they aren't provided by the user
         default_valued_params = get_default_args(self.exec_function)
```

### Comparing `easydags-0.0.7/easydags/ops.py` & `easydags-0.1.0/easydags/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .node import LazyExecNode, exec_nodes_lock
 
 
 # TODO: modify is_sequential's default value according to the pre used default
 def op(
     id_,
     func: Optional[Callable[..., Any]] = None,
-    depends_on = [],
+    depends_on=[],
     *,
     priority: int = 0,
     argument_name: Optional[str] = None,
     is_sequential: bool = Cfg.TAWAZI_IS_SEQUENTIAL,
 ) -> "LazyExecNode":
     """
     Decorate a function to make it an ExecNode. When the decorated function is called, you are actually calling
@@ -34,15 +34,17 @@
         is_sequential: whether to allow the execution of this ExecNode with others or not
 
     Returns:
         LazyExecNode
     """
 
     def my_custom_op(_func: Callable[..., Any]) -> "LazyExecNode":
-        lazy_exec_node = LazyExecNode(id_,_func,depends_on, priority, argument_name, is_sequential)
+        lazy_exec_node = LazyExecNode(
+            id_, _func, depends_on, priority, argument_name, is_sequential
+        )
         functools.update_wrapper(lazy_exec_node, _func)
         return lazy_exec_node
 
     # case #1: arguments are provided to the decorator
     if func is None:
         return my_custom_op  # type: ignore
     # case #2: no argument is provided to the decorator
@@ -75,15 +77,17 @@
 
     def intermediate_wrapper(_func: Callable[..., Any]) -> Callable[..., DAG]:
         def wrapped(*args: Any, **kwargs: Any) -> DAG:
             # TODO: modify this horrible pattern
             with exec_nodes_lock:
                 node.exec_nodes = []
                 _func(*args, **kwargs)
-                d = DAG(node.exec_nodes, max_concurrency=max_concurrency, behavior=behavior)
+                d = DAG(
+                    node.exec_nodes, max_concurrency=max_concurrency, behavior=behavior
+                )
                 node.exec_nodes = []
 
             return d
 
         return wrapped
 
     # case 1: arguments are provided to the decorator
```

### Comparing `easydags-0.0.7/easydags.egg-info/PKG-INFO` & `easydags-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: easydags
-Version: 0.0.7
-Summary: Dags made easy
-Author: Mateo Graciano
-Author-email: magralo@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Easydags: DAGs made easy
 
 This library heavily inspired this package: https://github.com/mindee/tawazi, and a little bit by Airflow.
 
 
 ## Easy install using pypi
 You can easily install this in a separate conda envioronment with the following:
@@ -173,14 +164,110 @@
 dag = DAG(nodes,max_concurrency=2) #Create the DAG as the list of nodes
 
 dag.execute() # execute the dag
 
 ```
 
 
+#### Another way to define hard and soft dependencies
+
+Following the idea from airflow we can do the following
+
+- A>B B depends on A (soft)
+- A>>B B depends on A (hard)
+
+For example we can define the ensemble as
+
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def prepro():
+    #print('beginning pre pro')
+    time.sleep(3)
+    #print('end pre pro')
+    return 'df with cool features'
+
+
+
+node0 = ExecNode(id_= 'pre_process',
+              exec_function = prepro,
+              output_name = 'my_cool_df'
+              ) 
+
+
+def model1(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 1')
+    time.sleep(3)
+    print('finish training model1')
+    
+    return 'model 1 37803'
+
+node1 = ExecNode(id_= 'model1',
+              exec_function = model1 ,
+              output_name = 'model1'
+              )   
+
+
+
+def model2(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 2')
+    time.sleep(3)
+    print('finished training model2')
+    
+    return 'model 2 5678'
+
+node2 = ExecNode(id_= 'model2',
+              exec_function = model2 ,
+              output_name = 'model2'
+              ) 
+
+
+
+def ensemble(**kwargs):
+    model1 = kwargs['model1']
+    model2 = kwargs['model2']
+    
+    result = f'{model1} and {model2}'
+    
+    print(result)
+    
+    return result 
+
+node3= ExecNode(id_= 'ensemble',
+              exec_function = ensemble ,
+              depends_on_hard= ['model1','model2'],
+              output_name = 'ensemble'
+              ) 
+
+node0>>node1
+node0>>node2
+
+node1>>node3
+node2>>node3
+
+nodes = [node0, node1, node3, node2]
+
+
+
+
+dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
+
+dag.execute()
+```
+
+
 #### Defining the simple ensemble
 
 ``` python
 from easydags import  ExecNode, DAG
 import time
 
 nodes = []
@@ -315,14 +402,18 @@
               ) )   
 
 dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
 
 dag.execute()
 ```
 
+
+![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
+
+
 You can also only draw your DAG without executing (maybe if you only want to show the structure of your dag to someone or to paste it on your documentation)
 
 ```python
 #See draw_ensemble.py
 from easydags import  ExecNode, DAG
 import time
 
@@ -400,16 +491,14 @@
 dag.only_draw(name = 'green dag')
 
 dag.only_draw(name = 'yellow dag', color = 'yellow')
 
 ```
 
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
-
 
 #### Another last cool feature: The number of trials
 
 There are some cases where simply rerunning your task is enough... that is why we implemented this feature; we can set several trials with the parameters n_trials in the creations of each node.
 
 ```python
 
@@ -431,14 +520,104 @@
               max_concurrency=3, 
               debug = False,
               error_type_fatal= False)
 
 dag.execute() # if there is an error we wont raise an exception because error_type_fatal= False 
 ```
 
+#### Running your dag since your last checkpoint
+
+This is a very important feature of this library, the dag object stores the states of the nodes after one execution... if you run/execute your dag for a second time we will only run the nodes that failed or that did not run in the previous execution. As an example you can execute the following code (Please note that when a node wont run you will see the follwing message: "{self.id} already in finished state, wont run")
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def prepro():
+    #print('beginning pre pro')
+    time.sleep(3)
+    #print('end pre pro')
+    return 'df with cool features'
+
+
+
+node0 = ExecNode(id_= 'pre_process',
+              exec_function = prepro,
+              output_name = 'my_cool_df'
+              ) 
+
+
+def model1(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 1')
+    time.sleep(3)
+    print('finish training model1')
+    
+    return 'model 1 37803'
+
+node1 = ExecNode(id_= 'model1',
+              exec_function = model1 ,
+              output_name = 'model1'
+              )   
+
+
+
+def model2(**kwargs):
+    df = kwargs['my_cool_df']
+    
+    #print(f'i am using {df} in model 2')
+    time.sleep(3)
+    print('finished training model2')
+    
+    return 'model 2 5678'
+
+node2 = ExecNode(id_= 'model2',
+              exec_function = model2 ,
+              output_name = 'model2'
+              ) 
+
+
+
+def ensemble(**kwargs):
+    model1 = kwargs['model1']
+    model2 = kwargs['model2']
+    
+    result = f'{model1} and {model2}'
+    
+    print(result)
+    
+    return result 
+
+node3= ExecNode(id_= 'ensemble',
+              exec_function = ensemble ,
+              depends_on_hard= ['model1','model2'],
+              output_name = 'ensemble'
+              ) 
+
+node0>>node1
+node0>>node2
+
+node1>>node3
+node2>>node3
+
+nodes = [node0, node1, node3, node2]
+
+
+dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
+
+dag.execute()
+    
+
+```
+
+
 
 
 ## Deploying your DAGs
 
 #### Deploying on serverless (GCP example)
 
 Basically the idea is that you can run one API where each endpoint is a different dag... as an example you can have the following api_example.py
@@ -588,8 +767,8 @@
 Basically the idea here is that you can create a different conda envioronment for each dag (or just one... do what you need here) and create bash script that:
 
 1. Activate the conda envioronment
 2. Run a python script with your dag
 
 After that you can use cronjobs to schedule your dags (please read how to use crontab -e on linux)
 
-You will need to to make the bash and python script executables with chmod +x {file}
+You will need to to make the bash and python script executables with chmod +x {file}
```

### Comparing `easydags-0.0.7/setup.py` & `easydags-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'easydags',         # How you named your package folder (MyLib)
   packages = ['easydags'],   # Chose the same as "name"
-  version = '0.0.7',      # Start with a small number and increase it with every change you make
+  version = '0.1.0',      # Start with a small number and increase it with every change you make
   description = 'Dags made easy',   # Give a short description about your library
   author = 'Mateo Graciano',                   # Type in your name
   author_email = 'magralo@gmail.com',      # Type in your E-Mail
   install_requires=[            # I get to this in a second
           'networkx==2.6.3',
           'pydantic==1.10',
           'loguru==0.6.0',
```

