# Comparing `tmp/ranked-0.0.1.tar.gz` & `tmp/ranked-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ranked-0.0.1.tar", last modified: Thu Dec 22 22:31:41 2022, max compression
+gzip compressed data, was "ranked-1.0.2.tar", last modified: Mon Jun 12 12:51:05 2023, max compression
```

## Comparing `ranked-0.0.1.tar` & `ranked-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 22:31:41.429804 ranked-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2022-12-22 22:30:24.000000 ranked-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-22 22:30:24.000000 ranked-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2022-12-22 22:31:41.429804 ranked-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2022-12-22 22:30:24.000000 ranked-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 22:31:41.425804 ranked-0.0.1/ranked/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 22:31:41.429804 ranked-0.0.1/ranked/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/datasets/dota2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/datasets/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/datasets/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/matchmaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 22:31:41.429804 ranked-0.0.1/ranked/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/models/elo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/models/elochess.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/models/glicko2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/models/noskill.py
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 22:31:41.429804 ranked-0.0.1/ranked/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2022-12-22 22:30:24.000000 ranked-0.0.1/ranked/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 22:31:41.425804 ranked-0.0.1/ranked.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2022-12-22 22:31:41.000000 ranked-0.0.1/ranked.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2022-12-22 22:31:41.000000 ranked-0.0.1/ranked.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 22:31:41.000000 ranked-0.0.1/ranked.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-22 22:31:41.000000 ranked-0.0.1/ranked.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-22 22:31:41.000000 ranked-0.0.1/ranked.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 22:31:33.000000 ranked-0.0.1/ranked.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 22:31:41.429804 ranked-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2022-12-22 22:30:24.000000 ranked-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:51:05.896932 ranked-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-12 12:49:40.000000 ranked-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-12 12:49:40.000000 ranked-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-12 12:51:05.896932 ranked-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-12 12:49:40.000000 ranked-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 12:49:40.000000 ranked-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:51:05.896932 ranked-1.0.2/ranked/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:51:05.896932 ranked-1.0.2/ranked/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/datasets/dota2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/datasets/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/datasets/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/matchmaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:51:05.896932 ranked-1.0.2/ranked/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/models/elo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/models/elochess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/models/glicko2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/models/noskill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/models/openskill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:51:05.896932 ranked-1.0.2/ranked/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-12 12:49:40.000000 ranked-1.0.2/ranked/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:51:05.896932 ranked-1.0.2/ranked.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-12 12:51:05.000000 ranked-1.0.2/ranked.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-12 12:51:05.000000 ranked-1.0.2/ranked.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:51:05.000000 ranked-1.0.2/ranked.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 12:51:05.000000 ranked-1.0.2/ranked.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 12:51:05.000000 ranked-1.0.2/ranked.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:51:00.000000 ranked-1.0.2/ranked.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:51:05.896932 ranked-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-12 12:49:40.000000 ranked-1.0.2/setup.py
```

### Comparing `ranked-0.0.1/LICENSE` & `ranked-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ranked-0.0.1/PKG-INFO` & `ranked-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranked
-Version: 0.0.1
+Version: 1.0.2
 Summary: Player Ranking Algorithm benchmarks
 Home-page: https://github.com/Delaunay/ranked
 Author: Pierre Delaunay
 Author-email: pierre@delaunay.io
 License: BSD-3-Clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -13,19 +13,19 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.*
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 License-File: LICENSE
 
 ranked
 ======
 
 |pypi| |py_versions| |license|
 |rtfd| |codecov| |style| |tests|
@@ -86,20 +86,38 @@
    of the ranking algorithm. It is up to the matchmaking algorithm to make sure
    the teams it builds are as fair as possible.
 
    The ranking algorithm only provide an estimate of each player'skill to help
    the matchmaker to make the best decision possible.
 
 
+Examples
+--------
+
+.. code-block:: python
+
+    ranker = ChessElo()
+    p1 = ranker.new_player((1613 - sub) / div)
+    p2 = ranker.new_player((1609 - sub) / div)
+
+    m1 = Match((p1, 0), (p2, 1)),  # p1 lost (lower score)
+
+    win_prob = ranker.win(m)
+
+    ranker.update(m)
+
+    # P1 lost so its skill got updated down
+    new_skill = p1.skill()  # 1603.19
+
+
 WIP
 ---
 
 * NoSkill2
 * Dota2 extracted matches
