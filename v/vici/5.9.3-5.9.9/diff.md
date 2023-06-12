# Comparing `tmp/vici-5.9.3.tar.gz` & `tmp/vici-5.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vici-5.9.3.tar", last modified: Thu Sep  9 10:26:12 2021, max compression
+gzip compressed data, was "vici-5.9.9.tar", last modified: Tue Jan  3 12:53:44 2023, max compression
```

## Comparing `vici-5.9.3.tar` & `vici-5.9.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 tbrunner  (1000) tbrunner  (1000)        0 2021-09-09 10:26:12.133778 vici-5.9.3/
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     1125 2021-08-27 12:06:38.000000 vici-5.9.3/LICENSE
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)       79 2021-08-27 12:06:38.000000 vici-5.9.3/MANIFEST.in
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     1842 2021-09-09 10:26:12.133778 vici-5.9.3/PKG-INFO
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)      782 2021-08-27 12:06:38.000000 vici-5.9.3/README.rst
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)       38 2021-09-09 10:26:12.133778 vici-5.9.3/setup.cfg
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     1067 2021-09-09 10:26:11.000000 vici-5.9.3/setup.py
-drwxrwxr-x   0 tbrunner  (1000) tbrunner  (1000)        0 2021-09-09 10:26:12.129683 vici-5.9.3/test/
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)        0 2021-08-27 12:06:38.000000 vici-5.9.3/test/__init__.py
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     5787 2021-08-27 12:06:38.000000 vici-5.9.3/test/test_protocol.py
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)      228 2021-09-08 09:27:14.000000 vici-5.9.3/tox.ini
-drwxrwxr-x   0 tbrunner  (1000) tbrunner  (1000)        0 2021-09-09 10:26:12.133778 vici-5.9.3/vici/
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)       29 2021-08-27 12:06:38.000000 vici-5.9.3/vici/__init__.py
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)    10549 2021-08-27 12:06:38.000000 vici-5.9.3/vici/command_wrappers.py
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)      305 2021-08-27 12:06:38.000000 vici-5.9.3/vici/compat.py
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)      402 2021-08-27 12:06:38.000000 vici-5.9.3/vici/exception.py
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     7067 2021-08-27 12:06:38.000000 vici-5.9.3/vici/protocol.py
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     6058 2021-08-27 12:06:38.000000 vici-5.9.3/vici/session.py
-drwxrwxr-x   0 tbrunner  (1000) tbrunner  (1000)        0 2021-09-09 10:26:12.133778 vici-5.9.3/vici.egg-info/
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     1842 2021-09-09 10:26:12.000000 vici-5.9.3/vici.egg-info/PKG-INFO
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)      306 2021-09-09 10:26:12.000000 vici-5.9.3/vici.egg-info/SOURCES.txt
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)        1 2021-09-09 10:26:12.000000 vici-5.9.3/vici.egg-info/dependency_links.txt
--rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)        5 2021-09-09 10:26:12.000000 vici-5.9.3/vici.egg-info/top_level.txt
+drwxrwxr-x   0 tbrunner  (1000) tbrunner  (1000)        0 2023-01-03 12:53:44.304940 vici-5.9.9/
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     1125 2022-09-12 15:33:32.000000 vici-5.9.9/LICENSE
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)       79 2022-10-12 14:32:15.000000 vici-5.9.9/MANIFEST.in
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     1891 2023-01-03 12:53:44.304940 vici-5.9.9/PKG-INFO
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)      782 2022-09-12 15:33:32.000000 vici-5.9.9/README.rst
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)       38 2023-01-03 12:53:44.304940 vici-5.9.9/setup.cfg
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     1115 2023-01-03 12:53:44.000000 vici-5.9.9/setup.py
+drwxrwxr-x   0 tbrunner  (1000) tbrunner  (1000)        0 2023-01-03 12:53:44.304940 vici-5.9.9/test/
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)        0 2022-10-12 14:32:15.000000 vici-5.9.9/test/__init__.py
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     6426 2022-12-22 10:10:30.000000 vici-5.9.9/test/test_protocol.py
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     3164 2022-12-22 10:10:30.000000 vici-5.9.9/test/test_session.py
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)      186 2022-12-22 10:10:30.000000 vici-5.9.9/tox.ini
+drwxrwxr-x   0 tbrunner  (1000) tbrunner  (1000)        0 2023-01-03 12:53:44.304940 vici-5.9.9/vici/
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)       29 2021-10-05 08:54:20.000000 vici-5.9.9/vici/__init__.py
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)    10549 2022-10-12 14:32:15.000000 vici-5.9.9/vici/command_wrappers.py
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)      402 2022-10-12 14:32:15.000000 vici-5.9.9/vici/exception.py
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     7178 2022-12-22 10:10:30.000000 vici-5.9.9/vici/protocol.py
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     6764 2022-12-22 10:10:30.000000 vici-5.9.9/vici/session.py
+drwxrwxr-x   0 tbrunner  (1000) tbrunner  (1000)        0 2023-01-03 12:53:44.304940 vici-5.9.9/vici.egg-info/
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)     1891 2023-01-03 12:53:44.000000 vici-5.9.9/vici.egg-info/PKG-INFO
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)      312 2023-01-03 12:53:44.000000 vici-5.9.9/vici.egg-info/SOURCES.txt
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)        1 2023-01-03 12:53:44.000000 vici-5.9.9/vici.egg-info/dependency_links.txt
+-rw-rw-r--   0 tbrunner  (1000) tbrunner  (1000)        5 2023-01-03 12:53:44.000000 vici-5.9.9/vici.egg-info/top_level.txt
```

### Comparing `vici-5.9.3/LICENSE` & `vici-5.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vici-5.9.3/PKG-INFO` & `vici-5.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: vici
-Version: 5.9.3
+Version: 5.9.9
 Summary: Native Python interface for strongSwan's VICI protocol
