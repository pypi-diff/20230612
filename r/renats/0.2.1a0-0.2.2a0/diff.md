# Comparing `tmp/renats-0.2.1a0.tar.gz` & `tmp/renats-0.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renats-0.2.1a0.tar", max compression
+gzip compressed data, was "renats-0.2.2a0.tar", max compression
```

## Comparing `renats-0.2.1a0.tar` & `renats-0.2.2a0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      866 2023-06-09 12:58:05.359460 renats-0.2.1a0/README.md
--rw-r--r--   0        0        0      382 2023-06-09 16:03:50.885001 renats-0.2.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.1a0/renats/__init__.py
--rw-r--r--   0        0        0       31 2023-06-09 15:07:47.060580 renats-0.2.1a0/renats/client/__init__.py
--rw-r--r--   0        0        0      203 2023-06-09 15:07:54.484606 renats-0.2.1a0/renats/client/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4880 2023-06-09 15:47:16.088045 renats-0.2.1a0/renats/client/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0      583 2023-06-09 14:45:21.475619 renats-0.2.1a0/renats/client/__pycache__/message.cpython-310.pyc
--rw-r--r--   0        0        0     1091 2023-06-09 15:45:43.959550 renats-0.2.1a0/renats/client/__pycache__/parser.cpython-310.pyc
--rw-r--r--   0        0        0      940 2023-06-09 14:45:21.475619 renats-0.2.1a0/renats/client/__pycache__/subscription.cpython-310.pyc
--rw-r--r--   0        0        0      506 2023-06-09 14:45:48.799735 renats-0.2.1a0/renats/client/__pycache__/types.cpython-310.pyc
--rw-r--r--   0        0        0     4603 2023-06-09 15:47:39.304167 renats-0.2.1a0/renats/client/client.py
--rw-r--r--   0        0        0      249 2023-06-09 13:19:02.292440 renats-0.2.1a0/renats/client/message.py
--rw-r--r--   0        0        0      926 2023-06-09 15:45:42.939545 renats-0.2.1a0/renats/client/parser.py
--rw-r--r--   0        0        0      530 2023-06-09 14:28:38.743445 renats-0.2.1a0/renats/client/subscription.py
--rw-r--r--   0        0        0      159 2023-06-09 14:45:44.555717 renats-0.2.1a0/renats/client/types.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.1a0/renats/connection/__init__.py
--rw-r--r--   0        0        0      166 2023-06-09 14:42:32.158897 renats-0.2.1a0/renats/connection/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1573 2023-06-09 14:42:32.158897 renats-0.2.1a0/renats/connection/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     2007 2023-06-09 14:45:48.799735 renats-0.2.1a0/renats/connection/__pycache__/tcp.cpython-310.pyc
--rw-r--r--   0        0        0      863 2023-06-09 12:14:24.557525 renats-0.2.1a0/renats/connection/base.py
--rw-r--r--   0        0        0       64 2023-06-09 12:14:24.557525 renats-0.2.1a0/renats/connection/connection.py
--rw-r--r--   0        0        0     1107 2023-06-09 12:14:24.557525 renats-0.2.1a0/renats/connection/tcp.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.1a0/renats/protocol/__init__.py
--rw-r--r--   0        0        0      164 2023-06-09 14:42:32.158897 renats-0.2.1a0/renats/protocol/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1378 2023-06-09 14:45:21.475619 renats-0.2.1a0/renats/protocol/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0      925 2023-06-09 14:42:32.158897 renats-0.2.1a0/renats/protocol/__pycache__/protocol.cpython-310.pyc
--rw-r--r--   0        0        0     2335 2023-06-09 14:45:21.475619 renats-0.2.1a0/renats/protocol/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0      530 2023-06-09 14:32:00.672258 renats-0.2.1a0/renats/protocol/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.1a0/renats/protocol/messages/__init__.py
--rw-r--r--   0        0        0      173 2023-06-09 14:45:21.475619 renats-0.2.1a0/renats/protocol/messages/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      702 2023-06-09 14:57:46.434759 renats-0.2.1a0/renats/protocol/messages/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      863 2023-06-09 14:45:21.475619 renats-0.2.1a0/renats/protocol/messages/__pycache__/msg.cpython-310.pyc
--rw-r--r--   0        0        0     1926 2023-06-09 15:04:32.367916 renats-0.2.1a0/renats/protocol/messages/__pycache__/pub.cpython-310.pyc
--rw-r--r--   0        0        0     2651 2023-06-09 15:41:51.790249 renats-0.2.1a0/renats/protocol/messages/__pycache__/service.cpython-310.pyc
--rw-r--r--   0        0        0     1711 2023-06-09 15:07:48.276584 renats-0.2.1a0/renats/protocol/messages/__pycache__/sub.cpython-310.pyc
--rw-r--r--   0        0        0      295 2023-06-09 14:57:08.722653 renats-0.2.1a0/renats/protocol/messages/base.py
--rw-r--r--   0        0        0      390 2023-06-09 14:36:47.625444 renats-0.2.1a0/renats/protocol/messages/msg.py
--rw-r--r--   0        0        0     1574 2023-06-09 15:04:22.467883 renats-0.2.1a0/renats/protocol/messages/pub.py
--rw-r--r--   0        0        0     1872 2023-06-09 15:41:50.058239 renats-0.2.1a0/renats/protocol/messages/service.py
--rw-r--r--   0        0        0     1213 2023-06-09 15:04:22.459883 renats-0.2.1a0/renats/protocol/messages/sub.py
--rw-r--r--   0        0        0      668 2023-06-09 13:31:51.097649 renats-0.2.1a0/renats/protocol/protocol.py
--rw-r--r--   0        0        0     1591 2023-06-09 14:44:25.191379 renats-0.2.1a0/renats/protocol/utils.py
--rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 renats-0.2.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1632 2023-06-12 13:52:41.717275 renats-0.2.2a0/README.md
+-rw-r--r--   0        0        0      402 2023-06-12 13:52:41.717275 renats-0.2.2a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-09 15:07:54.484606 renats-0.2.2a0/renats/client/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4428 2023-06-12 10:50:01.221016 renats-0.2.2a0/renats/client/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0      583 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/client/__pycache__/message.cpython-310.pyc
+-rw-r--r--   0        0        0     1087 2023-06-12 10:50:01.229016 renats-0.2.2a0/renats/client/__pycache__/parser.cpython-310.pyc
+-rw-r--r--   0        0        0     1355 2023-06-12 10:56:15.311568 renats-0.2.2a0/renats/client/__pycache__/subscription.cpython-310.pyc
+-rw-r--r--   0        0        0      809 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/base.py
+-rw-r--r--   0        0        0     6325 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/client.py
+-rw-r--r--   0        0        0      647 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/handler.py
+-rw-r--r--   0        0        0      264 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/message.py
+-rw-r--r--   0        0        0      937 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/parser.py
+-rw-r--r--   0        0        0     1654 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/client/subscription.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/connection/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-09 14:42:32.158897 renats-0.2.2a0/renats/connection/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1693 2023-06-12 10:50:01.229016 renats-0.2.2a0/renats/connection/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     2003 2023-06-12 10:50:01.233016 renats-0.2.2a0/renats/connection/__pycache__/tcp.cpython-310.pyc
+-rw-r--r--   0        0        0      951 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/connection/base.py
+-rw-r--r--   0        0        0       64 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/connection/connection.py
+-rw-r--r--   0        0        0     1099 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/connection/tcp.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/protocol/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-09 14:42:32.158897 renats-0.2.2a0/renats/protocol/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1378 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/protocol/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0      925 2023-06-09 14:42:32.158897 renats-0.2.2a0/renats/protocol/__pycache__/protocol.cpython-310.pyc
+-rw-r--r--   0        0        0     2335 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/protocol/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      530 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:14:24.557525 renats-0.2.2a0/renats/protocol/messages/__init__.py
+-rw-r--r--   0        0        0      173 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/protocol/messages/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      702 2023-06-09 14:57:46.434759 renats-0.2.2a0/renats/protocol/messages/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0      863 2023-06-09 14:45:21.475619 renats-0.2.2a0/renats/protocol/messages/__pycache__/msg.cpython-310.pyc
+-rw-r--r--   0        0        0     1926 2023-06-09 15:04:32.367916 renats-0.2.2a0/renats/protocol/messages/__pycache__/pub.cpython-310.pyc
+-rw-r--r--   0        0        0     2651 2023-06-09 15:41:51.790249 renats-0.2.2a0/renats/protocol/messages/__pycache__/service.cpython-310.pyc
+-rw-r--r--   0        0        0     1711 2023-06-09 15:07:48.276584 renats-0.2.2a0/renats/protocol/messages/__pycache__/sub.cpython-310.pyc
+-rw-r--r--   0        0        0      295 2023-06-09 14:57:08.722653 renats-0.2.2a0/renats/protocol/messages/base.py
+-rw-r--r--   0        0        0      390 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/messages/msg.py
+-rw-r--r--   0        0        0     1574 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/messages/pub.py
+-rw-r--r--   0        0        0     1749 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/messages/service.py
+-rw-r--r--   0        0        0     1167 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/messages/sub.py
+-rw-r--r--   0        0        0      668 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/protocol.py
+-rw-r--r--   0        0        0     1591 2023-06-12 13:52:41.717275 renats-0.2.2a0/renats/protocol/utils.py
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 renats-0.2.2a0/PKG-INFO
```

### Comparing `renats-0.2.1a0/renats/client/__pycache__/message.cpython-310.pyc` & `renats-0.2.2a0/renats/client/__pycache__/message.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/client/__pycache__/parser.cpython-310.pyc` & `renats-0.2.2a0/renats/client/__pycache__/parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 15:45:42 2023 UTC, .py size: 926 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-00000000: 6f0d 0d0a 0000 0000 2649 8364 9e03 0000  o.......&I.d....
+00000000: 6f0d 0d0a 0000 0000 eeec 8664 9203 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6500 a00a 6406  m.Z.m.Z...e...d.
 00000070: a101 5a0b 6407 650c 6408 6502 6409 6508  ..Z.d.e.d.e.d.e.
 00000080: 6606 640a 640b 8404 5a0d 6407 650c 6408  f.d.d...Z.d.e.d.
 00000090: 6502 6409 6509 6606 640c 640d 8404 5a0e  e.d.e.f.d.d...Z.