-* publish to Pypi
 
 
 .. code-block:: bash
 
    pip install ranked
```

### Comparing `ranked-0.0.1/README.rst` & `ranked-1.0.2/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,98 @@
-ranked
-======
-
-|pypi| |py_versions| |license|
-|rtfd| |codecov| |style| |tests|
-
-.. |pypi| image:: https://img.shields.io/pypi/v/ranked.svg
-    :target: https://pypi.python.org/pypi/ranked
-    :alt: Current PyPi Version
-
-.. |py_versions| image:: https://img.shields.io/pypi/pyversions/ranked.svg
-    :target: https://pypi.python.org/pypi/ranked
-    :alt: Supported Python Versions
-
-.. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-    :target: https://opensource.org/licenses/BSD-3-Clause
-    :alt: BSD 3-clause license
-
-.. |rtfd| image:: https://readthedocs.org/projects/ranked/badge/?version=stable
-    :target: https://orion.readthedocs.io/en/stable/?badge=stable
-    :alt: Documentation Status
-
-.. |codecov| image:: https://codecov.io/gh/Delaunay/ranked/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/Delaunay/ranked
-    :alt: Codecov Report
-
-.. |style| image:: https://github.com/Delaunay/Ranked/actions/workflows/style.yml/badge.svg
-    :target: https://github.com/Delaunay/Ranked/actions/workflows/style.yml
-    :alt: Github actions tests
-
-.. |tests| image:: https://github.com/Delaunay/Ranked/actions/workflows/test.yml/badge.svg
-    :target: https://github.com/Delaunay/Ranked/actions/workflows/test.yml
-    :alt: Github actions tests
-
-
-
-Features
-~~~~~~~~
-
-* A common interface for ranking algorithms
-* Elo (Chess & Generic)
-* Glicko2
-* NoSkill (similar to Trueskill, i.e bayesian inference on a bipartite graph)
-* Synthetics benchmarks
-* Basic match maker
-* Matchup replay to calibrate and experiment on real data
-* Model calibration using black-box optimizer Orion
-
-
-.. note::
-
-   For team based games; When benchmarking ranking algorithm against real data you have
-   to keep in mind that the matchmaking algorithm that created the groups
-   was based on its own external ranking system so any measure
-   that would come out of such benchmarks would end up being biased.
-
-.. note::
-
-   Similarly, matchmaking or the team building algorithm can impact the performance
-   of the ranking algorithm. It is up to the matchmaking algorithm to make sure
-   the teams it builds are as fair as possible.
-
-   The ranking algorithm only provide an estimate of each player'skill to help
-   the matchmaker to make the best decision possible.
-
-
-WIP
----
-
-* NoSkill2
-* Dota2 extracted matches
-* publish to Pypi
-
-
-.. code-block:: bash
-
-   pip install ranked
-
-
-.. image:: https://github.com/Delaunay/Ranked/blob/master/docs/_static/example.png?raw=true
+ranked
+======
+
+|pypi| |py_versions| |license|
+|rtfd| |codecov| |style| |tests|
+
+.. |pypi| image:: https://img.shields.io/pypi/v/ranked.svg
+    :target: https://pypi.python.org/pypi/ranked
+    :alt: Current PyPi Version
+
+.. |py_versions| image:: https://img.shields.io/pypi/pyversions/ranked.svg
+    :target: https://pypi.python.org/pypi/ranked
+    :alt: Supported Python Versions
+
+.. |license| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+    :target: https://opensource.org/licenses/BSD-3-Clause
+    :alt: BSD 3-clause license
+
+.. |rtfd| image:: https://readthedocs.org/projects/ranked/badge/?version=stable
+    :target: https://orion.readthedocs.io/en/stable/?badge=stable
+    :alt: Documentation Status
+
+.. |codecov| image:: https://codecov.io/gh/Delaunay/ranked/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/Delaunay/ranked
+    :alt: Codecov Report
+
+.. |style| image:: https://github.com/Delaunay/Ranked/actions/workflows/style.yml/badge.svg
+    :target: https://github.com/Delaunay/Ranked/actions/workflows/style.yml
+    :alt: Github actions tests
+
+.. |tests| image:: https://github.com/Delaunay/Ranked/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/Delaunay/Ranked/actions/workflows/test.yml
+    :alt: Github actions tests
+
+
+
+Features
+~~~~~~~~
+
+* A common interface for ranking algorithms
+* Elo (Chess & Generic)
+* Glicko2
+* NoSkill (similar to Trueskill, i.e bayesian inference on a bipartite graph)
+* Synthetics benchmarks
+* Basic match maker
+* Matchup replay to calibrate and experiment on real data
+* Model calibration using black-box optimizer Orion
+
+
+.. note::
+
+   For team based games; When benchmarking ranking algorithm against real data you have
+   to keep in mind that the matchmaking algorithm that created the groups
+   was based on its own external ranking system so any measure
+   that would come out of such benchmarks would end up being biased.
+
+.. note::
+
+   Similarly, matchmaking or the team building algorithm can impact the performance
+   of the ranking algorithm. It is up to the matchmaking algorithm to make sure
+   the teams it builds are as fair as possible.
+
+   The ranking algorithm only provide an estimate of each player'skill to help
+   the matchmaker to make the best decision possible.
+
+
+Examples
+--------
+
+.. code-block:: python
+
+    ranker = ChessElo()
+    p1 = ranker.new_player((1613 - sub) / div)
+    p2 = ranker.new_player((1609 - sub) / div)
+
+    m1 = Match((p1, 0), (p2, 1)),  # p1 lost (lower score)
+
+    win_prob = ranker.win(m)
+
+    ranker.update(m)
+
+    # P1 lost so its skill got updated down
+    new_skill = p1.skill()  # 1603.19
+
+
+WIP
+---
+
+* NoSkill2
+* Dota2 extracted matches
+
+
+.. code-block:: bash
+
+   pip install ranked
+
+
+.. image:: https://github.com/Delaunay/Ranked/blob/master/docs/_static/example.png?raw=true
```

### Comparing `ranked-0.0.1/ranked/calibration.py` & `ranked-1.0.2/ranked/calibration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import os
 
