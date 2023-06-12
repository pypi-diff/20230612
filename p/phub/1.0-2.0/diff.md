# Comparing `tmp/phub-1.0.tar.gz` & `tmp/phub-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-1.0.tar", last modified: Mon Jun 12 16:41:13 2023, max compression
+gzip compressed data, was "phub-2.0.tar", last modified: Mon Jun 12 16:51:18 2023, max compression
```

## Comparing `phub-1.0.tar` & `phub-2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:13.381150 phub-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 16:41:01.000000 phub-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-12 16:41:13.381150 phub-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-12 16:41:01.000000 phub-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 16:41:01.000000 phub-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-12 16:41:13.381150 phub-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 16:41:01.000000 phub-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:13.373149 phub-1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:13.381150 phub-1.0/src/phub/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-12 16:41:01.000000 phub-1.0/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-12 16:41:02.000000 phub-1.0/src/phub/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-12 16:41:02.000000 phub-1.0/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-12 16:41:02.000000 phub-1.0/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 16:41:02.000000 phub-1.0/src/phub/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-12 16:41:02.000000 phub-1.0/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:13.381150 phub-1.0/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-12 16:41:13.000000 phub-1.0/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-12 16:41:13.000000 phub-1.0/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:41:13.000000 phub-1.0/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 16:41:13.000000 phub-1.0/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 16:41:13.000000 phub-1.0/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:18.135808 phub-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 16:51:04.000000 phub-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 16:51:18.135808 phub-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-12 16:51:04.000000 phub-2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 16:51:04.000000 phub-2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 16:51:18.139808 phub-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 16:51:04.000000 phub-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:18.131808 phub-2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:18.135808 phub-2.0/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-12 16:51:04.000000 phub-2.0/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-12 16:51:04.000000 phub-2.0/src/phub/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-12 16:51:04.000000 phub-2.0/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-12 16:51:04.000000 phub-2.0/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 16:51:04.000000 phub-2.0/src/phub/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-12 16:51:04.000000 phub-2.0/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:18.135808 phub-2.0/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/top_level.txt
```

### Comparing `phub-1.0/LICENSE` & `phub-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-1.0/PKG-INFO` & `phub-2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 1.0
+Version: 2.0
 Summary: An API for PornHub
-Home-page: https://github.com/Egsagon/neko-sama-api/
+Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
 Platform: win32
 Platform: cygwin
```

### Comparing `phub-1.0/README.md` & `phub-2.0/README.md`

 * *Files identical despite different names*

### Comparing `phub-1.0/setup.cfg` & `phub-2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = phub
-version = 1.0
+version = 2.0
 description = An API for PornHub
 author = Egsagon
 author_email = egsagon12@gmail.com
-url = https://github.com/Egsagon/neko-sama-api/
+url = https://github.com/Egsagon/PHUB/
 license = GPLv3
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 platforms = unix, linux, win32, cygwin
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `phub-1.0/src/phub/__init__.py` & `phub-2.0/src/phub/__init__.py`

 * *Files identical despite different names*

### Comparing `phub-1.0/src/phub/classes.py` & `phub-2.0/src/phub/classes.py`

 * *Files identical despite different names*

### Comparing `phub-1.0/src/phub/consts.py` & `phub-2.0/src/phub/consts.py`

 * *Files identical despite different names*

### Comparing `phub-1.0/src/phub/core.py` & `phub-2.0/src/phub/core.py`

 * *Files identical despite different names*

### Comparing `phub-1.0/src/phub/parser.py` & `phub-2.0/src/phub/parser.py`

 * *Files identical despite different names*

### Comparing `phub-1.0/src/phub/utils.py` & `phub-2.0/src/phub/utils.py`

 * *Files identical despite different names*

### Comparing `phub-1.0/src/phub.egg-info/PKG-INFO` & `phub-2.0/src/phub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 1.0
+Version: 2.0
 Summary: An API for PornHub
-Home-page: https://github.com/Egsagon/neko-sama-api/
+Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
 Platform: win32
 Platform: cygwin
```