-000000a0: 6401 5300 290e e900 0000 004e 2901 da0e  d.S.)......N)...
-000000b0: 4261 7365 436f 6e6e 6563 7469 6f6e 2901  BaseConnection).
-000000c0: da05 7574 696c 7329 01da 1649 6e76 616c  ..utils)...Inval
-000000d0: 6964 5072 6f74 6f63 6f6c 4d65 7373 6167  idProtocolMessag
-000000e0: 6529 02da 124d 7367 5072 6f74 6f63 6f6c  e)...MsgProtocol
-000000f0: 4d65 7373 6167 65da 1348 4d73 6750 726f  Message..HMsgPro
-00000100: 746f 636f 6c4d 6573 7361 6765 7327 0000  tocolMessages'..
-00000110: 005e 4d53 475c 732b 285c 532b 295c 732b  .^MSG\s+(\S+)\s+
-00000120: 285c 532b 295c 732b 2828 5c53 2b29 5c73  (\S+)\s+((\S+)\s
-00000130: 2b29 3f28 5c64 2b29 da04 6865 6164 da0a  +)?(\d+)..head..
-00000140: 636f 6e6e 6563 7469 6f6e da06 7265 7475  connection..retu
-00000150: 726e 6302 0000 0000 0000 0000 0000 0009  rnc.............
-00000160: 0000 0007 0000 00c3 0000 0073 6000 0000  ...........s`...
-00000170: 8101 7400 a001 7402 7c00 a102 7d02 7c02  ..t...t.|...}.|.
-00000180: 6400 7500 720f 7403 7c00 8301 8201 7c02  d.u.r.t.|.....|.
-00000190: a004 a100 5c05 7d03 7d04 7d05 7d06 7d07  ....\.}.}.}.}.}.
-000001a0: 7c01 a005 7406 7c07 8301 7407 6a08 1700  |...t.|...t.j...
-000001b0: a101 4900 6400 4800 7d08 7409 7c03 7c04  ..I.d.H.}.t.|.|.
-000001c0: 7c06 7406 7c07 8301 7c08 6401 8d05 5300  |.t.|...|.d...S.
-000001d0: 2902 4e29 05da 0773 7562 6a65 6374 da03  ).N)...subject..
-000001e0: 7369 64da 0872 6570 6c79 5f74 6fda 0e70  sid..reply_to..p
-000001f0: 6179 6c6f 6164 5f6c 656e 6774 68da 0770  ayload_length..p
-00000200: 6179 6c6f 6164 290a da02 7265 da05 6d61  ayload)...re..ma
-00000210: 7463 68da 104d 5347 5f48 4541 445f 5041  tch..MSG_HEAD_PA
-00000220: 5454 4552 4e72 0400 0000 da06 6772 6f75  TTERNr......grou
-00000230: 7073 da0b 7265 6164 6578 6163 746c 79da  ps..readexactly.
-00000240: 0369 6e74 7203 0000 00da 0943 524c 465f  .intr......CRLF_
-00000250: 5349 5a45 7205 0000 0029 0972 0700 0000  SIZEr....).r....
-00000260: 7208 0000 0072 1000 0000 720a 0000 0072  r....r....r....r
-00000270: 0b00 0000 da01 5f72 0c00 0000 720d 0000  ......_r....r...
-00000280: 0072 0e00 0000 a900 7217 0000 00fa 432f  .r......r.....C/
-00000290: 686f 6d65 2f72 6573 7069 7265 6e73 2f68  home/respirens/h
-000002a0: 616e 6469 6365 652f 6465 7665 6c6f 702f  andicee/develop/
-000002b0: 7765 622f 5265 4e41 5453 2f72 656e 6174  web/ReNATS/renat
-000002c0: 732f 636c 6965 6e74 2f70 6172 7365 722e  s/client/parser.
-000002d0: 7079 da09 7061 7273 655f 6d73 670b 0000  py..parse_msg...
-000002e0: 0073 1a00 0000 0280 0c01 0801 0801 1201  .s..............
-000002f0: 1a01 0201 0201 0201 0201 0601 0201 06fb  ................
-00000300: 7219 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00000310: 0000 0200 0000 0100 0000 c300 0000 7306  ..............s.
-00000320: 0000 0081 0164 0053 0029 014e 7217 0000  .....d.S.).Nr...
-00000330: 0029 0272 0700 0000 7208 0000 0072 1700  .).r....r....r..
-00000340: 0000 7217 0000 0072 1800 0000 da0a 7061  ..r....r......pa
-00000350: 7273 655f 686d 7367 1a00 0000 7304 0000  rse_hmsg....s...
-00000360: 0002 8004 0172 1a00 0000 290f 720f 0000  .....r....).r...
-00000370: 00da 1672 656e 6174 732e 636f 6e6e 6563  ...renats.connec
-00000380: 7469 6f6e 2e62 6173 6572 0200 0000 da0f  tion.baser......
-00000390: 7265 6e61 7473 2e70 726f 746f 636f 6c72  renats.protocolr
-000003a0: 0300 0000 da1a 7265 6e61 7473 2e70 726f  ......renats.pro
-000003b0: 746f 636f 6c2e 6578 6365 7074 696f 6e73  tocol.exceptions
-000003c0: 7204 0000 00da 1c72 656e 6174 732e 7072  r......renats.pr
-000003d0: 6f74 6f63 6f6c 2e6d 6573 7361 6765 732e  otocol.messages.
-000003e0: 6d73 6772 0500 0000 7206 0000 00da 0763  msgr....r......c
-000003f0: 6f6d 7069 6c65 7211 0000 00da 0562 7974  ompiler......byt
-00000400: 6573 7219 0000 0072 1a00 0000 7217 0000  esr....r....r...
-00000410: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000420: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
-00000430: 0000 0008 000c 020c 010c 0110 010a 0216  ................
-00000440: 031a 0f                                  ...
+000000a0: 6401 5300 290e e900 0000 004e 2901 da0a  d.S.)......N)...
+000000b0: 436f 6e6e 6563 7469 6f6e 2901 da05 7574  Connection)...ut
+000000c0: 696c 7329 01da 1649 6e76 616c 6964 5072  ils)...InvalidPr
+000000d0: 6f74 6f63 6f6c 4d65 7373 6167 6529 02da  otocolMessage)..
+000000e0: 124d 7367 5072 6f74 6f63 6f6c 4d65 7373  .MsgProtocolMess
+000000f0: 6167 65da 1348 4d73 6750 726f 746f 636f  age..HMsgProtoco
+00000100: 6c4d 6573 7361 6765 7327 0000 005e 4d53  lMessages'...^MS
+00000110: 475c 732b 285c 532b 295c 732b 285c 532b  G\s+(\S+)\s+(\S+
+00000120: 295c 732b 2828 5c53 2b29 5c73 2b29 3f28  )\s+((\S+)\s+)?(
+00000130: 5c64 2b29 da04 6865 6164 da0a 636f 6e6e  \d+)..head..conn
+00000140: 6563 7469 6f6e da06 7265 7475 726e 6302  ection..returnc.
+00000150: 0000 0000 0000 0000 0000 0009 0000 0007  ................
+00000160: 0000 00c3 0000 0073 6000 0000 8101 7400  .......s`.....t.
+00000170: a001 7402 7c00 a102 7d02 7c02 6400 7500  ..t.|...}.|.d.u.
+00000180: 720f 7403 7c00 8301 8201 7c02 a004 a100  r.t.|.....|.....
+00000190: 5c05 7d03 7d04 7d05 7d06 7d07 7c01 a005  \.}.}.}.}.}.|...
+000001a0: 7406 7c07 8301 7407 6a08 1700 a101 4900  t.|...t.j.....I.
+000001b0: 6400 4800 7d08 7409 7c03 7c04 7c06 7406  d.H.}.t.|.|.|.t.
+000001c0: 7c07 8301 7c08 6401 8d05 5300 2902 4e29  |...|.d...S.).N)
+000001d0: 05da 0773 7562 6a65 6374 da03 7369 64da  ...subject..sid.
+000001e0: 0872 6570 6c79 5f74 6fda 0e70 6179 6c6f  .reply_to..paylo
+000001f0: 6164 5f6c 656e 6774 68da 0770 6179 6c6f  ad_length..paylo
+00000200: 6164 290a da02 7265 da05 6d61 7463 68da  ad)...re..match.
+00000210: 104d 5347 5f48 4541 445f 5041 5454 4552  .MSG_HEAD_PATTER
+00000220: 4e72 0400 0000 da06 6772 6f75 7073 da0b  Nr......groups..
+00000230: 7265 6164 6578 6163 746c 79da 0369 6e74  readexactly..int
+00000240: 7203 0000 00da 0943 524c 465f 5349 5a45  r......CRLF_SIZE
+00000250: 7205 0000 0029 0972 0700 0000 7208 0000  r....).r....r...
+00000260: 0072 1000 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000270: da01 5f72 0c00 0000 720d 0000 0072 0e00  .._r....r....r..
+00000280: 0000 a900 7217 0000 00fa 432f 686f 6d65  ....r.....C/home
+00000290: 2f72 6573 7069 7265 6e73 2f68 616e 6469  /respirens/handi
+000002a0: 6365 652f 6465 7665 6c6f 702f 7765 622f  cee/develop/web/
+000002b0: 5265 4e41 5453 2f72 656e 6174 732f 636c  ReNATS/renats/cl
+000002c0: 6965 6e74 2f70 6172 7365 722e 7079 da09  ient/parser.py..
+000002d0: 7061 7273 655f 6d73 670b 0000 0073 1a00  parse_msg....s..
+000002e0: 0000 0280 0c01 0801 0801 1201 1a01 0201  ................
+000002f0: 0201 0201 0201 0601 0201 06fb 7219 0000  ............r...
+00000300: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00000310: 0000 0100 0000 c300 0000 7306 0000 0081  ..........s.....
+00000320: 0164 0053 0029 014e 7217 0000 0029 0272  .d.S.).Nr....).r
+00000330: 0700 0000 7208 0000 0072 1700 0000 7217  ....r....r....r.
+00000340: 0000 0072 1800 0000 da0a 7061 7273 655f  ...r......parse_
+00000350: 686d 7367 1a00 0000 7304 0000 0002 8004  hmsg....s.......
+00000360: 0172 1a00 0000 290f 720f 0000 00da 1672  .r....).r......r
+00000370: 656e 6174 732e 636f 6e6e 6563 7469 6f6e  enats.connection
+00000380: 2e62 6173 6572 0200 0000 da0f 7265 6e61  .baser......rena
+00000390: 7473 2e70 726f 746f 636f 6c72 0300 0000  ts.protocolr....
+000003a0: da1a 7265 6e61 7473 2e70 726f 746f 636f  ..renats.protoco
+000003b0: 6c2e 6578 6365 7074 696f 6e73 7204 0000  l.exceptionsr...
+000003c0: 00da 1c72 656e 6174 732e 7072 6f74 6f63  ...renats.protoc
+000003d0: 6f6c 2e6d 6573 7361 6765 732e 6d73 6772  ol.messages.msgr
+000003e0: 0500 0000 7206 0000 00da 0763 6f6d 7069  ....r......compi
+000003f0: 6c65 7211 0000 00da 0562 7974 6573 7219  ler......bytesr.
+00000400: 0000 0072 1a00 0000 7217 0000 0072 1700  ...r....r....r..
+00000410: 0000 7217 0000 0072 1800 0000 da08 3c6d  ..r....r......<m
+00000420: 6f64 756c 653e 0100 0000 7310 0000 0008  odule>....s.....
+00000430: 000c 020c 010c 0110 010a 0216 031a 0f    ...............
```

### Comparing `renats-0.2.1a0/renats/client/client.py` & `renats-0.2.2a0/renats/client/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,137 +3,163 @@
 from asyncio import Task
 from typing import Final
 
 import msgspec.json
 from typing_extensions import Self
 
 from . import parser
