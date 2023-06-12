# Comparing `tmp/liveramp_automation_framework-0.0.6.tar.gz` & `tmp/liveramp_automation_framework-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation_framework-0.0.6.tar", last modified: Mon Jun 12 03:50:33 2023, max compression
+gzip compressed data, was "liveramp_automation_framework-0.0.7.tar", last modified: Mon Jun 12 07:53:16 2023, max compression
```

## Comparing `liveramp_automation_framework-0.0.6.tar` & `liveramp_automation_framework-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 03:50:33.782447 liveramp_automation_framework-0.0.6/
--rw-r--r--   0 jasqia     (502) staff       (20)      173 2023-06-12 03:50:33.781749 liveramp_automation_framework-0.0.6/PKG-INFO
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 03:50:33.775439 liveramp_automation_framework-0.0.6/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)      271 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.0.6/liveramp_automation/allure_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.0.6/liveramp_automation/logger.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3120 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.6/liveramp_automation/login_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.0.6/liveramp_automation/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.6/liveramp_automation/playwright_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2317 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.6/liveramp_automation/read_report.py
--rw-r--r--   0 jasqia     (502) staff       (20)     6985 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.6/liveramp_automation/request_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      836 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.6/liveramp_automation/selenium_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.0.6/liveramp_automation/time_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1050 2023-06-12 03:17:58.000000 liveramp_automation_framework-0.0.6/liveramp_automation/upload_util.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 03:50:33.780419 liveramp_automation_framework-0.0.6/liveramp_automation_framework.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)      173 2023-06-12 03:50:33.000000 liveramp_automation_framework-0.0.6/liveramp_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-12 03:50:33.000000 liveramp_automation_framework-0.0.6/liveramp_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-12 03:50:33.000000 liveramp_automation_framework-0.0.6/liveramp_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-06-12 03:50:33.000000 liveramp_automation_framework-0.0.6/liveramp_automation_framework.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-12 03:50:33.000000 liveramp_automation_framework-0.0.6/liveramp_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-12 03:50:33.782625 liveramp_automation_framework-0.0.6/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)      937 2023-06-12 03:50:30.000000 liveramp_automation_framework-0.0.6/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 07:53:16.509475 liveramp_automation_framework-0.0.7/
+-rw-r--r--   0 jasqia     (502) staff       (20)      809 2023-06-12 07:53:16.509026 liveramp_automation_framework-0.0.7/PKG-INFO
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 07:53:16.503373 liveramp_automation_framework-0.0.7/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)      271 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.0.7/liveramp_automation/allure_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.0.7/liveramp_automation/logger.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3120 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.7/liveramp_automation/login_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.0.7/liveramp_automation/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.7/liveramp_automation/playwright_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2317 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.7/liveramp_automation/read_report.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     6985 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.7/liveramp_automation/request_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      836 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.0.7/liveramp_automation/selenium_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.0.7/liveramp_automation/time_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      719 2023-06-12 07:52:52.000000 liveramp_automation_framework-0.0.7/liveramp_automation/upload_util.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-12 07:53:16.508115 liveramp_automation_framework-0.0.7/liveramp_automation_framework.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)      809 2023-06-12 07:53:16.000000 liveramp_automation_framework-0.0.7/liveramp_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-12 07:53:16.000000 liveramp_automation_framework-0.0.7/liveramp_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-12 07:53:16.000000 liveramp_automation_framework-0.0.7/liveramp_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-06-12 07:53:16.000000 liveramp_automation_framework-0.0.7/liveramp_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-12 07:53:16.000000 liveramp_automation_framework-0.0.7/liveramp_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-12 07:53:16.509619 liveramp_automation_framework-0.0.7/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1170 2023-06-12 07:53:13.000000 liveramp_automation_framework-0.0.7/setup.py
```

### Comparing `liveramp_automation_framework-0.0.6/liveramp_automation/logger.py` & `liveramp_automation_framework-0.0.7/liveramp_automation/logger.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.6/liveramp_automation/login_util.py` & `liveramp_automation_framework-0.0.7/liveramp_automation/login_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.6/liveramp_automation/parsers.py` & `liveramp_automation_framework-0.0.7/liveramp_automation/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.6/liveramp_automation/playwright_util.py` & `liveramp_automation_framework-0.0.7/liveramp_automation/playwright_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.6/liveramp_automation/read_report.py` & `liveramp_automation_framework-0.0.7/liveramp_automation/read_report.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.6/liveramp_automation/request_util.py` & `liveramp_automation_framework-0.0.7/liveramp_automation/request_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.6/liveramp_automation/selenium_util.py` & `liveramp_automation_framework-0.0.7/liveramp_automation/selenium_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.6/liveramp_automation/time_util.py` & `liveramp_automation_framework-0.0.7/liveramp_automation/time_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.0.6/liveramp_automation_framework.egg-info/SOURCES.txt` & `liveramp_automation_framework-0.0.7/liveramp_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

