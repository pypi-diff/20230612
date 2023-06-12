# Comparing `tmp/humanity_etl-0.0.1rc4.tar.gz` & `tmp/humanity_etl-0.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanity_etl-0.0.1rc4.tar", last modified: Thu Jun  8 18:52:11 2023, max compression
+gzip compressed data, was "humanity_etl-0.0.1rc5.tar", last modified: Mon Jun 12 20:31:05 2023, max compression
```

## Comparing `humanity_etl-0.0.1rc4.tar` & `humanity_etl-0.0.1rc5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:52:11.054214 humanity_etl-0.0.1rc4/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.0.1rc4/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-08 18:52:11.054214 humanity_etl-0.0.1rc4/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      984 2023-06-08 17:49:58.000000 humanity_etl-0.0.1rc4/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:52:11.054214 humanity_etl-0.0.1rc4/humanity_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 humanity_etl-0.0.1rc4/humanity_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-08 17:37:37.000000 humanity_etl-0.0.1rc4/humanity_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      328 2023-06-08 17:11:05.000000 humanity_etl-0.0.1rc4/humanity_etl/humanity_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:52:11.054214 humanity_etl-0.0.1rc4/humanity_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.0.1rc4/humanity_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4129 2023-06-08 18:00:43.000000 humanity_etl-0.0.1rc4/humanity_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 humanity_etl-0.0.1rc4/humanity_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      547 2023-06-08 18:02:02.000000 humanity_etl-0.0.1rc4/humanity_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5966 2023-06-08 18:01:30.000000 humanity_etl-0.0.1rc4/humanity_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:52:11.054214 humanity_etl-0.0.1rc4/humanity_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.0.1rc4/humanity_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4135 2023-06-08 18:00:43.000000 humanity_etl-0.0.1rc4/humanity_etl/tables/timeclocks.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:52:11.054214 humanity_etl-0.0.1rc4/humanity_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-08 18:52:11.000000 humanity_etl-0.0.1rc4/humanity_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      520 2023-06-08 18:52:11.000000 humanity_etl-0.0.1rc4/humanity_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-08 18:52:11.000000 humanity_etl-0.0.1rc4/humanity_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-08 18:52:11.000000 humanity_etl-0.0.1rc4/humanity_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-08 18:52:11.000000 humanity_etl-0.0.1rc4/humanity_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-08 18:52:11.054214 humanity_etl-0.0.1rc4/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      990 2023-06-08 18:51:52.000000 humanity_etl-0.0.1rc4/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:52:11.054214 humanity_etl-0.0.1rc4/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.0.1rc4/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.0.1rc5/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      984 2023-06-08 17:49:58.000000 humanity_etl-0.0.1rc5/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.792217 humanity_etl-0.0.1rc5/humanity_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 humanity_etl-0.0.1rc5/humanity_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-08 17:37:37.000000 humanity_etl-0.0.1rc5/humanity_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      328 2023-06-08 17:11:05.000000 humanity_etl-0.0.1rc5/humanity_etl/humanity_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/humanity_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4841 2023-06-12 19:40:35.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      547 2023-06-12 20:29:22.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5966 2023-06-08 18:01:30.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/humanity_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.0.1rc5/humanity_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4489 2023-06-12 20:29:08.000000 humanity_etl-0.0.1rc5/humanity_etl/tables/timeclocks.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.792217 humanity_etl-0.0.1rc5/humanity_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      520 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      990 2023-06-12 20:30:51.000000 humanity_etl-0.0.1rc5/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.0.1rc5/tests/__init__.py
```

### Comparing `humanity_etl-0.0.1rc4/PKG-INFO` & `humanity_etl-0.0.1rc5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity_etl
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `humanity_etl-0.0.1rc4/README_PUBLIC.md` & `humanity_etl-0.0.1rc5/README_PUBLIC.md`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc4/humanity_etl/libs/cnst.py` & `humanity_etl-0.0.1rc5/humanity_etl/libs/cnst.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,8 +88,24 @@
     ),
     "edm_timeclocks": "https://www.humanity.com/api/v2/timeclocks?access_token={}".format(
         os.environ.get("EDM_ACCESS_TOKEN")
     ),
     "edm_shifts": "https://www.humanity.com/api/v2/shifts?access_token={}".format(
         os.environ.get("EDM_ACCESS_TOKEN")
     ),
