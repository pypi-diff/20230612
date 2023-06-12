# Comparing `tmp/cutil-3.0.2.tar.gz` & `tmp/cutil-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutil-3.0.2.tar", last modified: Fri Oct 29 18:49:46 2021, max compression
+gzip compressed data, was "cutil-3.0.3.tar", last modified: Mon Jun 12 18:16:24 2023, max compression
```

## Comparing `cutil-3.0.2.tar` & `cutil-3.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 18:49:46.639317 cutil-3.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2021-04-07 21:06:24.000000 cutil-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17592 2021-10-29 18:49:46.639317 cutil-3.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    16997 2021-04-07 21:06:24.000000 cutil-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 18:49:46.639317 cutil-3.0.2/cutil/
--rw-rw-rw-   0 root         (0) root         (0)    14237 2021-04-07 21:06:24.000000 cutil-3.0.2/cutil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2021-04-07 21:06:24.000000 cutil-3.0.2/cutil/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2423 2021-04-07 21:06:24.000000 cutil-3.0.2/cutil/custom_terminal.py
--rw-rw-rw-   0 root         (0) root         (0)    11287 2021-04-07 21:06:24.000000 cutil-3.0.2/cutil/database.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2021-04-07 21:06:24.000000 cutil-3.0.2/cutil/repeating_timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 18:49:46.639317 cutil-3.0.2/cutil.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17592 2021-10-29 18:49:46.000000 cutil-3.0.2/cutil.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      272 2021-10-29 18:49:46.000000 cutil-3.0.2/cutil.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-29 18:49:46.000000 cutil-3.0.2/cutil.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2021-10-29 18:49:46.000000 cutil-3.0.2/cutil.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2021-10-29 18:49:46.000000 cutil-3.0.2/cutil.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-29 18:49:46.639317 cutil-3.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      905 2021-10-29 18:46:52.000000 cutil-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:16:24.124902 cutil-3.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2021-04-07 21:06:24.000000 cutil-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    17572 2023-06-12 18:16:24.124902 cutil-3.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    16997 2021-04-07 21:06:24.000000 cutil-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:16:24.120902 cutil-3.0.3/cutil/
+-rw-rw-rw-   0 root         (0) root         (0)    14241 2023-06-12 18:15:35.000000 cutil-3.0.3/cutil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      916 2021-04-07 21:06:24.000000 cutil-3.0.3/cutil/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2423 2021-04-07 21:06:24.000000 cutil-3.0.3/cutil/custom_terminal.py
+-rw-rw-rw-   0 root         (0) root         (0)    11287 2021-04-07 21:06:24.000000 cutil-3.0.3/cutil/database.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2021-04-07 21:06:24.000000 cutil-3.0.3/cutil/repeating_timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 18:16:24.124902 cutil-3.0.3/cutil.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17572 2023-06-12 18:16:24.000000 cutil-3.0.3/cutil.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-12 18:16:24.000000 cutil-3.0.3/cutil.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 18:16:24.000000 cutil-3.0.3/cutil.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-12 18:16:24.000000 cutil-3.0.3/cutil.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-12 18:16:24.000000 cutil-3.0.3/cutil.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 18:16:24.124902 cutil-3.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-12 18:15:35.000000 cutil-3.0.3/setup.py
```

### Comparing `cutil-3.0.2/LICENSE` & `cutil-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cutil-3.0.2/PKG-INFO` & `cutil-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cutil
-Version: 3.0.2
+Version: 3.0.3
 Summary: A collection of useful functions
 Home-page: https://github.com/xtream1101/cutil
 Author: Eddy Hintze
 Author-email: eddy@hintze.co
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
@@ -517,9 +516,7 @@
 
 Params:
 
 - **table** - _Type: String_ - _Positional argument_ - Table that data should be inserted into. Include schema.
 - **data_list** - _Type: List/Dict_ - _Positional argument_ - List or Dict of data to insert. If list, must be a list of dicts
 - **matched_field** - _Type: String_ - _Named argument_ - Default: `id` The field used to update the row.
 - **return_cols** - _Type: String/List_ - _Named argument_ - Default: `id` - List of fields (can be a string of a single field) to be returned of rows affected.
-
-
```

### Comparing `cutil-3.0.2/README.md` & `cutil-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cutil-3.0.2/cutil/__init__.py` & `cutil-3.0.3/cutil/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
 
 def update_dict(d, u):
     """
     Source: https://stackoverflow.com/questions/3232943/update-value-of-a-nested-dictionary-of-varying-depth
     """
     for k, v in u.items():
-        if isinstance(v, collections.Mapping):
+        if isinstance(v, collections.abc.Mapping):
             r = update_dict(d.get(k, {}), v)
             d[k] = r
         else:
             d[k] = u[k]
     return d
```

### Comparing `cutil-3.0.2/cutil/config.py` & `cutil-3.0.3/cutil/config.py`

 * *Files identical despite different names*

### Comparing `cutil-3.0.2/cutil/custom_terminal.py` & `cutil-3.0.3/cutil/custom_terminal.py`

 * *Files identical despite different names*

### Comparing `cutil-3.0.2/cutil/database.py` & `cutil-3.0.3/cutil/database.py`

 * *Files identical despite different names*

### Comparing `cutil-3.0.2/cutil/repeating_timer.py` & `cutil-3.0.3/cutil/repeating_timer.py`

 * *Files identical despite different names*

### Comparing `cutil-3.0.2/cutil.egg-info/PKG-INFO` & `cutil-3.0.3/cutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cutil
-Version: 3.0.2
+Version: 3.0.3
 Summary: A collection of useful functions
 Home-page: https://github.com/xtream1101/cutil
 Author: Eddy Hintze
 Author-email: eddy@hintze.co
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
@@ -517,9 +516,7 @@
 
 Params:
 
 - **table** - _Type: String_ - _Positional argument_ - Table that data should be inserted into. Include schema.
 - **data_list** - _Type: List/Dict_ - _Positional argument_ - List or Dict of data to insert. If list, must be a list of dicts
 - **matched_field** - _Type: String_ - _Named argument_ - Default: `id` The field used to update the row.
 - **return_cols** - _Type: String/List_ - _Named argument_ - Default: `id` - List of fields (can be a string of a single field) to be returned of rows affected.
-
-
```

### Comparing `cutil-3.0.2/setup.py` & `cutil-3.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 postgres = [
     'psycopg2-binary',
 ]
 
 setup(
     name='cutil',
     packages=['cutil'],
-    version='3.0.2',
+    version='3.0.3',
     description='A collection of useful functions',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Eddy Hintze',
     author_email="eddy@hintze.co",
     url="https://github.com/xtream1101/cutil",
     license='MIT',
```

