# Comparing `tmp/renats-0.2.2a0.tar.gz` & `tmp/renats-0.2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renats-0.2.2a0.tar", max compression
+gzip compressed data, was "renats-0.2.2a1.tar", max compression
```

## Comparing `renats-0.2.2a0.tar` & `renats-0.2.2a1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1632 2023-06-12 13:52:41.717275 renats-0.2.2a0/README.md
--rw-r--r--   0        0        0      402 2023-06-12 13:52:41.717275 renats-0.2.2a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/__init__.py
--rw-r--r--   0        0        0       60 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/__init__.py
--rw-r--r--   0        0        0      203 2023-06-09 15:07:54.484606 renats-0.2.2a0/renats/client/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4428 2023-06-12 10:50:01.221016 renats-0.2.2a0/renats/client/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0      583 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/client/__pycache__/message.cpython-310.pyc
--rw-r--r--   0        0        0     1087 2023-06-12 10:50:01.229016 renats-0.2.2a0/renats/client/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0        0        0     1355 2023-06-12 10:56:15.311568 renats-0.2.2a0/renats/client/__pycache__/subscription.cpython-310.pyc
--rw-r--r--   0        0        0      809 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/base.py
--rw-r--r--   0        0        0     6325 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/client.py
--rw-r--r--   0        0        0      647 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/handler.py
--rw-r--r--   0        0        0      264 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/message.py
--rw-r--r--   0        0        0      937 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/parser.py
--rw-r--r--   0        0        0     1654 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/subscription.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/connection/__init__.py
--rw-r--r--   0        0        0      166 2023-06-09 14:42:32.158897 renats-0.2.2a0/renats/connection/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1693 2023-06-12 10:50:01.229016 renats-0.2.2a0/renats/connection/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2003 2023-06-12 10:50:01.233016 renats-0.2.2a0/renats/connection/__pycache__/tcp.cpython-310.pyc
--rw-r--r--   0        0        0      951 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/connection/base.py
--rw-r--r--   0        0        0       64 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/connection/connection.py
--rw-r--r--   0        0        0     1099 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/connection/tcp.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/protocol/__init__.py
--rw-r--r--   0        0        0      164 2023-06-09 14:42:32.158897 renats-0.2.2a0/renats/protocol/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1378 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/protocol/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0      925 2023-06-09 14:42:32.158897 renats-0.2.2a0/renats/protocol/__pycache__/protocol.cpython-310.pyc
--rw-r--r--   0        0        0     2335 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/protocol/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0      530 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/protocol/messages/__init__.py
--rw-r--r--   0        0        0      173 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/protocol/messages/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      702 2023-06-09 14:57:46.434759 renats-0.2.2a0/renats/protocol/messages/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      863 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/protocol/messages/__pycache__/msg.cpython-310.pyc
--rw-r--r--   0        0        0     1926 2023-06-09 15:04:32.367916 renats-0.2.2a0/renats/protocol/messages/__pycache__/pub.cpython-310.pyc
--rw-r--r--   0        0        0     2651 2023-06-09 15:41:51.790249 renats-0.2.2a0/renats/protocol/messages/__pycache__/service.cpython-310.pyc
--rw-r--r--   0        0        0     1711 2023-06-09 15:07:48.276584 renats-0.2.2a0/renats/protocol/messages/__pycache__/sub.cpython-310.pyc
--rw-r--r--   0        0        0      295 2023-06-09 14:57:08.722653 renats-0.2.2a0/renats/protocol/messages/base.py
--rw-r--r--   0        0        0      390 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/messages/msg.py
--rw-r--r--   0        0        0     1574 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/messages/pub.py
--rw-r--r--   0        0        0     1749 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/messages/service.py
--rw-r--r--   0        0        0     1167 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/messages/sub.py
--rw-r--r--   0        0        0      668 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/protocol.py
--rw-r--r--   0        0        0     1591 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/utils.py
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 renats-0.2.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1632 2023-06-12 13:52:41.717275 renats-0.2.2a1/README.md
+-rw-r--r--   0        0        0      404 2023-06-12 13:58:33.138625 renats-0.2.2a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-09 15:07:54.484606 renats-0.2.2a1/renats/client/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4428 2023-06-12 10:50:01.221016 renats-0.2.2a1/renats/client/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0      583 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/client/__pycache__/message.cpython-310.pyc
+-rw-r--r--   0        0        0     1087 2023-06-12 10:50:01.229016 renats-0.2.2a1/renats/client/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     1355 2023-06-12 10:56:15.311568 renats-0.2.2a1/renats/client/__pycache__/subscription.cpython-310.pyc
+-rw-r--r--   0        0        0      809 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/base.py
+-rw-r--r--   0        0        0     6389 2023-06-12 13:58:33.138625 renats-0.2.2a1/renats/client/client.py
+-rw-r--r--   0        0        0      647 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/handler.py
+-rw-r--r--   0        0        0      264 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/message.py
+-rw-r--r--   0        0        0      937 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/parser.py
+-rw-r--r--   0        0        0     1654 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/client/subscription.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/connection/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-09 14:42:32.158897 renats-0.2.2a1/renats/connection/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1693 2023-06-12 10:50:01.229016 renats-0.2.2a1/renats/connection/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2003 2023-06-12 10:50:01.233016 renats-0.2.2a1/renats/connection/__pycache__/tcp.cpython-310.pyc
+-rw-r--r--   0        0        0      951 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/connection/base.py
+-rw-r--r--   0        0        0       64 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/connection/connection.py
+-rw-r--r--   0        0        0     1099 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/connection/tcp.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/protocol/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-09 14:42:32.158897 renats-0.2.2a1/renats/protocol/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1378 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/protocol/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0      925 2023-06-09 14:42:32.158897 renats-0.2.2a1/renats/protocol/__pycache__/protocol.cpython-310.pyc
+-rw-r--r--   0        0        0     2335 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/protocol/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      530 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a1/renats/protocol/messages/__init__.py
+-rw-r--r--   0        0        0      173 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/protocol/messages/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      702 2023-06-09 14:57:46.434759 renats-0.2.2a1/renats/protocol/messages/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      863 2023-06-09 14:45:21.475619 renats-0.2.2a1/renats/protocol/messages/__pycache__/msg.cpython-310.pyc
+-rw-r--r--   0        0        0     1926 2023-06-09 15:04:32.367916 renats-0.2.2a1/renats/protocol/messages/__pycache__/pub.cpython-310.pyc
+-rw-r--r--   0        0        0     2651 2023-06-09 15:41:51.790249 renats-0.2.2a1/renats/protocol/messages/__pycache__/service.cpython-310.pyc
+-rw-r--r--   0        0        0     1711 2023-06-09 15:07:48.276584 renats-0.2.2a1/renats/protocol/messages/__pycache__/sub.cpython-310.pyc
+-rw-r--r--   0        0        0      295 2023-06-09 14:57:08.722653 renats-0.2.2a1/renats/protocol/messages/base.py
+-rw-r--r--   0        0        0      390 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/messages/msg.py
+-rw-r--r--   0        0        0     1574 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/messages/pub.py
+-rw-r--r--   0        0        0     1749 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/messages/service.py
+-rw-r--r--   0        0        0     1167 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/messages/sub.py
+-rw-r--r--   0        0        0      668 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/protocol.py
+-rw-r--r--   0        0        0     1591 2023-06-12 13:52:41.717275 renats-0.2.2a1/renats/protocol/utils.py
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 renats-0.2.2a1/PKG-INFO
```

### Comparing `renats-0.2.2a0/README.md` & `renats-0.2.2a1/README.md`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/client/__pycache__/client.cpython-310.pyc` & `renats-0.2.2a1/renats/client/__pycache__/client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/client/__pycache__/message.cpython-310.pyc` & `renats-0.2.2a1/renats/client/__pycache__/message.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/client/__pycache__/parser.cpython-310.pyc` & `renats-0.2.2a1/renats/client/__pycache__/parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/client/__pycache__/subscription.cpython-310.pyc` & `renats-0.2.2a1/renats/client/__pycache__/subscription.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/client/base.py` & `renats-0.2.2a1/renats/client/base.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/client/client.py` & `renats-0.2.2a1/renats/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 from ..protocol.messages.service import InfoProtocolMessage, ConnectProtocolMessage
 from ..protocol.messages.sub import SubProtocolMessage, UnsubProtocolMessage
 
 DEFAULT_CONNECTION_TIMEOUT: Final[float] = 2
 DEFAULT_INFO_WAITING_TIMEOUT: Final[float] = 2
 
 CLIENT_LANGUAGE: Final[str] = "python3"
-CLIENT_VERSION: Final[str] = "0.2.2-alpha"
+CLIENT_VERSION: Final[str] = "0.2.2-alpha-1"
 
 CLIENT_CONNECTION_VERBOSE: Final[bool] = False
 CLIENT_CONNECTION_PEDANTIC: Final[bool] = True
+CLIENT_SUPPORT_HEADERS: Final[bool] = False
 
 HeadersType = dict[str, str]
 
 
 class NATSClient(NATS):
     def __init__(self):
         self._logger: logging.Logger = logging.getLogger(__name__)
@@ -70,15 +71,15 @@
         await self._connection.send(
             ConnectProtocolMessage(
                 verbose=CLIENT_CONNECTION_VERBOSE,
                 pedantic=CLIENT_CONNECTION_PEDANTIC,
                 tls_required=False,
                 lang=CLIENT_LANGUAGE,
                 version=CLIENT_VERSION,
-                headers=True
+                headers=CLIENT_SUPPORT_HEADERS
             ).dump()
         )
 
     async def _handle_message(self, protocol_message: MsgProtocolMessage | HMsgProtocolMessage):
         # Skip message if its subscription id not registered in subscription manager
         if protocol_message.sid not in self._subscriptions:
             return
```

