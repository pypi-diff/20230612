# Comparing `tmp/liveramp_automation_framework-0.0.2.tar.gz` & `tmp/liveramp_automation_framework-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation_framework-0.0.2.tar", last modified: Mon Jun 12 01:57:44 2023, max compression
+gzip compressed data, was "liveramp_automation_framework-0.0.3.tar", last modified: Mon Jun 12 02:27:10 2023, max compression
```

## Comparing `liveramp_automation_framework-0.0.2.tar` & `liveramp_automation_framework-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 01:57:44.262161 liveramp_automation_framework-0.0.2/
--rw-r--r--   0 jasqia     (502) staff       (20)      173 2023-06-12 01:57:44.261477 liveramp_automation_framework-0.0.2/PKG-INFO
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 01:57:44.254862 liveramp_automation_framework-0.0.2/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)      271 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.0.2/liveramp_automation/allure_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.0.2/liveramp_automation/logger.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3081 2023-06-08 08:34:38.000000 liveramp_automation_framework-0.0.2/liveramp_automation/login_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.0.2/liveramp_automation/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      798 2023-06-08 08:30:02.000000 liveramp_automation_framework-0.0.2/liveramp_automation/playwright_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2297 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.0.2/liveramp_automation/read_report.py
--rw-r--r--   0 jasqia     (502) staff       (20)     6946 2023-06-08 08:34:38.000000 liveramp_automation_framework-0.0.2/liveramp_automation/request_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      816 2023-06-08 08:34:38.000000 liveramp_automation_framework-0.0.2/liveramp_automation/selenium_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.0.2/liveramp_automation/time_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2375 2023-06-12 01:53:20.000000 liveramp_automation_framework-0.0.2/liveramp_automation/upload_util.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 01:57:44.260430 liveramp_automation_framework-0.0.2/liveramp_automation_framework.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)      173 2023-06-12 01:57:44.000000 liveramp_automation_framework-0.0.2/liveramp_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-12 01:57:44.000000 liveramp_automation_framework-0.0.2/liveramp_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-12 01:57:44.000000 liveramp_automation_framework-0.0.2/liveramp_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      294 2023-06-12 01:57:44.000000 liveramp_automation_framework-0.0.2/liveramp_automation_framework.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-12 01:57:44.000000 liveramp_automation_framework-0.0.2/liveramp_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-12 01:57:44.262404 liveramp_automation_framework-0.0.2/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)      795 2023-06-12 01:57:40.000000 liveramp_automation_framework-0.0.2/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 02:27:10.868607 liveramp_automation_framework-0.0.3/
+-rw-r--r--   0 jasqia     (502) staff       (20)      173 2023-06-12 02:27:10.868009 liveramp_automation_framework-0.0.3/PKG-INFO
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 02:27:10.862047 liveramp_automation_framework-0.0.3/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)      271 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.0.3/liveramp_automation/allure_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.0.3/liveramp_automation/logger.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3081 2023-06-08 08:34:38.000000 liveramp_automation_framework-0.0.3/liveramp_automation/login_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.0.3/liveramp_automation/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      798 2023-06-08 08:30:02.000000 liveramp_automation_framework-0.0.3/liveramp_automation/playwright_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2297 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.0.3/liveramp_automation/read_report.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     6946 2023-06-08 08:34:38.000000 liveramp_automation_framework-0.0.3/liveramp_automation/request_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      816 2023-06-08 08:34:38.000000 liveramp_automation_framework-0.0.3/liveramp_automation/selenium_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.0.3/liveramp_automation/time_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2375 2023-06-12 01:53:20.000000 liveramp_automation_framework-0.0.3/liveramp_automation/upload_util.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 02:27:10.867055 liveramp_automation_framework-0.0.3/liveramp_automation_framework.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)      173 2023-06-12 02:27:10.000000 liveramp_automation_framework-0.0.3/liveramp_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-12 02:27:10.000000 liveramp_automation_framework-0.0.3/liveramp_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-12 02:27:10.000000 liveramp_automation_framework-0.0.3/liveramp_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      294 2023-06-12 02:27:10.000000 liveramp_automation_framework-0.0.3/liveramp_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-12 02:27:10.000000 liveramp_automation_framework-0.0.3/liveramp_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-12 02:27:10.868762 liveramp_automation_framework-0.0.3/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)      795 2023-06-12 02:27:07.000000 liveramp_automation_framework-0.0.3/setup.py
```

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation/logger.py` & `liveramp_automation_framework-0.0.3/liveramp_automation/logger.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation/login_util.py` & `liveramp_automation_framework-0.0.3/liveramp_automation/login_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation/parsers.py` & `liveramp_automation_framework-0.0.3/liveramp_automation/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation/playwright_util.py` & `liveramp_automation_framework-0.0.3/liveramp_automation/playwright_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation/read_report.py` & `liveramp_automation_framework-0.0.3/liveramp_automation/read_report.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation/request_util.py` & `liveramp_automation_framework-0.0.3/liveramp_automation/request_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation/selenium_util.py` & `liveramp_automation_framework-0.0.3/liveramp_automation/selenium_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation/time_util.py` & `liveramp_automation_framework-0.0.3/liveramp_automation/time_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation/upload_util.py` & `liveramp_automation_framework-0.0.3/liveramp_automation/upload_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/liveramp_automation_framework.egg-info/SOURCES.txt` & `liveramp_automation_framework-0.0.3/liveramp_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.2/setup.py` & `liveramp_automation_framework-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='liveramp_automation_framework',
-    version='0.0.2',
+    version='0.0.3',
     description='liveramp_automation_framework',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     packages=['liveramp_automation'],
     install_requires=[
         'pytest',
         'pytest-bdd',
```