+    "mtl_employees": "https://www.humanity.com/api/v2/employees?access_token={}".format(
+        os.environ.get("MTL_ACCESS_TOKEN")
+    ),
+    "mtl_employees_disabled": "https://www.humanity.com/api/v2/employees?disabled=1&access_token={}".format(
+        os.environ.get("MTL_ACCESS_TOKEN")
+    ),
+    "mtl_positions": "https://www.humanity.com/api/v2/positions?access_token={}".format(
+        os.environ.get("MTL_ACCESS_TOKEN")
+    ),
+    "mtl_timeclocks": "https://www.humanity.com/api/v2/timeclocks?access_token={}".format(
+        os.environ.get("MTL_ACCESS_TOKEN")
+    ),
+    "mtl_shifts": "https://www.humanity.com/api/v2/shifts?access_token={}".format(
+        os.environ.get("MTL_ACCESS_TOKEN")
+    ),
+
 }
```

### Comparing `humanity_etl-0.0.1rc4/humanity_etl/libs/dbg.py` & `humanity_etl-0.0.1rc5/humanity_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc4/humanity_etl/libs/network.py` & `humanity_etl-0.0.1rc5/humanity_etl/libs/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 
 from humanity_etl.libs.dbg import dbg
 
 
 def get_data(api_url: str, headers: Dict[str, str]) -> Dict[str, Any]:
     """Make a GET request to the Humanity API and return the data."""
     dbg("Making request to {api_url}", api_url=api_url)
-    response = requests.get(api_url, headers=headers, timeout=10)
+    response = requests.get(api_url, headers=headers, timeout=20)
     dbg("{api_url} response code {code}", api_url=api_url, code=response.status_code)
     response.raise_for_status()
     data = json.loads(response.text)
     return data
```

### Comparing `humanity_etl-0.0.1rc4/humanity_etl/libs/transform.py` & `humanity_etl-0.0.1rc5/humanity_etl/libs/transform.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc4/humanity_etl/tables/timeclocks.py` & `humanity_etl-0.0.1rc5/humanity_etl/tables/timeclocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,20 @@
     )
     gta_timeclocks_df, gta_employees_df, gta_positions_df, gta_shifts_df = framer(
         frames["gta_timeclocks"],
         frames["gta_employees"],
         frames["gta_positions"],
         frames["gta_shifts"],
     )
+    mtl_timeclocks_df, mtl_employees_df, mtl_positions_df, mtl_shifts_df = framer(
+        frames["mtl_timeclocks"],
+        frames["mtl_employees"],
+        frames["mtl_positions"],
+        frames["mtl_shifts"],
+    )
 
     """
     Join regions dataframe into regions output, then into final humanity dataframe
     """
     gta_program_df = merger(
         gta_timeclocks_df, gta_positions_df, gta_employees_df, gta_shifts_df, "GTA"
     )
@@ -96,18 +102,21 @@
     )
     ott_program_df = merger(
         ott_timeclocks_df, ott_positions_df, ott_employees_df, ott_shifts_df, "OTT"
     )
     edm_program_df = merger(
         edm_timeclocks_df, edm_positions_df, edm_employees_df, edm_shifts_df, "EDM"
     )
+    mtl_program_df = merger(
+        mtl_timeclocks_df, mtl_positions_df, mtl_employees_df, mtl_shifts_df, "EDM"
+    )
 
     # "UNION" all region dataframes
     humanity_df = pd.concat(
-        [gta_program_df, cgy_program_df, wpg_program_df, edm_program_df, ott_program_df]
+        [gta_program_df, cgy_program_df, wpg_program_df, edm_program_df, ott_program_df, mtl_program_df]
     )
     humanity_final_df = humanity_df.merge(
         parent_employees_df2, left_on="employee_name", right_on="name", how="left"
     )
 
     # "Coalesce" emails to fill in blanks
     humanity_final_df["employee_email"] = humanity_final_df.email.combine_first(
```

### Comparing `humanity_etl-0.0.1rc4/humanity_etl.egg-info/PKG-INFO` & `humanity_etl-0.0.1rc5/humanity_etl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity-etl
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `humanity_etl-0.0.1rc4/humanity_etl.egg-info/SOURCES.txt` & `humanity_etl-0.0.1rc5/humanity_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc4/setup.py` & `humanity_etl-0.0.1rc5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="humanity_etl",
-    version="0.0.1rc4",
+    version="0.0.1rc5",
     description="Replicate humanity data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
```

