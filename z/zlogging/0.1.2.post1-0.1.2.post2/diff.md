# Comparing `tmp/zlogging-0.1.2.post1.tar.gz` & `tmp/zlogging-0.1.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlogging-0.1.2.post1.tar", last modified: Sun Apr 23 07:35:24 2023, max compression
+gzip compressed data, was "zlogging-0.1.2.post2.tar", last modified: Mon Jun 12 03:18:00 2023, max compression
```

## Comparing `zlogging-0.1.2.post1.tar` & `zlogging-0.1.2.post2.tar`

### file list

```diff
@@ -1,41 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/archive/
--rw-r--r--   0 runner    (1001) docker     (123)    30794 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/archive/blogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/archive/logparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/archive/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/gen/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/gen/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/gen/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28119 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/tests/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/util/bump_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/zlogging/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_exc.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/zlogging/enum/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    53151 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-23 07:35:10.000000 zlogging-0.1.2.post1/zlogging/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 07:35:24.882061 zlogging-0.1.2.post1/zlogging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 07:35:24.000000 zlogging-0.1.2.post1/zlogging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.255431 zlogging-0.1.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:18:00.255431 zlogging-0.1.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.243431 zlogging-0.1.2.post2/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)    30794 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/archive/blogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/archive/logparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/archive/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:18:00.255431 zlogging-0.1.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.243431 zlogging-0.1.2.post2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28119 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.247431 zlogging-0.1.2.post2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/util/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/util/conda-build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/util/conda-dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/util/wheel_rename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.247431 zlogging-0.1.2.post2/zlogging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.255431 zlogging-0.1.2.post2/zlogging/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/af_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/dce_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/known.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/load_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/management_controller_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/management_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/mount3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/net_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/nfs3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/open_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/protocol_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/smb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/software.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/sum_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/weird.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/zeek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/zeekygen_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53151 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.247431 zlogging-0.1.2.post2/zlogging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/top_level.txt
```

### Comparing `zlogging-0.1.2.post1/LICENSE` & `zlogging-0.1.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/PKG-INFO` & `zlogging-0.1.2.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlogging
-Version: 0.1.2.post1
+Version: 0.1.2.post2
 Summary: zlogging: Bro/Zeek logging framework for Python.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/zlogging/
 Project-URL: documentation, https://jarryshaw.github.io/zlogging/
 Project-URL: repository, https://github.com/JarryShaw/zlogging
