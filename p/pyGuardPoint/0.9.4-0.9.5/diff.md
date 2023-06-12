# Comparing `tmp/pyGuardPoint-0.9.4.tar.gz` & `tmp/pyGuardPoint-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.9.4.tar", last modified: Mon Jun 12 09:39:41 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.9.5.tar", last modified: Mon Jun 12 10:03:21 2023, max compression
```

## Comparing `pyGuardPoint-0.9.4.tar` & `pyGuardPoint-0.9.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 09:39:41.418538 pyGuardPoint-0.9.4/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.9.4/LICENSE.txt
--rw-rw-rw-   0        0        0     5739 2023-06-12 09:39:41.418538 pyGuardPoint-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.9.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 09:39:41.401598 pyGuardPoint-0.9.4/pyGuardPoint/
--rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.9.4/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11195 2023-04-20 13:33:25.000000 pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_cardholdertypes.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1195 2023-05-12 10:57:02.000000 pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.9.4/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.9.4/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2698 2023-06-12 09:36:22.000000 pyGuardPoint-0.9.4/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.9.4/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     6292 2023-06-12 09:05:46.000000 pyGuardPoint-0.9.4/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-0.9.4/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.9.4/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-0.9.4/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:39:41.417539 pyGuardPoint-0.9.4/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     5739 2023-06-12 09:39:41.000000 pyGuardPoint-0.9.4/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-06-12 09:39:41.000000 pyGuardPoint-0.9.4/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 09:39:41.000000 pyGuardPoint-0.9.4/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.9.4/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-06-12 09:39:41.000000 pyGuardPoint-0.9.4/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 09:39:41.000000 pyGuardPoint-0.9.4/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 09:39:41.418538 pyGuardPoint-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0      549 2023-06-12 08:58:19.000000 pyGuardPoint-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:03:21.564703 pyGuardPoint-0.9.5/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.9.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     5739 2023-06-12 10:03:21.564703 pyGuardPoint-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.9.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 10:03:21.550664 pyGuardPoint-0.9.5/pyGuardPoint/
+-rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.9.5/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11195 2023-04-20 13:33:25.000000 pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1195 2023-05-12 10:57:02.000000 pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5586 2023-04-20 11:51:01.000000 pyGuardPoint-0.9.5/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.9.5/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2698 2023-06-12 09:36:22.000000 pyGuardPoint-0.9.5/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.9.5/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     6318 2023-06-12 10:03:04.000000 pyGuardPoint-0.9.5/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-0.9.5/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.9.5/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-0.9.5/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:03:21.563702 pyGuardPoint-0.9.5/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     5739 2023-06-12 10:03:21.000000 pyGuardPoint-0.9.5/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-06-12 10:03:21.000000 pyGuardPoint-0.9.5/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:03:21.000000 pyGuardPoint-0.9.5/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.9.5/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-06-12 10:03:21.000000 pyGuardPoint-0.9.5/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 10:03:21.000000 pyGuardPoint-0.9.5/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:03:21.564703 pyGuardPoint-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      549 2023-06-12 10:03:04.000000 pyGuardPoint-0.9.5/setup.py
```

### Comparing `pyGuardPoint-0.9.4/LICENSE.txt` & `pyGuardPoint-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/PKG-INFO` & `pyGuardPoint-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.9.4/README.rst` & `pyGuardPoint-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_cardholdertypes.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_cardholdertypes.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.9.5/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.9.5/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.9.5/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.9.5/pyGuardPoint/guardpoint_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
             self.set_token(token)
         else:
             self.token = None
             self.token_issued = 0
             self.token_expiry = 0
         log.info(f"GP10 server connection: {self.baseurl}")
         if url_components['scheme'] == 'https':
-            # Loading System Defaults
-            context = ssl.create_default_context()
+            # Loading System Defaults for TLS Client
+            context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
 
             if cert_file and key_file:
                 # Loading of client certificate
                 context.load_cert_chain(certfile=cert_file, keyfile=key_file)
 
             if ca_file:
                 # Loading of CA certificate.
```

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.9.5/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.9.5/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-0.9.5/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.9.4/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.9.5/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.4/setup.py` & `pyGuardPoint-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.9.4",
+      version="0.9.5",
       author="John Owen",
       description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein'],
       packages=['pyGuardPoint'],
```