-from orion.client import build_experiment
+try:
+    from orion.client import build_experiment
+
+    ERROR = None
+except ImportError as err:
+    ERROR = err
 
 from ranked.datasets.synthetic import SimulationConfig, create_simulated_matchups
-from ranked.models.glicko2 import Glicko2
 from ranked.models.noskill import NoSkill
 from ranked.simulation import Simulation
 
 
 def optimize(klass, max_trials=1000):
+    if ERROR is not None:
+        raise ERROR
+
     center = 1500
 
     try:
         os.remove("orion.pkl")
-    except:
+    except OSError:
         pass
 
     experiment = build_experiment(
         "mm-calibration",
         space=klass.parameters(center),
         algorithms=None,
         storage={
```

### Comparing `ranked-0.0.1/ranked/datasets/__init__.py` & `ranked-1.0.2/ranked/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ranked-0.0.1/ranked/datasets/replay.py` & `ranked-1.0.2/ranked/datasets/replay.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def __init__(self, ranker, pool, matchupfs: str) -> None:
         self.ranker = ranker
         self.matches = []
         self.batches = []
         self.pool = pool
         self.step = 0
 
-        with open(matchupfs, "r") as data:
+        with open(matchupfs) as data:
             for line in data.readline():
                 #
                 match = json.loads(line)
 
                 batch = match.get("batch")
                 teams = match.get("teams")
                 leaderboard = []
@@ -55,9 +55,8 @@
                     self.batches.append((batch, m))
 
                 self.matches.append(m)
 
         self.batches.sort(key=lambda item: item[0])
 
     def matches(self) -> Batch:
-        for b in self.batches:
-            yield b
+        yield from self.batches
```

### Comparing `ranked-0.0.1/ranked/datasets/synthetic.py` & `ranked-1.0.2/ranked/datasets/synthetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import math
 from dataclasses import dataclass
 from typing import List, Tuple
 
 from scipy.stats import norm, uniform
 
 from ranked.datasets import Matchup
 from ranked.matchmaker import Matchmaker
@@ -39,15 +38,15 @@
 
     def save_model(self, model, player_filter=None):
         rows = []
 
         players = model.players
 
         with open("model.csv", "w") as fs:
-            fs.write(f"pid,skill,cons\n")
+            fs.write("pid,skill,cons\n")
 
             for i, p in enumerate(players):
                 if player_filter and i < player_filter:
                     continue
 
                 cols = [str(i), str(p.skill), str(p.consistency)]
                 rows.append(", ".join(cols))
@@ -199,14 +198,16 @@
         p = self.model.new_player(*args)
         self.model.player_pool.append(p)
         self._pool.append(self.ranker.new_player())
 
         # reset the matchmaker so he uses the updated pool
         self.reset()
 
+        return p
+
     def replace_player(self, *args, i=-1):
         """Replace an older player with a new one"""
         if self.pool is None:
             raise RuntimeError("No existing player pool")
 
         p = self.model.new_player(*args)
         self.model.player_pool[i] = p
```

### Comparing `ranked-0.0.1/ranked/matchmaker.py` & `ranked-1.0.2/ranked/matchmaker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import List, Tuple
+from typing import List
 
 import numpy as np
 
-from ranked.models import Batch, Match, Player, Ranker, Team
+from ranked.models import Player
 
 # List of player matched together
 MatchMakerTeam = List[int]
 # List of teams of a given match
 MatchMakerMatch = List[MatchMakerTeam]
```

### Comparing `ranked-0.0.1/ranked/models/__init__.py` & `ranked-1.0.2/ranked/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 from typing import Sequence, Union
 
 from ranked.utils import fetch_factories
 
 
 class Player:
     def skill(self) -> float:
@@ -25,35 +26,41 @@
 
     def __init__(self, *players, **config) -> None:
         self.players = players
         self.config = config
 
     def skill(self) -> float:
         """Returns the estimated skill of this team"""
-        return sum([player.skill() for player in self.players])
+        return sum(player.skill() for player in self.players)
 
     def __contains__(self, player):
         return player in self.players
 
     def __len__(self):
         return len(self.players)
 
-    def __getitem__(self):
-        return self.players[0]
+    def __getitem__(self, idx=0):
+        return self.players[idx]
 
     def __iter__(self):
         return iter(self.players)
 
     def __repr__(self) -> str:
         players = ", ".join([repr(p) for p in self.players])
         return f"{self.__class__.__name__}({players})"
 
 
 class Match:
-    """Represent a single match with N players"""
+    """Represent a single match with N players
+
+    >>> m = Match(('Player1', 10), ('Player2', 5))
+    >>> m.get_ranks()
+    [0, 1]
+
+    """
 
     def __init__(self, *leaderboard) -> None:
         self.players = [p for p, _ in leaderboard]
         self.scores = [r for _, r in leaderboard]
         self.leaderboard = leaderboard
 
     def __contains__(self, player):
@@ -62,14 +69,29 @@
     @property
     def teams(self):
         return self.players
 
     def get_score(self, index) -> float:
         return self.scores[index]
 
+    def get_ranks(self):
+        """Return ranks"""
+        scores = sorted(copy.deepcopy(self.scores), reverse=True)
+        ranks = []
+
+        for score in self.scores:
+
+            for rank, value in enumerate(scores):
+
+                if value == score:
+                    ranks.append(rank)
+                    continue
+
+        return ranks
+
     def get_enemy(self, player: Player) -> Player:
         """Get the enemy of the given player; only available for 1v1"""
         assert len(self.players) == 2
 
         if self.players[0] is player:
             return self.players[1]
```

### Comparing `ranked-0.0.1/ranked/models/elo.py` & `ranked-1.0.2/ranked/models/elo.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def skill(self) -> float:
         return self.mu
 
     @property
     def mu(self):
         if self._mu is None:
-            self._mu = sum([p.skill() for p in self.players])
+            self._mu = sum(p.skill() for p in self.players)
         return self._mu
 
     @mu.setter
     def mu(self, value):
         diff = value - self.mu
 
         for p in self.players:
```

### Comparing `ranked-0.0.1/ranked/models/elochess.py` & `ranked-1.0.2/ranked/models/elochess.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from scipy.stats import norm
-
 from ranked.models import Match, Ranker
 from ranked.models.elo import EloPlayer, EloTeam
 
 
 class ChessElo(Ranker):
     """Chess tweaked their distribution to match their data better of simplify the math"""
```

### Comparing `ranked-0.0.1/ranked/models/glicko2.py` & `ranked-1.0.2/ranked/models/glicko2.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,27 +38,27 @@
         self._rating = None
         self._deviation = None
         self._volatility = None
 
     @property
     def rating(self):
         if self._rating is None:
-            self._rating = sum([p.rating for p in self.players])
+            self._rating = sum(p.rating for p in self.players)
         return self._rating
 
     @property
     def deviation(self):
         if self._deviation is None:
-            self._deviation = math.sqrt(sum([p.deviation**2 for p in self.players]))
+            self._deviation = math.sqrt(sum(p.deviation**2 for p in self.players))
         return self._deviation
 
     @property
     def volatility(self):
         if self._volatility is None:
-            self._volatility = math.sqrt(sum([p.volatility**2 for p in self.players]))
+            self._volatility = math.sqrt(sum(p.volatility**2 for p in self.players))
 
         return self._volatility
 
     @rating.setter
     def rating(self, value):
         diff = value - self.rating
 
@@ -69,15 +69,15 @@
 
     @deviation.setter
     def deviation(self, value):
         # Volatility of the team is sqrt(sum(players))
         #   i.e the volatility of the overall team is not proportional
         #
         # Because we only observe the result of the overall team
-        # we cant really estimate the deviation of individual players
+        # we can't really estimate the deviation of individual players
 
         diff = value - self.deviation
 
         for p in self.players:
             p.deviation += diff * (p.deviation / self.deviation)
 
         self._deviation = None
```

### Comparing `ranked-0.0.1/ranked/models/noskill.py` & `ranked-1.0.2/ranked/models/noskill.py`

 * *Files identical despite different names*

### Comparing `ranked-0.0.1/ranked/simulation.py` & `ranked-1.0.2/ranked/simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-import json
 from collections import defaultdict
-from nis import match
-from typing import List
 
-from ranked.models import Batch, Match, Player, Ranker, Team
+from ranked.models import Batch, Match, Team
 
 
 class SaveEvolution:
     def __init__(self, fname: str, pool, ranker) -> None:
         self.fs = None
         if fname is not None:
             self.fs = open(fname, "w")
 
         self.header()
         self.ranker = ranker.__class__.__name__
         self.pool = pool
 
-        name = fname.rsplit(".", maxsplit=1)[0]
+        fname.rsplit(".", maxsplit=1)[0]
         self.previous = dict()
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args, **kwargs):
         if self.fs:
             self.fs.__exit__(*args, **kwargs)
 
     def header(self):
         if not self.fs:
             return
 
-        self.fs.write(f"#match,pid,skill,cons,method,diff,win\n")
+        self.fs.write("#match,pid,skill,cons,method,diff,win\n")
 
     def save(self, iter, method, player_filter=None):
         if not self.fs:
             return
 
         rows = []
         for pid, p in enumerate(self.pool):
@@ -62,15 +59,15 @@
 
         self.fs.write("\n".join(rows) + "\n")
 
 
 class Simulation:
     """Simulate ranking estimation evolution using simulated matches
 
-    On one side the matchmaker is working torwards making teams of equal strength
+    On one side the matchmaker is working towards making teams of equal strength
     while the Ranker is estimating the skill of each players from which the win
     probability of a given match can be deduced.
 
     Notes
     -----
     In case of simulated matchup, the matchmaker and the Ranker are both
     working for and against each other, for each other because the estimated
@@ -116,15 +113,15 @@
                     print(f"    Simulated {i + 1} matches")
 
             if i != last_print:
                 print(f"    Simulated {i + 1} matches")
 
     def benchmark(self, playerid=None):
         """Use the latest skill estimate for each player and estimate the win probabilities
-        for each matchup, if the Ranker estimated their skill corectly the precision should higher than 50%
+        for each matchup, if the Ranker estimated their skill correctly the precision should higher than 50%
         """
         acc = 0
         count = 0
         batch: Batch
         match: Match
         team: Team
         stats = dict()
@@ -157,15 +154,15 @@
                     avg += tskill
 
                     team_score = tskill
                     estimated_leaderboard.append((team, team_score))
 
                 # average skill diff in this match
                 avg = avg / len(match.teams)
-                avg_diff = sum([abs(team.skill() - avg) for team in match.teams]) / len(
+                avg_diff = sum(abs(team.skill() - avg) for team in match.teams) / len(
                     match.teams
                 )
 
                 diff += avg_diff
                 match_count += 1
 
                 # sort both
@@ -186,16 +183,16 @@
 
         # The average score difference between teams
         # smaller is better
         stats["matchmaker_diff"] = diff / match_count
 
         # Overall skill for every team should be even
         # regardless of their position inside the team array
-        avg = sum([v for _, v in team_skill.items()]) / len(team_skill)
-        avg_diff = sum([abs(v) - avg for _, v in team_skill.items()]) / len(team_skill)
+        avg = sum(v for _, v in team_skill.items()) / len(team_skill)
+        avg_diff = sum(abs(v) - avg for _, v in team_skill.items()) / len(team_skill)
 
         # Is the matchmaker biased toward a team
         # should be 0
         stats["matchmaker_team_bias"] = avg_diff
 
         return stats
 
@@ -231,15 +228,15 @@
 
     highlight_lines = encoded_lines.mark_line().encode(
         size=alt.condition(~highlight, alt.value(1), alt.value(3))
     )
 
     lines = points + highlight_lines
 
-    # put consitency at the bottom
+    # put consistency at the bottom
     x_ticks = (
         chart.mark_line()
         .encode(
             alt.X("#match:Q"),
             alt.Y("cons:Q", title="volatility"),
             color="pid:N",
             strokeDash="type:N",
@@ -318,22 +315,23 @@
     modeln = model.copy()
     modeln["#match"] = n_match
 
     data = pd.concat([evol, model, modeln])
     return data[data["pid"] >= n_players]
 
 
-def synthetic_main(n_matches_bootstrap=100, n_maches_newplayers=20, n_benchmark=100):
+def synthetic_main(n_matches_bootstrap=400, n_maches_newplayers=20, n_benchmark=200):
     """Simulates player and their skill estimate"""
     print("Synthetic Benchmark")
     print("===================")
 
     from ranked.datasets.synthetic import SimulationConfig, create_simulated_matchups
     from ranked.models.glicko2 import Glicko2
     from ranked.models.noskill import NoSkill
+    from ranked.models.openskill import OpenSkill
 
     center = 1500
     var = 64
     beta = 16
     n_players = 100
 
     config = SimulationConfig(
@@ -373,14 +371,16 @@
         # Impacts how spread out the score are going to be
         500 / 3,
         beta,
         tau=0.2,
         draw_probability=0,
     )
 
+    ranker = OpenSkill(mu=center, sigma=500 / 3, beta=beta, tau=0.2, initial_sigma=150)
+
     matchup = create_simulated_matchups(
         ranker,
         n_players,
         n_matches=n_matches_bootstrap,
         n_team=2,
         n_player_per_team=5,
         config=config,
@@ -391,16 +391,22 @@
     # Create the initial pool of players
     print("1. Bootstrap Player pool")
     sim.simulate(statfs="bootstrap.csv")
 
     # Benchmark
     print("2. Benchmark")
     matchup.n_matches = n_benchmark
-    for k, v in sim.benchmark().items():
-        print(f"{k:>30}: {v:.4f}")
+    repeat = 1
+    avg = defaultdict(int)
+    for _ in range(repeat):
+        for k, v in sim.benchmark().items():
+            avg[k] += v
+
+    for k, v in avg.items():
+        print(f"{k:>30}: {v / repeat:.4f}")
 
     # Check how new players are doing
     print("3. Add New Players")
 
     # Current pool of players have a perfect estimate
     matchup.set_estimate_to_truth()
 
@@ -414,16 +420,23 @@
 
     matchup.n_matches = n_maches_newplayers
     sim.simulate(statfs="newplayers.csv", filter=n_players)
 
     # Benchmark
     print("4. New Player Benchmark")
     matchup.n_matches = n_benchmark
-    for k, v in sim.benchmark(n_players).items():
-        print(f"{k:>30}: {v:.4f}")
+    repeat = 1
+    avg = defaultdict(int)
+
+    for _ in range(repeat):
+        for k, v in sim.benchmark(n_players).items():
+            avg[k] += v
+
+    for k, v in avg.items():
+        print(f"{k:>30}: {v / repeat:.4f}")
 
     # Plot skill estimation trajectories
     print("4. Generate Graphs")
     generate_viz()
 
 
 def generate_viz():
```

### Comparing `ranked-0.0.1/ranked/utils/__init__.py` & `ranked-1.0.2/ranked/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ranked-0.0.1/ranked.egg-info/PKG-INFO` & `ranked-1.0.2/ranked.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranked
-Version: 0.0.1
+Version: 1.0.2
 Summary: Player Ranking Algorithm benchmarks
 Home-page: https://github.com/Delaunay/ranked
 Author: Pierre Delaunay
 Author-email: pierre@delaunay.io
 License: BSD-3-Clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -13,19 +13,19 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.*
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 License-File: LICENSE
 
 ranked
 ======
 
 |pypi| |py_versions| |license|
 |rtfd| |codecov| |style| |tests|
@@ -86,20 +86,38 @@
    of the ranking algorithm. It is up to the matchmaking algorithm to make sure
    the teams it builds are as fair as possible.
 
    The ranking algorithm only provide an estimate of each player'skill to help
    the matchmaker to make the best decision possible.
 
 
+Examples
+--------
+
+.. code-block:: python
+
+    ranker = ChessElo()
+    p1 = ranker.new_player((1613 - sub) / div)
+    p2 = ranker.new_player((1609 - sub) / div)
+
+    m1 = Match((p1, 0), (p2, 1)),  # p1 lost (lower score)
+
+    win_prob = ranker.win(m)
+
+    ranker.update(m)
+
+    # P1 lost so its skill got updated down
+    new_skill = p1.skill()  # 1603.19
+
+
 WIP
 ---
 
 * NoSkill2
 * Dota2 extracted matches
-* publish to Pypi
 
 
 .. code-block:: bash
 
    pip install ranked
```

### Comparing `ranked-0.0.1/ranked.egg-info/SOURCES.txt` & `ranked-1.0.2/ranked.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 ranked/__init__.py
 ranked/calibration.py
 ranked/matchmaker.py
 ranked/simulation.py
 ranked.egg-info/PKG-INFO
 ranked.egg-info/SOURCES.txt
@@ -17,8 +18,9 @@
 ranked/datasets/replay.py
 ranked/datasets/synthetic.py
 ranked/models/__init__.py
 ranked/models/elo.py
 ranked/models/elochess.py
 ranked/models/glicko2.py
 ranked/models/noskill.py
+ranked/models/openskill.py
 ranked/utils/__init__.py
```

### Comparing `ranked-0.0.1/setup.py` & `ranked-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 #!/usr/bin/env python
-from setuptools import setup
+import os
 from pathlib import Path
 
-import os
+from setuptools import setup
 
 repo_root = os.path.dirname(os.path.abspath(__file__))
 
 
 with open("ranked/__init__.py") as file:
     for line in file.readlines():
-        if 'version' in line:
-            version = line.split('=')[1].strip().replace('"', "")
+        if "version" in line:
+            version = line.split("=")[1].strip().replace('"', "")
             break
 
 args = dict(
     name="ranked",
-    version="0.0.1",
+    version=version,
     description="Player Ranking Algorithm benchmarks",
     long_description=(Path(__file__).parent / "README.rst").read_text(),
     author="Pierre Delaunay",
     author_email="pierre@delaunay.io",
-    license='BSD-3-Clause',
+    license="BSD-3-Clause",
     url="https://github.com/Delaunay/ranked",
     packages=[
         "ranked",
         "ranked.models",
         "ranked.datasets",
         "ranked.utils",
     ],
     zip_safe=True,
-    python_requires='>=3.7.*',
+    python_requires=">=3.7",
     install_requires=[
         "scipy",
         "altair",
         "trueskill",
+        "openskill",
         "numpy",
-        'orion',
-        'typing_extensions',
+        "orion",
+        "typing_extensions",
     ],
     setup_requires=["setuptools"],
 )
 
 args["classifiers"] = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Developers",
@@ -48,11 +49,13 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
-] + [("Programming Language :: Python :: %s" % x) for x in "3 3.7 3.8 3.9 3.10".split()]
+] + [
+    ("Programming Language :: Python :: %s" % x) for x in "3 3.8 3.9 3.10 3.11".split()
+]
 
 if __name__ == "__main__":
     setup(**args)
```