```

### Comparing `zlogging-0.1.2.post1/README.rst` & `zlogging-0.1.2.post2/README.rst`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/archive/blogging.py` & `zlogging-0.1.2.post2/archive/blogging.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/archive/logparser.py` & `zlogging-0.1.2.post2/archive/logparser.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/gen/make.py` & `zlogging-0.1.2.post2/zlogging/_gen.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 # -*- coding: utf-8 -*-
+"""Bro/Zeek enumeration namespace generator."""
 
+import argparse
 import collections
+import importlib
 import keyword
 import os
+import pathlib
 import re
 import shutil
 import subprocess  # nosec: B404
 import sys
 import textwrap
+import urllib.parse as urllib_parse
+
+###############################################################################
+# ``typing`` module support
+_local = sys.path.pop(0)
+###############################################################################
 
 import bs4
 import html2text
+import requests
+
+###############################################################################
+# ``typing`` module support
+sys.path.insert(0, _local)
+###############################################################################
 
-ROOT = os.path.dirname(os.path.abspath(__file__))
-PATH = os.path.abspath(os.path.join(ROOT, '..', 'zlogging', 'enum'))
-os.makedirs(PATH, exist_ok=True)
-shutil.rmtree(PATH)
-os.makedirs(PATH, exist_ok=True)
+ROOT = os.path.dirname(os.path.realpath(__file__))
+PATH = os.path.abspath(os.path.join(ROOT, 'enum'))
 
 # regular expression
-REGEX_ENUM = re.compile(r'((?P<namespace>[_a-z]+[_a-z0-9]*)::)?(?P<enum>[_a-z]+[_a-z0-9]*)', re.IGNORECASE)
+REGEX_ENUM = re.compile(r'((?P<namespace>([_a-z]+[_a-z0-9]*)(::[_a-z]+[_a-z0-9]*)*)::)?(?P<enum>[_a-z]+[_a-z0-9]*)', re.IGNORECASE)
 REGEX_LINK = re.compile(r'\[(?P<name>.*?)\]\(.*?\)', re.IGNORECASE)
 
 # file template
 TEMPLATE_ENUM = '''\
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long
 """Namespace: ``{namespace}``."""
@@ -64,170 +77,254 @@
         For back-port compatibility, the ``bro`` namespace is an alias of the
         ``zeek`` namespace.
 
     """
     if bare:
         enum_data = {}  # type: dict[str, Enum]
     else:
-        enum_data = _enum_zeek.copy()
+        enum_data = builtins.globals()['ZLogging::zeek'].copy()
     for namespace in namespaces:
         if namespace == 'bro':
             warnings.warn("Use of 'bro' is deprecated. "
                           "Please use 'zeek' instead.", BroDeprecationWarning)
             namespace = 'zeek'
 
-        enum_dict = builtins.globals().get('_enum_%s' % namespace)  # pylint: disable=consider-using-f-string
+        enum_dict = builtins.globals().get('ZLogging::%s' % namespace)  # pylint: disable=consider-using-f-string
         if enum_dict is None:
             raise ValueError('undefined namespace: %s' % namespace)  # pylint: disable=consider-using-f-string
         enum_data.update(enum_dict)
     return enum_data
 '''
 
 
-file_list = []  # type: list[str]
-for dirpath, _, filenames in os.walk(os.path.join(ROOT, 'sources')):
-    file_list.extend(map(
-        lambda name: os.path.join(ROOT, 'sources', dirpath, name),  # pylint: disable=cell-var-from-loop
-        filter(lambda name: os.path.splitext(name)[1] == '.html', filenames)
-    ))
-
-# namespace, enum, name
-enum_records = []  # type: list[tuple[str, str, str, str]]
-
-# postpone checks
-dest_list = []
-for html_file in sorted(file_list):
-    print(f'+ {html_file}')
-    with open(html_file, encoding='utf-8') as file:
-        html = file.read()
-
-    soup = bs4.BeautifulSoup(html, 'html5lib')
-    for tag in soup.select('dl.type'):
-        descname = tag.select('dt code.descname')
-        if not descname:
-            continue
-        name = descname[0].text.strip()
-        print(f'++ {name}')
+def fetch() -> 'None':
+    """Fetch Bro/Zeek documentation.
 
-        selected = tag.select('dd td p.first span.pre')
-        if not selected:
-            continue
-        type = selected[0].text.strip()  # pylint: disable=redefined-builtin
-        if type != 'enum':
+    Args:
+        caching: Enable caching files.
+
+    """
+    link = 'https://docs.zeek.org/en/stable/script-reference/scripts.html'
+    resp = requests.get(link)  # nosec B113
+    if not resp.ok:
+        raise RuntimeError(resp)
+
+    page = resp.text
+    soup = bs4.BeautifulSoup(page, 'html5lib')
+    for tag in soup.select('.toctree-wrapper li > a'):
+        print(f'+ {tag.text}')
+
+        href = tag.get('href')
+        if href is None:
+            raise RuntimeError(tag)
+        name = pathlib.PurePosixPath(tag.text)
+        path = pathlib.Path(os.path.join(ROOT, '_cache', *name.parts))
+        if os.path.isfile(f'{path}.html'):
             continue
 
-        enum_list = []
-        for dl in tag.select('dd td dl.enum'):
-            enum_name = dl.select('dt code.descname')[0].text.strip()
-            enum_docs = dl.select('dd')[0].text.strip()
-            enum_list.append((enum_name, enum_docs))
-
-        docs_list = []
-        for p in tag.select('dd')[0].children:
-            if p.name != 'p':
+        dest = urllib_parse.urljoin(link, href)
+        docs = requests.get(dest)  # nosec B113
+        if not docs.ok:
+            raise RuntimeError(docs)
+
+        os.makedirs(path.parent, exist_ok=True)
+        with open(f'{path}.html', 'wb') as file:
+            file.write(docs.content)
+
+
+def make() -> 'None':
+    """Make Bro/Zeek enumeration namespace."""
+    if os.path.exists(PATH):
+        shutil.rmtree(PATH)
+    os.makedirs(PATH, exist_ok=True)
+
+    file_list = []  # type: list[str]
+    for dirpath, _, filenames in os.walk(os.path.join(ROOT, '_cache')):
+        file_list.extend(map(
+            lambda name: os.path.join(ROOT, '_cache', dirpath, name),  # pylint: disable=cell-var-from-loop
+            filter(lambda name: os.path.splitext(name)[1] == '.html', filenames)
+        ))
+
+    # namespace, module_name, enum, name, enum_name
+    enum_records = []  # type: list[tuple[str, str, str, str, str]]
+
+    # postpone checks
+    dest_list = []
+    for html_file in sorted(file_list):
+        print(f'+ {html_file}')
+        with open(html_file, encoding='utf-8') as file:
+            html = file.read()
+
+        soup = bs4.BeautifulSoup(html, 'html5lib')
+        for tag in soup.select('dl.type'):
+            descname = tag.select('dt.sig span.pre')
+            if not descname:
                 continue
-            docs = '\n    '.join(
-                textwrap.wrap(
-                    REGEX_LINK.sub(
-                        r'\g<name>',
-                        html2text.html2text(
-                            str(p).replace('\n', ' ')
-                        ).replace('\n', ' ')
-                    ).replace('`', '``').strip(),
-                    100, break_on_hyphens=False,
-                )
-            )
-            if not docs.endswith('.'):
-                docs += '.'
-            docs_list.append(docs)
-
-        match = REGEX_ENUM.fullmatch(name)
-        if match is None:
-            raise ValueError(name)
+            name = descname[0].text.strip()
 