-from .subscription import Subscription
-from .types import Server
-from ..connection.base import BaseConnection
+from .base import NATS
+from .message import Message
+from .subscription import Subscription, SubscriptionManager, SubscriptionCallbackType
+from ..connection.base import Connection
 from ..connection.tcp import TcpConnection
 from ..protocol import protocol
 from ..protocol.messages.msg import MsgProtocolMessage, HMsgProtocolMessage
 from ..protocol.messages.pub import PubProtocolMessage, HPubProtocolMessage
 from ..protocol.messages.service import InfoProtocolMessage, ConnectProtocolMessage
+from ..protocol.messages.sub import SubProtocolMessage, UnsubProtocolMessage
 
 DEFAULT_CONNECTION_TIMEOUT: Final[float] = 2
-DEFAULT_INFO_TIMEOUT: Final[float] = 2
+DEFAULT_INFO_WAITING_TIMEOUT: Final[float] = 2
+
 CLIENT_LANGUAGE: Final[str] = "python3"
-CLIENT_VERSION: Final[str] = "0.0.1-alpha"
+CLIENT_VERSION: Final[str] = "0.2.2-alpha"
+
+CLIENT_CONNECTION_VERBOSE: Final[bool] = False
+CLIENT_CONNECTION_PEDANTIC: Final[bool] = True
+
+HeadersType = dict[str, str]
 
 
-class NATSClient:
+class NATSClient(NATS):
     def __init__(self):
         self._logger: logging.Logger = logging.getLogger(__name__)