-Home-page: https://wiki.strongswan.org/projects/strongswan/wiki/Vici
+Home-page: https://docs.strongswan.org/docs/5.9/plugins/vici.html
 Author: strongSwan Project
 Author-email: info@strongswan.org
 License: MIT
 Description: About
         -----
         
         The strongSwan VICI protocol allows external applications to monitor, configure
@@ -33,14 +33,15 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `vici-5.9.3/README.rst` & `vici-5.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `vici-5.9.3/setup.py` & `vici-5.9.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     long_description = file.read()
 
 setup(
     name="vici",
-    version="5.9.3",
+    version="5.9.9",
     description="Native Python interface for strongSwan's VICI protocol",
     long_description=long_description,
     author="strongSwan Project",
     author_email="info@strongswan.org",
-    url="https://wiki.strongswan.org/projects/strongswan/wiki/Vici",
+    url="https://docs.strongswan.org/docs/5.9/plugins/vici.html",
     license="MIT",
     packages=["vici"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Security",
         "Topic :: Software Development :: Libraries",
     ]
 )
```

### Comparing `vici-5.9.3/test/test_protocol.py` & `vici-5.9.9/test/test_protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
+import socket
 
-from vici.protocol import Packet, Message, FiniteStream
+from vici.protocol import Packet, Message, FiniteStream, Transport
 from vici.exception import DeserializationException
 
 
 class TestPacket(object):
     # test data definitions for outgoing packet types
     cmd_request = b"\x00\x0c" b"command_type"
     cmd_request_msg = b"\x00\x07" b"command" b"payload"
@@ -138,7 +139,30 @@
         deserialized_message = Message.deserialize(serialized_message)
 
         # ensure that list items and key values remain as undecoded bytes
         deserialized_section = deserialized_message["section1"]
         assert deserialized_message["key1"] == b"value1"
         assert deserialized_section["sub-section"]["key2"] == b"value2"
         assert deserialized_section["list1"] == [b"item1", b"item2"]
+
+
+class TestTransport(object):
+
+    def interconnect(self):
+        c, s = socket.socketpair(socket.AF_UNIX)
+        return Transport(c), Transport(s)
+
+    def test_sendrecv(self):
+        c, s = self.interconnect()
+        c.send(b"foo")
+        assert s.receive() == b"foo"
+        s.send(b"foobarbaz")
+        s.send(b"")
+        assert c.receive() == b"foobarbaz"
+        assert c.receive() == b""
+
+    def test_timeout(self):
+        c, s = self.interconnect()
+        c.send(b"foo")
+        assert s.receive(timeout=1) == b"foo"
+        with pytest.raises(socket.timeout):
+            s.receive(timeout=0.1)
```

### Comparing `vici-5.9.3/vici/command_wrappers.py` & `vici-5.9.9/vici/command_wrappers.py`

 * *Files identical despite different names*

### Comparing `vici-5.9.3/vici/protocol.py` & `vici-5.9.9/vici/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import io
 import socket
 import struct
 
 from collections import namedtuple
 from collections import OrderedDict
 
