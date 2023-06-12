# Comparing `tmp/alltime_athletics_python-0.8.0.tar.gz` & `tmp/alltime_athletics_python-1.0.20230612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alltime_athletics_python-0.8.0.tar", max compression
+gzip compressed data, was "alltime_athletics_python-1.0.20230612.tar", max compression
```

## Comparing `alltime_athletics_python-0.8.0.tar` & `alltime_athletics_python-1.0.20230612.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-0.8.0/LICENSE
--rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-0.8.0/alltime_athletics_python/__init__.py
--rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-0.8.0/alltime_athletics_python/get_content.py
--rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-0.8.0/alltime_athletics_python/get_content_urls.py
--rw-r--r--   0        0        0     3602 2023-06-05 09:07:54.851615 alltime_athletics_python-0.8.0/alltime_athletics_python/io.py
--rw-r--r--   0        0        0    11784 2023-06-05 09:05:25.415701 alltime_athletics_python-0.8.0/alltime_athletics_python/pipes.py
--rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-0.8.0/alltime_athletics_python/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-0.8.0/alltime_athletics_python/utils/config.py
--rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-0.8.0/alltime_athletics_python/utils/logger.py
--rw-r--r--   0        0        0     1077 2023-06-05 09:11:59.949022 alltime_athletics_python-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 alltime_athletics_python-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-1.0.20230612/LICENSE
+-rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-1.0.20230612/alltime_athletics_python/__init__.py
+-rw-r--r--   0        0        0      469 2023-06-12 08:42:56.348792 alltime_athletics_python-1.0.20230612/alltime_athletics_python/app.py
+-rw-r--r--   0        0        0     2478 2023-06-05 13:49:25.196214 alltime_athletics_python-1.0.20230612/alltime_athletics_python/events.py
+-rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-1.0.20230612/alltime_athletics_python/get_content.py
+-rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-1.0.20230612/alltime_athletics_python/get_content_urls.py
+-rw-r--r--   0        0        0     5231 2023-06-06 05:25:55.084484 alltime_athletics_python-1.0.20230612/alltime_athletics_python/io.py
+-rw-r--r--   0        0        0    11029 2023-06-06 05:25:59.032322 alltime_athletics_python-1.0.20230612/alltime_athletics_python/pipes.py
+-rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-1.0.20230612/alltime_athletics_python/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-1.0.20230612/alltime_athletics_python/utils/config.py
+-rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-1.0.20230612/alltime_athletics_python/utils/logger.py
+-rw-r--r--   0        0        0     1146 2023-06-12 08:46:41.454461 alltime_athletics_python-1.0.20230612/pyproject.toml
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 alltime_athletics_python-1.0.20230612/PKG-INFO
```

### Comparing `alltime_athletics_python-0.8.0/LICENSE` & `alltime_athletics_python-1.0.20230612/LICENSE`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.8.0/alltime_athletics_python/get_content.py` & `alltime_athletics_python-1.0.20230612/alltime_athletics_python/get_content.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.8.0/alltime_athletics_python/get_content_urls.py` & `alltime_athletics_python-1.0.20230612/alltime_athletics_python/get_content_urls.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.8.0/alltime_athletics_python/pipes.py` & `alltime_athletics_python-1.0.20230612/alltime_athletics_python/pipes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,27 @@
 import polars as pl
 
+from alltime_athletics_python.events import event_list
+
 
 def pipe_remove_invalid(df: pl.DataFrame) -> pl.DataFrame:
     return (
         df.sort("event", "rank")
         .with_columns(
             (
                 pl.col("result seconds") >= pl.col("result seconds").over("event").min()
             ).alias("valid")
         )
         .filter(pl.col("valid"))
     )
 
 
 def pipe_get_event_distance(df: pl.DataFrame) -> pl.DataFrame:
-    def distance_mapping(event):
-        d = {
-            "200 metres": 200,
-            "marathon": 42195,
-            "1 Mile": 1609,
-            "1500 metres": 1500,
-            "50 km race walk": 50000,
-            "3000m steeplechase": 3000,
-            "400 metres": 400,
-            "5000 metres": 5000,
-            "20 km race walk": 20000,
-            "3000 metres": 3000,
-            "400m hurdles": 400,
-            "100 metres": 100,
-            "800 metres": 800,
-            "100m hurdles": 100,
-            "110m hurdles": 110,
-            "half-marathon": 21097.5,
-            "10000 metres": 10000,
-        }
+    def distance_mapping(event) -> float:
+        d = {event.name: event.distance for event in event_list}
         return d[event]
 
     return df.with_columns(  # get event distances
         pl.col("event").apply(lambda e: distance_mapping(e)).alias("distance")
     )
 
 
@@ -53,90 +37,36 @@
         ).alias("percentage of wr")
     ).with_columns(
         pl.col("percentage of wr").rank().over("event").cast(int).alias("rank")
     )
 
 
 def pipe_assign_sprint_middle_long_distance(df: pl.DataFrame) -> pl.DataFrame:
-    def assign(event):
-        d = {
-            "100m hurdles": "sprint",
-            "110m hurdles": "sprint",
-            "1500 metres": "middle distance",
-            "3000m steeplechase": "middle distance",
-            "1 Mile": "middle distance",
-            "20 km race walk": "long distance",
-            "200 metres": "sprint",
-            "100 metres": "sprint",
-            "half-marathon": "long distance",
-            "10000 metres": "long distance",
-            "5000 metres": "long distance",
-            "marathon": "long distance",
-            "3000 metres": "middle distance",
-            "50 km race walk": "long distance",
-            "800 metres": "middle distance",
-            "400 metres": "sprint",
-            "400m hurdles": "sprint",
-        }
+    def assign(event) -> str:
+        d = {event.name: event.distance_type for event in event_list}
         return d[event]
 
     return df.with_columns(
         pl.col("event").apply(lambda e: assign(e)).alias("distance type")
     )
 
 
 def pipe_assign_has_hurdles_or_not(df: pl.DataFrame) -> pl.DataFrame:
-    def assign(event):
-        d = {
-            "100m hurdles": True,
-            "110m hurdles": True,
-            "1500 metres": False,
-            "3000m steeplechase": True,
-            "1 Mile": False,
-            "20 km race walk": False,
-            "200 metres": False,
-            "100 metres": False,
-            "half-marathon": False,
-            "10000 metres": False,
-            "5000 metres": False,
-            "marathon": False,
-            "3000 metres": False,
-            "50 km race walk": False,
-            "800 metres": False,
-            "400 metres": False,
-            "400m hurdles": True,
-        }
+    def assign(event) -> bool:
+        d = {event.name: event.has_hurdles for event in event_list}
         return d[event]
 
     return df.with_columns(
         pl.col("event").apply(lambda e: assign(e)).alias("has hurdles")
     )
 
 
 def pipe_assign_track_event_or_not(df: pl.DataFrame) -> pl.DataFrame:
     def assign(event):
-        d = {
-            "100m hurdles": True,
-            "110m hurdles": True,
-            "1500 metres": True,
-            "3000m steeplechase": True,
-            "1 Mile": True,
-            "20 km race walk": False,
-            "200 metres": True,
-            "100 metres": True,
-            "half-marathon": False,
-            "10000 metres": True,
-            "5000 metres": True,
-            "marathon": False,
-            "3000 metres": True,
-            "50 km race walk": False,
-            "800 metres": True,
-            "400 metres": True,
-            "400m hurdles": True,
-        }
+        d = {event.name: event.is_track for event in event_list}
         return d[event]
 
     return df.with_columns(pl.col("event").apply(lambda e: assign(e)).alias("on track"))
 
 
 def pipe_fix_issue_with_half_marathon_distance(df: pl.DataFrame) -> pl.DataFrame:
     return df.with_columns(
@@ -145,15 +75,15 @@
         .otherwise(pl.col("distance"))
         .alias("distance")
     )
 
 
 def pipe_convert_time_to_seconds(df: pl.DataFrame) -> pl.DataFrame:
     def convert_time_to_seconds(time_string):
-        to_replace = ["A", "y", "+", "#", "a", "d", "´", "@", "p"]
+        to_replace = ["A", "y", "+", "#", "a", "d", "´", "@", "p", "m", "*", "e"]
         for r in to_replace:
             time_string = time_string.replace(r, "")
 
         time_parts = time_string.split(":")
         if len(time_parts) == 3:  # hours:minutes:seconds
             return (
                 int(time_parts[0]) * 3600
@@ -172,20 +102,25 @@
 
 def pipe_fix_dtype(df: pl.DataFrame) -> pl.DataFrame:
     return df.with_columns(pl.col("rank").cast(int))
 
 
 def pipe_rename_columns_names_men(df: pl.DataFrame) -> pl.DataFrame:
     def decide_mapping_men(name, number_columns, mappings):
+        if "200m hurdles" in name:
+            return mappings[4]
+        if "300 metres" in name:
+            return mappings[5]
         if "half" in name:
             return mappings[2]
         if "1500" in name or "400m hurdles" in name:
             return mappings[3]
         if number_columns == 12:
             return mappings[0]
+
         return mappings[1]
 
     def get_mappings_men() -> list[dict[str, str]]:
         return [
             {
                 "0": "rank",
                 "1": "result",
@@ -223,34 +158,57 @@
                 "2": "name",
                 "4": "nationality",
                 "5": "date of birth",
                 "6": "rank in event",
                 "7": "location of event",
                 "8": "date of event",
             },
+            {
+                "0": "rank",
+                "1": "result",
+                "2": "wind",
+                "3": "name",
+                "4": "nationality",
+                "5": "date of birth",
+                "6": "rank in event",
+                "7": "location of event",
+                "10": "date of event",
+            },
+            {
+                "0": "rank",
+                "1": "result",
+                "2": "name",
+                "4": "nationality",
+                "5": "date of birth",
+                "6": "rank in event",
+                "7": "location of event",
+                "8": "date of event",
+            },
         ]
 
     mappings = get_mappings_men()
 
     return df.with_columns([pl.col(c).cast(str) for c in df.columns]).rename(
         mapping=decide_mapping_men(df["event"].unique()[0], len(df.columns), mappings)
     )
 
 
 def pipe_rename_columns_names_women(df: pl.DataFrame) -> pl.DataFrame:
-    def decide_mapping_men(name, number_columns, mappings):
+    def decide_mapping_women(name, number_columns, mappings):
+        if "15k" in name or "20km" in name:
+            return mappings[3]
         if "half" in name:
             return mappings[2]
         # if "1500" in name or "400m hurdles" in name:
         #    return mappings[3]
         if number_columns == 12:
             return mappings[0]
         return mappings[1]
 
-    def get_mappings_men() -> list[dict[str, str]]:
+    def get_mappings_women() -> list[dict[str, str]]:
         return [
             {
                 "0": "rank",
                 "1": "result",
                 "2": "wind",
                 "3": "name",
                 "4": "nationality",
@@ -279,40 +237,40 @@
                 "6": "location of event",
                 "8": "date of event",
             },
             {
                 "0": "rank",
                 "1": "result",
                 "2": "name",
-                "4": "nationality",
-                "5": "date of birth",
-                "6": "rank in event",
-                "7": "location of event",
+                "3": "nationality",
+                "4": "date of birth",
+                "5": "rank in event",
+                "6": "location of event",
                 "8": "date of event",
             },
         ]
 
-    mappings = get_mappings_men()
+    mappings = get_mappings_women()
 
     return df.with_columns([pl.col(c).cast(str) for c in df.columns]).rename(
-        mapping=decide_mapping_men(df["event"].unique()[0], len(df.columns), mappings)
+        mapping=decide_mapping_women(df["event"].unique()[0], len(df.columns), mappings)
     )
 
 
 def pipe_assign_file_name(df: pl.DataFrame, file: str) -> pl.DataFrame:
     return df.with_columns(
         [
             pl.lit(file.split("/")[4]).alias("event"),
             pl.lit(file).alias("file"),
         ]
     )
 
 
 def pipe_drop_unwanted_columns(df: pl.DataFrame) -> pl.DataFrame:
-    should_be_dropped = ["3", "valid", "", "7"]
+    should_be_dropped = ["3", "valid", "", "7", "8", "9", "10"]
     columns = [c for c in should_be_dropped if c in df.columns]
     return df.drop(columns=columns)
 
 
 def pipe_get_wr_strength_by_comparing_with_tenth(df: pl.DataFrame) -> pl.DataFrame:
     return df.with_columns(  # add percentages w.r.t world records
         (
@@ -356,14 +314,15 @@
         ]
     )
 
 
 def pipe_reorder_and_select_subset_of_columns(df: pl.DataFrame) -> pl.DataFrame:
     return df.select(
         "event",
+        "event type",
         "distance",
         "sex",
         "rank",
         "rank in event",
         "name",
         "nationality",
         "date of birth",
@@ -375,7 +334,24 @@
         "distance type",
         "has hurdles",
         "on track",
         # "percentage of wr",
         # "percentage of 10th",
         "file",
     )
+
+
+def pipe_compute_age_at_event(df: pl.DataFrame) -> pl.DataFrame:
+    return df.with_columns(
+        ((pl.col("date of event") - pl.col("date of birth")).dt.days() / 365).alias(
+            "age at event in years"
+        )
+    )
+
+
+def pipe_give_same_name_to_100m_and_110m_hurdles(df: pl.DataFrame) -> pl.DataFrame:
+    return df.with_columns(
+        pl.when(pl.col("event").is_in(["110m hurdles", "100m hurdles"]))
+        .then(pl.lit("100m/110m hurdles"))
+        .otherwise(pl.col("event"))
+        .alias("event")
+    )
```

