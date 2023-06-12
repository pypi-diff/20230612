# Comparing `tmp/paintera-0.34.0.tar.gz` & `tmp/paintera-0.34.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paintera-0.34.0.tar", last modified: Mon Jun  5 21:25:07 2023, max compression
+gzip compressed data, was "paintera-0.34.1.tar", last modified: Mon Jun 12 20:38:48 2023, max compression
```

## Comparing `paintera-0.34.0.tar` & `paintera-0.34.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-05 21:25:07.765394 paintera-0.34.0/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)    18092 2021-02-01 16:33:27.000000 paintera-0.34.0/LICENSE
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      329 2023-06-05 21:25:07.765394 paintera-0.34.0/PKG-INFO
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       75 2021-02-01 16:33:27.000000 paintera-0.34.0/README
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-05 21:25:07.765394 paintera-0.34.0/paintera/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     5847 2022-06-16 21:07:44.000000 paintera-0.34.0/paintera/__init__.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     4074 2022-10-03 13:15:20.000000 paintera-0.34.0/paintera/javafx_modules.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)     1012 2023-06-05 21:25:04.000000 paintera-0.34.0/paintera/version.py
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-05 21:25:07.765394 paintera-0.34.0/paintera.egg-info/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      329 2023-06-05 21:25:07.000000 paintera-0.34.0/paintera.egg-info/PKG-INFO
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      285 2023-06-05 21:25:07.000000 paintera-0.34.0/paintera.egg-info/SOURCES.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)        1 2023-06-05 21:25:07.000000 paintera-0.34.0/paintera.egg-info/dependency_links.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      134 2023-06-05 21:25:07.000000 paintera-0.34.0/paintera.egg-info/entry_points.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       45 2023-06-05 21:25:07.000000 paintera-0.34.0/paintera.egg-info/requires.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)        9 2023-06-05 21:25:07.000000 paintera-0.34.0/paintera.egg-info/top_level.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       38 2023-06-05 21:25:07.765394 paintera-0.34.0/setup.cfg
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      971 2021-06-18 02:42:10.000000 paintera-0.34.0/setup.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-12 20:38:48.913354 paintera-0.34.1/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    18092 2021-02-01 16:33:27.000000 paintera-0.34.1/LICENSE
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      329 2023-06-12 20:38:48.913354 paintera-0.34.1/PKG-INFO
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       75 2021-02-01 16:33:27.000000 paintera-0.34.1/README
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-12 20:38:48.909354 paintera-0.34.1/paintera/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     5847 2022-06-16 21:07:44.000000 paintera-0.34.1/paintera/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     4074 2022-10-03 13:15:20.000000 paintera-0.34.1/paintera/javafx_modules.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1012 2023-06-12 20:37:29.000000 paintera-0.34.1/paintera/version.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-12 20:38:48.913354 paintera-0.34.1/paintera.egg-info/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      329 2023-06-12 20:38:48.000000 paintera-0.34.1/paintera.egg-info/PKG-INFO
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      285 2023-06-12 20:38:48.000000 paintera-0.34.1/paintera.egg-info/SOURCES.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        1 2023-06-12 20:38:48.000000 paintera-0.34.1/paintera.egg-info/dependency_links.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      134 2023-06-12 20:38:48.000000 paintera-0.34.1/paintera.egg-info/entry_points.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       45 2023-06-12 20:38:48.000000 paintera-0.34.1/paintera.egg-info/requires.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        9 2023-06-12 20:38:48.000000 paintera-0.34.1/paintera.egg-info/top_level.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       38 2023-06-12 20:38:48.913354 paintera-0.34.1/setup.cfg
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      971 2021-06-18 02:42:10.000000 paintera-0.34.1/setup.py
```

### Comparing `paintera-0.34.0/LICENSE` & `paintera-0.34.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paintera-0.34.0/paintera/__init__.py` & `paintera-0.34.1/paintera/__init__.py`

 * *Files identical despite different names*

### Comparing `paintera-0.34.0/paintera/javafx_modules.py` & `paintera-0.34.1/paintera/javafx_modules.py`

 * *Files identical despite different names*

### Comparing `paintera-0.34.0/paintera/version.py` & `paintera-0.34.1/paintera/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 
     def is_release(self):
         return self.tag() == ''
 
     def __str__(self):
         return self.python_version()
 
-_paintera_version = _Version(0, 34, 0, '')
+_paintera_version = _Version(0, 34, 1, '')
```

### Comparing `paintera-0.34.0/setup.py` & `paintera-0.34.1/setup.py`

 * *Files identical despite different names*