-        namespace = match.group('namespace')
-        if namespace is None:
-            namespace = 'zeek'
-        enum_name = match.group('enum')
+            selected = tag.select('dd dl p')
+            if not selected:
+                print(f'++ {name} (no type)')
+                continue
 
-        dest = os.path.join(PATH, f'{namespace}.py')
-        if not os.path.isfile(dest):
-            with open(dest, 'w', encoding='utf-8') as file:
-                file.write(TEMPLATE_ENUM.format(namespace=namespace))
-        docs_list.insert(0, f'Enum: ``{name}``.')
+            type = selected[0].text.strip()  # pylint: disable=redefined-builtin
+            print(f'++ {name} ({type})')
+            if type != 'enum':
+                continue
 
-        html_path = os.path.splitext(os.path.relpath(html_file, os.path.join(ROOT, 'sources')))[0]
-        docs_list.append(f'See Also:\n        `{html_path} <https://docs.zeek.org/en/stable/scripts/{html_path}.html#type-{name}>`__\n\n    ')  # pylint: disable=line-too-long
+            enum_list = []
+            for dl in tag.select('dd dl dl.enum'):
+                enum_name = dl.select('dt.sig span.pre')[0].text.strip()
+                enum_docs = dl.select('dd')[0].text.strip()
+                enum_list.append((enum_name, enum_docs))
+
+            docs_list = []
+            for p in tag.select('dd')[0].children:
+                if p.name != 'p':
+                    continue
+                docs = '\n    '.join(
+                    textwrap.wrap(
+                        REGEX_LINK.sub(
+                            r'\g<name>',
+                            html2text.html2text(
+                                str(p).replace('\n', ' ')
+                            ).replace('\n', ' ')
+                        ).replace('`', '``').strip(),
+                        100, break_on_hyphens=False,
+                    )
+                )
+                if not docs.endswith('.'):
+                    docs += '.'
+                docs_list.append(docs)
+
+            match = REGEX_ENUM.fullmatch(name)
+            if match is None:
+                raise ValueError(name)
+
+            namespace = match.group('namespace')
+            if namespace is None:
+                namespace = 'zeek'
+            enum_name = match.group('enum')
+            print(f'+++ {namespace}::{enum_name}')
+
+            ns_parts = namespace.replace('::', '_').split('_')
+            for index, part in enumerate(ns_parts):
+                if part.isupper():
+                    ns_parts[index] = part.lower()
+                else:
+                    ns_parts[index] = re.sub(r'([A-Z])', r'_\1', part).lower().lstrip('_')
+            module_name = '_'.join(ns_parts)
 