-        self._connection: BaseConnection | None = None
-        self._server: Server | None = None
+        self._connection: Connection | None = None
+        self._connection_info: InfoProtocolMessage | None = None
         self._handler_task: Task | None = None
-        self._subscriptions: dict[str, Subscription] = {}
-
-    @property
-    def connection(self):
-        return self._connection
-
-    @connection.setter
-    def connection(self, value: BaseConnection):
-        if self._connection is not None and not self._connection.closed:
-            raise RuntimeError("Replacing non-closed connection is not allowed")
-        self._connection = value
+        self._subscriptions: SubscriptionManager = SubscriptionManager()
 
     @property
-    def available(self):
-        return (
-                self._connection is not None
-                and
-                not self._connection.closed
-                and
-                self._server is not None
+    def available(self) -> bool:
+        return all(
+            (
+                self._connection is not None,
+                not self._connection.closed,
+                self._connection_info is not None
+            )
         )
 
     @property
-    def server(self):
-        return self._server
+    def connection(self) -> Connection:
+        return self._connection
 
     @property
-    def logger(self):
-        return self._logger
+    def connection_info(self) -> InfoProtocolMessage:
+        return self._connection_info
 
-    async def send(self, message: bytes):
-        self._connection.write(message)
-        await self._connection.drain()
-
-    async def _process_connection_init(self):
+    async def _init_connection(self):
+        # Wait for INFO protocol message and parse it
         info = msgspec.json.decode(
-            (await self.connection.readline()).split(b" ", 1)[1].decode(),
+            (await self._connection.readline()).split(b" ", 1)[1].decode(),
             type=InfoProtocolMessage
         )
-        self._server = Server(
-            id=info.server_id,
-            headers_support=info.headers,
-            max_payload=info.max_payload,
-            name=info.server_name,
-            protocol=info.proto,
-            version=info.version
-        )
-        await self.send(
+
+        # Save INFO protocol message in the client class
+        self._connection_info = info
+
+        # Send CONNECT protocol message
+        await self._connection.send(
             ConnectProtocolMessage(
-                verbose=False,
-                pedantic=True,
+                verbose=CLIENT_CONNECTION_VERBOSE,
+                pedantic=CLIENT_CONNECTION_PEDANTIC,
                 tls_required=False,
                 lang=CLIENT_LANGUAGE,
                 version=CLIENT_VERSION,
                 headers=True
             ).dump()
         )
 
-    async def _process_msg(self, msg: MsgProtocolMessage):
-        pass
+    async def _handle_message(self, protocol_message: MsgProtocolMessage | HMsgProtocolMessage):
+        # Skip message if its subscription id not registered in subscription manager
+        if protocol_message.sid not in self._subscriptions:
+            return
+
+        # Create Message class instance from MsgProtocolMessage or HMsgProtocolMessage
+        message = Message(
+            subject=protocol_message.subject,
+            payload=protocol_message.payload,
+            reply_subject=protocol_message.reply_to,
+            headers=protocol_message.headers if isinstance(protocol_message, HMsgProtocolMessage) else None
+        )
 
-    async def _process_hmsg(self, msg: HMsgProtocolMessage):
-        pass
+        # Create message handler task (message handled by subscription manager)
+        asyncio.create_task(self._subscriptions.handle(protocol_message.sid, message))
 
-    async def _handler(self):
+    async def _handle_connection_input(self):
         while True:
-            line = await self.connection.readline()
-            head = line.split(b" ", 1)
-            match head[0].strip():
-                case protocol.PING:
-                    await self.send(protocol.PONG_MESSAGE)
-                case protocol.ERR:
-                    self.logger.error("Received NATS Error: %s", head[1])
-                case protocol.MSG:
-                    await self._process_msg(await parser.parse_msg(line, self.connection))
-                case protocol.HMSG:
-                    await self._process_hmsg(await parser.parse_hmsg(line, self.connection))
-                case _:
-                    self.logger.warning(f"Received unknown NATS protocol message: %s", line)
+            # Wait for "head" line and read it
+            # The "head" is the first line of the protocol message.
+            head_line = await self.connection.readline()
+
+            # Split the "head" line to method and params line
+            head = head_line.split(b" ", 1)
+            method = head[0].strip()
+
+            if method == protocol.PING:
+                await self._connection.send(protocol.PONG_MESSAGE)
+            elif method == protocol.ERR:
+                self._logger.error("Received NATS error: %s", head[1])
+            elif method == protocol.MSG:
+                protocol_message = await parser.parse_msg(head_line, self._connection)
+                await self._handle_message(protocol_message)
+            elif method == protocol.HMSG:
+                protocol_message = await parser.parse_hmsg(head_line, self._connection)
+                await self._handle_message(protocol_message)
+            else:
+                self._logger.warning("Received unknown NATS protocol message: %s", head_line)
+
+    async def connect(self, servers: tuple[tuple[str, int]]) -> Self:
+        # Temporary. This will be updated for using multiserver connection
+        host, port = servers[0]
 
-    async def connect(self, host: str, port: int) -> Self:
-        self.connection = TcpConnection()
+        self._connection = TcpConnection()
         await self.connection.connect(host, port, DEFAULT_CONNECTION_TIMEOUT)
-        await self._process_connection_init()
-        self._handler_task = asyncio.get_running_loop().create_task(self._handler())
+        await self._init_connection()
+        self._handler_task = asyncio.get_running_loop().create_task(self._handle_connection_input())
         return self
 
     async def close(self):
         self._handler_task.cancel()
         await self.connection.close()
 
-    async def publish(self, subject: str, data: bytes = b"", reply: str = None, headers: dict[str, str] = None):
-        if self.server.headers_support and headers is not None:
-            await self.send(
-                HPubProtocolMessage(
-                    subject=subject,
-                    payload=data,
-                    reply_to=reply,
-                    headers=headers
-                ).dump()
+    async def publish(self, subject: str, payload: bytes = b"", reply_subject: str = None, headers: HeadersType = None):
+        if self._connection_info.headers and headers is not None:
+            message = HPubProtocolMessage(
+                subject=subject,
+                payload=payload,
+                reply_to=reply_subject,
+                headers=headers
             )
-            return
-        await self.send(
-            PubProtocolMessage(
+        else:
+            message = PubProtocolMessage(
                 subject=subject,
-                payload=data,
-                reply_to=reply
-            ).dump()
+                payload=payload,
+                reply_to=reply_subject
+            )
+        await self._connection.send(message.dump())
+
+    async def subscribe(self, subject: str, callback: SubscriptionCallbackType) -> Subscription:
+        subscription = self._subscriptions.create(subject, callback, self)
+        message = SubProtocolMessage(
+            subject=subscription.subject,
+            sid=subscription.id
+        )
+        await self._connection.send(message.dump())
+        return subscription
+
+    async def unsubscribe(self, subscription_id: str, messages_left: int = 0):
+        message = UnsubProtocolMessage(
+            sid=subscription_id,
+            max_msgs=messages_left
         )
+        await self._connection.send(message.dump())
+        self._subscriptions.delete(subscription_id, messages_left)
```

### Comparing `renats-0.2.1a0/renats/client/parser.py` & `renats-0.2.2a0/renats/client/parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import re
 
-from renats.connection.base import BaseConnection
+from renats.connection.base import Connection
 from renats.protocol import utils
 from renats.protocol.exceptions import InvalidProtocolMessage
 from renats.protocol.messages.msg import MsgProtocolMessage, HMsgProtocolMessage
 
 MSG_HEAD_PATTERN = re.compile(br"^MSG\s+(\S+)\s+(\S+)\s+((\S+)\s+)?(\d+)")
 
 
-async def parse_msg(head: bytes, connection: BaseConnection) -> MsgProtocolMessage:
+async def parse_msg(head: bytes, connection: Connection) -> MsgProtocolMessage:
     match = re.match(MSG_HEAD_PATTERN, head)
     if match is None:
         raise InvalidProtocolMessage(head)
     subject, sid, _, reply_to, payload_length = match.groups()
     payload = await connection.readexactly(int(payload_length) + utils.CRLF_SIZE)
     return MsgProtocolMessage(
         subject=subject,
         sid=sid,
         reply_to=reply_to,
         payload_length=int(payload_length),
         payload=payload
     )
 
 
-async def parse_hmsg(head: bytes, connection: BaseConnection) -> HMsgProtocolMessage:
-    pass
+async def parse_hmsg(head: bytes, connection: Connection) -> HMsgProtocolMessage:
+    raise NotImplementedError()
```

### Comparing `renats-0.2.1a0/renats/connection/__pycache__/tcp.cpython-310.pyc` & `renats-0.2.2a0/renats/connection/__pycache__/tcp.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun  9 12:14:24 2023 UTC, .py size: 1107 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-00000000: 6f0d 0d0a 0000 0000 a017 8364 5304 0000  o..........dS...
+00000000: 6f0d 0d0a 0000 0000 27f4 8664 4b04 0000  o.......'..dK...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 6d02 5a02 0100 6403 6404 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000060: 5a05 6401 5300 2907 e900 0000 004e 2902  Z.d.S.)......N).
 00000070: da0c 5374 7265 616d 5265 6164 6572 da0c  ..StreamReader..
 00000080: 5374 7265 616d 5772 6974 6572 e901 0000  StreamWriter....
-00000090: 0029 01da 0e42 6173 6543 6f6e 6e65 6374  .)...BaseConnect
-000000a0: 696f 6e63 0000 0000 0000 0000 0000 0000  ionc............
-000000b0: 0000 0000 0600 0000 4000 0000 738c 0000  ........@...s...
-000000c0: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
-000000d0: 0364 0365 0464 0465 0564 0565 0666 0664  .d.e.d.e.d.e.f.d
-000000e0: 0664 0784 045a 0764 0865 0564 0965 0866  .d...Z.d.e.d.e.f
-000000f0: 0464 0a64 0b84 045a 0964 0865 0564 0965  .d.d...Z.d.e.d.e
-00000100: 0866 0464 0c64 0d84 045a 0a64 0965 0866  .f.d.d...Z.d.e.f
-00000110: 0264 0e64 0f84 045a 0b64 1065 0866 0264  .d.d...Z.d.e.f.d
-00000120: 1164 1284 045a 0c64 1364 1484 005a 0d64  .d...Z.d.d...Z.d
-00000130: 1564 1684 005a 0e65 0f64 0965 1066 0264  .d...Z.e.d.e.f.d
-00000140: 1764 1884 0483 015a 1164 1953 0029 1ada  .d.....Z.d.S.)..
-00000150: 0d54 6370 436f 6e6e 6563 7469 6f6e 6301  .TcpConnectionc.
-00000160: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000170: 0000 0043 0000 0073 1600 0000 6400 7c00  ...C...s....d.|.
-00000180: 5f00 6400 7c00 5f01 6401 7c00 5f02 6400  _.d.|._.d.|._.d.
-00000190: 5300 a902 4e54 2903 da07 5f72 6561 6465  S...NT)..._reade
-000001a0: 72da 075f 7772 6974 6572 da07 5f63 6c6f  r.._writer.._clo
-000001b0: 7365 64a9 01da 0473 656c 66a9 0072 0d00  sed....self..r..
-000001c0: 0000 fa44 2f68 6f6d 652f 7265 7370 6972  ...D/home/respir
-000001d0: 656e 732f 6861 6e64 6963 6565 2f64 6576  ens/handicee/dev
-000001e0: 656c 6f70 2f77 6562 2f52 654e 4154 532f  elop/web/ReNATS/
-000001f0: 7265 6e61 7473 2f63 6f6e 6e65 6374 696f  renats/connectio
-00000200: 6e2f 7463 702e 7079 da08 5f5f 696e 6974  n/tcp.py..__init
-00000210: 5f5f 0800 0000 7306 0000 0006 0106 010a  __....s.........
-00000220: 017a 1654 6370 436f 6e6e 6563 7469 6f6e  .z.TcpConnection
-00000230: 2e5f 5f69 6e69 745f 5fda 0468 6f73 74da  .__init__..host.
-00000240: 0470 6f72 74da 0774 696d 656f 7574 6304  .port..timeoutc.
-00000250: 0000 0000 0000 0000 0000 0004 0000 0006  ................
-00000260: 0000 00c3 0000 0073 2e00 0000 8101 7400  .......s......t.
-00000270: a001 7400 a002 7c01 7c02 a102 7c03 a102  ..t...|.|...|...
-00000280: 4900 6400 4800 5c02 7c00 5f03 7c00 5f04  I.d.H.\.|._.|._.
-00000290: 6401 7c00 5f05 6400 5300 2902 4e46 2906  d.|._.d.S.).NF).
-000002a0: da07 6173 796e 6369 6fda 0877 6169 745f  ..asyncio..wait_
-000002b0: 666f 72da 0f6f 7065 6e5f 636f 6e6e 6563  for..open_connec
-000002c0: 7469 6f6e 7208 0000 0072 0900 0000 720a  tionr....r....r.
-000002d0: 0000 0029 0472 0c00 0000 7210 0000 0072  ...).r....r....r
-000002e0: 1100 0000 7212 0000 0072 0d00 0000 720d  ....r....r....r.
-000002f0: 0000 0072 0e00 0000 da07 636f 6e6e 6563  ...r......connec
-00000300: 740d 0000 0073 0600 0000 0280 2201 0a01  t....s......"...
-00000310: 7a15 5463 7043 6f6e 6e65 6374 696f 6e2e  z.TcpConnection.
-00000320: 636f 6e6e 6563 74da 0473 697a 65da 0672  connect..size..r
-00000330: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
-00000340: 0000 0200 0000 0300 0000 c300 0000 f314  ................
-00000350: 0000 0081 017c 006a 00a0 017c 01a1 0149  .....|.j...|...I
-00000360: 0064 0048 0053 00a9 014e 2902 7208 0000  .d.H.S...N).r...
-00000370: 00da 0472 6561 64a9 0272 0c00 0000 7217  ...read..r....r.
-00000380: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000390: 0000 721b 0000 0011 0000 00f3 0400 0000  ..r.............
-000003a0: 0280 1201 7a12 5463 7043 6f6e 6e65 6374  ....z.TcpConnect
-000003b0: 696f 6e2e 7265 6164 6302 0000 0000 0000  ion.readc.......
-000003c0: 0000 0000 0002 0000 0003 0000 00c3 0000  ................
-000003d0: 0072 1900 0000 721a 0000 0029 0272 0800  .r....r....).r..
-000003e0: 0000 da0b 7265 6164 6578 6163 746c 7972  ....readexactlyr
-000003f0: 1c00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00000400: 0000 0072 1e00 0000 1400 0000 721d 0000  ...r........r...
-00000410: 007a 1954 6370 436f 6e6e 6563 7469 6f6e  .z.TcpConnection
-00000420: 2e72 6561 6465 7861 6374 6c79 6301 0000  .readexactlyc...
-00000430: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000440: 00c3 0000 0073 1200 0000 8101 7c00 6a00  .....s......|.j.
-00000450: a001 a100 4900 6400 4800 5300 721a 0000  ....I.d.H.S.r...
-00000460: 0029 0272 0800 0000 da08 7265 6164 6c69  .).r......readli
-00000470: 6e65 720b 0000 0072 0d00 0000 720d 0000  ner....r....r...
-00000480: 0072 0e00 0000 721f 0000 0017 0000 0073  .r....r........s
-00000490: 0400 0000 0280 1001 7a16 5463 7043 6f6e  ........z.TcpCon
-000004a0: 6e65 6374 696f 6e2e 7265 6164 6c69 6e65  nection.readline
-000004b0: da04 6461 7461 6302 0000 0000 0000 0000  ..datac.........
-000004c0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-000004d0: 1000 0000 7c00 6a00 a001 7c01 a101 0100  ....|.j...|.....
-000004e0: 6400 5300 721a 0000 0029 0272 0900 0000  d.S.r....).r....
-000004f0: da05 7772 6974 6529 0272 0c00 0000 7220  ..write).r....r 
-00000500: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000510: 0000 7221 0000 001a 0000 0073 0200 0000  ..r!.......s....
-00000520: 1001 7a13 5463 7043 6f6e 6e65 6374 696f  ..z.TcpConnectio
-00000530: 6e2e 7772 6974 6563 0100 0000 0000 0000  n.writec........
-00000540: 0000 0000 0100 0000 0200 0000 c300 0000  ................
-00000550: 7316 0000 0081 017c 006a 00a0 01a1 0049  s......|.j.....I
-00000560: 0064 0048 0001 0064 0053 0072 1a00 0000  .d.H...d.S.r....
-00000570: 2902 7209 0000 00da 0564 7261 696e 720b  ).r......drainr.
-00000580: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000590: 0000 7222 0000 001d 0000 0073 0400 0000  ..r".......s....
-000005a0: 0280 1401 7a13 5463 7043 6f6e 6e65 6374  ....z.TcpConnect
-000005b0: 696f 6e2e 6472 6169 6e63 0100 0000 0000  ion.drainc......
-000005c0: 0000 0000 0000 0100 0000 0200 0000 c300  ................
-000005d0: 0000 7326 0000 0081 017c 006a 00a0 01a1  ..s&.....|.j....
-000005e0: 0001 007c 006a 00a0 02a1 0049 0064 0048  ...|.j.....I.d.H
-000005f0: 0001 0064 017c 005f 0364 0053 0072 0700  ...d.|._.d.S.r..
-00000600: 0000 2904 7209 0000 00da 0563 6c6f 7365  ..).r......close
-00000610: da0b 7761 6974 5f63 6c6f 7365 6472 0a00  ..wait_closedr..
-00000620: 0000 720b 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000630: 0072 0e00 0000 7223 0000 0020 0000 0073  .r....r#... ...s
-00000640: 0800 0000 0280 0a01 1001 0a01 7a13 5463  ............z.Tc
-00000650: 7043 6f6e 6e65 6374 696f 6e2e 636c 6f73  pConnection.clos
-00000660: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000670: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
-00000680: 006a 0053 0072 1a00 0000 2901 720a 0000  .j.S.r....).r...
-00000690: 0072 0b00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-000006a0: 720e 0000 00da 0663 6c6f 7365 6425 0000  r......closed%..
-000006b0: 0073 0200 0000 0602 7a14 5463 7043 6f6e  .s......z.TcpCon
-000006c0: 6e65 6374 696f 6e2e 636c 6f73 6564 4e29  nection.closedN)
-000006d0: 12da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000006e0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000006f0: 616d 655f 5f72 0f00 0000 da03 7374 72da  ame__r......str.
-00000700: 0369 6e74 da05 666c 6f61 7472 1600 0000  .int..floatr....
-00000710: da05 6279 7465 7372 1b00 0000 721e 0000  ..bytesr....r...
-00000720: 0072 1f00 0000 7221 0000 0072 2200 0000  .r....r!...r"...
-00000730: 7223 0000 00da 0870 726f 7065 7274 79da  r#.....property.
-00000740: 0462 6f6f 6c72 2500 0000 720d 0000 0072  .boolr%...r....r
-00000750: 0d00 0000 720d 0000 0072 0e00 0000 7206  ....r....r....r.
-00000760: 0000 0007 0000 0073 1600 0000 0800 0801  .......s........
-00000770: 1605 1204 1203 0e03 0e03 0803 0803 0205  ................
-00000780: 1401 7206 0000 0029 0672 1300 0000 7202  ..r....).r....r.
-00000790: 0000 0072 0300 0000 da04 6261 7365 7205  ...r......baser.
-000007a0: 0000 0072 0600 0000 720d 0000 0072 0d00  ...r....r....r..
-000007b0: 0000 720d 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
-000007c0: 6f64 756c 653e 0100 0000 7308 0000 0008  odule>....s.....
-000007d0: 0010 010c 0214 03                        .......
+00000090: 0029 01da 0a43 6f6e 6e65 6374 696f 6e63  .)...Connectionc
+000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000000b0: 0600 0000 4000 0000 738c 0000 0065 005a  ....@...s....e.Z
+000000c0: 0164 005a 0264 0164 0284 005a 0364 0365  .d.Z.d.d...Z.d.e
+000000d0: 0464 0465 0564 0565 0666 0664 0664 0784  .d.e.d.e.f.d.d..
+000000e0: 045a 0764 0865 0564 0965 0866 0464 0a64  .Z.d.e.d.e.f.d.d
+000000f0: 0b84 045a 0964 0865 0564 0965 0866 0464  ...Z.d.e.d.e.f.d
+00000100: 0c64 0d84 045a 0a64 0965 0866 0264 0e64  .d...Z.d.e.f.d.d
+00000110: 0f84 045a 0b64 1065 0866 0264 1164 1284  ...Z.d.e.f.d.d..
+00000120: 045a 0c64 1364 1484 005a 0d64 1564 1684  .Z.d.d...Z.d.d..
+00000130: 005a 0e65 0f64 0965 1066 0264 1764 1884  .Z.e.d.e.f.d.d..
+00000140: 0483 015a 1164 1953 0029 1ada 0d54 6370  ...Z.d.S.)...Tcp
+00000150: 436f 6e6e 6563 7469 6f6e 6301 0000 0000  Connectionc.....
+00000160: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00000170: 0000 0073 1600 0000 6400 7c00 5f00 6400  ...s....d.|._.d.
+00000180: 7c00 5f01 6401 7c00 5f02 6400 5300 a902  |._.d.|._.d.S...
+00000190: 4e54 2903 da07 5f72 6561 6465 72da 075f  NT)..._reader.._
+000001a0: 7772 6974 6572 da07 5f63 6c6f 7365 64a9  writer.._closed.
+000001b0: 01da 0473 656c 66a9 0072 0d00 0000 fa44  ...self..r.....D
+000001c0: 2f68 6f6d 652f 7265 7370 6972 656e 732f  /home/respirens/
+000001d0: 6861 6e64 6963 6565 2f64 6576 656c 6f70  handicee/develop
+000001e0: 2f77 6562 2f52 654e 4154 532f 7265 6e61  /web/ReNATS/rena
+000001f0: 7473 2f63 6f6e 6e65 6374 696f 6e2f 7463  ts/connection/tc
+00000200: 702e 7079 da08 5f5f 696e 6974 5f5f 0800  p.py..__init__..
+00000210: 0000 7306 0000 0006 0106 010a 017a 1654  ..s..........z.T
+00000220: 6370 436f 6e6e 6563 7469 6f6e 2e5f 5f69  cpConnection.__i
+00000230: 6e69 745f 5fda 0468 6f73 74da 0470 6f72  nit__..host..por
+00000240: 74da 0774 696d 656f 7574 6304 0000 0000  t..timeoutc.....
+00000250: 0000 0000 0000 0004 0000 0006 0000 00c3  ................
+00000260: 0000 0073 2e00 0000 8101 7400 a001 7400  ...s......t...t.
+00000270: a002 7c01 7c02 a102 7c03 a102 4900 6400  ..|.|...|...I.d.
+00000280: 4800 5c02 7c00 5f03 7c00 5f04 6401 7c00  H.\.|._.|._.d.|.
+00000290: 5f05 6400 5300 2902 4e46 2906 da07 6173  _.d.S.).NF)...as
+000002a0: 796e 6369 6fda 0877 6169 745f 666f 72da  yncio..wait_for.
+000002b0: 0f6f 7065 6e5f 636f 6e6e 6563 7469 6f6e  .open_connection
+000002c0: 7208 0000 0072 0900 0000 720a 0000 0029  r....r....r....)
+000002d0: 0472 0c00 0000 7210 0000 0072 1100 0000  .r....r....r....
+000002e0: 7212 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+000002f0: 0e00 0000 da07 636f 6e6e 6563 740d 0000  ......connect...
+00000300: 0073 0600 0000 0280 2201 0a01 7a15 5463  .s......"...z.Tc
+00000310: 7043 6f6e 6e65 6374 696f 6e2e 636f 6e6e  pConnection.conn
+00000320: 6563 74da 0473 697a 65da 0672 6574 7572  ect..size..retur
+00000330: 6e63 0200 0000 0000 0000 0000 0000 0200  nc..............
+00000340: 0000 0300 0000 c300 0000 f314 0000 0081  ................
+00000350: 017c 006a 00a0 017c 01a1 0149 0064 0048  .|.j...|...I.d.H
+00000360: 0053 00a9 014e 2902 7208 0000 00da 0472  .S...N).r......r
+00000370: 6561 64a9 0272 0c00 0000 7217 0000 0072  ead..r....r....r
+00000380: 0d00 0000 720d 0000 0072 0e00 0000 721b  ....r....r....r.
+00000390: 0000 0011 0000 00f3 0400 0000 0280 1201  ................
+000003a0: 7a12 5463 7043 6f6e 6e65 6374 696f 6e2e  z.TcpConnection.
+000003b0: 7265 6164 6302 0000 0000 0000 0000 0000  readc...........
+000003c0: 0002 0000 0003 0000 00c3 0000 0072 1900  .............r..
+000003d0: 0000 721a 0000 0029 0272 0800 0000 da0b  ..r....).r......
+000003e0: 7265 6164 6578 6163 746c 7972 1c00 0000  readexactlyr....
+000003f0: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000400: 1e00 0000 1400 0000 721d 0000 007a 1954  ........r....z.T
+00000410: 6370 436f 6e6e 6563 7469 6f6e 2e72 6561  cpConnection.rea
+00000420: 6465 7861 6374 6c79 6301 0000 0000 0000  dexactlyc.......
+00000430: 0000 0000 0001 0000 0002 0000 00c3 0000  ................
+00000440: 0073 1200 0000 8101 7c00 6a00 a001 a100  .s......|.j.....
+00000450: 4900 6400 4800 5300 721a 0000 0029 0272  I.d.H.S.r....).r
+00000460: 0800 0000 da08 7265 6164 6c69 6e65 720b  ......readliner.
+00000470: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000480: 0000 721f 0000 0017 0000 0073 0400 0000  ..r........s....
+00000490: 0280 1001 7a16 5463 7043 6f6e 6e65 6374  ....z.TcpConnect
+000004a0: 696f 6e2e 7265 6164 6c69 6e65 da04 6461  ion.readline..da
+000004b0: 7461 6302 0000 0000 0000 0000 0000 0002  tac.............
+000004c0: 0000 0003 0000 0043 0000 0073 1000 0000  .......C...s....
+000004d0: 7c00 6a00 a001 7c01 a101 0100 6400 5300  |.j...|.....d.S.
+000004e0: 721a 0000 0029 0272 0900 0000 da05 7772  r....).r......wr
+000004f0: 6974 6529 0272 0c00 0000 7220 0000 0072  ite).r....r ...r
+00000500: 0d00 0000 720d 0000 0072 0e00 0000 7221  ....r....r....r!
+00000510: 0000 001a 0000 0073 0200 0000 1001 7a13  .......s......z.
+00000520: 5463 7043 6f6e 6e65 6374 696f 6e2e 7772  TcpConnection.wr
+00000530: 6974 6563 0100 0000 0000 0000 0000 0000  itec............
+00000540: 0100 0000 0200 0000 c300 0000 7316 0000  ............s...
+00000550: 0081 017c 006a 00a0 01a1 0049 0064 0048  ...|.j.....I.d.H
+00000560: 0001 0064 0053 0072 1a00 0000 2902 7209  ...d.S.r....).r.
+00000570: 0000 00da 0564 7261 696e 720b 0000 0072  .....drainr....r
+00000580: 0d00 0000 720d 0000 0072 0e00 0000 7222  ....r....r....r"
+00000590: 0000 001d 0000 0073 0400 0000 0280 1401  .......s........
+000005a0: 7a13 5463 7043 6f6e 6e65 6374 696f 6e2e  z.TcpConnection.
+000005b0: 6472 6169 6e63 0100 0000 0000 0000 0000  drainc..........
+000005c0: 0000 0100 0000 0200 0000 c300 0000 7326  ..............s&
+000005d0: 0000 0081 017c 006a 00a0 01a1 0001 007c  .....|.j.......|
+000005e0: 006a 00a0 02a1 0049 0064 0048 0001 0064  .j.....I.d.H...d
+000005f0: 017c 005f 0364 0053 0072 0700 0000 2904  .|._.d.S.r....).
+00000600: 7209 0000 00da 0563 6c6f 7365 da0b 7761  r......close..wa
+00000610: 6974 5f63 6c6f 7365 6472 0a00 0000 720b  it_closedr....r.
+00000620: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000630: 0000 7223 0000 0020 0000 0073 0800 0000  ..r#... ...s....
+00000640: 0280 0a01 1001 0a01 7a13 5463 7043 6f6e  ........z.TcpCon
+00000650: 6e65 6374 696f 6e2e 636c 6f73 6563 0100  nection.closec..
+00000660: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00000670: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+00000680: 0072 1a00 0000 2901 720a 0000 0072 0b00  .r....).r....r..
+00000690: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+000006a0: 00da 0663 6c6f 7365 6425 0000 0073 0200  ...closed%...s..
+000006b0: 0000 0602 7a14 5463 7043 6f6e 6e65 6374  ....z.TcpConnect
+000006c0: 696f 6e2e 636c 6f73 6564 4e29 12da 085f  ion.closedN)..._
+000006d0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000006e0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000006f0: 5f72 0f00 0000 da03 7374 72da 0369 6e74  _r......str..int
+00000700: da05 666c 6f61 7472 1600 0000 da05 6279  ..floatr......by
+00000710: 7465 7372 1b00 0000 721e 0000 0072 1f00  tesr....r....r..
+00000720: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
+00000730: 00da 0870 726f 7065 7274 79da 0462 6f6f  ...property..boo
+00000740: 6c72 2500 0000 720d 0000 0072 0d00 0000  lr%...r....r....
+00000750: 720d 0000 0072 0e00 0000 7206 0000 0007  r....r....r.....
+00000760: 0000 0073 1600 0000 0800 0801 1605 1204  ...s............
+00000770: 1203 0e03 0e03 0803 0803 0205 1401 7206  ..............r.
+00000780: 0000 0029 0672 1300 0000 7202 0000 0072  ...).r....r....r
+00000790: 0300 0000 da04 6261 7365 7205 0000 0072  ......baser....r
+000007a0: 0600 0000 720d 0000 0072 0d00 0000 720d  ....r....r....r.
+000007b0: 0000 0072 0e00 0000 da08 3c6d 6f64 756c  ...r......<modul
+000007c0: 653e 0100 0000 7308 0000 0008 0010 010c  e>....s.........
+000007d0: 0214 03                                  ...
```

### Comparing `renats-0.2.1a0/renats/connection/base.py` & `renats-0.2.2a0/renats/connection/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 
 