### Comparing `renats-0.2.2a0/renats/client/handler.py` & `renats-0.2.2a1/renats/client/handler.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/client/parser.py` & `renats-0.2.2a1/renats/client/parser.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/client/subscription.py` & `renats-0.2.2a1/renats/client/subscription.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/connection/__pycache__/base.cpython-310.pyc` & `renats-0.2.2a1/renats/connection/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/connection/__pycache__/tcp.cpython-310.pyc` & `renats-0.2.2a1/renats/connection/__pycache__/tcp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/connection/base.py` & `renats-0.2.2a1/renats/connection/base.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/connection/tcp.py` & `renats-0.2.2a1/renats/connection/tcp.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/__pycache__/exceptions.cpython-310.pyc` & `renats-0.2.2a1/renats/protocol/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/__pycache__/protocol.cpython-310.pyc` & `renats-0.2.2a1/renats/protocol/__pycache__/protocol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/__pycache__/utils.cpython-310.pyc` & `renats-0.2.2a1/renats/protocol/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/exceptions.py` & `renats-0.2.2a1/renats/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/messages/__pycache__/base.cpython-310.pyc` & `renats-0.2.2a1/renats/protocol/messages/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/messages/__pycache__/msg.cpython-310.pyc` & `renats-0.2.2a1/renats/protocol/messages/__pycache__/msg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/messages/__pycache__/pub.cpython-310.pyc` & `renats-0.2.2a1/renats/protocol/messages/__pycache__/pub.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/messages/__pycache__/service.cpython-310.pyc` & `renats-0.2.2a1/renats/protocol/messages/__pycache__/service.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/messages/__pycache__/sub.cpython-310.pyc` & `renats-0.2.2a1/renats/protocol/messages/__pycache__/sub.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/messages/pub.py` & `renats-0.2.2a1/renats/protocol/messages/pub.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/messages/service.py` & `renats-0.2.2a1/renats/protocol/messages/service.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/messages/sub.py` & `renats-0.2.2a1/renats/protocol/messages/sub.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/protocol.py` & `renats-0.2.2a1/renats/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/renats/protocol/utils.py` & `renats-0.2.2a1/renats/protocol/utils.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.2a0/PKG-INFO` & `renats-0.2.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renats
-Version: 0.2.2a0
+Version: 0.2.2a1
 Summary: 
 Author: Respirens
 Author-email: thesergiyprotsanin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

