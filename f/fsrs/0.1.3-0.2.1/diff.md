# Comparing `tmp/fsrs-0.1.3.tar.gz` & `tmp/fsrs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs-0.1.3.tar", last modified: Tue Apr 11 11:03:03 2023, max compression
+gzip compressed data, was "fsrs-0.2.1.tar", last modified: Mon Jun 12 06:06:41 2023, max compression
```

## Comparing `fsrs-0.1.3.tar` & `fsrs-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.311644 fsrs-0.1.3/
--rw-r--r--   0 jarrettye   (501) staff       (20)     1079 2022-11-28 10:42:22.000000 fsrs-0.1.3/LICENSE
--rw-r--r--   0 jarrettye   (501) staff       (20)     3340 2023-04-11 11:03:03.311195 fsrs-0.1.3/PKG-INFO
--rw-r--r--   0 jarrettye   (501) staff       (20)     1647 2023-02-27 08:38:12.000000 fsrs-0.1.3/README.md
--rw-r--r--   0 jarrettye   (501) staff       (20)      593 2023-04-11 10:58:40.000000 fsrs-0.1.3/pyproject.toml
--rw-r--r--   0 jarrettye   (501) staff       (20)       38 2023-04-11 11:03:03.311714 fsrs-0.1.3/setup.cfg
--rw-r--r--   0 jarrettye   (501) staff       (20)       37 2022-11-28 09:57:57.000000 fsrs-0.1.3/setup.py
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.307133 fsrs-0.1.3/src/
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.309379 fsrs-0.1.3/src/fsrs/
--rw-r--r--   0 jarrettye   (501) staff       (20)       97 2023-04-11 10:58:57.000000 fsrs-0.1.3/src/fsrs/__init__.py
--rw-r--r--   0 jarrettye   (501) staff       (20)     4575 2023-04-11 10:50:58.000000 fsrs-0.1.3/src/fsrs/fsrs.py
--rw-r--r--   0 jarrettye   (501) staff       (20)     4423 2023-04-11 10:50:58.000000 fsrs-0.1.3/src/fsrs/models.py
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.310618 fsrs-0.1.3/src/fsrs.egg-info/
--rw-r--r--   0 jarrettye   (501) staff       (20)     3340 2023-04-11 11:03:03.000000 fsrs-0.1.3/src/fsrs.egg-info/PKG-INFO
--rw-r--r--   0 jarrettye   (501) staff       (20)      245 2023-04-11 11:03:03.000000 fsrs-0.1.3/src/fsrs.egg-info/SOURCES.txt
--rw-r--r--   0 jarrettye   (501) staff       (20)        1 2023-04-11 11:03:03.000000 fsrs-0.1.3/src/fsrs.egg-info/dependency_links.txt
--rw-r--r--   0 jarrettye   (501) staff       (20)        5 2023-04-11 11:03:03.000000 fsrs-0.1.3/src/fsrs.egg-info/top_level.txt
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-04-11 11:03:03.310808 fsrs-0.1.3/tests/
--rw-r--r--   0 jarrettye   (501) staff       (20)     1535 2022-11-30 08:56:29.000000 fsrs-0.1.3/tests/test_fsrs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 06:06:19.000000 fsrs-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-12 06:06:41.140491 fsrs-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-12 06:06:19.000000 fsrs-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-12 06:06:19.000000 fsrs-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 06:06:41.140491 fsrs-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 06:06:19.000000 fsrs-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/src/fsrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-12 06:06:19.000000 fsrs-0.2.1/src/fsrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-12 06:06:19.000000 fsrs-0.2.1/src/fsrs/fsrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-12 06:06:19.000000 fsrs-0.2.1/src/fsrs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/src/fsrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-12 06:06:41.000000 fsrs-0.2.1/src/fsrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-12 06:06:41.000000 fsrs-0.2.1/src/fsrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 06:06:41.000000 fsrs-0.2.1/src/fsrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 06:06:41.000000 fsrs-0.2.1/src/fsrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-12 06:06:19.000000 fsrs-0.2.1/tests/test_fsrs.py
```

### Comparing `fsrs-0.1.3/LICENSE` & `fsrs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fsrs-0.1.3/PKG-INFO` & `fsrs-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 0.1.3
+Version: 0.2.1
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-0.1.3/README.md` & `fsrs-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fsrs-0.1.3/pyproject.toml` & `fsrs-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fsrs"
-version = "0.1.3"
+version = "0.2.1"
 description = "Free Spaced Repetition Scheduler"
 readme = "README.md"
 authors = [{ name = "Jarrett Ye", email = "jarrett.ye@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `fsrs-0.1.3/src/fsrs/fsrs.py` & `fsrs-0.2.1/src/fsrs/fsrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             retrievability = math.exp(math.log(0.9) * interval / last_s)
             self.next_ds(s, last_d, last_s, retrievability)
 
             hard_interval = self.next_interval(last_s * self.p.hard_factor)
             good_interval = self.next_interval(s.good.stability)
             hard_interval = min(hard_interval, good_interval)
             good_interval = max(good_interval, hard_interval + 1)
-            easy_interval = max(self.next_interval(s.easy.stability * self.p.hard_factor), good_interval + 1)
+            easy_interval = max(self.next_interval(s.easy.stability * self.p.easy_bonus), good_interval + 1)
             s.schedule(now, hard_interval, good_interval, easy_interval)
         return s.record_log(card, now)
 
     def init_ds(self, s: SchedulingCards) -> None:
         s.again.difficulty = self.init_difficulty(Rating.Again)
         s.again.stability = self.init_stability(Rating.Again)
         s.hard.difficulty = self.init_difficulty(Rating.Hard)
```

### Comparing `fsrs-0.1.3/src/fsrs/models.py` & `fsrs-0.2.1/src/fsrs/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime, timedelta
 import copy
-from typing import Tuple
+import math
+from typing import Tuple, Optional
 from enum import IntEnum
 
 
 class State(IntEnum):
     New = 0
     Learning = 1
     Review = 2
@@ -50,14 +51,22 @@
         self.difficulty = 0
         self.elapsed_days = 0
         self.scheduled_days = 0
         self.reps = 0
         self.lapses = 0
         self.state = State.New
 
+    
+    def get_retrievability(self, now: datetime) -> Optional[float]:
+        if self.state == State.Review:
+            elapsed_days = max(0, (now - self.last_review).days)
+            return math.exp(math.log(0.9) * elapsed_days / self.stability)
+        else:
+            return None
+
 
 class SchedulingInfo:
     card: Card
     Review_log: ReviewLog
 
     def __init__(self, card: Card, review_log: ReviewLog) -> None:
         self.card = card
```

### Comparing `fsrs-0.1.3/src/fsrs.egg-info/PKG-INFO` & `fsrs-0.2.1/src/fsrs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 0.1.3
+Version: 0.2.1
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-0.1.3/tests/test_fsrs.py` & `fsrs-0.2.1/tests/test_fsrs.py`

 * *Files identical despite different names*