-class BaseConnection(ABC):
+class Connection(ABC):
     @abstractmethod
     async def connect(self, host: str, port: int, timeout: float):
         raise NotImplementedError()
 
     @abstractmethod
     async def read(self, size: int) -> bytes:
         raise NotImplementedError()
@@ -22,14 +22,18 @@
     def write(self, data: bytes):
         raise NotImplementedError()
 
     @abstractmethod
     async def drain(self):
         raise NotImplementedError()
 
+    async def send(self, data: bytes):
+        self.write(data)
+        await self.drain()
+
     @abstractmethod
     async def close(self):
         raise NotImplementedError()
 
     @property
     @abstractmethod
     async def closed(self) -> bool:
```

### Comparing `renats-0.2.1a0/renats/connection/tcp.py` & `renats-0.2.2a0/renats/connection/tcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from asyncio import StreamReader, StreamWriter
 
-from .base import BaseConnection
+from .base import Connection
 
 
-class TcpConnection(BaseConnection):
+class TcpConnection(Connection):
     def __init__(self):
         self._reader: StreamReader | None = None
         self._writer: StreamWriter | None = None
         self._closed: bool = True
 
     async def connect(self, host: str, port: int, timeout: float):
         self._reader, self._writer = await asyncio.wait_for(asyncio.open_connection(host, port), timeout)
