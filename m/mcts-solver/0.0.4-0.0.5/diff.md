# Comparing `tmp/mcts_solver-0.0.4.tar.gz` & `tmp/mcts_solver-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcts_solver-0.0.4.tar", last modified: Fri Apr 21 06:31:28 2023, max compression
+gzip compressed data, was "mcts_solver-0.0.5.tar", last modified: Mon Jun 12 12:00:31 2023, max compression
```

## Comparing `mcts_solver-0.0.4.tar` & `mcts_solver-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 06:31:28.083349 mcts_solver-0.0.4/
--rw-rw-r--   0 root         (0) root         (0)    35149 2022-08-10 12:06:43.000000 mcts_solver-0.0.4/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       46 2022-08-10 13:01:54.000000 mcts_solver-0.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2023-04-21 06:31:28.083349 mcts_solver-0.0.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      406 2022-08-11 08:42:20.000000 mcts_solver-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 06:31:28.059349 mcts_solver-0.0.4/mcts_solver/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-11 08:28:31.000000 mcts_solver-0.0.4/mcts_solver/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4783 2023-04-19 11:16:11.000000 mcts_solver-0.0.4/mcts_solver/mcts_solver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 06:31:28.083349 mcts_solver-0.0.4/mcts_solver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-21 06:31:27.000000 mcts_solver-0.0.4/mcts_solver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 06:31:28.083349 mcts_solver-0.0.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1674 2023-04-19 12:25:15.000000 mcts_solver-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:00:31.271558 mcts_solver-0.0.5/
+-rw-rw-r--   0 root         (0) root         (0)    35149 2022-08-10 12:06:43.000000 mcts_solver-0.0.5/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       46 2022-08-10 13:01:54.000000 mcts_solver-0.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-12 12:00:31.267557 mcts_solver-0.0.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      406 2022-08-11 08:42:20.000000 mcts_solver-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:00:31.243558 mcts_solver-0.0.5/mcts_solver/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-11 08:28:31.000000 mcts_solver-0.0.5/mcts_solver/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5803 2023-06-11 11:47:19.000000 mcts_solver-0.0.5/mcts_solver/mcts_solver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 12:00:31.259558 mcts_solver-0.0.5/mcts_solver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-12 12:00:30.000000 mcts_solver-0.0.5/mcts_solver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-12 12:00:30.000000 mcts_solver-0.0.5/mcts_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 12:00:30.000000 mcts_solver-0.0.5/mcts_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 12:00:30.000000 mcts_solver-0.0.5/mcts_solver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-12 12:00:30.000000 mcts_solver-0.0.5/mcts_solver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 12:00:30.000000 mcts_solver-0.0.5/mcts_solver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 12:00:31.271558 mcts_solver-0.0.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1674 2023-06-12 11:44:33.000000 mcts_solver-0.0.5/setup.py
```

### Comparing `mcts_solver-0.0.4/LICENSE` & `mcts_solver-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mcts_solver-0.0.4/PKG-INFO` & `mcts_solver-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcts_solver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Monte-Carlo tree search solver for chess-ant
 Home-page: https://github.com/akuroiwa/mcts-solver
 Author: Akihiro Kuroiwa
 Author-email: akuroiwa@env-reform.com
 License: GNU/GPLv3+
 Keywords: mcts,monte,carlo,tree,search,solver
 Platform: any
```

### Comparing `mcts_solver-0.0.4/mcts_solver/mcts_solver.py` & `mcts_solver-0.0.5/mcts_solver/mcts_solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,111 @@
 from mcts import mcts, treeNode
 import multiprocessing
+from multiprocessing import Lock
 
 class AntLionTreeNode(treeNode):
 
     def __init__(self, state, parent):
         super().__init__(state, parent)
         self.value = None
 
 class AntLionMcts(mcts):
 
     def __init__(self, timeLimit=None, iterationLimit=None):
         super().__init__(timeLimit, iterationLimit)
         self.dl = False
         self.regression = False
+        self.lock = Lock()
 
     def dl_method(self, state):
         '''Rewards output by deep learning that you can override.
         '''
         pass
 
     def mctsSolver(self, node):
         '''This is based on pseudocode from the following paper:
         `Winands, Mark & Björnsson, Yngvi & Saito, Jahn-Takeshi. (2008). Monte-Carlo Tree Search Solver. 25-36. 10.1007/978-3-540-87608-3_3.
         <https://www.researchgate.net/publication/220962507_Monte-Carlo_Tree_Search_Solver>`__
         Parallel processing is possible thanks to OpenAI's ChatGPT advice.
         '''
-        if node.isTerminal:
-            if  node.state.getReward() == 1:
-                node.value = float("inf")
-            elif node.state.getReward() == -1:
-                node.value = float("-inf")
-            else:
-                return 0
+        with self.lock:
+            if node.isTerminal:
+                if  node.state.getReward() == 1:
+                    node.value = float("inf")
+                elif node.state.getReward() == -1:
+                    node.value = float("-inf")
+                else:
+                    return 0
 
-        bestChild = node
+            bestChild = node
 
