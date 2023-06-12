# Comparing `tmp/SensorsAnalyticsSDK-1.7.1.tar.gz` & `tmp/SensorsAnalyticsSDK-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SensorsAnalyticsSDK-1.7.1.tar", last modified: Fri Jul  7 17:41:59 2017, max compression
+gzip compressed data, was "dist/SensorsAnalyticsSDK-1.7.5.tar", last modified: Tue Mar 13 14:34:12 2018, max compression
```

## Comparing `SensorsAnalyticsSDK-1.7.1.tar` & `SensorsAnalyticsSDK-1.7.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
-drwxr-xr-x   0 zouyuhan   (501) staff       (20)        0 2017-07-07 17:41:58.000000 SensorsAnalyticsSDK-1.7.1/
--rw-r--r--   0 zouyuhan   (501) staff       (20)      658 2017-07-07 17:41:58.000000 SensorsAnalyticsSDK-1.7.1/PKG-INFO
--rw-r--r--   0 zouyuhan   (501) staff       (20)      273 2016-03-14 15:50:55.000000 SensorsAnalyticsSDK-1.7.1/README.txt
-drwxr-xr-x   0 zouyuhan   (501) staff       (20)        0 2017-07-07 17:41:58.000000 SensorsAnalyticsSDK-1.7.1/sensorsanalytics/
--rw-r--r--   0 zouyuhan   (501) staff       (20)       19 2016-08-16 13:36:47.000000 SensorsAnalyticsSDK-1.7.1/sensorsanalytics/__init__.py
--rw-r--r--   0 zouyuhan   (501) staff       (20)    25728 2017-07-07 10:35:33.000000 SensorsAnalyticsSDK-1.7.1/sensorsanalytics/sdk.py
--rw-r--r--   0 zouyuhan   (501) staff       (20)      959 2017-07-07 08:15:38.000000 SensorsAnalyticsSDK-1.7.1/sensorsanalytics/test.py
--rw-r--r--   0 zouyuhan   (501) staff       (20)     8602 2017-06-19 09:26:54.000000 SensorsAnalyticsSDK-1.7.1/sensorsanalytics/test_sdk.py
--rw-r--r--   0 zouyuhan   (501) staff       (20)      385 2017-07-07 10:35:39.000000 SensorsAnalyticsSDK-1.7.1/setup.py
+drwxr-xr-x   0 zouyuhan   (501) staff       (20)        0 2018-03-13 14:34:12.000000 SensorsAnalyticsSDK-1.7.5/
+-rw-r--r--   0 zouyuhan   (501) staff       (20)      658 2018-03-13 14:34:12.000000 SensorsAnalyticsSDK-1.7.5/PKG-INFO
+-rw-r--r--   0 zouyuhan   (501) staff       (20)      273 2018-03-13 14:15:29.000000 SensorsAnalyticsSDK-1.7.5/README.txt
+drwxr-xr-x   0 zouyuhan   (501) staff       (20)        0 2018-03-13 14:34:12.000000 SensorsAnalyticsSDK-1.7.5/sensorsanalytics/
+-rw-r--r--   0 zouyuhan   (501) staff       (20)       19 2018-03-13 14:15:29.000000 SensorsAnalyticsSDK-1.7.5/sensorsanalytics/__init__.py
+-rw-r--r--   0 zouyuhan   (501) staff       (20)    30097 2018-03-13 14:15:29.000000 SensorsAnalyticsSDK-1.7.5/sensorsanalytics/sdk.py
+-rw-r--r--   0 zouyuhan   (501) staff       (20)     8602 2018-03-13 14:15:29.000000 SensorsAnalyticsSDK-1.7.5/sensorsanalytics/test_sdk.py
+-rw-r--r--   0 zouyuhan   (501) staff       (20)      385 2018-03-13 14:15:29.000000 SensorsAnalyticsSDK-1.7.5/setup.py
```

### Comparing `SensorsAnalyticsSDK-1.7.1/PKG-INFO` & `SensorsAnalyticsSDK-1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: SensorsAnalyticsSDK
-Version: 1.7.1
+Version: 1.7.5
 Summary: This is the official Python SDK for Sensors Analytics.
 Home-page: http://www.sensorsdata.cn
 Author: Yuhan ZOU
 Author-email: zouyuhan@sensorsdata.cn
 License: LICENSE.txt
 Description: =====================
         Sensors Analytics SDK
