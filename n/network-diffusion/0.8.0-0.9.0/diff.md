# Comparing `tmp/network_diffusion-0.8.0.tar.gz` & `tmp/network_diffusion-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network_diffusion-0.8.0.tar", last modified: Tue Mar 21 06:50:41 2023, max compression
+gzip compressed data, was "network_diffusion-0.9.0.tar", last modified: Thu May 18 16:45:33 2023, max compression
```

## Comparing `network_diffusion-0.8.0.tar` & `network_diffusion-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:50:41.181440 network_diffusion-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-21 06:50:41.181440 network_diffusion-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:50:41.177440 network_diffusion-0.8.0/network_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/experiment_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:50:41.177440 network_diffusion-0.8.0/network_diffusion/mln/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/mln/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/mln/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/mln/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/mln/mlnetwork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:50:41.177440 network_diffusion-0.8.0/network_diffusion/models/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/models/dsaa_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/models/mlt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:50:41.177440 network_diffusion-0.8.0/network_diffusion/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/models/utils/compartmental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/models/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/multi_spreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:50:41.181440 network_diffusion-0.8.0/network_diffusion/seeding/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/seeding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/seeding/base_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/seeding/degreecentrality_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/seeding/kshell_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/seeding/mocky_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/seeding/neighbourhoodsize_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/seeding/pagerank_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/seeding/random_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/seeding/voterank_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/network_diffusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 06:50:41.177440 network_diffusion-0.8.0/network_diffusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-21 06:50:41.000000 network_diffusion-0.8.0/network_diffusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-21 06:50:41.000000 network_diffusion-0.8.0/network_diffusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 06:50:41.000000 network_diffusion-0.8.0/network_diffusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-21 06:50:41.000000 network_diffusion-0.8.0/network_diffusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-21 06:50:41.000000 network_diffusion-0.8.0/network_diffusion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 06:50:41.181440 network_diffusion-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-21 06:49:37.000000 network_diffusion-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:45:33.904113 network_diffusion-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-18 16:45:33.904113 network_diffusion-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:45:33.900113 network_diffusion-0.9.0/network_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/experiment_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:45:33.900113 network_diffusion-0.9.0/network_diffusion/mln/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/mln/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/mln/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/mln/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/mln/mlnetwork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:45:33.900113 network_diffusion-0.9.0/network_diffusion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/models/dsaa_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/models/mic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/models/mlt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:45:33.900113 network_diffusion-0.9.0/network_diffusion/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/models/utils/compartmental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/models/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/multi_spreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:45:33.904113 network_diffusion-0.9.0/network_diffusion/seeding/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/seeding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/seeding/base_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/seeding/degreecentrality_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/seeding/kshell_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/seeding/mocky_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/seeding/neighbourhoodsize_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/seeding/pagerank_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/seeding/random_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/seeding/voterank_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/network_diffusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:45:33.900113 network_diffusion-0.9.0/network_diffusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-18 16:45:33.000000 network_diffusion-0.9.0/network_diffusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-18 16:45:33.000000 network_diffusion-0.9.0/network_diffusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:45:33.000000 network_diffusion-0.9.0/network_diffusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-18 16:45:33.000000 network_diffusion-0.9.0/network_diffusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 16:45:33.000000 network_diffusion-0.9.0/network_diffusion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:45:33.904113 network_diffusion-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-18 16:44:17.000000 network_diffusion-0.9.0/setup.py
```

### Comparing `network_diffusion-0.8.0/LICENSE` & `network_diffusion-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/PKG-INFO` & `network_diffusion-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network_diffusion
-Version: 0.8.0
+Version: 0.9.0
 Summary: Package to design and run diffusion phenomena in networks.
 Home-page: https://github.com/anty-filidor/network_diffusion
 Author: Michał Czuba, Piotr Bródka
 Author-email: michal.czuba@pwr.edu.pl, piotr.brodka@pwr.edu.pl
 License: GPL
 Project-URL: Documentation, https://network-diffusion.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/anty-filidor/network_diffusion
```

### Comparing `network_diffusion-0.8.0/README.md` & `network_diffusion-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/__init__.py` & `network_diffusion-0.9.0/network_diffusion/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # flake8: noqa
 
 from network_diffusion import models, seeding
 from network_diffusion.mln.actor import MLNetworkActor
 from network_diffusion.mln.mlnetwork import MultilayerNetwork
 from network_diffusion.multi_spreading import MultiSpreading
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
```

### Comparing `network_diffusion-0.8.0/network_diffusion/experiment_logger.py` & `network_diffusion-0.9.0/network_diffusion/experiment_logger.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/mln/actor.py` & `network_diffusion-0.9.0/network_diffusion/mln/actor.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/mln/functions.py` & `network_diffusion-0.9.0/network_diffusion/mln/functions.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/mln/mlnetwork.py` & `network_diffusion-0.9.0/network_diffusion/mln/mlnetwork.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/models/base_model.py` & `network_diffusion-0.9.0/network_diffusion/models/base_model.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/models/dsaa_model.py` & `network_diffusion-0.9.0/network_diffusion/models/dsaa_model.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/models/mlt_model.py` & `network_diffusion-0.9.0/network_diffusion/models/mlt_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     def __str__(self) -> str:
         """Return string representation of the object."""
         descr = f"{BOLD_UNDERLINE}\nMultilayer Linear Threshold Model"
         descr += f"\n{THIN_UNDERLINE}\n"
         descr += self._compartmental_graph.describe()
         descr += str(self._seed_selector)
         descr += f"{BOLD_UNDERLINE}\nauxiliary parameters\n{THIN_UNDERLINE}"
