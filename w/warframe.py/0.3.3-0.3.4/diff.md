# Comparing `tmp/warframe.py-0.3.3.tar.gz` & `tmp/warframe.py-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warframe.py-0.3.3.tar", last modified: Sun Jun 11 16:06:47 2023, max compression
+gzip compressed data, was "warframe.py-0.3.4.tar", last modified: Mon Jun 12 16:02:41 2023, max compression
```

## Comparing `warframe.py-0.3.3.tar` & `warframe.py-0.3.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.545903 warframe.py-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-11 16:06:17.000000 warframe.py-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-11 16:06:47.545903 warframe.py-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-11 16:06:17.000000 warframe.py-0.3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-11 16:06:17.000000 warframe.py-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 16:06:47.545903 warframe.py-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-11 16:06:17.000000 warframe.py-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe/worldstate/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe/worldstate/common/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/common/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/common/types_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe/worldstate/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/mission_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/enums/syndicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.545903 warframe.py-0.3.3/warframe/worldstate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/archon_hunt.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/cambion_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/cetus.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/counted_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/daily_deal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/fissure.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/flash_sale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/invasion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/mission.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/orb_vallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/sortie.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/models/void_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:17.000000 warframe.py-0.3.3/warframe/worldstate/worldstate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:06:47.541903 warframe.py-0.3.3/warframe.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 16:06:47.000000 warframe.py-0.3.3/warframe.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:02:41.054150 warframe.py-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-12 16:01:14.000000 warframe.py-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-12 16:02:41.054150 warframe.py-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-12 16:01:14.000000 warframe.py-0.3.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-12 16:01:14.000000 warframe.py-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 16:02:41.054150 warframe.py-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-12 16:01:14.000000 warframe.py-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:02:41.050150 warframe.py-0.3.4/warframe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:02:41.050150 warframe.py-0.3.4/warframe/worldstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:02:41.050150 warframe.py-0.3.4/warframe/worldstate/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/common/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/common/types_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:02:41.050150 warframe.py-0.3.4/warframe/worldstate/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/enums/faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/enums/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/enums/mission_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/enums/syndicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:02:41.054150 warframe.py-0.3.4/warframe/worldstate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/archon_hunt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/cambion_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/cetus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/counted_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/daily_deal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/fissure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/flash_sale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/invasion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/orb_vallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/sortie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/models/void_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:01:14.000000 warframe.py-0.3.4/warframe/worldstate/worldstate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:02:41.050150 warframe.py-0.3.4/warframe.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-12 16:02:40.000000 warframe.py-0.3.4/warframe.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-12 16:02:41.000000 warframe.py-0.3.4/warframe.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:02:40.000000 warframe.py-0.3.4/warframe.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 16:02:40.000000 warframe.py-0.3.4/warframe.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 16:02:40.000000 warframe.py-0.3.4/warframe.py.egg-info/top_level.txt
```

### Comparing `warframe.py-0.3.3/LICENSE` & `warframe.py-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/PKG-INFO` & `warframe.py-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.3.3
+Version: 0.3.4
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.3.3/README.rst` & `warframe.py-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/setup.py` & `warframe.py-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/client.py` & `warframe.py-0.3.4/warframe/worldstate/client.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/common/core.py` & `warframe.py-0.3.4/warframe/worldstate/common/core.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/common/types_.py` & `warframe.py-0.3.4/warframe/worldstate/common/types_.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/endpoints.py` & `warframe.py-0.3.4/warframe/worldstate/endpoints.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/enums/mission_type.py` & `warframe.py-0.3.4/warframe/worldstate/enums/mission_type.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/exceptions.py` & `warframe.py-0.3.4/warframe/worldstate/exceptions.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/arbitration.py` & `warframe.py-0.3.4/warframe/worldstate/models/arbitration.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/archon_hunt.py` & `warframe.py-0.3.4/warframe/worldstate/models/archon_hunt.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/daily_deal.py` & `warframe.py-0.3.4/warframe/worldstate/models/daily_deal.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/event.py` & `warframe.py-0.3.4/warframe/worldstate/models/event.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/fissure.py` & `warframe.py-0.3.4/warframe/worldstate/models/fissure.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/flash_sale.py` & `warframe.py-0.3.4/warframe/worldstate/models/flash_sale.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/invasion.py` & `warframe.py-0.3.4/warframe/worldstate/models/invasion.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,25 +58,19 @@
     "The node string"
 
     required_runs: int
     "The amount of runs required to qualify for the reward. (most likely 3)"
 
     vs_infested: bool = field(name="vsInfestation")
     "Whether the fight is against infested enemies"
+
     attacker: Attacker
     "The invading faction information"
 
     defender: Defender
     "The defending faction information"
 
-    # optional
-    expiry: Optional[datetime] = None
-    "The time the Invasion ends"
-
-    start_string: Optional[str] = None
+    start_string: str
     "Short-time-formatted duration string of the start of the Invasion"
 
-    active: Optional[bool] = None
-    "Whether the invasion is currently active"
-
-    reward_types: Optional[List[ItemRewardType]] = None
+    reward_types: List[ItemRewardType]
     "A list of reward types"
```

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/mission.py` & `warframe.py-0.3.4/warframe/worldstate/models/mission.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/reward.py` & `warframe.py-0.3.4/warframe/worldstate/models/reward.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/sortie.py` & `warframe.py-0.3.4/warframe/worldstate/models/sortie.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe/worldstate/models/void_trader.py` & `warframe.py-0.3.4/warframe/worldstate/models/void_trader.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.3.3/warframe.py.egg-info/PKG-INFO` & `warframe.py-0.3.4/warframe.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.3.3
+Version: 0.3.4
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.3.3/warframe.py.egg-info/SOURCES.txt` & `warframe.py-0.3.4/warframe.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