```

### Comparing `SensorsAnalyticsSDK-1.7.1/sensorsanalytics/sdk.py` & `SensorsAnalyticsSDK-1.7.5/sensorsanalytics/sdk.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # coding=utf-8
 
 from __future__ import unicode_literals
 import base64
 import datetime
-import time
-import json
 import gzip
+import json
+import logging
+import logging.handlers
+import os
 import re
 import sys
 import threading
+import time
 import traceback
-import logging
-import logging.handlers
 
 try:
     from urllib.parse import urlparse
     import queue
     import urllib.parse as urllib
     import urllib.request as urllib2
 except ImportError:
     from urlparse import urlparse
     import Queue as queue
     import urllib2
     import urllib
 
-SDK_VERSION = '1.7.1'
+SDK_VERSION = '1.7.5'
 
 try:
     isinstance("", basestring)
     def is_str(s):
         return isinstance(s, basestring)
 except NameError:
     def is_str(s):
@@ -56,21 +57,91 @@
 class SensorsAnalyticsNetworkException(SensorsAnalyticsException):
     """
     在因为网络或者不可预知的问题导致数据无法发送时，SDK会抛出此异常，用户应当捕获并处理。
     """
     pass
 
 
+class SensorsAnalyticsFileLockException(SensorsAnalyticsException):
+    """
+    当 ConcurrentLoggingConsumer 文件锁异常时，SDK 会抛出此异常，用户应当捕获并记录错误日志。
+    """
+    pass
+
+
 class SensorsAnalyticsDebugException(Exception):
     """
     Debug模式专用的异常
     """
     pass
 
 
+if os.name == 'nt':  # pragma: no cover
+    import msvcrt
+
+    def lock(file_):
+        try:
+            savepos = file_.tell()
+           
+            file_.seek(0)
+
+            try:
+                msvcrt.locking(file_.fileno(), msvcrt.LK_LOCK, 1)
+            except IOError as e:
+                raise SensorsAnalyticsFileLockException(e) 
+            finally:
+                if savepos:
+                    file_.seek(savepos)
+        except IOError as e:
+            raise SensorsAnalyticsFileLockException(e) 
+
+    def unlock(file_):
+        try:
+            savepos = file_.tell()
+            if savepos:
+                file_.seek(0)
+            
+            try:
+                msvcrt.locking(file_.fileno(), msvcrt.LK_UNLCK, 1)
+            except IOError as e:
+                raise SensorsAnalyticsFileLockException(e) 
+            finally:
+                if savepos:
+                    file_.seek(savepos)
+        except IOError as e:
+            raise SensorsAnalyticsFileLockException(e) 
+
+elif os.name == 'posix':  # pragma: no cover
+    import fcntl
+
+    def lock(file_):
+        try:
+            fcntl.flock(file_.fileno(), fcntl.LOCK_EX)
+        except IOError as e:
+            raise SensorsAnalyticsFileLockException(e) 
+
+    def unlock(file_):
+        fcntl.flock(file_.fileno(), fcntl.LOCK_UN)
+
+else:
+    raise SensorsAnalyticsFileLockException("SensorsAnalytics SDK is defined for NT and POSIX system.") 
+
+
+class SAFileLock(object):
+    
+    def __init__(self, file_handler):
+        self._file_handler = file_handler
+
+    def __enter__(self):
+        lock(self._file_handler)
+        return self
+
+    def __exit__(self, t, v, tb):
+        unlock(self._file_handler)
+
 class SensorsAnalytics(object):
     """
     使用一个 SensorsAnalytics 的实例来进行数据发送。
     """
 
     NAME_PATTERN = re.compile(r"^((?!^distinct_id$|^original_id$|^time$|^properties$|^id$|^first_id$|^second_id$|^users$|^events$|^event$|^user_id$|^date$|^datetime$)[a-zA-Z_$][a-zA-Z\d_$]{0,99})$", re.I)
 
