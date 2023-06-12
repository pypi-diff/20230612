# Comparing `tmp/gitcoll-0.0.16.tar.gz` & `tmp/gitcoll-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitcoll-0.0.16.tar", last modified: Sun Jun 11 12:39:40 2023, max compression
+gzip compressed data, was "gitcoll-0.0.17.tar", last modified: Mon Jun 12 09:40:16 2023, max compression
```

## Comparing `gitcoll-0.0.16.tar` & `gitcoll-0.0.17.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.405138 gitcoll-0.0.16/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 12:39:37.000000 gitcoll-0.0.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12145 2023-06-11 12:39:40.405138 gitcoll-0.0.16/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11731 2023-06-11 11:48:27.000000 gitcoll-0.0.16/README.md
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-11 11:48:27.000000 gitcoll-0.0.16/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-06-11 12:39:40.405138 gitcoll-0.0.16/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-06-11 11:48:27.000000 gitcoll-0.0.16/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.401138 gitcoll-0.0.16/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.405138 gitcoll-0.0.16/src/gcln/
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6751 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/cfg_file.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7232 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    43203 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/main.py
--rw-rw-rw-   0 root         (0) root         (0)    29661 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/main_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/records.py
--rw-rw-rw-   0 root         (0) root         (0)    12693 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln/srv_connector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.405138 gitcoll-0.0.16/src/gcln2/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-11 12:39:37.000000 gitcoll-0.0.16/src/gcln2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5317 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/db.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8917 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    37630 2023-06-11 12:39:37.000000 gitcoll-0.0.16/src/gcln2/main.py
--rw-rw-rw-   0 root         (0) root         (0)     2238 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-11 11:48:27.000000 gitcoll-0.0.16/src/gcln2/yaml_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 12:39:40.405138 gitcoll-0.0.16/src/gitcoll.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12145 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-11 12:39:40.000000 gitcoll-0.0.16/src/gitcoll.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:40:16.329189 gitcoll-0.0.17/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 09:40:13.000000 gitcoll-0.0.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12145 2023-06-12 09:40:16.329189 gitcoll-0.0.17/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2023-06-11 11:48:27.000000 gitcoll-0.0.17/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-06-11 11:48:27.000000 gitcoll-0.0.17/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-12 09:40:16.329189 gitcoll-0.0.17/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-06-11 11:48:27.000000 gitcoll-0.0.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:40:16.321189 gitcoll-0.0.17/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:40:16.329189 gitcoll-0.0.17/src/gcln/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6751 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln/cfg_file.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7232 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    43203 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    29661 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln/main_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln/records.py
+-rw-rw-rw-   0 root         (0) root         (0)    12693 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln/srv_connector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:40:16.329189 gitcoll-0.0.17/src/gcln2/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-12 09:40:13.000000 gitcoll-0.0.17/src/gcln2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5317 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln2/db.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln2/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8917 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln2/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    37630 2023-06-11 12:39:37.000000 gitcoll-0.0.17/src/gcln2/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2238 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln2/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-11 11:48:27.000000 gitcoll-0.0.17/src/gcln2/yaml_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:40:16.329189 gitcoll-0.0.17/src/gitcoll.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12145 2023-06-12 09:40:16.000000 gitcoll-0.0.17/src/gitcoll.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-12 09:40:16.000000 gitcoll-0.0.17/src/gitcoll.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 09:40:16.000000 gitcoll-0.0.17/src/gitcoll.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-12 09:40:16.000000 gitcoll-0.0.17/src/gitcoll.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2023-06-12 09:40:16.000000 gitcoll-0.0.17/src/gitcoll.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 09:40:16.000000 gitcoll-0.0.17/src/gitcoll.egg-info/top_level.txt
```

### Comparing `gitcoll-0.0.16/PKG-INFO` & `gitcoll-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitcoll
-Version: 0.0.16
+Version: 0.0.17
 Summary: Git collection utilities
 Home-page: https://gitlab.com/jesrib/gitcoll
 Author: Jesper Ribbe
 Author-email: jesper@ribbe.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gitcoll-0.0.16/README.md` & `gitcoll-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/setup.cfg` & `gitcoll-0.0.17/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 install_requires = 
 	pyyaml
 	python-gitlab >= 3.14
 	pygit2 >= 1.12
 	filelock
 	python-dateutil
 	pydantic
+	pywin32;platform_system=='Windows'
 
 [options.entry_points]
 console_scripts = 
 	gcln = gcln.main:main
 	gcln2 = gcln2.main:main_no_args
 
 [egg_info]
```

### Comparing `gitcoll-0.0.16/src/gcln/cfg_file.py` & `gitcoll-0.0.17/src/gcln/cfg_file.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gcln/helpers.py` & `gitcoll-0.0.17/src/gcln/helpers.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gcln/main.py` & `gitcoll-0.0.17/src/gcln/main.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gcln/main_context.py` & `gitcoll-0.0.17/src/gcln/main_context.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gcln/records.py` & `gitcoll-0.0.17/src/gcln/records.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gcln/srv_connector.py` & `gitcoll-0.0.17/src/gcln/srv_connector.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gcln2/db.py` & `gitcoll-0.0.17/src/gcln2/db.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gcln2/helpers.py` & `gitcoll-0.0.17/src/gcln2/helpers.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gcln2/main.py` & `gitcoll-0.0.17/src/gcln2/main.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gcln2/schema.py` & `gitcoll-0.0.17/src/gcln2/schema.py`

 * *Files identical despite different names*

### Comparing `gitcoll-0.0.16/src/gitcoll.egg-info/PKG-INFO` & `gitcoll-0.0.17/src/gitcoll.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitcoll
-Version: 0.0.16
+Version: 0.0.17
 Summary: Git collection utilities
 Home-page: https://gitlab.com/jesrib/gitcoll
 Author: Jesper Ribbe
 Author-email: jesper@ribbe.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gitcoll-0.0.16/src/gitcoll.egg-info/SOURCES.txt` & `gitcoll-0.0.17/src/gitcoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