-        descr += f"\n\tprotocole: {self.protocol.__name__}"
+        descr += f"\n\tprotocol: {self.protocol.__name__}"
         descr += f"\n\tactive state abbreviation: {self.ACTIVE_STATE}"
         descr += f"\n\tinactive state abbreviation: {self.INACTIVE_STATE}"
         descr += f"\n{BOLD_UNDERLINE}"
         return descr
 
     def _create_compartments(
         self,
@@ -177,15 +177,15 @@
         net: MLNetwork,
     ) -> str:
         """
         Try to change state of given actor of the network according to model.
 
         :param agent: actor to evaluate in given layer
         :param layer_name: a layer where the actor exists
-        :param network: a network where the actor exists
+        :param net: a network where the actor exists
 
         :return: state of the actor in particular layer to be set after epoch
         """
         l_graph: nx.Graph = net.layers[layer_name]
 
         # trivial case - node is already activated
         current_state = l_graph.nodes[agent.actor_id]["status"]
```

### Comparing `network_diffusion-0.8.0/network_diffusion/models/utils/compartmental.py` & `network_diffusion-0.9.0/network_diffusion/models/utils/compartmental.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/models/utils/types.py` & `network_diffusion-0.9.0/network_diffusion/models/utils/types.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/multi_spreading.py` & `network_diffusion-0.9.0/network_diffusion/multi_spreading.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/seeding/__init__.py` & `network_diffusion-0.9.0/network_diffusion/seeding/__init__.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/seeding/base_selector.py` & `network_diffusion-0.9.0/network_diffusion/seeding/base_selector.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/seeding/degreecentrality_selector.py` & `network_diffusion-0.9.0/network_diffusion/seeding/degreecentrality_selector.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/seeding/kshell_selector.py` & `network_diffusion-0.9.0/network_diffusion/seeding/kshell_selector.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/seeding/mocky_selector.py` & `network_diffusion-0.9.0/network_diffusion/seeding/mocky_selector.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/seeding/neighbourhoodsize_selector.py` & `network_diffusion-0.9.0/network_diffusion/seeding/neighbourhoodsize_selector.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/seeding/pagerank_selector.py` & `network_diffusion-0.9.0/network_diffusion/seeding/pagerank_selector.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/seeding/random_selector.py` & `network_diffusion-0.9.0/network_diffusion/seeding/random_selector.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/seeding/voterank_selector.py` & `network_diffusion-0.9.0/network_diffusion/seeding/voterank_selector.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion/utils.py` & `network_diffusion-0.9.0/network_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `network_diffusion-0.8.0/network_diffusion.egg-info/PKG-INFO` & `network_diffusion-0.9.0/network_diffusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-diffusion
-Version: 0.8.0
+Version: 0.9.0
 Summary: Package to design and run diffusion phenomena in networks.
 Home-page: https://github.com/anty-filidor/network_diffusion
 Author: Michał Czuba, Piotr Bródka
 Author-email: michal.czuba@pwr.edu.pl, piotr.brodka@pwr.edu.pl
 License: GPL
 Project-URL: Documentation, https://network-diffusion.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/anty-filidor/network_diffusion
```

### Comparing `network_diffusion-0.8.0/network_diffusion.egg-info/SOURCES.txt` & `network_diffusion-0.9.0/network_diffusion.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 network_diffusion/mln/__init__.py
 network_diffusion/mln/actor.py
 network_diffusion/mln/functions.py
 network_diffusion/mln/mlnetwork.py
 network_diffusion/models/__init__.py
 network_diffusion/models/base_model.py
 network_diffusion/models/dsaa_model.py
+network_diffusion/models/mic_model.py
 network_diffusion/models/mlt_model.py
 network_diffusion/models/utils/__init__.py
 network_diffusion/models/utils/compartmental.py
 network_diffusion/models/utils/types.py
 network_diffusion/seeding/__init__.py
 network_diffusion/seeding/base_selector.py
 network_diffusion/seeding/degreecentrality_selector.py
```

### Comparing `network_diffusion-0.8.0/setup.py` & `network_diffusion-0.9.0/setup.py`

 * *Files identical despite different names*