```

### Comparing `renats-0.2.1a0/renats/protocol/__pycache__/exceptions.cpython-310.pyc` & `renats-0.2.2a0/renats/protocol/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/__pycache__/protocol.cpython-310.pyc` & `renats-0.2.2a0/renats/protocol/__pycache__/protocol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/__pycache__/utils.cpython-310.pyc` & `renats-0.2.2a0/renats/protocol/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/exceptions.py` & `renats-0.2.2a0/renats/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/messages/__pycache__/base.cpython-310.pyc` & `renats-0.2.2a0/renats/protocol/messages/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/messages/__pycache__/msg.cpython-310.pyc` & `renats-0.2.2a0/renats/protocol/messages/__pycache__/msg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/messages/__pycache__/pub.cpython-310.pyc` & `renats-0.2.2a0/renats/protocol/messages/__pycache__/pub.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/messages/__pycache__/service.cpython-310.pyc` & `renats-0.2.2a0/renats/protocol/messages/__pycache__/service.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/messages/__pycache__/sub.cpython-310.pyc` & `renats-0.2.2a0/renats/protocol/messages/__pycache__/sub.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/messages/pub.py` & `renats-0.2.2a0/renats/protocol/messages/pub.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/messages/service.py` & `renats-0.2.2a0/renats/protocol/messages/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,7 @@
 
     def dump(self) -> bytes:
         """
         Dump NATS protocol CONNECT message to bytes
         :return: NATS protocol CONNECT message as bytes-encoded string
         """
         return b"CONNECT " + msgspec.json.encode(self) + b"\r\n"
