# Comparing `tmp/zlogging-0.1.2.post4.tar.gz` & `tmp/zlogging-0.1.2.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlogging-0.1.2.post4.tar", last modified: Mon Jun 12 03:40:39 2023, max compression
+gzip compressed data, was "zlogging-0.1.2.post5.tar", last modified: Mon Jun 12 03:58:46 2023, max compression
```

## Comparing `zlogging-0.1.2.post4.tar` & `zlogging-0.1.2.post5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:40:39.109835 zlogging-0.1.2.post4/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:40:39.109835 zlogging-0.1.2.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:40:39.077835 zlogging-0.1.2.post4/archive/
--rw-r--r--   0 runner    (1001) docker     (123)    30794 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/archive/blogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/archive/logparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/archive/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:40:39.109835 zlogging-0.1.2.post4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:40:39.077835 zlogging-0.1.2.post4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28119 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/tests/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:40:39.081835 zlogging-0.1.2.post4/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/util/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/util/conda-build.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/util/conda-dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/util/enum_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/util/wheel_rename.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:40:39.085835 zlogging-0.1.2.post4/zlogging/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/_exc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:40:39.109835 zlogging-0.1.2.post4/zlogging/enum/
--rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/af_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/dce_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/known.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/load_balancing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/management.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/management_controller_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/management_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/mount3.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/net_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/nfs3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/open_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/protocol_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/smb.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/software.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/sum_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/weird.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/zeek.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/enum/zeekygen_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    53151 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-06-12 03:40:24.000000 zlogging-0.1.2.post4/zlogging/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:40:39.089835 zlogging-0.1.2.post4/zlogging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:40:39.000000 zlogging-0.1.2.post4/zlogging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-12 03:40:39.000000 zlogging-0.1.2.post4/zlogging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:40:39.000000 zlogging-0.1.2.post4/zlogging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 03:40:39.000000 zlogging-0.1.2.post4/zlogging.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:40:38.000000 zlogging-0.1.2.post4/zlogging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 03:40:39.000000 zlogging-0.1.2.post4/zlogging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 03:40:39.000000 zlogging-0.1.2.post4/zlogging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:58:46.361223 zlogging-0.1.2.post5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:58:46.361223 zlogging-0.1.2.post5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:58:46.353223 zlogging-0.1.2.post5/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)    30794 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/archive/blogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/archive/logparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/archive/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:58:46.361223 zlogging-0.1.2.post5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:58:46.353223 zlogging-0.1.2.post5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28119 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:58:46.353223 zlogging-0.1.2.post5/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/util/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/util/conda-build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/util/conda-dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/util/enum_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/util/wheel_rename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:58:46.357223 zlogging-0.1.2.post5/zlogging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/_exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:58:46.361223 zlogging-0.1.2.post5/zlogging/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/af_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/dce_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/known.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/load_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/management_controller_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/management_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/mount3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/net_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/nfs3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/open_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/protocol_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/smb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/software.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/sum_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/weird.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/zeek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/enum/zeekygen_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53151 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-06-12 03:58:36.000000 zlogging-0.1.2.post5/zlogging/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:58:46.357223 zlogging-0.1.2.post5/zlogging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:58:46.000000 zlogging-0.1.2.post5/zlogging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-12 03:58:46.000000 zlogging-0.1.2.post5/zlogging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:58:46.000000 zlogging-0.1.2.post5/zlogging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 03:58:46.000000 zlogging-0.1.2.post5/zlogging.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:58:46.000000 zlogging-0.1.2.post5/zlogging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 03:58:46.000000 zlogging-0.1.2.post5/zlogging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 03:58:46.000000 zlogging-0.1.2.post5/zlogging.egg-info/top_level.txt
```

### Comparing `zlogging-0.1.2.post4/LICENSE` & `zlogging-0.1.2.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/PKG-INFO` & `zlogging-0.1.2.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlogging
-Version: 0.1.2.post4
+Version: 0.1.2.post5
 Summary: zlogging: Bro/Zeek logging framework for Python.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/zlogging/
 Project-URL: documentation, https://jarryshaw.github.io/zlogging/
 Project-URL: repository, https://github.com/JarryShaw/zlogging
```

### Comparing `zlogging-0.1.2.post4/README.rst` & `zlogging-0.1.2.post5/README.rst`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/archive/blogging.py` & `zlogging-0.1.2.post5/archive/blogging.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/archive/logparser.py` & `zlogging-0.1.2.post5/archive/logparser.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/pyproject.toml` & `zlogging-0.1.2.post5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/setup.py` & `zlogging-0.1.2.post5/setup.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/tests/test_types.py` & `zlogging-0.1.2.post5/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/util/bump_version.py` & `zlogging-0.1.2.post5/util/bump_version.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/util/enum_docs.py` & `zlogging-0.1.2.post5/util/enum_docs.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/util/wheel_rename.py` & `zlogging-0.1.2.post5/util/wheel_rename.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/__init__.py` & `zlogging-0.1.2.post5/zlogging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 
     'AddrType', 'BoolType', 'CountType', 'DoubleType', 'EnumType',
     'IntervalType', 'IntType', 'PortType', 'RecordType', 'SetType',
     'StringType', 'SubnetType', 'TimeType', 'VectorType',
 ]
 
 # version string
-__version__ = '0.1.2.post4'
+__version__ = '0.1.2.post5'
```

