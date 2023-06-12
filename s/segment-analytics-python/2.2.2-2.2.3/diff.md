# Comparing `tmp/segment-analytics-python-2.2.2.tar.gz` & `tmp/segment-analytics-python-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-analytics-python-2.2.2.tar", last modified: Tue Nov 29 17:01:56 2022, max compression
+gzip compressed data, was "segment-analytics-python-2.2.3.tar", last modified: Mon Jun 12 18:37:10 2023, max compression
```

## Comparing `segment-analytics-python-2.2.2.tar` & `segment-analytics-python-2.2.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.840767 segment-analytics-python-2.2.2/
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.804112 segment-analytics-python-2.2.2/.buildscripts/
--rwxr-xr-x   0 michaelgh   (501) staff       (20)      517 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/.buildscripts/e2e.sh
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.804771 segment-analytics-python-2.2.2/.circleci/
--rw-r--r--   0 michaelgh   (501) staff       (20)     2620 2022-09-01 22:29:40.000000 segment-analytics-python-2.2.2/.circleci/config.yml
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.805276 segment-analytics-python-2.2.2/.github/
--rw-r--r--   0 michaelgh   (501) staff       (20)      156 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/.github/dependabot.yml
--rw-r--r--   0 michaelgh   (501) staff       (20)       98 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/.gitignore
--rw-r--r--   0 michaelgh   (501) staff       (20)    16666 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/.pylintrc
--rw-r--r--   0 michaelgh   (501) staff       (20)     3934 2022-11-29 16:56:00.000000 segment-analytics-python-2.2.2/HISTORY.md
--rw-r--r--   0 michaelgh   (501) staff       (20)     1078 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/LICENSE
--rw-r--r--   0 michaelgh   (501) staff       (20)       18 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/MANIFEST.in
--rw-r--r--   0 michaelgh   (501) staff       (20)      325 2022-09-01 22:55:40.000000 segment-analytics-python-2.2.2/Makefile
--rw-r--r--   0 michaelgh   (501) staff       (20)     1242 2022-11-29 17:01:56.840874 segment-analytics-python-2.2.2/PKG-INFO
--rw-r--r--   0 michaelgh   (501) staff       (20)     5528 2022-09-06 22:41:44.000000 segment-analytics-python-2.2.2/README.md
--rw-r--r--   0 michaelgh   (501) staff       (20)      346 2022-11-29 16:59:22.000000 segment-analytics-python-2.2.2/RELEASING.md
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.807886 segment-analytics-python-2.2.2/analytics/
--rw-r--r--   0 michaelgh   (501) staff       (20)     4360 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/analytics/consumer.py
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.814130 segment-analytics-python-2.2.2/analytics/test/
--rw-r--r--   0 michaelgh   (501) staff       (20)    12986 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/analytics/test/client.py
--rwxr-xr-x   0 michaelgh   (501) staff       (20)       45 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/e2e_test.sh
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.782148 segment-analytics-python-2.2.2/segment/
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.830123 segment-analytics-python-2.2.2/segment/analytics/
--rw-r--r--   0 michaelgh   (501) staff       (20)     1981 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/__init__.py
--rw-r--r--   0 michaelgh   (501) staff       (20)    11207 2022-11-29 16:50:40.000000 segment-analytics-python-2.2.2/segment/analytics/client.py
--rw-r--r--   0 michaelgh   (501) staff       (20)     4457 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/consumer.py
--rw-r--r--   0 michaelgh   (501) staff       (20)     2367 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/request.py
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.834070 segment-analytics-python-2.2.2/segment/analytics/test/
--rw-r--r--   0 michaelgh   (501) staff       (20)     2607 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/test/__init__.py
--rw-r--r--   0 michaelgh   (501) staff       (20)    13127 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/test/client.py
--rw-r--r--   0 michaelgh   (501) staff       (20)     7182 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/test/consumer.py
--rw-r--r--   0 michaelgh   (501) staff       (20)     1155 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/test/module.py
--rw-r--r--   0 michaelgh   (501) staff       (20)     2022 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/test/request.py
--rw-r--r--   0 michaelgh   (501) staff       (20)     2141 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/test/utils.py
--rw-r--r--   0 michaelgh   (501) staff       (20)     2468 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/segment/analytics/utils.py
--rw-r--r--   0 michaelgh   (501) staff       (20)       18 2022-11-29 16:54:13.000000 segment-analytics-python-2.2.2/segment/analytics/version.py
-drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2022-11-29 17:01:56.840195 segment-analytics-python-2.2.2/segment_analytics_python.egg-info/
--rw-r--r--   0 michaelgh   (501) staff       (20)     1242 2022-11-29 17:01:56.000000 segment-analytics-python-2.2.2/segment_analytics_python.egg-info/PKG-INFO
--rw-r--r--   0 michaelgh   (501) staff       (20)      853 2022-11-29 17:01:56.000000 segment-analytics-python-2.2.2/segment_analytics_python.egg-info/SOURCES.txt
--rw-r--r--   0 michaelgh   (501) staff       (20)        1 2022-11-29 17:01:56.000000 segment-analytics-python-2.2.2/segment_analytics_python.egg-info/dependency_links.txt
--rw-r--r--   0 michaelgh   (501) staff       (20)      111 2022-11-29 17:01:56.000000 segment-analytics-python-2.2.2/segment_analytics_python.egg-info/requires.txt
--rw-r--r--   0 michaelgh   (501) staff       (20)       18 2022-11-29 17:01:56.000000 segment-analytics-python-2.2.2/segment_analytics_python.egg-info/top_level.txt
--rw-r--r--   0 michaelgh   (501) staff       (20)       67 2022-11-29 17:01:56.841641 segment-analytics-python-2.2.2/setup.cfg
--rw-r--r--   0 michaelgh   (501) staff       (20)     1995 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/setup.py
--rw-r--r--   0 michaelgh   (501) staff       (20)     2725 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.2/simulator.py
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.066062 segment-analytics-python-2.2.3/
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.046781 segment-analytics-python-2.2.3/.buildscripts/
+-rwxr-xr-x   0 michaelgh   (501) staff       (20)      517 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/.buildscripts/e2e.sh
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.047133 segment-analytics-python-2.2.3/.circleci/
+-rw-r--r--   0 michaelgh   (501) staff       (20)     2620 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/.circleci/config.yml
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.050423 segment-analytics-python-2.2.3/.github/
+-rw-r--r--   0 michaelgh   (501) staff       (20)      156 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.3/.github/dependabot.yml
+-rw-r--r--   0 michaelgh   (501) staff       (20)       98 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/.gitignore
+-rw-r--r--   0 michaelgh   (501) staff       (20)    16666 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/.pylintrc
+-rw-r--r--   0 michaelgh   (501) staff       (20)     4040 2023-06-12 18:28:47.000000 segment-analytics-python-2.2.3/HISTORY.md
+-rw-r--r--   0 michaelgh   (501) staff       (20)     1078 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/LICENSE
+-rw-r--r--   0 michaelgh   (501) staff       (20)       18 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.3/MANIFEST.in
+-rw-r--r--   0 michaelgh   (501) staff       (20)      325 2023-06-12 18:30:21.000000 segment-analytics-python-2.2.3/Makefile
+-rw-r--r--   0 michaelgh   (501) staff       (20)     1324 2023-06-12 18:37:10.066127 segment-analytics-python-2.2.3/PKG-INFO
+-rw-r--r--   0 michaelgh   (501) staff       (20)     5536 2023-06-12 18:28:47.000000 segment-analytics-python-2.2.3/README.md
+-rw-r--r--   0 michaelgh   (501) staff       (20)      346 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/RELEASING.md
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.050907 segment-analytics-python-2.2.3/analytics/
+-rw-r--r--   0 michaelgh   (501) staff       (20)     4360 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/analytics/consumer.py
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.051257 segment-analytics-python-2.2.3/analytics/test/
+-rw-r--r--   0 michaelgh   (501) staff       (20)    12986 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/analytics/test/client.py
+-rwxr-xr-x   0 michaelgh   (501) staff       (20)       45 2022-09-01 00:06:05.000000 segment-analytics-python-2.2.3/e2e_test.sh
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.036135 segment-analytics-python-2.2.3/segment/
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.057932 segment-analytics-python-2.2.3/segment/analytics/
+-rw-r--r--   0 michaelgh   (501) staff       (20)     2030 2023-06-12 18:28:47.000000 segment-analytics-python-2.2.3/segment/analytics/__init__.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)    11207 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/client.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)     4457 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/consumer.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)     2367 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/request.py
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.062914 segment-analytics-python-2.2.3/segment/analytics/test/
+-rw-r--r--   0 michaelgh   (501) staff       (20)     2607 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/test/__init__.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)    13127 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/test/client.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)     7182 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/test/consumer.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)     1155 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/test/module.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)     2022 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/test/request.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)     2141 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/test/utils.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)     2468 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/segment/analytics/utils.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)       18 2023-06-12 18:28:47.000000 segment-analytics-python-2.2.3/segment/analytics/version.py
+drwxr-xr-x   0 michaelgh   (501) staff       (20)        0 2023-06-12 18:37:10.065864 segment-analytics-python-2.2.3/segment_analytics_python.egg-info/
+-rw-r--r--   0 michaelgh   (501) staff       (20)     1324 2023-06-12 18:37:10.000000 segment-analytics-python-2.2.3/segment_analytics_python.egg-info/PKG-INFO
+-rw-r--r--   0 michaelgh   (501) staff       (20)      853 2023-06-12 18:37:10.000000 segment-analytics-python-2.2.3/segment_analytics_python.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelgh   (501) staff       (20)        1 2023-06-12 18:37:10.000000 segment-analytics-python-2.2.3/segment_analytics_python.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelgh   (501) staff       (20)      111 2023-06-12 18:37:10.000000 segment-analytics-python-2.2.3/segment_analytics_python.egg-info/requires.txt
+-rw-r--r--   0 michaelgh   (501) staff       (20)       18 2023-06-12 18:37:10.000000 segment-analytics-python-2.2.3/segment_analytics_python.egg-info/top_level.txt
+-rw-r--r--   0 michaelgh   (501) staff       (20)       67 2023-06-12 18:37:10.066407 segment-analytics-python-2.2.3/setup.cfg
+-rw-r--r--   0 michaelgh   (501) staff       (20)     2095 2023-06-12 18:28:47.000000 segment-analytics-python-2.2.3/setup.py
+-rw-r--r--   0 michaelgh   (501) staff       (20)     2725 2023-06-12 18:28:39.000000 segment-analytics-python-2.2.3/simulator.py
```

### Comparing `segment-analytics-python-2.2.2/.buildscripts/e2e.sh` & `segment-analytics-python-2.2.3/.buildscripts/e2e.sh`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/.circleci/config.yml` & `segment-analytics-python-2.2.3/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/.pylintrc` & `segment-analytics-python-2.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/HISTORY.md` & `segment-analytics-python-2.2.3/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 2.2.3 / 2023-06-12
+- Support for Python 3.10 and 3.11
+- Return values for function calls via the proxy
+
 # 2.2.2 / 2022-11-29
 - Specifying milliseconds as the isoformat rather than the default microseconds in timestamp
 
 # 2.2.1 / 2022-06-23
 - Empty Catch fix #217
 - Build Isolation fix #216
 - Removing remaining string_type references
```