-        enum_docs = '\n\n    '.join(docs_list)
-        with open(dest, 'a', encoding='utf-8') as file:
-            print('', file=file)
-            print('', file=file)
-            print('@enum.unique', file=file)
-            print(f'class {enum_name}(enum.IntFlag):', file=file)
-            if enum_docs:
-                print(f'    """{enum_docs}"""', file=file)
-                print('', file=file)
-            print(f"    _ignore_ = '{enum_name} _'", file=file)
-            print(f'    {enum_name} = vars()', file=file)
-            print('', file=file)
+            dest = os.path.join(PATH, f'{module_name}.py')
+            if not os.path.isfile(dest):
+                with open(dest, 'w', encoding='utf-8') as file:
+                    file.write(TEMPLATE_ENUM.format(namespace=namespace))
+            docs_list.insert(0, f'Enum: ``{name}``.')
 
-            length = len(enum_list)
-            for index, (enum, docs) in enumerate(enum_list, start=1):
-                safe_docs = docs.replace('\n', '\n    #: ').replace('_', r'\_')
-                safe_enum = re.sub(f'{namespace}::', '', enum)
-                if '::' in safe_enum:
-                    safe_docs = f'{enum}\n    #: ' + safe_docs
-                    safe_enum = safe_enum.replace('::', '_')
-                if safe_docs:
-                    print(f'    #: {safe_docs}', file=file)
-                if keyword.iskeyword(safe_enum):
-                    print(f'    {enum_name}[{safe_enum!r}] = enum.auto()', file=file)
-                else:
-                    print(f'    {safe_enum} = enum.auto()', file=file)
-                if index != length:
+            html_path = os.path.splitext(os.path.relpath(html_file, os.path.join(ROOT, '_cache')))[0]
+            docs_list.append(f'See Also:\n        `{html_path} <https://docs.zeek.org/en/stable/scripts/{html_path}.html#type-{name}>`__\n\n    ')  # pylint: disable=line-too-long
+
+            enum_docs = '\n\n    '.join(docs_list)
+            with open(dest, 'a', encoding='utf-8') as file:
+                print('', file=file)
+                print('', file=file)
+                print('@enum.unique', file=file)
+                print(f'class {enum_name}(enum.IntFlag):', file=file)
+                if enum_docs:
+                    print(f'    """{enum_docs}"""', file=file)
                     print('', file=file)
-                enum_records.append((namespace, enum_name, enum, safe_enum))
+                print(f"    _ignore_ = '{enum_name} _'", file=file)
+                print(f'    {enum_name} = vars()', file=file)
+                print('', file=file)
 
-        dest_list.append(dest)
+                length = len(enum_list)
+                for index, (enum, docs) in enumerate(enum_list, start=1):
+                    safe_docs = docs.replace('\n', '\n    #: ').replace('_', r'\_')
+                    safe_enum = re.sub(f'{namespace}::', '', enum)
+                    if '::' in safe_enum:
+                        safe_docs = f'{enum}\n    #: ' + safe_docs
+                        safe_enum = safe_enum.replace('::', '_')
+                    if safe_docs:
+                        print(f'    #: {safe_docs}', file=file)
+                    if keyword.iskeyword(safe_enum):
+                        print(f'    {enum_name}[{safe_enum!r}] = enum.auto()', file=file)
+                    else:
+                        print(f'    {safe_enum} = enum.auto()', file=file)
+                    if index != length:
+                        print('', file=file)
+                    enum_records.append((namespace, module_name, enum_name, enum, safe_enum))
+
+            dest_list.append(dest)
+
+    imported = []
+    enum_line = collections.defaultdict(list)
+    with open(os.path.join(PATH, '__init__.py'), 'w', encoding='utf-8') as file:
+        file.write(TEMPLATE_INIT)
+        for namespace, module_name, enum, name, enum_name in sorted(enum_records):
+            safe_namespace = namespace.replace('::', '_')
+            if (namespace, enum) not in imported:
+                print(f'from zlogging.enum.{module_name} import {enum} as {safe_namespace}_{enum}', file=file)
+                imported.append((namespace, enum))
+
+                enum_line[namespace].append(f'    {enum!r}: {safe_namespace}_{enum},')
+
+            match = REGEX_ENUM.fullmatch(name)
+            if match is None:
+                raise ValueError(name)
+            match_namespace = match.group('namespace')
+            if match_namespace is None:
+                match_namespace = namespace
+            safe_name = match.group('enum')
+            if keyword.iskeyword(enum_name):
+                enum_line[match_namespace].append(f'    {safe_name!r}: {safe_namespace}_{enum}[{enum_name!r}],  # type: ignore[misc]')  # pylint: disable=line-too-long
+            else:
+                enum_line[match_namespace].append(f'    {enum_name!r}: {safe_namespace}_{enum}.{enum_name},')
+        print('', file=file)
+        print("__all__ = ['globals']", file=file)
+        print('', file=file)
+        print('if TYPE_CHECKING:', file=file)
+        print('    from enum import Enum', file=file)
+        print('', file=file)
 