### Comparing `zlogging-0.1.2.post4/zlogging/_aux.py` & `zlogging-0.1.2.post5/zlogging/_aux.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/_compat.py` & `zlogging-0.1.2.post5/zlogging/_compat.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/_data.py` & `zlogging-0.1.2.post5/zlogging/_data.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/_exc.py` & `zlogging-0.1.2.post5/zlogging/_exc.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/_gen.py` & `zlogging-0.1.2.post5/zlogging/_gen.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/_typing.py` & `zlogging-0.1.2.post5/zlogging/_typing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/dumper.py` & `zlogging-0.1.2.post5/zlogging/dumper.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/__init__.py` & `zlogging-0.1.2.post5/zlogging/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/af_packet.py` & `zlogging-0.1.2.post5/zlogging/enum/af_packet.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/broker.py` & `zlogging-0.1.2.post5/zlogging/enum/broker.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/cluster.py` & `zlogging-0.1.2.post5/zlogging/enum/cluster.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/dce_rpc.py` & `zlogging-0.1.2.post5/zlogging/enum/dce_rpc.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/http.py` & `zlogging-0.1.2.post5/zlogging/enum/http.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/input.py` & `zlogging-0.1.2.post5/zlogging/enum/input.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/intel.py` & `zlogging-0.1.2.post5/zlogging/enum/intel.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/json.py` & `zlogging-0.1.2.post5/zlogging/enum/json.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/known.py` & `zlogging-0.1.2.post5/zlogging/enum/known.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/load_balancing.py` & `zlogging-0.1.2.post5/zlogging/enum/load_balancing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/log.py` & `zlogging-0.1.2.post5/zlogging/enum/log.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/management.py` & `zlogging-0.1.2.post5/zlogging/enum/management.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/management_controller_runtime.py` & `zlogging-0.1.2.post5/zlogging/enum/management_controller_runtime.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/management_log.py` & `zlogging-0.1.2.post5/zlogging/enum/management_log.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/mount3.py` & `zlogging-0.1.2.post5/zlogging/enum/mount3.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/net_control.py` & `zlogging-0.1.2.post5/zlogging/enum/net_control.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/nfs3.py` & `zlogging-0.1.2.post5/zlogging/enum/nfs3.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/notice.py` & `zlogging-0.1.2.post5/zlogging/enum/notice.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/open_flow.py` & `zlogging-0.1.2.post5/zlogging/enum/open_flow.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/pcap.py` & `zlogging-0.1.2.post5/zlogging/enum/pcap.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/protocol_detector.py` & `zlogging-0.1.2.post5/zlogging/enum/protocol_detector.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/signatures.py` & `zlogging-0.1.2.post5/zlogging/enum/signatures.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/smb.py` & `zlogging-0.1.2.post5/zlogging/enum/smb.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/socks.py` & `zlogging-0.1.2.post5/zlogging/enum/socks.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/software.py` & `zlogging-0.1.2.post5/zlogging/enum/software.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/ssl.py` & `zlogging-0.1.2.post5/zlogging/enum/ssl.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/sum_stats.py` & `zlogging-0.1.2.post5/zlogging/enum/sum_stats.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/supervisor.py` & `zlogging-0.1.2.post5/zlogging/enum/supervisor.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/telemetry.py` & `zlogging-0.1.2.post5/zlogging/enum/telemetry.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/tunnel.py` & `zlogging-0.1.2.post5/zlogging/enum/tunnel.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/weird.py` & `zlogging-0.1.2.post5/zlogging/enum/weird.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/zeek.py` & `zlogging-0.1.2.post5/zlogging/enum/zeek.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/enum/zeekygen_example.py` & `zlogging-0.1.2.post5/zlogging/enum/zeekygen_example.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/loader.py` & `zlogging-0.1.2.post5/zlogging/loader.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/model.py` & `zlogging-0.1.2.post5/zlogging/model.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/types.py` & `zlogging-0.1.2.post5/zlogging/types.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging/typing.py` & `zlogging-0.1.2.post5/zlogging/typing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post4/zlogging.egg-info/PKG-INFO` & `zlogging-0.1.2.post5/zlogging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlogging
-Version: 0.1.2.post4
+Version: 0.1.2.post5
 Summary: zlogging: Bro/Zeek logging framework for Python.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/zlogging/
 Project-URL: documentation, https://jarryshaw.github.io/zlogging/
 Project-URL: repository, https://github.com/JarryShaw/zlogging
```

### Comparing `zlogging-0.1.2.post4/zlogging.egg-info/SOURCES.txt` & `zlogging-0.1.2.post5/zlogging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