### Comparing `segment-analytics-python-2.2.2/LICENSE` & `segment-analytics-python-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/PKG-INFO` & `segment-analytics-python-2.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: segment-analytics-python
-Version: 2.2.2
+Version: 2.2.3
 Summary: The hassle-free way to integrate analytics into any python application.
 Home-page: https://github.com/segmentio/analytics-python
 Author: Segment
 Author-email: friends@segment.com
 Maintainer: Segment
 Maintainer-email: friends@segment.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6.0
 Provides-Extra: test
 License-File: LICENSE
 
 
 Segment is the simplest way to integrate analytics into your application.
 One API allows you to turn on any other analytics service. No more learning
 new APIs, repeated code, and wasted development time.
 
 This is the official python client that wraps the Segment REST API (https://segment.com).
 
 Documentation and more details at https://github.com/segmentio/analytics-python
-
-
```

### Comparing `segment-analytics-python-2.2.2/README.md` & `segment-analytics-python-2.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ```sql
     select * from app.order_completed
     order by price desc
     ```
 
 ## 👨‍💻 Getting Started
 
-Install `analytics-python` using pip:
+Install `segment-analytics-python` using pip:
 
 ```bash
 pip3 install segment-analytics-python
 ```
 
 or you can clone this repo:
 ```bash
```

#### html2text {}

```diff
@@ -32,20 +32,20 @@
 and send it on to any tool. 4. **Query your data in SQL**. Slice, dice, and
 analyze your data in detail with Segment SQL. We'll transform and load your
 customer behavioral data directly from your apps into Amazon Redshift, Google
 BigQuery, or Postgres. Save weeks of engineering time by not having to invent
 your data warehouse and ETL pipeline. For example, you can capture data on any
 app: ```python analytics.track('Order Completed', { price: 99.84 }) ``` Then,
 query the resulting data in SQL: ```sql select * from app.order_completed order
-by price desc ``` ## ð¨âð» Getting Started Install `analytics-python`
-using pip: ```bash pip3 install segment-analytics-python ``` or you can clone
-this repo: ```bash git clone https://github.com/segmentio/analytics-python.git
-cd analytics-python sudo python3 setup.py install ``` Now inside your app,
-you'll want to **set your** `write_key` before making any analytics calls:
-```python import segment.analytics as analytics analytics.write_key =
+by price desc ``` ## ð¨âð» Getting Started Install `segment-analytics-
+python` using pip: ```bash pip3 install segment-analytics-python ``` or you can
+clone this repo: ```bash git clone https://github.com/segmentio/analytics-
+python.git cd analytics-python sudo python3 setup.py install ``` Now inside
+your app, you'll want to **set your** `write_key` before making any analytics
+calls: ```python import segment.analytics as analytics analytics.write_key =
 'YOUR_WRITE_KEY' ``` **Note** If you need to send data to multiple Segment
 sources, you can initialize a new Client for each `write_key` ### ð Startup
 Program
   [https://user-images.githubusercontent.com/16131737/53128952-08d3d400-351b-
                           11e9-9730-7da35adda781.png]
 If you are part of a new startup (<$5M raised, <2 years since founding), we
 just launched a new startup program for you. You can get a Segment Team plan
```

### Comparing `segment-analytics-python-2.2.2/analytics/consumer.py` & `segment-analytics-python-2.2.3/analytics/consumer.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/analytics/test/client.py` & `segment-analytics-python-2.2.3/analytics/test/client.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/__init__.py` & `segment-analytics-python-2.2.3/segment/analytics/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,40 +17,40 @@
 max_retries = Client.DefaultConfig.max_retries
 
 default_client = None
 
 
 def track(*args, **kwargs):
     """Send a track call."""
-    _proxy('track', *args, **kwargs)
+    return _proxy('track', *args, **kwargs)
 
 
 def identify(*args, **kwargs):
     """Send a identify call."""
-    _proxy('identify', *args, **kwargs)
+    return _proxy('identify', *args, **kwargs)
 
 
 def group(*args, **kwargs):
     """Send a group call."""
-    _proxy('group', *args, **kwargs)
+    return _proxy('group', *args, **kwargs)
 
 
 def alias(*args, **kwargs):
     """Send a alias call."""
-    _proxy('alias', *args, **kwargs)
+    return _proxy('alias', *args, **kwargs)
 
 
 def page(*args, **kwargs):
     """Send a page call."""
-    _proxy('page', *args, **kwargs)
+    return _proxy('page', *args, **kwargs)
 
 
 def screen(*args, **kwargs):
     """Send a screen call."""
-    _proxy('screen', *args, **kwargs)
+    return _proxy('screen', *args, **kwargs)
 
 
 def flush():
     """Tell the client to flush."""
     _proxy('flush')
 
 
@@ -72,8 +72,8 @@
         default_client = Client(write_key, host=host, debug=debug,
                                 max_queue_size=max_queue_size,
                                 send=send, on_error=on_error,
                                 gzip=gzip, max_retries=max_retries,
                                 sync_mode=sync_mode, timeout=timeout)
 
     fn = getattr(default_client, method)
-    fn(*args, **kwargs)
+    return fn(*args, **kwargs)
```

### Comparing `segment-analytics-python-2.2.2/segment/analytics/client.py` & `segment-analytics-python-2.2.3/segment/analytics/client.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/consumer.py` & `segment-analytics-python-2.2.3/segment/analytics/consumer.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/request.py` & `segment-analytics-python-2.2.3/segment/analytics/request.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/test/__init__.py` & `segment-analytics-python-2.2.3/segment/analytics/test/__init__.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/test/client.py` & `segment-analytics-python-2.2.3/segment/analytics/test/client.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/test/consumer.py` & `segment-analytics-python-2.2.3/segment/analytics/test/consumer.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/test/module.py` & `segment-analytics-python-2.2.3/segment/analytics/test/module.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/test/request.py` & `segment-analytics-python-2.2.3/segment/analytics/test/request.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/test/utils.py` & `segment-analytics-python-2.2.3/segment/analytics/test/utils.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment/analytics/utils.py` & `segment-analytics-python-2.2.3/segment/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/segment_analytics_python.egg-info/PKG-INFO` & `segment-analytics-python-2.2.3/segment_analytics_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: segment-analytics-python
-Version: 2.2.2
+Version: 2.2.3
 Summary: The hassle-free way to integrate analytics into any python application.
 Home-page: https://github.com/segmentio/analytics-python
 Author: Segment
 Author-email: friends@segment.com
 Maintainer: Segment
 Maintainer-email: friends@segment.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6.0
 Provides-Extra: test
 License-File: LICENSE
 
 
 Segment is the simplest way to integrate analytics into your application.
 One API allows you to turn on any other analytics service. No more learning
 new APIs, repeated code, and wasted development time.
 
 This is the official python client that wraps the Segment REST API (https://segment.com).
 
 Documentation and more details at https://github.com/segmentio/analytics-python
-
-
```

### Comparing `segment-analytics-python-2.2.2/segment_analytics_python.egg-info/SOURCES.txt` & `segment-analytics-python-2.2.3/segment_analytics_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segment-analytics-python-2.2.2/setup.py` & `segment-analytics-python-2.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,9 +56,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `segment-analytics-python-2.2.2/simulator.py` & `segment-analytics-python-2.2.3/simulator.py`

 * *Files identical despite different names*