-
-
-class ErrProtocolMessage(Struct):
-    """
-    NATS protocol message model for ERR message
-    """
-    error_message: str
```

### Comparing `renats-0.2.1a0/renats/protocol/messages/sub.py` & `renats-0.2.2a0/renats/protocol/messages/sub.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from msgspec import Struct
 
-from .base import SerializableProtocolMessage
 from .. import utils, protocol
 
 
 class SubProtocolMessage(Struct):
     """
     NATS protocol message model for SUB message
     """
```

### Comparing `renats-0.2.1a0/renats/protocol/protocol.py` & `renats-0.2.2a0/renats/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/renats/protocol/utils.py` & `renats-0.2.2a0/renats/protocol/utils.py`

 * *Files identical despite different names*

### Comparing `renats-0.2.1a0/PKG-INFO` & `renats-0.2.2a0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,79 @@
 Metadata-Version: 2.1
 Name: renats
-Version: 0.2.1a0
+Version: 0.2.2a0
 Summary: 
 Author: Respirens
 Author-email: thesergiyprotsanin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: msgspec (>=0.15.1,<0.16.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
+Requires-Dist: uuid6 (>=2023.5.2,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # ReNATS
 
 > Elegant, modern and asynchronous NATS Client API library written in pure Python
 
 ```python
-from renats.client import NATSClient
+import asyncio
+from renats.client import NATSClient, Message
 
+servers = (
+    ("127.0.0.1", 4222),
+)
 
-client = await NATSClient().connect("127.0.0.1", 4222)
+client = await NATSClient().connect(servers)
 
 # Publish message to subject 'my.subject' with payload 'My payload =)'
 await client.publish("my.subject", b"My payload =)")
 
 # Publish message to subject 'my.subject' with payload 'My payload =)',
 # reply subject 'my.reply.subject' and header 'MyHeader' with value 'MyValue'
 await client.publish(
     subject="my.subject",
-    data=b"My payload =)",
-    reply="my.reply.subject",
+    payload=b"My payload =)",
+    reply_subject="my.reply.subject",
     headers={
         "MyHeader": "MyValue"
     }
 )
 
+
+# Callbacks can be sync or async (def or async def)
+def callback(message: Message):
+    print(f"Received message in sync callback from {message.subject}: {message.payload}")
+
+
+async def async_callback(message: Message):
+    await asyncio.sleep(3)
+    print(f"Received message in async callback from {message.subject}: {message.payload}")
+
+
+subscription = await client.subscribe("foo.bar", callback)
+another_subscription = await client.subscribe("foo.baz", async_callback)
+
+await client.publish("foo.bar", b"Hello world! (to subscription with sync callback)")
+await client.publish("foo.baz", b"Hello world! (to subscription with async callback)")
+
+await subscription.unsubscribe()
+await another_subscription.unsubscribe()
+
 # Closing client
 await client.close()
 ```
 
 ### Installation
 ```bash
 pip install renats
 ```
 
----
-
 ### TODO
-- Subscriptions
 - Request-Reply
 - JetStream
 - ObjectStorage
 - Request-Reply API Framework for microservices
 - And more, maybe...
```

