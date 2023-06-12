# Comparing `tmp/easydags-0.1.0.tar.gz` & `tmp/easydags-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydags-0.1.0.tar", last modified: Mon Jun 12 08:01:26 2023, max compression
+gzip compressed data, was "easydags-0.1.1.tar", last modified: Mon Jun 12 08:12:17 2023, max compression
```

## Comparing `easydags-0.1.0.tar` & `easydags-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-12 08:01:26.263112 easydags-0.1.0/
--rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.1.0/LICENSE
--rw-r--r--   0 mateograciano   (501) staff       (20)    20483 2023-06-12 08:01:26.262859 easydags-0.1.0/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)    20288 2023-06-12 07:57:01.000000 easydags-0.1.0/README.md
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-12 08:01:26.261669 easydags-0.1.0/easydags/
--rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.1.0/easydags/__init__.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.1.0/easydags/config.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    23016 2023-06-12 07:48:19.000000 easydags-0.1.0/easydags/dag.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.1.0/easydags/errors.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    12266 2023-06-12 07:39:41.000000 easydags-0.1.0/easydags/node.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)     3829 2023-06-12 07:21:06.000000 easydags-0.1.0/easydags/ops.py
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-12 08:01:26.262596 easydags-0.1.0/easydags.egg-info/
--rw-r--r--   0 mateograciano   (501) staff       (20)    20483 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/SOURCES.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/dependency_links.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/requires.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-12 08:01:26.000000 easydags-0.1.0/easydags.egg-info/top_level.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.1.0/pyproject.toml
--rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-12 08:01:26.263170 easydags-0.1.0/setup.cfg
--rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-12 07:57:43.000000 easydags-0.1.0/setup.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-12 08:12:17.710392 easydags-0.1.1/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.1.1/LICENSE
+-rw-r--r--   0 mateograciano   (501) staff       (20)    21551 2023-06-12 08:12:17.710156 easydags-0.1.1/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)    21356 2023-06-12 08:11:31.000000 easydags-0.1.1/README.md
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-12 08:12:17.708922 easydags-0.1.1/easydags/
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.1.1/easydags/__init__.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.1.1/easydags/config.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    23016 2023-06-12 07:48:19.000000 easydags-0.1.1/easydags/dag.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.1.1/easydags/errors.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    12266 2023-06-12 07:39:41.000000 easydags-0.1.1/easydags/node.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)     3829 2023-06-12 07:21:06.000000 easydags-0.1.1/easydags/ops.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-12 08:12:17.709835 easydags-0.1.1/easydags.egg-info/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    21551 2023-06-12 08:12:17.000000 easydags-0.1.1/easydags.egg-info/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-12 08:12:17.000000 easydags-0.1.1/easydags.egg-info/SOURCES.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-12 08:12:17.000000 easydags-0.1.1/easydags.egg-info/dependency_links.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-12 08:12:17.000000 easydags-0.1.1/easydags.egg-info/requires.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-12 08:12:17.000000 easydags-0.1.1/easydags.egg-info/top_level.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)      116 2023-06-06 21:08:56.000000 easydags-0.1.1/pyproject.toml
+-rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-12 08:12:17.710474 easydags-0.1.1/setup.cfg
+-rw-r--r--   0 mateograciano   (501) staff       (20)      945 2023-06-12 08:12:02.000000 easydags-0.1.1/setup.py
```

### Comparing `easydags-0.1.0/LICENSE` & `easydags-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easydags-0.1.0/PKG-INFO` & `easydags-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydags
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dags made easy
 Author: Mateo Graciano
 Author-email: magralo@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easydags: DAGs made easy