### Comparing `alltime_athletics_python-0.8.0/alltime_athletics_python/utils/config.py` & `alltime_athletics_python-1.0.20230612/alltime_athletics_python/utils/config.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.8.0/alltime_athletics_python/utils/logger.py` & `alltime_athletics_python-1.0.20230612/alltime_athletics_python/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.8.0/pyproject.toml` & `alltime_athletics_python-1.0.20230612/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "alltime_athletics_python"
-version = "0.8.0"
+version = "1.0.20230612"
 description = "Scrapes and post-processes data from Alltime Athletics (website by Peter Larsson)"
 homepage= "https://github.com/thomascamminady/alltime_athletics_python"
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.2"
 lxml = "^4.9.2"
 html5lib = "^1.1"
 rich = "^13.4.1"
 polars = "^0.18.0"
+ipywidgets = "^8.0.6"
+pyarrow = "^12.0.0"
+tabulate = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
 ruff = "^0.0.253"
 black = "^23.1.0"
 pyclean = "^2.2.0"
 pre-commit = "^3.1.1"
```

### Comparing `alltime_athletics_python-0.8.0/PKG-INFO` & `alltime_athletics_python-1.0.20230612/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: alltime-athletics-python
-Version: 0.8.0
+Version: 1.0.20230612
 Summary: Scrapes and post-processes data from Alltime Athletics (website by Peter Larsson)
 Home-page: https://github.com/thomascamminady/alltime_athletics_python
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: html5lib (>=1.1,<2.0)
+Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: polars (>=0.18.0,<0.19.0)
+Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
```

