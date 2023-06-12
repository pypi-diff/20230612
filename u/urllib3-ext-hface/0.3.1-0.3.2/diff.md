# Comparing `tmp/urllib3_ext_hface-0.3.1.tar.gz` & `tmp/urllib3_ext_hface-0.3.2.tar.gz`

## Comparing `urllib3_ext_hface-0.3.1.tar` & `urllib3_ext_hface-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/CHANGELOG.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/dev-requirements.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/__init__.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_configuration.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_error_codes.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_typing.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/py.typed
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/events/__init__.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/events/_events.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/__init__.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/_factories.py
--rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/_protocols.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/_helpers.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http3/_aioquic.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/tests/helpers.py
--rw-r--r--   0        0        0    19739 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/tests/test_http1.py
--rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/tests/test_http2.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/tests/test_integration.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/AUTHORS
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/NOTICE
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/README.rst
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/CHANGELOG.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/dev-requirements.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/__init__.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_configuration.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_error_codes.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_typing.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/py.typed
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/events/__init__.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/events/_events.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/__init__.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/_factories.py
+-rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/_helpers.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http3/_aioquic.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/tests/helpers.py
+-rw-r--r--   0        0        0    19739 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/tests/test_http1.py
+-rw-r--r--   0        0        0    16162 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/tests/test_http2.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/tests/test_integration.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/AUTHORS
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/NOTICE
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/README.rst
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 urllib3_ext_hface-0.3.2/PKG-INFO
```

### Comparing `urllib3_ext_hface-0.3.1/CHANGELOG.rst` & `urllib3_ext_hface-0.3.2/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v0.3.2 (2023-06-12)
+-------------------
+
+* Properly forward ConnectionTerminated event from the QUIC layer in `HTTP3ProtocolAioQuicImpl`.
+
 v0.3.1 (2023-06-10)
 -------------------
 
 * Allow passing extra config parameter for HTTP2Protocol through the factory.
 * Remove server-side code in the primary (h11) HTTP1Protocol.
 
 v0.3.0 (2023-06-03)
```

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/__init__.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_configuration.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_error_codes.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/_typing.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/events/__init__.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/events/_events.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/__init__.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/_factories.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/_protocols.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/__init__.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/_h11.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/_h11.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http1/_helpers.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http1/_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http2/__init__.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http2/_h2.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http2/_h2.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http3/__init__.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/src/urllib3_ext_hface/protocols/http3/_aioquic.py` & `urllib3_ext_hface-0.3.2/src/urllib3_ext_hface/protocols/http3/_aioquic.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,17 @@
         assert self._http is not None
 
         for quic_event in iter(self._quic.next_event, None):
             self._event_buffer += self._map_quic_event(quic_event)
             for h3_event in self._http.handle_event(quic_event):
                 self._event_buffer += self._map_h3_event(h3_event)
 
+        if hasattr(self._quic, "_close_event") and self._quic._close_event is not None:
+            self._event_buffer += self._map_quic_event(self._quic._close_event)
+
     def _map_quic_event(self, quic_event: quic_events.QuicEvent) -> Iterable[Event]:
         if isinstance(quic_event, quic_events.ConnectionIdIssued):
             self._connection_ids.add(quic_event.connection_id)
         elif isinstance(quic_event, quic_events.ConnectionIdRetired):
             try:
                 self._connection_ids.remove(quic_event.connection_id)
             except (
```

### Comparing `urllib3_ext_hface-0.3.1/tests/helpers.py` & `urllib3_ext_hface-0.3.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/tests/test_http1.py` & `urllib3_ext_hface-0.3.2/tests/test_http1.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/tests/test_http2.py` & `urllib3_ext_hface-0.3.2/tests/test_http2.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/tests/test_integration.py` & `urllib3_ext_hface-0.3.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/LICENSE` & `urllib3_ext_hface-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/NOTICE` & `urllib3_ext_hface-0.3.2/NOTICE`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/README.rst` & `urllib3_ext_hface-0.3.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     protocol.bytes_to_send()  # Out to your network I/O implementation
     # ...
     protocol.bytes_received()  # Whatever comes from your network I/O implementation
     # ...
     protocol.next_event()  # Output the next event in order that the state-machine generated
 
 Here ``protocol`` is either of type ``HTTPOverQUICProtocol`` or ``HTTPOverTCPProtocol``, depending
-on the foremost, you will either be on a DRAM (UDP) or STREAM (TCP) socket.
+on the foremost, you will either be on a DGRAM (UDP) or STREAM (TCP) socket.
 
 Find just bellow a somewhat stupid example that can help you get started.
 
 .. code-block:: python
 
     from urllib3_ext_hface import HTTPProtocolFactory, HTTP1Protocol, HTTP2Protocol, HTTP3Protocol
     import ssl
```

### Comparing `urllib3_ext_hface-0.3.1/pyproject.toml` & `urllib3_ext_hface-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `urllib3_ext_hface-0.3.1/PKG-INFO` & `urllib3_ext_hface-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3-ext-hface
-Version: 0.3.1
+Version: 0.3.2
 Summary: urllib3 extension to support HTTP/1.1, HTTP/2 and HTTP/3 independently of Python httplib
 Project-URL: Changelog, https://github.com/Ousret/urllib3-ext-hface/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/Ousret/urllib3-ext-hface
 Project-URL: Issue tracker, https://github.com/Ousret/urllib3-ext-hface/issues
 Author-email: Miloslav Pojman <mpojman@akamai.com>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
@@ -72,15 +72,15 @@
     protocol.bytes_to_send()  # Out to your network I/O implementation
     # ...
     protocol.bytes_received()  # Whatever comes from your network I/O implementation
     # ...
     protocol.next_event()  # Output the next event in order that the state-machine generated
 
 Here ``protocol`` is either of type ``HTTPOverQUICProtocol`` or ``HTTPOverTCPProtocol``, depending
-on the foremost, you will either be on a DRAM (UDP) or STREAM (TCP) socket.
+on the foremost, you will either be on a DGRAM (UDP) or STREAM (TCP) socket.
 
 Find just bellow a somewhat stupid example that can help you get started.
 
 .. code-block:: python
 
     from urllib3_ext_hface import HTTPProtocolFactory, HTTP1Protocol, HTTP2Protocol, HTTP3Protocol
     import ssl
```

