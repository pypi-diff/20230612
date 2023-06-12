# Comparing `tmp/common_utils_pkg-0.0.3.tar.gz` & `tmp/common_utils_pkg-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common_utils_pkg-0.0.3.tar", last modified: Sun May 28 08:02:26 2023, max compression
+gzip compressed data, was "common_utils_pkg-0.1.0.tar", last modified: Mon Jun 12 09:04:16 2023, max compression
```

## Comparing `common_utils_pkg-0.0.3.tar` & `common_utils_pkg-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-05-28 08:02:26.188034 common_utils_pkg-0.0.3/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-05-28 08:02:26.187731 common_utils_pkg-0.0.3/PKG-INFO
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-05-28 08:02:26.184491 common_utils_pkg-0.0.3/common_utils_pkg/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      111 2023-05-28 07:52:20.000000 common_utils_pkg-0.0.3/common_utils_pkg/__init__.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     2628 2023-05-28 07:54:54.000000 common_utils_pkg-0.0.3/common_utils_pkg/logger.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1026 2023-05-28 07:07:47.000000 common_utils_pkg-0.0.3/common_utils_pkg/notifications.py
--rw-r--r--   0 nikitagetman   (501) staff       (20)     1021 2023-05-28 07:55:01.000000 common_utils_pkg-0.0.3/common_utils_pkg/scheduler.py
-drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-05-28 08:02:26.187102 common_utils_pkg-0.0.3/common_utils_pkg.egg-info/
--rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-05-28 08:02:26.000000 common_utils_pkg-0.0.3/common_utils_pkg.egg-info/PKG-INFO
--rw-r--r--   0 nikitagetman   (501) staff       (20)      327 2023-05-28 08:02:26.000000 common_utils_pkg-0.0.3/common_utils_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)        1 2023-05-28 08:02:26.000000 common_utils_pkg-0.0.3/common_utils_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-05-28 08:02:26.000000 common_utils_pkg-0.0.3/common_utils_pkg.egg-info/requires.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-05-28 08:02:26.000000 common_utils_pkg-0.0.3/common_utils_pkg.egg-info/top_level.txt
--rw-r--r--   0 nikitagetman   (501) staff       (20)       38 2023-05-28 08:02:26.188210 common_utils_pkg-0.0.3/setup.cfg
--rw-r--r--   0 nikitagetman   (501) staff       (20)      793 2023-05-28 08:01:17.000000 common_utils_pkg-0.0.3/setup.py
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-12 09:04:16.839375 common_utils_pkg-0.1.0/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-06-12 09:04:16.839048 common_utils_pkg-0.1.0/PKG-INFO
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-12 09:04:16.836143 common_utils_pkg-0.1.0/common_utils_pkg/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      111 2023-05-28 07:52:20.000000 common_utils_pkg-0.1.0/common_utils_pkg/__init__.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      787 2023-06-12 09:00:48.000000 common_utils_pkg-0.1.0/common_utils_pkg/aws_adapter.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     2628 2023-05-28 07:54:54.000000 common_utils_pkg-0.1.0/common_utils_pkg/logger.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1026 2023-05-28 07:07:47.000000 common_utils_pkg-0.1.0/common_utils_pkg/notifications.py
+-rw-r--r--   0 nikitagetman   (501) staff       (20)     1021 2023-05-28 07:55:01.000000 common_utils_pkg-0.1.0/common_utils_pkg/scheduler.py
+drwxr-xr-x   0 nikitagetman   (501) staff       (20)        0 2023-06-12 09:04:16.838524 common_utils_pkg-0.1.0/common_utils_pkg.egg-info/
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      520 2023-06-12 09:04:16.000000 common_utils_pkg-0.1.0/common_utils_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      359 2023-06-12 09:04:16.000000 common_utils_pkg-0.1.0/common_utils_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)        1 2023-06-12 09:04:16.000000 common_utils_pkg-0.1.0/common_utils_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-06-12 09:04:16.000000 common_utils_pkg-0.1.0/common_utils_pkg.egg-info/requires.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       17 2023-06-12 09:04:16.000000 common_utils_pkg-0.1.0/common_utils_pkg.egg-info/top_level.txt
+-rw-r--r--   0 nikitagetman   (501) staff       (20)       38 2023-06-12 09:04:16.839507 common_utils_pkg-0.1.0/setup.cfg
+-rw-r--r--   0 nikitagetman   (501) staff       (20)      793 2023-06-12 09:04:04.000000 common_utils_pkg-0.1.0/setup.py
```

### Comparing `common_utils_pkg-0.0.3/PKG-INFO` & `common_utils_pkg-0.1.0/common_utils_pkg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: common_utils_pkg
-Version: 0.0.3
+Name: common-utils-pkg
+Version: 0.1.0
 Summary: Common utils package. With some basic classes.
 Author: John Johny
 Author-email: love.dev.2020@email.com
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `common_utils_pkg-0.0.3/common_utils_pkg/logger.py` & `common_utils_pkg-0.1.0/common_utils_pkg/logger.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.0.3/common_utils_pkg/notifications.py` & `common_utils_pkg-0.1.0/common_utils_pkg/notifications.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.0.3/common_utils_pkg/scheduler.py` & `common_utils_pkg-0.1.0/common_utils_pkg/scheduler.py`

 * *Files identical despite different names*

### Comparing `common_utils_pkg-0.0.3/common_utils_pkg.egg-info/PKG-INFO` & `common_utils_pkg-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: common-utils-pkg
-Version: 0.0.3
+Name: common_utils_pkg
+Version: 0.1.0
 Summary: Common utils package. With some basic classes.
 Author: John Johny
 Author-email: love.dev.2020@email.com
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `common_utils_pkg-0.0.3/setup.py` & `common_utils_pkg-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.1.0"
 DESCRIPTION = "Common utils package. With some basic classes."
 LONG_DESCRIPTION = "Package with common utils for new projects."
 
 setup(
     name="common_utils_pkg",
     version=VERSION,
     author="John Johny",
```