-from .compat import iteritems
 from .exception import DeserializationException
 
 
 class Transport(object):
     HEADER_LENGTH = 4
     MAX_SEGMENT = 512 * 1024
 
     def __init__(self, sock):
         self.socket = sock
 
     def send(self, packet):
         self.socket.sendall(struct.pack("!I", len(packet)) + packet)
 
-    def receive(self):
-        raw_length = self._recvall(self.HEADER_LENGTH)
+    def receive(self, timeout=None):
+        raw_length = self._recvall(self.HEADER_LENGTH, timeout)
         length, = struct.unpack("!I", raw_length)
         payload = self._recvall(length)
         return payload
 
     def close(self):
         self.socket.shutdown(socket.SHUT_RDWR)
         self.socket.close()
 
-    def _recvall(self, count):
+    def _recvall(self, count, timeout=None):
         """Ensure to read count bytes from the socket"""
         data = b""
+        if count > 0:
+            self.socket.settimeout(timeout)
         while len(data) < count:
             buf = self.socket.recv(count - len(data))
+            self.socket.settimeout(None)
             if not buf:
                 raise socket.error('Connection closed')
             data += buf
         return data
 
 
 class Packet(object):
@@ -117,15 +119,15 @@
             segment = bytes()
             for item in lst:
                 segment += struct.pack("!B", cls.LIST_ITEM) + encode_blob(item)
             return segment
 
         def serialize_dict(d):
             segment = bytes()
-            for key, value in iteritems(d):
+            for key, value in d.items():
                 if isinstance(value, dict):
                     segment += (
                         encode_named_type(cls.SECTION_START, key)
                         + serialize_dict(value)
                         + struct.pack("!B", cls.SECTION_END)
                     )
                 elif isinstance(value, list):
```

### Comparing `vici-5.9.3/vici/session.py` & `vici-5.9.9/vici/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,17 @@
         else:
             packet = Packet.unregister_event(event_type)
         response = self._communicate(packet)
         if response.response_type == Packet.EVENT_UNKNOWN:
             raise EventUnknownException(
                 "Unknown event type '{event}'".format(event=event_type)
             )
-        elif response.response_type != Packet.EVENT_CONFIRM:
+        while response.response_type == Packet.EVENT:
+            response = Packet.parse(self.transport.receive())
+        if response.response_type != Packet.EVENT_CONFIRM:
             raise SessionException(
                 "Unexpected response type {type}, "
                 "expected '{confirm}' (EVENT_CONFIRM)".format(
                     type=response.response_type,
                     confirm=Packet.EVENT_CONFIRM,
                 )
             )
@@ -135,28 +137,40 @@
             if command_response["success"] != b"yes":
                 raise CommandException(
                     "Command failed: {errmsg}".format(
                         errmsg=command_response["errmsg"].decode("UTF-8")
                     )
                 )
 
-    def listen(self, event_types):
+    def listen(self, event_types, timeout=None):
         """Register and listen for the given events.
 
+        If a timeout is given, the generator produces a (None, None) tuple
+        if no event has been received for that time. This allows the caller
+        to either abort by breaking from the generator, or perform periodic
+        tasks while staying registered within listen(), and then continue
+        waiting for more events.
+
         :param event_types: event types to register
         :type event_types: list
+        :param timeout: timeout to wait for events, in fractions of a second
+        :type timeout: float
         :return: generator for streamed event responses as (event_type, dict)
         :rtype: generator
         """
         for event_type in event_types:
             self._register_unregister(event_type, True)
 
         try:
             while True:
-                response = Packet.parse(self.transport.receive())
+                try:
+                    response = Packet.parse(self.transport.receive(timeout))
+                except socket.timeout:
+                    yield None, None
+                    continue
                 if response.response_type == Packet.EVENT:
                     try:
                         msg = Message.deserialize(response.payload)
                         yield response.event_type, msg
                     except GeneratorExit:
                         break
```

### Comparing `vici-5.9.3/vici.egg-info/PKG-INFO` & `vici-5.9.9/vici.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: vici
-Version: 5.9.3
+Version: 5.9.9
 Summary: Native Python interface for strongSwan's VICI protocol
-Home-page: https://wiki.strongswan.org/projects/strongswan/wiki/Vici
+Home-page: https://docs.strongswan.org/docs/5.9/plugins/vici.html
 Author: strongSwan Project
 Author-email: info@strongswan.org
 License: MIT
 Description: About
         -----
         
         The strongSwan VICI protocol allows external applications to monitor, configure
@@ -33,14 +33,15 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
```