-imported = []
-enum_line = collections.defaultdict(list)
-with open(os.path.join(PATH, '__init__.py'), 'w', encoding='utf-8') as file:
-    file.write(TEMPLATE_INIT)
-    for namespace, enum, name, enum_name in sorted(enum_records):
-        if (namespace, enum) not in imported:
-            print(f'from zlogging.enum.{namespace} import {enum} as {namespace}_{enum}', file=file)
-            imported.append((namespace, enum))
-
-            enum_line[namespace].append(f'    {enum!r}: {namespace}_{enum},')
-
-        match = REGEX_ENUM.fullmatch(name)
-        if match is None:
-            raise ValueError(name)
-        safe_namespace = match.group('namespace')
-        if safe_namespace is None:
-            safe_namespace = namespace
-        safe_name = match.group('enum')
-        if keyword.iskeyword(enum_name):
-            enum_line[safe_namespace].append(f'    {safe_name!r}: {namespace}_{enum}[{enum_name!r}],  # type: ignore[misc]')  # pylint: disable=line-too-long
-        else:
-            enum_line[safe_namespace].append(f'    {enum_name!r}: {namespace}_{enum}.{enum_name},')
-    print('', file=file)
-    print("__all__ = ['globals']", file=file)
-    print('', file=file)
-    print('if TYPE_CHECKING:', file=file)
-    print('    from enum import Enum', file=file)
-    print('', file=file)
-
-    for namespace in sorted(enum_line):
-        print(f'_enum_{namespace} = {{', file=file)
-        for line in sorted(enum_line[namespace]):
-            print(line, file=file)
-        print('}', file=file)
+        for namespace in sorted(enum_line):
+            print(f"builtins.globals()['ZLogging::{namespace}'] = {{", file=file)
+            for line in sorted(enum_line[namespace]):
+                print(line, file=file)
+            print('}', file=file)
+            print('', file=file)
         print('', file=file)
-    print('', file=file)
-    file.write(TEMPLATE_FUNC)
+        file.write(TEMPLATE_FUNC)
+
+
+def test() -> 'None':
+    """Test the generated code."""
+    module = importlib.import_module('zlogging.enum')
+    assert 'tcp' in module.globals()  # nosec B101
+
+    for dest in filter(lambda x: x.endswith('.py'), os.listdir(PATH)):
+        if dest == '__init__.py':
+            continue
+
+        module_name = os.path.splitext(dest)[0]
+        importlib.import_module(f'zlogging.enum.{module_name}')
+
+
+def main() -> 'int':
+    """Entrypoint."""
+    parser = argparse.ArgumentParser(prog='zlogging-vendor',
+                                     description='update Bro/Zeek enumeration namespace')
+    parser.add_argument('-c', '--caching', action='store_true',
+                        help='use cached downloaded files')
+
+    args = parser.parse_args()
+    if not args.caching and os.path.exists(os.path.join(ROOT, '_cache')):
+        shutil.rmtree(os.path.join(ROOT, '_cache'))
+
+    fetch()
+    make()
+    test()
+
+    return 0
+
 