@@ -69,15 +69,15 @@
 This library will help you get through all those challenges if you use it wisely; I really hope that this helps someone with a real-world problem. 
 
 
 ## Why do we need DAGs
 
 This is a tricky question... after all, all your processes might be ok. But I will try to explain the main reason with one example:
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrence_imp.png)
+![Motivation](https://raw.githubusercontent.com/magralo/easydags/main/resource_readme/concurrence_imp.png)
               
 
 Unless you are using DAGs, there is a high possibility that you are following the lineal DAG.. but thats inefficient; there is a high possibility that you have a lot of processes that can run in parallel thats why DAGs are so useful; they do not only give us one execution order, they also help us realize which task can be parallelized... and of course, this library implements that using threads (we can define the maximum number of threads with the parameter max_concurrency in the DAG constructor)
 
 
 
 
@@ -180,186 +180,264 @@
 #### Another way to define hard and soft dependencies
 
 Following the idea from airflow we can do the following
 
 - A>B B depends on A (soft)
 - A>>B B depends on A (hard)
 
-For example we can define the ensemble as
+For example we can define the soft dependecy as 
 
 
 ```python
 from easydags import  ExecNode, DAG
 import time
 
 nodes = []
 
 
+def example0():
+    print('beginning 0')
+    time.sleep(3)
+    print('end 0')
+
+
+node1= ExecNode(id_= 'f0',
+              exec_function = example0
+              )
+
+
+
+def example1():
+    print('beginning 1')
+    print('end 1')
+
+node2= ExecNode(id_= 'f1',
+              exec_function = example1 ,
+              ) 
+
+
+
+
+
+node1 > node2
+
+nodes = [node2,node1]
+```
+
+
+and the hard dependency as
+
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def example0():
+    print('beginning 0')
+    time.sleep(3)
+    print('end 0')
+    return 4
+
+
+
+node0 = ExecNode(id_= 'f0',
+              exec_function = example0
+              )   
+
+
+def example1(**kwargs):
+    f0_result = kwargs['f0_result']
+    print('beginning 1')
+    print('end 1')
+    print(f0_result + 8 )
+
+node1 = ExecNode(id_= 'last',
+              exec_function = example1 
+              )    
+
+node0 >> node1
+
+nodes = [node0,node1]
+```
+
+
+
+#### Defining the simple ensemble
+
+``` python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
 def prepro():
-    #print('beginning pre pro')
+    print('beginning pre pro')
     time.sleep(3)
-    #print('end pre pro')
-    return 'df with cool features'
+    print('end pre pro')
+    return 'df with cool features
 
 
 
-node0 = ExecNode(id_= 'pre_process',
+nodes.append( ExecNode(id_= 'pre_process',
               exec_function = prepro,
               output_name = 'my_cool_df'
-              ) 
+              ) )  
 
 
 def model1(**kwargs):
     df = kwargs['my_cool_df']
     
-    #print(f'i am using {df} in model 1')
+    print(f'i am using {df} in model 1')
     time.sleep(3)
     print('finish training model1')
     
     return 'model 1 37803'
 
-node1 = ExecNode(id_= 'model1',
+nodes.append( ExecNode(id_= 'model1',
               exec_function = model1 ,
+              depends_on_hard= ['pre_process'],
               output_name = 'model1'
-              )   
+              ) )   
 
 
 
 def model2(**kwargs):
     df = kwargs['my_cool_df']
     
-    #print(f'i am using {df} in model 2')
+    print(f'i am using {df} in model 2')
     time.sleep(3)
     print('finished training model2')
     
-    return 'model 2 5678'
+    return 'model 2 78373'
 
-node2 = ExecNode(id_= 'model2',
+nodes.append( ExecNode(id_= 'model2',
               exec_function = model2 ,
+              depends_on_hard= ['pre_process'],
               output_name = 'model2'
-              ) 
+              ) )  
 
 
 
 def ensemble(**kwargs):
     model1 = kwargs['model1']
     model2 = kwargs['model2']
     
     result = f'{model1} and {model2}'
     
     print(result)
     
     return result 
 
-node3= ExecNode(id_= 'ensemble',
+nodes.append( ExecNode(id_= 'ensemble',
               exec_function = ensemble ,
               depends_on_hard= ['model1','model2'],
               output_name = 'ensemble'
-              ) 
-
-node0>>node1
-node0>>node2
-
-node1>>node3
-node2>>node3
-
-nodes = [node0, node1, node3, node2]
-
+              ) )  
 
 
 
-dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
+dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
 
 dag.execute()
 ```
+Please note that we can check the logs to verify that model 1 and model ran in parallel
+
+![Motivation](https://raw.githubusercontent.com/magralo/easydags/main/resource_readme/concurrent_check.png)
 
 
-#### Defining the simple ensemble
+
+#### Defining the simple ensemble (using >>)
 
 ``` python
 from easydags import  ExecNode, DAG
 import time
 
 nodes = []
 
 
 def prepro():
-    print('beginning pre pro')
+    #print('beginning pre pro')
     time.sleep(3)
-    print('end pre pro')
-    return 'df with cool features
+    #print('end pre pro')
+    return 'df with cool features'
 
 
 
-nodes.append( ExecNode(id_= 'pre_process',
+node0 = ExecNode(id_= 'pre_process',
               exec_function = prepro,
               output_name = 'my_cool_df'
-              ) )  
+              ) 
 
 
 def model1(**kwargs):
     df = kwargs['my_cool_df']
     
-    print(f'i am using {df} in model 1')
+    #print(f'i am using {df} in model 1')
     time.sleep(3)
     print('finish training model1')
     
     return 'model 1 37803'
 
-nodes.append( ExecNode(id_= 'model1',
+node1 = ExecNode(id_= 'model1',
               exec_function = model1 ,
-              depends_on_hard= ['pre_process'],
               output_name = 'model1'
-              ) )   
+              )   
 
 
 
 def model2(**kwargs):
     df = kwargs['my_cool_df']
     
-    print(f'i am using {df} in model 2')
+    #print(f'i am using {df} in model 2')
     time.sleep(3)
     print('finished training model2')
     
-    return 'model 2 78373'
+    return 'model 2 5678'
 
-nodes.append( ExecNode(id_= 'model2',
+node2 = ExecNode(id_= 'model2',
               exec_function = model2 ,
-              depends_on_hard= ['pre_process'],
               output_name = 'model2'
-              ) )  
+              ) 
 
 
 
 def ensemble(**kwargs):
     model1 = kwargs['model1']
     model2 = kwargs['model2']
     
     result = f'{model1} and {model2}'
     
     print(result)
     
     return result 
 
-nodes.append( ExecNode(id_= 'ensemble',
+node3= ExecNode(id_= 'ensemble',
               exec_function = ensemble ,
               depends_on_hard= ['model1','model2'],
               output_name = 'ensemble'
-              ) )  
+              ) 
 
+node0>>node1
+node0>>node2
 
+node1>>node3
+node2>>node3
 
-dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
+nodes = [node0, node1, node3, node2]
 
-dag.execute()
-```
-Please note that we can check the logs to verify that model 1 and model ran in parallel
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrent_check.png)
+dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
 
+dag.execute()
+    
+```
 
 
 #### Checking the HTML output
 
 One of the coolest features of Airflow is that once you have built your DAG, you can see it on their UI and check the status of the latest run!
 
 Well, my friend, we can do it here too.
@@ -412,15 +490,15 @@
 
 dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
 
 dag.execute()
 ```
 
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
+![Motivation](https://raw.githubusercontent.com/magralo/easydags/main/resource_readme/html_output.png)
 
 
 You can also only draw your DAG without executing (maybe if you only want to show the structure of your dag to someone or to paste it on your documentation)
 
 ```python
 #See draw_ensemble.py
 from easydags import  ExecNode, DAG
```

### Comparing `easydags-0.1.0/README.md` & `easydags-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 This library will help you get through all those challenges if you use it wisely; I really hope that this helps someone with a real-world problem. 
 
 
 ## Why do we need DAGs
 
 This is a tricky question... after all, all your processes might be ok. But I will try to explain the main reason with one example:
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrence_imp.png)
+![Motivation](https://raw.githubusercontent.com/magralo/easydags/main/resource_readme/concurrence_imp.png)
               
 
 Unless you are using DAGs, there is a high possibility that you are following the lineal DAG.. but thats inefficient; there is a high possibility that you have a lot of processes that can run in parallel thats why DAGs are so useful; they do not only give us one execution order, they also help us realize which task can be parallelized... and of course, this library implements that using threads (we can define the maximum number of threads with the parameter max_concurrency in the DAG constructor)
 
 
 
 
@@ -171,186 +171,264 @@
 #### Another way to define hard and soft dependencies
 
 Following the idea from airflow we can do the following
 
 - A>B B depends on A (soft)
 - A>>B B depends on A (hard)
 
-For example we can define the ensemble as
+For example we can define the soft dependecy as 
 
 
 ```python
 from easydags import  ExecNode, DAG
 import time
 
 nodes = []
 
 
+def example0():
+    print('beginning 0')
+    time.sleep(3)
+    print('end 0')
+
+
+node1= ExecNode(id_= 'f0',
+              exec_function = example0
+              )
+
+
+
+def example1():
+    print('beginning 1')
+    print('end 1')
+
+node2= ExecNode(id_= 'f1',
+              exec_function = example1 ,
+              ) 
+
+
+
+
+
+node1 > node2
+
+nodes = [node2,node1]
+```
+
+
+and the hard dependency as
+
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def example0():
+    print('beginning 0')
+    time.sleep(3)
+    print('end 0')
+    return 4
+
+
+
+node0 = ExecNode(id_= 'f0',
+              exec_function = example0
+              )   
+
+
+def example1(**kwargs):
+    f0_result = kwargs['f0_result']
+    print('beginning 1')
+    print('end 1')
+    print(f0_result + 8 )
+
+node1 = ExecNode(id_= 'last',
+              exec_function = example1 
+              )    
+
+node0 >> node1
+
+nodes = [node0,node1]
+```
+
+
+
+#### Defining the simple ensemble
+
+``` python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
 def prepro():
-    #print('beginning pre pro')
+    print('beginning pre pro')
     time.sleep(3)
-    #print('end pre pro')
-    return 'df with cool features'
+    print('end pre pro')
+    return 'df with cool features
 
 
 
-node0 = ExecNode(id_= 'pre_process',
+nodes.append( ExecNode(id_= 'pre_process',
               exec_function = prepro,
               output_name = 'my_cool_df'
-              ) 
+              ) )  
 
 
 def model1(**kwargs):
     df = kwargs['my_cool_df']
     
-    #print(f'i am using {df} in model 1')
+    print(f'i am using {df} in model 1')
     time.sleep(3)
     print('finish training model1')
     
     return 'model 1 37803'
 
-node1 = ExecNode(id_= 'model1',
+nodes.append( ExecNode(id_= 'model1',
               exec_function = model1 ,
+              depends_on_hard= ['pre_process'],
               output_name = 'model1'
-              )   
+              ) )   
 
 
 
 def model2(**kwargs):
     df = kwargs['my_cool_df']
     
-    #print(f'i am using {df} in model 2')
+    print(f'i am using {df} in model 2')
     time.sleep(3)
     print('finished training model2')
     
-    return 'model 2 5678'
+    return 'model 2 78373'
 
-node2 = ExecNode(id_= 'model2',
+nodes.append( ExecNode(id_= 'model2',
               exec_function = model2 ,
+              depends_on_hard= ['pre_process'],
               output_name = 'model2'
-              ) 
+              ) )  
 
 
 
 def ensemble(**kwargs):
     model1 = kwargs['model1']
     model2 = kwargs['model2']
     
     result = f'{model1} and {model2}'
     
     print(result)
     
     return result 
 
-node3= ExecNode(id_= 'ensemble',
+nodes.append( ExecNode(id_= 'ensemble',
               exec_function = ensemble ,
               depends_on_hard= ['model1','model2'],
               output_name = 'ensemble'
-              ) 
-
-node0>>node1
-node0>>node2
-
-node1>>node3
-node2>>node3
-
-nodes = [node0, node1, node3, node2]
-
+              ) )  
 
 
 
-dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
+dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
 
 dag.execute()
 ```
+Please note that we can check the logs to verify that model 1 and model ran in parallel
+
+![Motivation](https://raw.githubusercontent.com/magralo/easydags/main/resource_readme/concurrent_check.png)
 
 
-#### Defining the simple ensemble
+
+#### Defining the simple ensemble (using >>)
 
 ``` python
 from easydags import  ExecNode, DAG
 import time
 
 nodes = []
 
 
 def prepro():
-    print('beginning pre pro')
+    #print('beginning pre pro')
     time.sleep(3)
-    print('end pre pro')
-    return 'df with cool features
+    #print('end pre pro')
+    return 'df with cool features'
 
 
 
-nodes.append( ExecNode(id_= 'pre_process',
+node0 = ExecNode(id_= 'pre_process',
               exec_function = prepro,
               output_name = 'my_cool_df'
-              ) )  
+              ) 
 
 
 def model1(**kwargs):
     df = kwargs['my_cool_df']
     
-    print(f'i am using {df} in model 1')
+    #print(f'i am using {df} in model 1')
     time.sleep(3)
     print('finish training model1')
     
     return 'model 1 37803'
 
-nodes.append( ExecNode(id_= 'model1',
+node1 = ExecNode(id_= 'model1',
               exec_function = model1 ,
-              depends_on_hard= ['pre_process'],
               output_name = 'model1'
-              ) )   
+              )   
 
 
 
 def model2(**kwargs):
     df = kwargs['my_cool_df']
     
-    print(f'i am using {df} in model 2')
+    #print(f'i am using {df} in model 2')
     time.sleep(3)
     print('finished training model2')
     
-    return 'model 2 78373'
+    return 'model 2 5678'
 
-nodes.append( ExecNode(id_= 'model2',
+node2 = ExecNode(id_= 'model2',
               exec_function = model2 ,
-              depends_on_hard= ['pre_process'],
               output_name = 'model2'
-              ) )  
+              ) 
 
 
 
 def ensemble(**kwargs):
     model1 = kwargs['model1']
     model2 = kwargs['model2']
     
     result = f'{model1} and {model2}'
     
     print(result)
     
     return result 
 
-nodes.append( ExecNode(id_= 'ensemble',
+node3= ExecNode(id_= 'ensemble',
               exec_function = ensemble ,
               depends_on_hard= ['model1','model2'],
               output_name = 'ensemble'
-              ) )  
+              ) 
 
+node0>>node1
+node0>>node2
 
+node1>>node3
+node2>>node3
 
-dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
+nodes = [node0, node1, node3, node2]
 
-dag.execute()
-```
-Please note that we can check the logs to verify that model 1 and model ran in parallel
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrent_check.png)
+dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
 
+dag.execute()
+    
+```
 
 
 #### Checking the HTML output
 
 One of the coolest features of Airflow is that once you have built your DAG, you can see it on their UI and check the status of the latest run!
 
 Well, my friend, we can do it here too.
@@ -403,15 +481,15 @@
 
 dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
 
 dag.execute()
 ```
 
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
+![Motivation](https://raw.githubusercontent.com/magralo/easydags/main/resource_readme/html_output.png)
 
 
 You can also only draw your DAG without executing (maybe if you only want to show the structure of your dag to someone or to paste it on your documentation)
 
 ```python
 #See draw_ensemble.py
 from easydags import  ExecNode, DAG
```

### Comparing `easydags-0.1.0/easydags/dag.py` & `easydags-0.1.1/easydags/dag.py`

 * *Files identical despite different names*

### Comparing `easydags-0.1.0/easydags/node.py` & `easydags-0.1.1/easydags/node.py`

 * *Files identical despite different names*

### Comparing `easydags-0.1.0/easydags/ops.py` & `easydags-0.1.1/easydags/ops.py`

 * *Files identical despite different names*

### Comparing `easydags-0.1.0/easydags.egg-info/PKG-INFO` & `easydags-0.1.1/easydags.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydags
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dags made easy
 Author: Mateo Graciano
 Author-email: magralo@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easydags: DAGs made easy
@@ -69,15 +69,15 @@
 This library will help you get through all those challenges if you use it wisely; I really hope that this helps someone with a real-world problem. 
 
 
 ## Why do we need DAGs
 
 This is a tricky question... after all, all your processes might be ok. But I will try to explain the main reason with one example:
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrence_imp.png)
+![Motivation](https://raw.githubusercontent.com/magralo/easydags/main/resource_readme/concurrence_imp.png)
               
 
 Unless you are using DAGs, there is a high possibility that you are following the lineal DAG.. but thats inefficient; there is a high possibility that you have a lot of processes that can run in parallel thats why DAGs are so useful; they do not only give us one execution order, they also help us realize which task can be parallelized... and of course, this library implements that using threads (we can define the maximum number of threads with the parameter max_concurrency in the DAG constructor)
 
 
 
 
@@ -180,186 +180,264 @@
 #### Another way to define hard and soft dependencies
 
 Following the idea from airflow we can do the following
 
 - A>B B depends on A (soft)
 - A>>B B depends on A (hard)
 
-For example we can define the ensemble as
+For example we can define the soft dependecy as 
 
 
 ```python
 from easydags import  ExecNode, DAG
 import time
 
 nodes = []
 
 
+def example0():
+    print('beginning 0')
+    time.sleep(3)
+    print('end 0')
+
+
+node1= ExecNode(id_= 'f0',
+              exec_function = example0
+              )
+
+
+
+def example1():
+    print('beginning 1')
+    print('end 1')
+
+node2= ExecNode(id_= 'f1',
+              exec_function = example1 ,
+              ) 
+
+
+
+
+
+node1 > node2
+
+nodes = [node2,node1]
+```
+
+
+and the hard dependency as
+
+
+```python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
+def example0():
+    print('beginning 0')
+    time.sleep(3)
+    print('end 0')
+    return 4
+
+
+
+node0 = ExecNode(id_= 'f0',
+              exec_function = example0
+              )   
+
+
+def example1(**kwargs):
+    f0_result = kwargs['f0_result']
+    print('beginning 1')
+    print('end 1')
+    print(f0_result + 8 )
+
+node1 = ExecNode(id_= 'last',
+              exec_function = example1 
+              )    
+
+node0 >> node1
+
+nodes = [node0,node1]
+```
+
+
+
+#### Defining the simple ensemble
+
+``` python
+from easydags import  ExecNode, DAG
+import time
+
+nodes = []
+
+
 def prepro():
-    #print('beginning pre pro')
+    print('beginning pre pro')
     time.sleep(3)
-    #print('end pre pro')
-    return 'df with cool features'
+    print('end pre pro')
+    return 'df with cool features
 
 
 
-node0 = ExecNode(id_= 'pre_process',
+nodes.append( ExecNode(id_= 'pre_process',
               exec_function = prepro,
               output_name = 'my_cool_df'
-              ) 
+              ) )  
 
 
 def model1(**kwargs):
     df = kwargs['my_cool_df']
     
-    #print(f'i am using {df} in model 1')
+    print(f'i am using {df} in model 1')
     time.sleep(3)
     print('finish training model1')
     
     return 'model 1 37803'
 
-node1 = ExecNode(id_= 'model1',
+nodes.append( ExecNode(id_= 'model1',
               exec_function = model1 ,
+              depends_on_hard= ['pre_process'],
               output_name = 'model1'
-              )   
+              ) )   
 
 
 
 def model2(**kwargs):
     df = kwargs['my_cool_df']
     
-    #print(f'i am using {df} in model 2')
+    print(f'i am using {df} in model 2')
     time.sleep(3)
     print('finished training model2')
     
-    return 'model 2 5678'
+    return 'model 2 78373'
 
-node2 = ExecNode(id_= 'model2',
+nodes.append( ExecNode(id_= 'model2',
               exec_function = model2 ,
+              depends_on_hard= ['pre_process'],
               output_name = 'model2'
-              ) 
+              ) )  
 
 
 
 def ensemble(**kwargs):
     model1 = kwargs['model1']
     model2 = kwargs['model2']
     
     result = f'{model1} and {model2}'
     
     print(result)
     
     return result 
 
-node3= ExecNode(id_= 'ensemble',
+nodes.append( ExecNode(id_= 'ensemble',
               exec_function = ensemble ,
               depends_on_hard= ['model1','model2'],
               output_name = 'ensemble'
-              ) 
-
-node0>>node1
-node0>>node2
-
-node1>>node3
-node2>>node3
-
-nodes = [node0, node1, node3, node2]
-
+              ) )  
 
 
 
-dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
+dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
 
 dag.execute()
 ```
+Please note that we can check the logs to verify that model 1 and model ran in parallel
+
+![Motivation](https://raw.githubusercontent.com/magralo/easydags/main/resource_readme/concurrent_check.png)
 
 
-#### Defining the simple ensemble
+
+#### Defining the simple ensemble (using >>)
 
 ``` python
 from easydags import  ExecNode, DAG
 import time
 
 nodes = []
 
 
 def prepro():
-    print('beginning pre pro')
+    #print('beginning pre pro')
     time.sleep(3)
-    print('end pre pro')
-    return 'df with cool features
+    #print('end pre pro')
+    return 'df with cool features'
 
 
 
-nodes.append( ExecNode(id_= 'pre_process',
+node0 = ExecNode(id_= 'pre_process',
               exec_function = prepro,
               output_name = 'my_cool_df'
-              ) )  
+              ) 
 
 
 def model1(**kwargs):
     df = kwargs['my_cool_df']
     
-    print(f'i am using {df} in model 1')
+    #print(f'i am using {df} in model 1')
     time.sleep(3)
     print('finish training model1')
     
     return 'model 1 37803'
 
-nodes.append( ExecNode(id_= 'model1',
+node1 = ExecNode(id_= 'model1',
               exec_function = model1 ,
-              depends_on_hard= ['pre_process'],
               output_name = 'model1'
-              ) )   
+              )   
 
 
 
 def model2(**kwargs):
     df = kwargs['my_cool_df']
     
-    print(f'i am using {df} in model 2')
+    #print(f'i am using {df} in model 2')
     time.sleep(3)
     print('finished training model2')
     
-    return 'model 2 78373'
+    return 'model 2 5678'
 
-nodes.append( ExecNode(id_= 'model2',
+node2 = ExecNode(id_= 'model2',
               exec_function = model2 ,
-              depends_on_hard= ['pre_process'],
               output_name = 'model2'
-              ) )  
+              ) 
 
 
 
 def ensemble(**kwargs):
     model1 = kwargs['model1']
     model2 = kwargs['model2']
     
     result = f'{model1} and {model2}'
     
     print(result)
     
     return result 
 
-nodes.append( ExecNode(id_= 'ensemble',
+node3= ExecNode(id_= 'ensemble',
               exec_function = ensemble ,
               depends_on_hard= ['model1','model2'],
               output_name = 'ensemble'
-              ) )  
+              ) 
 
+node0>>node1
+node0>>node2
 
+node1>>node3
+node2>>node3
 
-dag = DAG(nodes,name = 'Ensemble example',max_concurrency=3, debug = False)
+nodes = [node0, node1, node3, node2]
 
-dag.execute()
-```
-Please note that we can check the logs to verify that model 1 and model ran in parallel
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/concurrent_check.png)
+dag = DAG(nodes,name = 'Ensemble example2',max_concurrency=3, debug = False)
 
+dag.execute()
+    
+```
 
 
 #### Checking the HTML output
 
 One of the coolest features of Airflow is that once you have built your DAG, you can see it on their UI and check the status of the latest run!
 
 Well, my friend, we can do it here too.
@@ -412,15 +490,15 @@
 
 dag = DAG(nodes,name = 'NO HTML OUTPUT',max_concurrency=8, debug = False, draw = False)
 
 dag.execute()
 ```
 
 
-![Motivation](https://github.com/magralo/easydags/blob/main/resource_readme/html_output.png)
+![Motivation](https://raw.githubusercontent.com/magralo/easydags/main/resource_readme/html_output.png)
 
 
 You can also only draw your DAG without executing (maybe if you only want to show the structure of your dag to someone or to paste it on your documentation)
 
 ```python
 #See draw_ensemble.py
 from easydags import  ExecNode, DAG
```

### Comparing `easydags-0.1.0/setup.py` & `easydags-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'easydags',         # How you named your package folder (MyLib)
   packages = ['easydags'],   # Chose the same as "name"
-  version = '0.1.0',      # Start with a small number and increase it with every change you make
+  version = '0.1.1',      # Start with a small number and increase it with every change you make
   description = 'Dags made easy',   # Give a short description about your library
   author = 'Mateo Graciano',                   # Type in your name
   author_email = 'magralo@gmail.com',      # Type in your E-Mail
   install_requires=[            # I get to this in a second
           'networkx==2.6.3',
           'pydantic==1.10',
           'loguru==0.6.0',
```