-        if bestChild.value != float("-inf") and bestChild.value != float("inf"):
-            if bestChild.numVisits == 0:
-                if self.dl:
-                    reward = self.dl_method(bestChild.state)
+            if bestChild.value != float("-inf") and bestChild.value != float("inf"):
+                if bestChild.numVisits == 0:
+                    if self.dl:
+                        reward = self.dl_method(bestChild.state)
+                    else:
+                        reward = bestChild.state.getCurrentPlayer() * -self.rollout(bestChild.state)
+
+                        # with self.lock:
+                        #     reward = bestChild.state.getCurrentPlayer() * -self.rollout(bestChild.state)
+
+                        # with multiprocessing.Pool() as pool:
+                        #     num_processes = multiprocessing.cpu_count()
+                        #     multiple_results = [pool.apply_async(self.rollout, args=(bestChild.state,)) for i in range(num_processes)]
+                        #     pool.close()
+                        #     pool.join()
+                        #     results = [res for res in multiple_results if res.ready() and res.successful()]
+                        #     if results:
+                        #         # reward = bestChild.state.getCurrentPlayer() * max([-res.get() for res in results])
+                        #         reward = bestChild.state.getCurrentPlayer() * min([-res.get() for res in results])
+                        #     else:
+                        #         reward = 0
+                    return reward
                 else:
-                    # reward = bestChild.state.getCurrentPlayer() * -self.rollout(bestChild.state)
-                    with multiprocessing.Pool() as pool:
-                        num_processes = multiprocessing.cpu_count()
-                        multiple_results = [pool.apply_async(self.rollout, args=(bestChild.state,)) for i in range(num_processes)]
-                        pool.close()
-                        pool.join()
-                        results = [res for res in multiple_results if res.ready() and res.successful()]
-                        if results:
-                            reward = bestChild.state.getCurrentPlayer() * -max([res.get() for res in results])
-                        else:
-                            reward = 0
-                return reward
+                    # with multiprocessing.Pool() as pool:
+                    #     m = pool.apply_async(self.mctsSolver, args=(bestChild,))
+                    #     reward = -m.get()
+
+                    # with self.lock:
+                    #     reward = -self.mctsSolver(bestChild)
+
+                    reward = -self.mctsSolver(bestChild)
             else:
-                with multiprocessing.Pool() as pool:
-                    m = pool.apply_async(-self.mctsSolver, args=(bestChild,))
-                    reward = m.get()
-                # reward = -self.mctsSolver(bestChild)
-        else:
-            reward = bestChild.value
+                reward = bestChild.value
 
-        if reward == float("inf"):
-            node.parent.value = float("-inf")
-            return reward
-        else:
-            if reward == float("-inf"):
-                for child in node.parent.children.values():
-                    try:
-                        if child.value != reward:
-                            reward = -1
+            if reward == float("inf"):
+                node.parent.value = float("-inf")
+                return reward
+            else:
+                if reward == float("-inf"):
+                    for child in node.parent.children.values():
+                        try:
+                            if child.value != reward:
+                                reward = -1
+                                return reward
+                        except:
+                            node.parent.value = float("inf")
                             return reward
-                    except:
-                        node.parent.value = float("inf")
-                        return reward
-        return reward
+            return reward
 
     def selectNode_num(self, node, explorationConstant):
-        while not node.isTerminal:
-            if node.isFullyExpanded:
-                node = self.getBestChild(node, explorationConstant)
-            else:
-                return self.expand(node)
+        '''Parallel processing is possible thanks to Google Bard and OpenAI's ChatGPT advice.
+        '''
+        with self.lock:
+            while not node.isTerminal:
+                if node.isFullyExpanded:
+                    node = self.getBestChild(node, explorationConstant)
+
+                    # with self.lock:
+                    #     node = self.getBestChild(node, explorationConstant)
+                else:
+                    return self.expand(node)
+
+                    # with self.lock:
+                    #     return self.expand(node)
         return node
 
     def expand(self, node):
         actions = node.state.getPossibleActions()
         for action in actions:
             if action not in node.children:
                 newNode = AntLionTreeNode(node.state.takeAction(action), node)
```

### Comparing `mcts_solver-0.0.4/mcts_solver.egg-info/PKG-INFO` & `mcts_solver-0.0.5/mcts_solver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcts-solver
-Version: 0.0.4
+Version: 0.0.5
 Summary: Monte-Carlo tree search solver for chess-ant
 Home-page: https://github.com/akuroiwa/mcts-solver
 Author: Akihiro Kuroiwa
 Author-email: akuroiwa@env-reform.com
 License: GNU/GPLv3+
 Keywords: mcts,monte,carlo,tree,search,solver
 Platform: any
```

### Comparing `mcts_solver-0.0.4/setup.py` & `mcts_solver-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import glob
 from setuptools import setup, find_packages
 
 setup(
     name='mcts_solver',
-    version='0.0.4',
+    version='0.0.5',
     url='https://github.com/akuroiwa/mcts-solver',
     # # PyPI url
     # download_url='',
     license='GNU/GPLv3+',
     author='Akihiro Kuroiwa',
     author_email='akuroiwa@env-reform.com',
     description='Monte-Carlo tree search solver for chess-ant',
```

