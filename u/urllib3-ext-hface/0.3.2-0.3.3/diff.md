# Comparing `tmp/urllib3_ext_hface-0.3.2.tar.gz` & `tmp/urllib3_ext_hface-0.3.3.tar.gz`

## Comparing `urllib3_ext_hface-0.3.2.tar` & `urllib3_ext_hface-0.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/CHANGELOG.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/dev-requirements.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/__init__.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_configuration.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_error_codes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_typing.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/py.typed
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/events/__init__.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/events/_events.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/__init__.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/_factories.py
--rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/_protocols.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/_helpers.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http3/_aioquic.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/tests/helpers.py
--rw-r--r--   0        0        0    19739 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/tests/test_http1.py
--rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/tests/test_http2.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/tests/test_integration.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/AUTHORS
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/NOTICE
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/README.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/CHANGELOG.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/dev-requirements.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/__init__.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_error_codes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_typing.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/py.typed
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/events/__init__.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/events/_events.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/__init__.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/_factories.py
+-rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/_helpers.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http3/_aioquic.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/tests/helpers.py
+-rw-r--r--   0        0        0    19739 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/tests/test_http1.py
+-rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/tests/test_http2.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/tests/test_integration.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/AUTHORS
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/NOTICE
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/README.rst
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.3/PKG-INFO
```

### Comparing `urllib3_ext_hface-0.3.2/CHANGELOG.rst` & `urllib3_ext_hface-0.3.3/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+v0.3.3 (2023-06-12)
+-------------------
+
+* Push the ``HandshakeCompleted`` event for the ``HTTP2ProtocolHyperImpl``.
+
 v0.3.2 (2023-06-12)
 -------------------
 
-* Properly forward ConnectionTerminated event from the QUIC layer in `HTTP3ProtocolAioQuicImpl`.
+* Properly forward ConnectionTerminated event from the QUIC layer in ``HTTP3ProtocolAioQuicImpl``.
 
 v0.3.1 (2023-06-10)
 -------------------
 
 * Allow passing extra config parameter for HTTP2Protocol through the factory.
 * Remove server-side code in the primary (h11) HTTP1Protocol.
```

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/__init__.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_configuration.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_error_codes.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_typing.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/events/__init__.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/events/_events.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/__init__.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/_factories.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/_protocols.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/__init__.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/_h11.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/_h11.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/_helpers.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http1/_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http2/__init__.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http2/_h2.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http2/_h2.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from ..._typing import HeadersType
 from ...events import (
     ConnectionTerminated,
     DataReceived,
     Event,
     GoawayReceived,
+    HandshakeCompleted,
     HeadersReceived,
     StreamResetReceived,
     StreamResetSent,
 )
 from .._protocols import HTTP2Protocol
 
 
@@ -123,14 +124,16 @@
                 # ConnectionTerminated from h2 means that GOAWAY was received.
                 # A server can send GOAWAY for graceful shutdown, where clients
                 # do not open new streams, but inflight requests can be completed.
                 #
                 # Saying "connection was terminated" can be confusing,
                 # so we emit an event called "GoawayReceived".
                 yield GoawayReceived(e.last_stream_id, e.error_code)
+            elif isinstance(e, h2.events.SettingsAcknowledged):
+                yield HandshakeCompleted(alpn_protocol="h2")
 
     def connection_lost(self) -> None:
         self._connection_terminated()
 
     def eof_received(self) -> None:
         self._connection_terminated()
```

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http3/__init__.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http3/_aioquic.py` & `urllib3_ext_hface-0.3.3/src/urllib3_ext_hface/protocols/http3/_aioquic.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/tests/helpers.py` & `urllib3_ext_hface-0.3.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/tests/test_http1.py` & `urllib3_ext_hface-0.3.3/tests/test_http1.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/tests/test_http2.py` & `urllib3_ext_hface-0.3.3/tests/test_http2.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/tests/test_integration.py` & `urllib3_ext_hface-0.3.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/LICENSE` & `urllib3_ext_hface-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/NOTICE` & `urllib3_ext_hface-0.3.3/NOTICE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/README.rst` & `urllib3_ext_hface-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/pyproject.toml` & `urllib3_ext_hface-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.2/PKG-INFO` & `urllib3_ext_hface-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3-ext-hface
-Version: 0.3.2
+Version: 0.3.3
 Summary: urllib3 extension to support HTTP/1.1, HTTP/2 and HTTP/3 independently of Python httplib
 Project-URL: Changelog, https://github.com/Ousret/urllib3-ext-hface/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/Ousret/urllib3-ext-hface
 Project-URL: Issue tracker, https://github.com/Ousret/urllib3-ext-hface/issues
 Author-email: Miloslav Pojman <mpojman@akamai.com>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
```

