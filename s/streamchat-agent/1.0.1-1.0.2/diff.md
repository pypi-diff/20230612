# Comparing `tmp/streamchat-agent-1.0.1.tar.gz` & `tmp/streamchat-agent-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamchat-agent-1.0.1.tar", last modified: Sat May 27 15:21:05 2023, max compression
+gzip compressed data, was "streamchat-agent-1.0.2.tar", last modified: Mon Jun 12 17:01:20 2023, max compression
```

## Comparing `streamchat-agent-1.0.1.tar` & `streamchat-agent-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-27 00:41:12.000000 streamchat-agent-1.0.1/LICENSE
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       24 2023-05-27 00:41:12.000000 streamchat-agent-1.0.1/MANIFEST.in
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5590 2023-05-27 15:05:43.000000 streamchat-agent-1.0.1/README.md
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       14 2023-05-27 00:41:12.000000 streamchat-agent-1.0.1/requirements.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/setup.cfg
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1177 2023-05-27 15:02:40.000000 streamchat-agent-1.0.1/setup.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/src/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3381 2023-05-27 14:35:40.000000 streamchat-agent-1.0.1/src/StreamChatAgent.py
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       53 2023-05-27 15:03:02.000000 streamchat-agent-1.0.1/src/__init__.py
-drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-05-27 15:21:05.367494 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/PKG-INFO
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      356 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/SOURCES.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/dependency_links.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/not-zip-safe
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/requires.txt
--rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       25 2023-05-27 15:21:05.000000 streamchat-agent-1.0.1/src/streamchat_agent.egg-info/top_level.txt
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:01:20.558882 streamchat-agent-1.0.2/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1069 2023-05-27 00:41:12.000000 streamchat-agent-1.0.2/LICENSE
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       24 2023-05-27 00:41:12.000000 streamchat-agent-1.0.2/MANIFEST.in
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-06-12 17:01:20.558882 streamchat-agent-1.0.2/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     5590 2023-06-12 16:59:03.000000 streamchat-agent-1.0.2/README.md
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       14 2023-05-27 00:41:12.000000 streamchat-agent-1.0.2/requirements.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       38 2023-06-12 17:01:20.558882 streamchat-agent-1.0.2/setup.cfg
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     1178 2023-06-12 16:27:56.000000 streamchat-agent-1.0.2/setup.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:01:20.558882 streamchat-agent-1.0.2/src/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)     3407 2023-06-11 16:45:23.000000 streamchat-agent-1.0.2/src/StreamChatAgent.py
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       54 2023-06-12 16:27:37.000000 streamchat-agent-1.0.2/src/__init__.py
+drwxr-xr-x   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        0 2023-06-12 17:01:20.558882 streamchat-agent-1.0.2/src/streamchat_agent.egg-info/
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      610 2023-06-12 17:01:20.000000 streamchat-agent-1.0.2/src/streamchat_agent.egg-info/PKG-INFO
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)      356 2023-06-12 17:01:20.000000 streamchat-agent-1.0.2/src/streamchat_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-06-12 17:01:20.000000 streamchat-agent-1.0.2/src/streamchat_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)        1 2023-05-27 15:21:05.000000 streamchat-agent-1.0.2/src/streamchat_agent.egg-info/not-zip-safe
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       15 2023-06-12 17:01:20.000000 streamchat-agent-1.0.2/src/streamchat_agent.egg-info/requires.txt
+-rw-r--r--   0 GeneralYadoc  (1001) GeneralYadoc  (1001)       25 2023-06-12 17:01:20.000000 streamchat-agent-1.0.2/src/streamchat_agent.egg-info/top_level.txt
```

### Comparing `streamchat-agent-1.0.1/LICENSE` & `streamchat-agent-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamchat-agent-1.0.1/PKG-INFO` & `streamchat-agent-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamchat-agent
-Version: 1.0.1
+Version: 1.0.2
 Summary: Get YouTube chat comments with minimum time lag
 Home-page: https://github.com/GeneralYadoc/StreamChatAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `streamchat-agent-1.0.1/README.md` & `streamchat-agent-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # StreamChatAgent
 YouTube chat poller which can get massages very smothly by using internal queue.
 
 ## The user of this library can
 - receive YouTube chat messages continiously by registering callback.
 - natively obtain high performance by using internal queue.
 
-## Hou to install
+## How to install
 You can select from following ways.
 
 ### Install from PyPI
 - Install package to your environment.<br>
     ```install
     $ pip install streamchat-agent
     ```
```

### Comparing `streamchat-agent-1.0.1/setup.py` & `streamchat-agent-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def _requires_from_file(filename):
     return open(filename).read().splitlines()
 
 
 setup(
     name="streamchat-agent",
-    version="1.0.1",
+    version="1.0.2",
     license="MIT",
     description="Get YouTube chat comments with minimum time lag",
     author="General Yadoc",
     author_email="133023047+GeneralYadoc@users.noreply.github.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
@@ -30,8 +30,8 @@
     package_dir={"": "src"},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     zip_safe=False,
     install_requires=_requires_from_file('requirements.txt'),
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "pytest-cov"]
-)
+)
```

### Comparing `streamchat-agent-1.0.1/src/StreamChatAgent.py` & `streamchat-agent-1.0.2/src/StreamChatAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     self.__post_filter_cb = params.post_filter_cb
     self.__item_queue = queue.Queue(params.max_queue_size)
     self.__interval_sec = params.interval_sec
     self.__keeping_connection = False
 
     self.__chat = pytchat.create(video_id=params.video_id)
 
-    self.__my_put_thread = threading.Thread(target=self.__put_items)
-    self.__my_get_thread = threading.Thread(target=self.__get_items)
+    self.__my_put_thread = threading.Thread(target=self.__put_items, daemon=True)
+    self.__my_get_thread = threading.Thread(target=self.__get_items, daemon=True)
 
     super(StreamChatAgent, self).__init__(daemon=True)
 
   def connect(self):
     self.start()
     self.join()
```

### Comparing `streamchat-agent-1.0.1/src/streamchat_agent.egg-info/PKG-INFO` & `streamchat-agent-1.0.2/src/streamchat_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamchat-agent
-Version: 1.0.1
+Version: 1.0.2
 Summary: Get YouTube chat comments with minimum time lag
 Home-page: https://github.com/GeneralYadoc/StreamChatAgent
 Author: General Yadoc
 Author-email: 133023047+GeneralYadoc@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

