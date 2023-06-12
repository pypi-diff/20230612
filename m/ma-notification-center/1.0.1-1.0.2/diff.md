# Comparing `tmp/ma_notification_center-1.0.1.tar.gz` & `tmp/ma_notification_center-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma_notification_center-1.0.1.tar", last modified: Mon Jun 12 10:13:59 2023, max compression
+gzip compressed data, was "ma_notification_center-1.0.2.tar", last modified: Mon Jun 12 10:20:18 2023, max compression
```

## Comparing `ma_notification_center-1.0.1.tar` & `ma_notification_center-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 10:13:59.293811 ma_notification_center-1.0.1/
--rw-rw-rw-   0        0        0     1055 2023-06-12 09:34:49.000000 ma_notification_center-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2598 2023-06-12 10:13:59.293811 ma_notification_center-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      879 2023-06-12 10:13:38.000000 ma_notification_center-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 10:13:59.287432 ma_notification_center-1.0.1/ma_notification_center.egg-info/
--rw-rw-rw-   0        0        0     2598 2023-06-12 10:13:59.000000 ma_notification_center-1.0.1/ma_notification_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-06-12 10:13:59.000000 ma_notification_center-1.0.1/ma_notification_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 10:13:59.000000 ma_notification_center-1.0.1/ma_notification_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-12 10:13:59.000000 ma_notification_center-1.0.1/ma_notification_center.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-06-12 10:13:59.000000 ma_notification_center-1.0.1/ma_notification_center.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-12 10:13:59.000000 ma_notification_center-1.0.1/ma_notification_center.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      824 2023-06-12 10:13:00.000000 ma_notification_center-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 10:13:59.294786 ma_notification_center-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-06-12 10:13:11.000000 ma_notification_center-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 10:13:59.263552 ma_notification_center-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 10:13:59.292789 ma_notification_center-1.0.1/src/notification_center/
--rw-rw-rw-   0        0        0       28 2023-06-12 09:16:01.000000 ma_notification_center-1.0.1/src/notification_center/__init__.py
--rw-rw-rw-   0        0        0      223 2023-06-12 09:30:38.000000 ma_notification_center-1.0.1/src/notification_center/__main__.py
--rw-rw-rw-   0        0        0     4485 2023-06-12 09:25:05.000000 ma_notification_center-1.0.1/src/notification_center/notification_center.py
--rw-rw-rw-   0        0        0     1078 2023-06-12 09:33:29.000000 ma_notification_center-1.0.1/src/notification_center/sqs_services.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:20:18.584109 ma_notification_center-1.0.2/
+-rw-rw-rw-   0        0        0     1055 2023-06-12 09:34:49.000000 ma_notification_center-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2634 2023-06-12 10:20:18.583146 ma_notification_center-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      915 2023-06-12 10:19:53.000000 ma_notification_center-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 10:20:18.576058 ma_notification_center-1.0.2/ma_notification_center.egg-info/
+-rw-rw-rw-   0        0        0     2634 2023-06-12 10:20:18.000000 ma_notification_center-1.0.2/ma_notification_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-06-12 10:20:18.000000 ma_notification_center-1.0.2/ma_notification_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:20:18.000000 ma_notification_center-1.0.2/ma_notification_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-12 10:20:18.000000 ma_notification_center-1.0.2/ma_notification_center.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-06-12 10:20:18.000000 ma_notification_center-1.0.2/ma_notification_center.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-12 10:20:18.000000 ma_notification_center-1.0.2/ma_notification_center.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      824 2023-06-12 10:20:01.000000 ma_notification_center-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:20:18.584109 ma_notification_center-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-06-12 10:19:57.000000 ma_notification_center-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:20:18.551123 ma_notification_center-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 10:20:18.582112 ma_notification_center-1.0.2/src/notification_center/
+-rw-rw-rw-   0        0        0       28 2023-06-12 09:16:01.000000 ma_notification_center-1.0.2/src/notification_center/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-06-12 09:30:38.000000 ma_notification_center-1.0.2/src/notification_center/__main__.py
+-rw-rw-rw-   0        0        0     4485 2023-06-12 09:25:05.000000 ma_notification_center-1.0.2/src/notification_center/notification_center.py
+-rw-rw-rw-   0        0        0     1078 2023-06-12 09:33:29.000000 ma_notification_center-1.0.2/src/notification_center/sqs_services.py
```

### Comparing `ma_notification_center-1.0.1/LICENSE` & `ma_notification_center-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ma_notification_center-1.0.1/PKG-INFO` & `ma_notification_center-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma_notification_center
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for sending notifications internally for MobileArts
 Author: Fatima Medlij
 Author-email: Fatima Medlij <medlijfatima@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -28,26 +28,27 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ma-notification-center version 1.0.1
+# ma-notification-center version 1.0.2
 ## Functions
 
 - send_email()
 - send_telegram()
 - send_sms()
 - send_telegram_photo()
 - send_telegram_document()
 
 ## Installation
 Install the dependencies.
 ```sh
+pip install ma_notification_center
 pip install -r requirements.txt
 ```
 
 ## Usage
 After installation add requirement to your code
 ```sh
 import ma_notification_center
```

### Comparing `ma_notification_center-1.0.1/ma_notification_center.egg-info/PKG-INFO` & `ma_notification_center-1.0.2/ma_notification_center.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma-notification-center
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for sending notifications internally for MobileArts
 Author: Fatima Medlij
 Author-email: Fatima Medlij <medlijfatima@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -28,26 +28,27 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ma-notification-center version 1.0.1
+# ma-notification-center version 1.0.2
 ## Functions
 
 - send_email()
 - send_telegram()
 - send_sms()
 - send_telegram_photo()
 - send_telegram_document()
 
 ## Installation
 Install the dependencies.
 ```sh
+pip install ma_notification_center
 pip install -r requirements.txt
 ```
 
 ## Usage
 After installation add requirement to your code
 ```sh
 import ma_notification_center
```

### Comparing `ma_notification_center-1.0.1/pyproject.toml` & `ma_notification_center-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ma_notification_center"
-version = "1.0.1"
+version = "1.0.2"
 description = "A package for sending notifications internally for MobileArts"
 readme = "README.md"
 authors = [{ name = "Fatima Medlij", email = "medlijfatima@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `ma_notification_center-1.0.1/setup.py` & `ma_notification_center-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="ma_notification_center",
-    version="1.0.1",
+    version="1.0.2",
     description="A package for sending notifications internally for MobileArts",
     author="Fatima Medlij",
     author_email="medlijfatima@gmail.com",
     packages=find_namespace_packages(include=["src.*"]),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
```

### Comparing `ma_notification_center-1.0.1/src/notification_center/notification_center.py` & `ma_notification_center-1.0.2/src/notification_center/notification_center.py`

 * *Files identical despite different names*

### Comparing `ma_notification_center-1.0.1/src/notification_center/sqs_services.py` & `ma_notification_center-1.0.2/src/notification_center/sqs_services.py`

 * *Files identical despite different names*

