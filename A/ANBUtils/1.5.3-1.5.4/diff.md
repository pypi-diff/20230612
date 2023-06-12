# Comparing `tmp/ANBUtils-1.5.3.tar.gz` & `tmp/ANBUtils-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.5.3.tar", last modified: Tue Jun  6 06:05:52 2023, max compression
+gzip compressed data, was "dist/ANBUtils-1.5.4.tar", last modified: Mon Jun 12 11:58:38 2023, max compression
```

## Comparing `ANBUtils-1.5.3.tar` & `ANBUtils-1.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-06 06:05:52.455417 ANBUtils-1.5.3/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-06 06:05:52.454136 ANBUtils-1.5.3/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)      860 2023-06-06 05:14:01.000000 ANBUtils-1.5.3/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     2483 2023-06-05 18:09:00.000000 ANBUtils-1.5.3/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)     5636 2023-06-06 04:02:14.000000 ANBUtils-1.5.3/ANBUtils/db_worker.py
--rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.5.3/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)      628 2023-06-06 04:53:39.000000 ANBUtils-1.5.3/ANBUtils/environ_cheker.py
--rw-r--r--   0 redbson    (501) staff       (20)     3509 2023-06-06 05:12:32.000000 ANBUtils-1.5.3/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)     1127 2023-06-06 05:13:30.000000 ANBUtils-1.5.3/ANBUtils/messager.py
--rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.5.3/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-06 06:05:52.454981 ANBUtils-1.5.3/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)     4916 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      343 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-06 06:05:52.000000 ANBUtils-1.5.3/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)     4916 2023-06-06 06:05:52.455222 ANBUtils-1.5.3/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)     4526 2023-06-06 04:58:53.000000 ANBUtils-1.5.3/README.md
--rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-06 06:05:52.455479 ANBUtils-1.5.3/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      817 2023-06-06 05:14:01.000000 ANBUtils-1.5.3/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-12 11:58:38.747028 ANBUtils-1.5.4/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-12 11:58:38.745784 ANBUtils-1.5.4/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)      860 2023-06-12 11:57:56.000000 ANBUtils-1.5.4/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     2483 2023-06-05 18:09:00.000000 ANBUtils-1.5.4/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)     6872 2023-06-12 11:56:40.000000 ANBUtils-1.5.4/ANBUtils/db_worker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.5.4/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)      226 2023-06-05 18:59:08.000000 ANBUtils-1.5.4/ANBUtils/environ_cheker.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3509 2023-06-06 05:12:32.000000 ANBUtils-1.5.4/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1127 2023-06-06 05:13:30.000000 ANBUtils-1.5.4/ANBUtils/messager.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.5.4/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-12 11:58:38.746595 ANBUtils-1.5.4/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)      123 2023-06-12 11:58:38.000000 ANBUtils-1.5.4/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      343 2023-06-12 11:58:38.000000 ANBUtils-1.5.4/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-12 11:58:38.000000 ANBUtils-1.5.4/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-12 11:58:38.000000 ANBUtils-1.5.4/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-12 11:58:38.000000 ANBUtils-1.5.4/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)      123 2023-06-12 11:58:38.746828 ANBUtils-1.5.4/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4526 2023-06-06 04:58:53.000000 ANBUtils-1.5.4/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-12 11:58:38.747091 ANBUtils-1.5.4/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      405 2023-06-12 11:58:27.000000 ANBUtils-1.5.4/setup.py
```

### Comparing `ANBUtils-1.5.3/ANBUtils/__init__.py` & `ANBUtils-1.5.4/ANBUtils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = 'ANBUtils'
-__version__ = '1.5.3'
+__version__ = '1.5.4'
 __author__ = 'redbson'
 __email__ = 'redbson@gmail.com'
 
 from .environ_cheker import environment_checker as _checker
 _checker()
```

### Comparing `ANBUtils-1.5.3/ANBUtils/a.py` & `ANBUtils-1.5.4/ANBUtils/a.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.3/ANBUtils/db_worker.py` & `ANBUtils-1.5.4/ANBUtils/db_worker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:UTF-8 -*-
 import os
 import sys
 
 import pandas as pd
 import pymongo
 import requests
-
+import math
 
 def in_severs():
     if sys.platform.startswith('linux'):
         return True
     return False
 
 
@@ -72,22 +72,53 @@
 
     def to_df(self, col: object, match: object = None, projection: object = None, sort: object = None, skip: object = 0,
               limit: object = 0) -> object:
         self.__link(col)
         return df_creator(
             list(self.col[col].find(filter=match, projection=projection, sort=sort, skip=skip, limit=limit)))
 
-    def to_df_many(self, cols, match=None, projection=None, sort=None, skip=0, limit=0):
+
+    def to_df_large(self, col: object, match: object = None, projection: object = None, verbose = True) -> object:
+        self.__link(col)
+
+        col_status = self.get_col_statas( col )
+        st_size = col_status['size'] / 1024 / 1024
+        st_count = col_status['count']
+        n = math.ceil( st_size / 200 )
+        step = math.ceil( st_count / n )
+        if n > 1:
+            if verbose:
+                print( '{col} has {count:,d} records, {size:,.2f} MB, split to {n} parts'.format( col=col, count=st_count,
+                                                                                      size=st_size, n=n ) )
+            dfs = []
+            for i in range( n ):
+                if verbose:
+                    print( 'processing {i:>2d} part ...'.format( i=i+1 ))
+                _df = self.to_df( col, match = match, projection= projection, skip=i * step, limit=step )
+                dfs.append( _df )
+            df = pd.concat( dfs )
+            df.drop_duplicates( subset=['_id'], inplace=True )
+            df.reset_index( inplace=True, drop=True )
+            if verbose:
+                print( 'done' )
+
+        else:
+            df = self.to_df( col, match = match, projection= projection )
+
+        return df
+
+    def to_df_many(self, cols, match=None, projection=None):
         dfs = list()
         for c in cols:
-            dfs.append(self.to_df(c, match, projection, sort, skip, limit))
+            dfs.append(self.to_df_large(c, match = match, projection= projection))
         df = pd.concat(dfs)
         df.reset_index(inplace=True, drop=True)
         return df
 
+
     def insert_df(self, df, col):
         self.__link(col)
         data = df.to_dict('records')
         # data = json.loads(df.T.to_json()).values()
         self.col[col].insert_many(data)
 
     def update_df(self, df, col, key):
```

### Comparing `ANBUtils-1.5.3/ANBUtils/easy_pickle.py` & `ANBUtils-1.5.4/ANBUtils/easy_pickle.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.3/ANBUtils/id_work.py` & `ANBUtils-1.5.4/ANBUtils/id_work.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.3/ANBUtils/messager.py` & `ANBUtils-1.5.4/ANBUtils/messager.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.3/ANBUtils/tbox.py` & `ANBUtils-1.5.4/ANBUtils/tbox.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.3/ANBUtils.egg-info/PKG-INFO` & `ANBUtils-1.5.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: ANBUtils
-Version: 1.5.3
-Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
-Home-page: https://github.com/redbson/ANBUilts
-Author: redbson
-Author-email: redbson@gmail.com
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # ANBUilts
 
 ANBUilts is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
 ## Installation
 
 You can install ANBUilts using pip:
@@ -131,8 +121,8 @@
 
 ANBUilts is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUilts).
 
 For support or general questions, you can reach out to the project maintainers or the community through the GitHub repository.
 
 ## License
 
-ANBUilts is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
+ANBUilts is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
```