@@ -569,15 +640,15 @@
             self.need_flush.set()
 
     def flush(self):
         self.need_flush.set()
 
     def sync_flush(self, throw_exception=True):
         """
-        执行一次同步发送。 throw_exception 表示在发送失败时是否向外抛出异常。
+        执行一次同步发送。 throw_exception 表示在发送失败时是否向外抛出异常
         """
         flush_success = False
 
         if len(self._flush_buffer) == 0:
             for i in range(self._max_batch_size):
                 if not self._queue.empty():
                     self._flush_buffer.append(self._queue.get_nowait())
@@ -720,7 +791,93 @@
         self.logger.info(msg)
 
     def flush(self):
         self.logger.handlers[0].flush()
 
     def close(self):
         self.logger.handlers[0].close()
+
+class ConcurrentLoggingConsumer(object):
+    """
+    将数据输出到指定路径，并按天切割，支持多进程并行输出到同一个文件名
+    """
+
+    class ConcurrentFileWriter(object):
+
+        def __init__(self, filename):
+            self._filename = filename
+            self._file = open(filename, 'a')
+
+        def close(self):
+            self._file.close()
+
+        def isValid(self, filename):
+            return self._filename == filename 
+
+        def write(self, messages):
+            with SAFileLock(self._file):
+                for message in messages:
+                    self._file.write(message)
+                    self._file.write('\n')
+                self._file.flush()
+
+    @classmethod
+    def construct_filename(cls, prefix):
+        return prefix + '.' + datetime.datetime.now().strftime('%Y-%m-%d') 
+
+    def __init__(self, prefix, bufferSize=8192):
+        self._prefix = prefix
+
+        self._buffer = []
+        self._bufferSize = bufferSize
+
+        self._mutex = queue.Queue()
+        self._mutex.put(1)
+
+        filename = ConcurrentLoggingConsumer.construct_filename(self._prefix)
+        self._writer = ConcurrentLoggingConsumer.ConcurrentFileWriter(filename)
+
+    def send(self, msg):
+        messages = None
+
+        self._mutex.get(block=True, timeout=None)
+
+        self._buffer.append(msg)
+
+        if len(self._buffer) > self._bufferSize:
+            messages = self._buffer
+
+            filename = ConcurrentLoggingConsumer.construct_filename(self._prefix)    
+            if not self._writer.isValid(filename):
+                self._writer.close()
+                self._writer = ConcurrentLoggingConsumer.ConcurrentFileWriter(filename)
+
+            self._buffer = []
+
+        self._mutex.put(1)
+   
+        if messages:
+            self._writer.write(messages)
+
+    def flush(self):
+        messages = None
+
+        self._mutex.get(block=True, timeout=None)
+
+        if len(self._buffer) > 0:
+            messages = self._buffer
+
+            filename = ConcurrentLoggingConsumer.construct_filename(self._prefix)    
+            if not self._writer.isValid(filename):
+                self._writer.close()
+                self._writer = ConcurrentLoggingConsumer.ConcurrentFileWriter(filename)
+
+            self._buffer = []
+
+        self._mutex.put(1)
+   
+        if messages:
+            self._writer.write(messages)
+
+    def close(self):
+        self.flush()
+        self._writer.close()
```

### Comparing `SensorsAnalyticsSDK-1.7.1/sensorsanalytics/test_sdk.py` & `SensorsAnalyticsSDK-1.7.5/sensorsanalytics/test_sdk.py`

 * *Files identical despite different names*

