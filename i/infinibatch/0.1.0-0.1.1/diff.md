# Comparing `tmp/infinibatch-0.1.0.tar.gz` & `tmp/infinibatch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infinibatch-0.1.0.tar", last modified: Thu Jun  8 21:01:47 2023, max compression
+gzip compressed data, was "infinibatch-0.1.1.tar", last modified: Mon Jun 12 16:57:31 2023, max compression
```

## Comparing `infinibatch-0.1.0.tar` & `infinibatch-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)        0 2023-06-08 21:01:47.659155 infinibatch-0.1.0/
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)     1141 2023-06-08 20:53:31.000000 infinibatch-0.1.0/LICENSE
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)      328 2023-06-08 21:01:47.659155 infinibatch-0.1.0/PKG-INFO
--rwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)    16011 2023-06-08 20:53:31.000000 infinibatch-0.1.0/README.md
-drwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)        0 2023-06-08 21:01:47.655156 infinibatch-0.1.0/infinibatch/
--rwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)    13987 2023-06-08 20:53:31.000000 infinibatch-0.1.0/infinibatch/__init__.py
--rwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)     3976 2023-06-08 20:53:31.000000 infinibatch-0.1.0/infinibatch/datasets.py
--rwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)    73702 2023-06-08 20:53:31.000000 infinibatch-0.1.0/infinibatch/iterators.py
-drwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)        0 2023-06-08 21:01:47.655156 infinibatch-0.1.0/infinibatch.egg-info/
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)      328 2023-06-08 21:01:47.000000 infinibatch-0.1.0/infinibatch.egg-info/PKG-INFO
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)      321 2023-06-08 21:01:47.000000 infinibatch-0.1.0/infinibatch.egg-info/SOURCES.txt
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)        1 2023-06-08 21:01:47.000000 infinibatch-0.1.0/infinibatch.egg-info/dependency_links.txt
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)       12 2023-06-08 21:01:47.000000 infinibatch-0.1.0/infinibatch.egg-info/top_level.txt
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)       30 2023-06-08 20:53:31.000000 infinibatch-0.1.0/pyproject.toml
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)       38 2023-06-08 21:01:47.659155 infinibatch-0.1.0/setup.cfg
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)      401 2023-06-08 20:53:31.000000 infinibatch-0.1.0/setup.py
-drwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)        0 2023-06-08 21:01:47.659155 infinibatch-0.1.0/test/
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)     4958 2023-06-08 20:53:31.000000 infinibatch-0.1.0/test/test_datasets.py
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)      372 2023-06-08 20:53:31.000000 infinibatch-0.1.0/test/test_doctests.py
--rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)    42594 2023-06-08 20:57:16.000000 infinibatch-0.1.0/test/test_iterators.py
+drwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)        0 2023-06-12 16:57:31.453442 infinibatch-0.1.1/
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)     1141 2023-06-08 20:53:31.000000 infinibatch-0.1.1/LICENSE
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)    16549 2023-06-12 16:57:31.449442 infinibatch-0.1.1/PKG-INFO
+-rwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)    16011 2023-06-08 20:53:31.000000 infinibatch-0.1.1/README.md
+drwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)        0 2023-06-12 16:57:31.449442 infinibatch-0.1.1/infinibatch/
+-rwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)    13987 2023-06-09 18:50:21.000000 infinibatch-0.1.1/infinibatch/__init__.py
+-rwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)     3976 2023-06-08 20:53:31.000000 infinibatch-0.1.1/infinibatch/datasets.py
+-rwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)    73702 2023-06-08 20:53:31.000000 infinibatch-0.1.1/infinibatch/iterators.py
+drwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)        0 2023-06-12 16:57:31.449442 infinibatch-0.1.1/infinibatch.egg-info/
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)    16549 2023-06-12 16:57:31.000000 infinibatch-0.1.1/infinibatch.egg-info/PKG-INFO
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)      321 2023-06-12 16:57:31.000000 infinibatch-0.1.1/infinibatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)        1 2023-06-12 16:57:31.000000 infinibatch-0.1.1/infinibatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)       12 2023-06-12 16:57:31.000000 infinibatch-0.1.1/infinibatch.egg-info/top_level.txt
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)       30 2023-06-08 20:53:31.000000 infinibatch-0.1.1/pyproject.toml
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)       38 2023-06-12 16:57:31.453442 infinibatch-0.1.1/setup.cfg
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)     1156 2023-06-12 16:55:23.000000 infinibatch-0.1.1/setup.py
+drwxrwxr-x   0 thammegowda  (1024) thammegowda  (1024)        0 2023-06-12 16:57:31.449442 infinibatch-0.1.1/test/
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)     4958 2023-06-08 20:53:31.000000 infinibatch-0.1.1/test/test_datasets.py
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)      372 2023-06-08 20:53:31.000000 infinibatch-0.1.1/test/test_doctests.py
+-rw-rw-r--   0 thammegowda  (1024) thammegowda  (1024)    42595 2023-06-09 18:55:40.000000 infinibatch-0.1.1/test/test_iterators.py
```

### Comparing `infinibatch-0.1.0/LICENSE` & `infinibatch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `infinibatch-0.1.0/README.md` & `infinibatch-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `infinibatch-0.1.0/infinibatch/__init__.py` & `infinibatch-0.1.1/infinibatch/__init__.py`

 * *Files identical despite different names*

### Comparing `infinibatch-0.1.0/infinibatch/datasets.py` & `infinibatch-0.1.1/infinibatch/datasets.py`

 * *Files identical despite different names*

### Comparing `infinibatch-0.1.0/infinibatch/iterators.py` & `infinibatch-0.1.1/infinibatch/iterators.py`

 * *Files identical despite different names*

### Comparing `infinibatch-0.1.0/test/test_datasets.py` & `infinibatch-0.1.1/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `infinibatch-0.1.0/test/test_iterators.py` & `infinibatch-0.1.1/test/test_iterators.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 class TestFiniteIteratorMixin:
     """
     Mixin to be used in combination with TestBase
     to test basic function of finite CheckpointableIterators
     """
 
     def test_basic(self):
+
         for case_name, expected_result, it in self.test_cases:
             with self.subTest(case_name):
                 result = list(it)
                 self.assertEqual(result, expected_result)
 
 
 class TestFiniteIteratorCheckpointingMixin:
```

