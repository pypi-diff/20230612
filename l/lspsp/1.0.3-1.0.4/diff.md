# Comparing `tmp/lspsp-1.0.3.tar.gz` & `tmp/lspsp-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lspsp-1.0.3.tar", last modified: Thu Jun  8 10:24:30 2023, max compression
+gzip compressed data, was "lspsp-1.0.4.tar", last modified: Mon Jun 12 16:06:01 2023, max compression
```

## Comparing `lspsp-1.0.3.tar` & `lspsp-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:30.439299 lspsp-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 10:24:20.000000 lspsp-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 10:24:30.439299 lspsp-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 10:24:20.000000 lspsp-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-08 10:24:20.000000 lspsp-1.0.3/config.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:30.435299 lspsp-1.0.3/lspsp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/lspmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/lspnotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/lspsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/mailbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/monexec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:30.439299 lspsp-1.0.3/lspsp/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/resource/mail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/resource/test.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:30.439299 lspsp-1.0.3/lspsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:24:30.439299 lspsp-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-08 10:24:20.000000 lspsp-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:06:01.632460 lspsp-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 16:05:52.000000 lspsp-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-12 16:06:01.632460 lspsp-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 16:05:52.000000 lspsp-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-12 16:05:52.000000 lspsp-1.0.4/config.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:06:01.632460 lspsp-1.0.4/lspsp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/lspmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/lspnotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/lspsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/mailbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/monexec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:06:01.632460 lspsp-1.0.4/lspsp/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/resource/mail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-12 16:05:52.000000 lspsp-1.0.4/lspsp/resource/test.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:06:01.632460 lspsp-1.0.4/lspsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-12 16:06:01.000000 lspsp-1.0.4/lspsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-12 16:06:01.000000 lspsp-1.0.4/lspsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:06:01.000000 lspsp-1.0.4/lspsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 16:06:01.000000 lspsp-1.0.4/lspsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 16:06:01.000000 lspsp-1.0.4/lspsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 16:06:01.000000 lspsp-1.0.4/lspsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:06:01.632460 lspsp-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-12 16:05:52.000000 lspsp-1.0.4/setup.py
```

### Comparing `lspsp-1.0.3/lspsp/lspmon.py` & `lspsp-1.0.4/lspsp/lspmon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
+import time
 from apscheduler.schedulers.blocking import BlockingScheduler
 from lspsp.lspnotify import LspNotify
 
 import logging
 from lspsp.lspsp import Lspsp
 
 
 class Lspmon:
     _interval = 60
     _current = {}
+    _last_notify = {}
 
     def __init__(self, mode) -> None:
         f = open('config.json', 'r')
         text = f.read()
         f.close()
         data = json.loads(text)
         self._notify_config = data['notify_config']
@@ -31,15 +33,20 @@
         for key in data.keys():
             if self._current.get(key) == None:
                 diff[key] = data[key]
         return diff
 
     def notify(self, diff):
         self._logger.info("New goods available found: %s", diff)
+        current_time = time.time()
         for key in self._notify_config.keys():
+            delta = current_time - self._last_notify.get(key, 0)
+            if delta < self._notify_config[key]['rate_limit']:
+                continue
+            self._last_notify[key] = current_time
             if self._notify_config[key]['enabled']:
                 notify_method = getattr(self._notifier, key)
                 notify_method(self._notify_config[key], diff)
 
     def job(self):
         data = self._api.list()
         diff = self.diff(data)
```

### Comparing `lspsp-1.0.3/lspsp/lspnotify.py` & `lspsp-1.0.4/lspsp/lspnotify.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from email.header import Header
-from email.mime.text import MIMEText
 import logging
 import smtplib
 from jinja2 import Environment, FileSystemLoader
 import os
 
 from lspsp.mailbuilder import MailBuilder
```

### Comparing `lspsp-1.0.3/lspsp/lspsp.py` & `lspsp-1.0.4/lspsp/lspsp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from bs4 import BeautifulSoup
 import requests
 
 LSP_HOST = 'https://www.lspsp.me'
 
 
 class Lspsp:
```

### Comparing `lspsp-1.0.3/lspsp/mailbuilder.py` & `lspsp-1.0.4/lspsp/mailbuilder.py`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.3/lspsp/monexec.py` & `lspsp-1.0.4/lspsp/monexec.py`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.3/lspsp/resource/mail.html` & `lspsp-1.0.4/lspsp/resource/mail.html`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.3/lspsp/resource/test.html` & `lspsp-1.0.4/lspsp/resource/test.html`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.3/setup.py` & `lspsp-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="lspsp",
-    version="1.0.3",
+    version="1.0.4",
     license='GPL',
     description='LSPSP.ME Monitor',
     long_description='LSPSP.ME Monitor Service',
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
     install_requires=[
```