-subprocess.check_call([sys.executable, os.path.join(PATH, '__init__.py')])  # nosec: B603
-for dest in dest_list:
-    subprocess.check_call([sys.executable, dest])  # nosec: B603
+if __name__ == '__main__':
+    sys.exit(main())
```

### Comparing `zlogging-0.1.2.post1/pyproject.toml` & `zlogging-0.1.2.post2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 [build-system]
 requires = [
     "setuptools>=61.0.0",
+
+    # version compatibility
+    "bpc-f2format; python_version < '3.6'",
+    "bpc-poseur; python_version < '3.8'",
+    "bpc-walrus; python_version < '3.8'",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zlogging"
 dynamic = [ "version", "readme" ]
 authors = [
@@ -27,25 +32,33 @@
     'Topic :: Software Development',
     'Topic :: Utilities',
 ]
 dependencies = [
     'typing-inspect',
     'typing_extensions',
 
+    # PyBPC
+    "bpc-f2format; python_version < '3.6'",
+    "bpc-poseur; python_version < '3.8'",
+    "bpc-walrus; python_version < '3.8'",
+
     # version compatibility
     'dataclasses; python_version < "3.7"',
     'aenum; python_version < "3.7"',
 ]
 
 [project.urls]
 homepage = "https://jarryshaw.github.io/zlogging/"
 documentation = "https://jarryshaw.github.io/zlogging/"
 repository = "https://github.com/JarryShaw/zlogging"
 changelog = "https://github.com/JarryShaw/zlogging/releases"
 
+[project.scripts]
+zlogging-gen = "zlogging._gen:main"
+
 [project.optional-dependencies]
 docs = [
     "Sphinx>=6.1.3",
     "sphinx-autodoc-typehints", "sphinx-opengraph", "sphinx-copybutton",
     "furo",
 ]
```

### Comparing `zlogging-0.1.2.post1/tests/test_types.py` & `zlogging-0.1.2.post2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/util/bump_version.py` & `zlogging-0.1.2.post2/util/bump_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,7 +54,10 @@
         if line.startswith('__version__'):
             line = f'__version__ = {new_ver!r}'
         contents.append(line)
 
 with open (path, 'w', encoding='utf-8') as out_file:
     out_file.writelines(contents)
     out_file.write('\n')
+
+with open(os.path.join('conda', 'build'), 'w') as build:
+    build.write('0')
```

### Comparing `zlogging-0.1.2.post1/zlogging/__init__.py` & `zlogging-0.1.2.post2/zlogging/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 # -*- coding: utf-8 -*-
 """Bro/Zeek logging framework."""
 
+###############################################################################
+# conda ``_extern`` module support
+
+import os
+import sys
+
+_extern = os.path.join(os.path.dirname(os.path.realpath(__file__)), '_extern')
+if os.path.exists(_extern):
+    sys.path.append(_extern)
+
+###############################################################################
+
 from zlogging.dumper import dump, dumps, write
 from zlogging.loader import load, loads, parse
 from zlogging.model import Model, new_model
 from zlogging.types import (AddrType, BoolType, CountType, DoubleType, EnumType, IntervalType,
                             IntType, PortType, RecordType, SetType, StringType, SubnetType,
                             TimeType, VectorType)
 
@@ -16,8 +28,8 @@
 
     'AddrType', 'BoolType', 'CountType', 'DoubleType', 'EnumType',
     'IntervalType', 'IntType', 'PortType', 'RecordType', 'SetType',
     'StringType', 'SubnetType', 'TimeType', 'VectorType',
 ]
 
 # version string
-__version__ = '0.1.2.post1'
+__version__ = '0.1.2.post2'
```

### Comparing `zlogging-0.1.2.post1/zlogging/_aux.py` & `zlogging-0.1.2.post2/zlogging/_aux.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging/_compat.py` & `zlogging-0.1.2.post2/zlogging/_compat.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging/_data.py` & `zlogging-0.1.2.post2/zlogging/_data.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging/_exc.py` & `zlogging-0.1.2.post2/zlogging/_exc.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging/_typing.py` & `zlogging-0.1.2.post2/zlogging/_typing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging/dumper.py` & `zlogging-0.1.2.post2/zlogging/dumper.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging/loader.py` & `zlogging-0.1.2.post2/zlogging/loader.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging/model.py` & `zlogging-0.1.2.post2/zlogging/model.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging/types.py` & `zlogging-0.1.2.post2/zlogging/types.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging/typing.py` & `zlogging-0.1.2.post2/zlogging/typing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post1/zlogging.egg-info/PKG-INFO` & `zlogging-0.1.2.post2/zlogging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlogging
-Version: 0.1.2.post1
+Version: 0.1.2.post2
 Summary: zlogging: Bro/Zeek logging framework for Python.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/zlogging/
 Project-URL: documentation, https://jarryshaw.github.io/zlogging/
 Project-URL: repository, https://github.com/JarryShaw/zlogging
```

