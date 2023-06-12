# Comparing `tmp/testinfra-bdd-2.2.5.tar.gz` & `tmp/testinfra-bdd-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testinfra-bdd-2.2.5.tar", last modified: Sun Feb 26 09:56:58 2023, max compression
+gzip compressed data, was "testinfra-bdd-2.2.6.tar", last modified: Mon Jun 12 14:31:10 2023, max compression
```

## Comparing `testinfra-bdd-2.2.5.tar` & `testinfra-bdd-2.2.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 09:56:58.568571 testinfra-bdd-2.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-02-26 09:56:58.568571 testinfra-bdd-2.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-26 09:56:58.568571 testinfra-bdd-2.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 09:56:58.568571 testinfra-bdd-2.2.5/testinfra_bdd/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/exception_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/given.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/testinfra_bdd/when.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 09:56:58.568571 testinfra-bdd-2.2.5/testinfra_bdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-02-26 09:56:58.000000 testinfra-bdd-2.2.5/testinfra_bdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-26 09:56:58.000000 testinfra-bdd-2.2.5/testinfra_bdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 09:56:58.000000 testinfra-bdd-2.2.5/testinfra_bdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-26 09:56:58.000000 testinfra-bdd-2.2.5/testinfra_bdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-26 09:56:58.000000 testinfra-bdd-2.2.5/testinfra_bdd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 09:56:58.568571 testinfra-bdd-2.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-02-26 09:56:32.000000 testinfra-bdd-2.2.5/tests/test_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:31:10.187882 testinfra-bdd-2.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-12 14:31:10.187882 testinfra-bdd-2.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 14:31:10.187882 testinfra-bdd-2.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:31:10.183882 testinfra-bdd-2.2.6/testinfra_bdd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/exception_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/given.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/testinfra_bdd/when.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:31:10.183882 testinfra-bdd-2.2.6/testinfra_bdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-12 14:31:10.000000 testinfra-bdd-2.2.6/testinfra_bdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-12 14:31:10.000000 testinfra-bdd-2.2.6/testinfra_bdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:31:10.000000 testinfra-bdd-2.2.6/testinfra_bdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 14:31:10.000000 testinfra-bdd-2.2.6/testinfra_bdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 14:31:10.000000 testinfra-bdd-2.2.6/testinfra_bdd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:31:10.187882 testinfra-bdd-2.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 14:30:42.000000 testinfra-bdd-2.2.6/tests/test_exceptions.py
```

### Comparing `testinfra-bdd-2.2.5/LICENSE` & `testinfra-bdd-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/PKG-INFO` & `testinfra-bdd-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testinfra-bdd
-Version: 2.2.5
+Version: 2.2.6
 Summary: An interface between pytest-bdd and pytest-testinfra.
 Home-page: https://github.com/cbdq-io/testinfra-bdd
 Author: Cloud Based DQ Ltd.
 Author-email: info@cbdq.io
 Project-URL: Bug Tracker, https://github.com/cbdq-io/testinfra-bdd/issues
 Keywords: testinfra,bdd
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testinfra-bdd-2.2.5/README.md` & `testinfra-bdd-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/setup.py` & `testinfra-bdd-2.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/__init__.py` & `testinfra-bdd-2.2.6/testinfra_bdd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ]
 
 """The version of the module.
 
 This is used by setuptools and by gitchangelog to identify the name of the name
 of the release.
 """
-__version__ = '2.2.5'
+__version__ = '2.2.6'
 
 
 def get_host_fixture(hostspec, timeout=0):
     """
     Return a host that is confirmed as ready.
 
     hostspec : str
```

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/address.py` & `testinfra-bdd-2.2.6/testinfra_bdd/address.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/command.py` & `testinfra-bdd-2.2.6/testinfra_bdd/command.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/exception_message.py` & `testinfra-bdd-2.2.6/testinfra_bdd/exception_message.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/file.py` & `testinfra-bdd-2.2.6/testinfra_bdd/file.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/fixture.py` & `testinfra-bdd-2.2.6/testinfra_bdd/fixture.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/given.py` & `testinfra-bdd-2.2.6/testinfra_bdd/given.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/group.py` & `testinfra-bdd-2.2.6/testinfra_bdd/group.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/package.py` & `testinfra-bdd-2.2.6/testinfra_bdd/package.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/parsers.py` & `testinfra-bdd-2.2.6/testinfra_bdd/parsers.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/pip.py` & `testinfra-bdd-2.2.6/testinfra_bdd/pip.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/process.py` & `testinfra-bdd-2.2.6/testinfra_bdd/process.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/service.py` & `testinfra-bdd-2.2.6/testinfra_bdd/service.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/socket.py` & `testinfra-bdd-2.2.6/testinfra_bdd/socket.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/user.py` & `testinfra-bdd-2.2.6/testinfra_bdd/user.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd/when.py` & `testinfra-bdd-2.2.6/testinfra_bdd/when.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd.egg-info/PKG-INFO` & `testinfra-bdd-2.2.6/testinfra_bdd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testinfra-bdd
-Version: 2.2.5
+Version: 2.2.6
 Summary: An interface between pytest-bdd and pytest-testinfra.
 Home-page: https://github.com/cbdq-io/testinfra-bdd
 Author: Cloud Based DQ Ltd.
 Author-email: info@cbdq.io
 Project-URL: Bug Tracker, https://github.com/cbdq-io/testinfra-bdd/issues
 Keywords: testinfra,bdd
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testinfra-bdd-2.2.5/testinfra_bdd.egg-info/SOURCES.txt` & `testinfra-bdd-2.2.6/testinfra_bdd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-2.2.5/tests/test_exceptions.py` & `testinfra-bdd-2.2.6/tests/test_exceptions.py`

 * *Files identical despite different names*

