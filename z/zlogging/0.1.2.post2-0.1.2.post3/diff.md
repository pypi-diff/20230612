# Comparing `tmp/zlogging-0.1.2.post2.tar.gz` & `tmp/zlogging-0.1.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlogging-0.1.2.post2.tar", last modified: Mon Jun 12 03:18:00 2023, max compression
+gzip compressed data, was "zlogging-0.1.2.post3.tar", last modified: Mon Jun 12 03:30:22 2023, max compression
```

## Comparing `zlogging-0.1.2.post2.tar` & `zlogging-0.1.2.post3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.255431 zlogging-0.1.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:18:00.255431 zlogging-0.1.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.243431 zlogging-0.1.2.post2/archive/
--rw-r--r--   0 runner    (1001) docker     (123)    30794 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/archive/blogging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/archive/logparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/archive/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:18:00.255431 zlogging-0.1.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.243431 zlogging-0.1.2.post2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28119 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/tests/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.247431 zlogging-0.1.2.post2/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/util/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/util/conda-build.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/util/conda-dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/util/wheel_rename.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.247431 zlogging-0.1.2.post2/zlogging/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_exc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.255431 zlogging-0.1.2.post2/zlogging/enum/
--rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/af_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/dce_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/known.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/load_balancing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/management.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/management_controller_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/management_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/mount3.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/net_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/nfs3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/open_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/protocol_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/smb.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/software.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/sum_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/weird.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/zeek.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/enum/zeekygen_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    53151 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-06-12 03:17:47.000000 zlogging-0.1.2.post2/zlogging/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:18:00.247431 zlogging-0.1.2.post2/zlogging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 03:18:00.000000 zlogging-0.1.2.post2/zlogging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:30:22.472408 zlogging-0.1.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-12 03:30:11.000000 zlogging-0.1.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 03:30:11.000000 zlogging-0.1.2.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:30:22.472408 zlogging-0.1.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-06-12 03:30:11.000000 zlogging-0.1.2.post3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:30:22.464408 zlogging-0.1.2.post3/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)    30794 2023-06-12 03:30:11.000000 zlogging-0.1.2.post3/archive/blogging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-12 03:30:11.000000 zlogging-0.1.2.post3/archive/logparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 03:30:11.000000 zlogging-0.1.2.post3/archive/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:30:22.472408 zlogging-0.1.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:30:22.464408 zlogging-0.1.2.post3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28119 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:30:22.464408 zlogging-0.1.2.post3/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/util/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/util/conda-build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/util/conda-dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/util/wheel_rename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:30:22.464408 zlogging-0.1.2.post3/zlogging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/_exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25373 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:30:22.472408 zlogging-0.1.2.post3/zlogging/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/af_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/dce_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/known.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/load_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/management_controller_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/management_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/mount3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/net_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/nfs3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/open_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/protocol_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/smb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/software.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/sum_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/weird.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/zeek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/enum/zeekygen_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53151 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-06-12 03:30:12.000000 zlogging-0.1.2.post3/zlogging/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:30:22.468408 zlogging-0.1.2.post3/zlogging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-06-12 03:30:22.000000 zlogging-0.1.2.post3/zlogging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-12 03:30:22.000000 zlogging-0.1.2.post3/zlogging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:30:22.000000 zlogging-0.1.2.post3/zlogging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 03:30:22.000000 zlogging-0.1.2.post3/zlogging.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:30:22.000000 zlogging-0.1.2.post3/zlogging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 03:30:22.000000 zlogging-0.1.2.post3/zlogging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 03:30:22.000000 zlogging-0.1.2.post3/zlogging.egg-info/top_level.txt
```

### Comparing `zlogging-0.1.2.post2/LICENSE` & `zlogging-0.1.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/PKG-INFO` & `zlogging-0.1.2.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlogging
-Version: 0.1.2.post2
+Version: 0.1.2.post3
 Summary: zlogging: Bro/Zeek logging framework for Python.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/zlogging/
 Project-URL: documentation, https://jarryshaw.github.io/zlogging/
 Project-URL: repository, https://github.com/JarryShaw/zlogging
```

### Comparing `zlogging-0.1.2.post2/README.rst` & `zlogging-0.1.2.post3/README.rst`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/archive/blogging.py` & `zlogging-0.1.2.post3/archive/blogging.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/archive/logparser.py` & `zlogging-0.1.2.post3/archive/logparser.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/pyproject.toml` & `zlogging-0.1.2.post3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/setup.py` & `zlogging-0.1.2.post3/setup.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/tests/test_types.py` & `zlogging-0.1.2.post3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/util/bump_version.py` & `zlogging-0.1.2.post3/util/bump_version.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/util/wheel_rename.py` & `zlogging-0.1.2.post3/util/wheel_rename.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/__init__.py` & `zlogging-0.1.2.post3/zlogging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 
     'AddrType', 'BoolType', 'CountType', 'DoubleType', 'EnumType',
     'IntervalType', 'IntType', 'PortType', 'RecordType', 'SetType',
     'StringType', 'SubnetType', 'TimeType', 'VectorType',
 ]
 
 # version string
-__version__ = '0.1.2.post2'
+__version__ = '0.1.2.post3'
```

### Comparing `zlogging-0.1.2.post2/zlogging/_aux.py` & `zlogging-0.1.2.post3/zlogging/_aux.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/_compat.py` & `zlogging-0.1.2.post3/zlogging/_compat.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/_data.py` & `zlogging-0.1.2.post3/zlogging/_data.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/_exc.py` & `zlogging-0.1.2.post3/zlogging/_exc.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/_gen.py` & `zlogging-0.1.2.post3/zlogging/_gen.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/_typing.py` & `zlogging-0.1.2.post3/zlogging/_typing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/dumper.py` & `zlogging-0.1.2.post3/zlogging/dumper.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/__init__.py` & `zlogging-0.1.2.post3/zlogging/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/af_packet.py` & `zlogging-0.1.2.post3/zlogging/enum/af_packet.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/broker.py` & `zlogging-0.1.2.post3/zlogging/enum/broker.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/cluster.py` & `zlogging-0.1.2.post3/zlogging/enum/cluster.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/dce_rpc.py` & `zlogging-0.1.2.post3/zlogging/enum/dce_rpc.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/http.py` & `zlogging-0.1.2.post3/zlogging/enum/http.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/input.py` & `zlogging-0.1.2.post3/zlogging/enum/input.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/intel.py` & `zlogging-0.1.2.post3/zlogging/enum/intel.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/json.py` & `zlogging-0.1.2.post3/zlogging/enum/json.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/known.py` & `zlogging-0.1.2.post3/zlogging/enum/known.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/load_balancing.py` & `zlogging-0.1.2.post3/zlogging/enum/load_balancing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/log.py` & `zlogging-0.1.2.post3/zlogging/enum/log.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/management.py` & `zlogging-0.1.2.post3/zlogging/enum/management.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/management_controller_runtime.py` & `zlogging-0.1.2.post3/zlogging/enum/management_controller_runtime.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/management_log.py` & `zlogging-0.1.2.post3/zlogging/enum/management_log.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/mount3.py` & `zlogging-0.1.2.post3/zlogging/enum/mount3.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/net_control.py` & `zlogging-0.1.2.post3/zlogging/enum/net_control.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/nfs3.py` & `zlogging-0.1.2.post3/zlogging/enum/nfs3.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/notice.py` & `zlogging-0.1.2.post3/zlogging/enum/notice.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/open_flow.py` & `zlogging-0.1.2.post3/zlogging/enum/open_flow.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/pcap.py` & `zlogging-0.1.2.post3/zlogging/enum/pcap.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/protocol_detector.py` & `zlogging-0.1.2.post3/zlogging/enum/protocol_detector.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/signatures.py` & `zlogging-0.1.2.post3/zlogging/enum/signatures.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/smb.py` & `zlogging-0.1.2.post3/zlogging/enum/smb.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/socks.py` & `zlogging-0.1.2.post3/zlogging/enum/socks.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/software.py` & `zlogging-0.1.2.post3/zlogging/enum/software.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/ssl.py` & `zlogging-0.1.2.post3/zlogging/enum/ssl.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/sum_stats.py` & `zlogging-0.1.2.post3/zlogging/enum/sum_stats.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/supervisor.py` & `zlogging-0.1.2.post3/zlogging/enum/supervisor.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/telemetry.py` & `zlogging-0.1.2.post3/zlogging/enum/telemetry.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/tunnel.py` & `zlogging-0.1.2.post3/zlogging/enum/tunnel.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/weird.py` & `zlogging-0.1.2.post3/zlogging/enum/weird.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/zeek.py` & `zlogging-0.1.2.post3/zlogging/enum/zeek.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/enum/zeekygen_example.py` & `zlogging-0.1.2.post3/zlogging/enum/zeekygen_example.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/loader.py` & `zlogging-0.1.2.post3/zlogging/loader.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/model.py` & `zlogging-0.1.2.post3/zlogging/model.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/types.py` & `zlogging-0.1.2.post3/zlogging/types.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging/typing.py` & `zlogging-0.1.2.post3/zlogging/typing.py`

 * *Files identical despite different names*

### Comparing `zlogging-0.1.2.post2/zlogging.egg-info/PKG-INFO` & `zlogging-0.1.2.post3/zlogging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlogging
-Version: 0.1.2.post2
+Version: 0.1.2.post3
 Summary: zlogging: Bro/Zeek logging framework for Python.
 Author-email: Jarry Shaw <jarryshaw@icloud.com>
 Maintainer: Jarry Shaw
 License: BSD 3-Clause License
 Project-URL: homepage, https://jarryshaw.github.io/zlogging/
 Project-URL: documentation, https://jarryshaw.github.io/zlogging/
 Project-URL: repository, https://github.com/JarryShaw/zlogging
```

### Comparing `zlogging-0.1.2.post2/zlogging.egg-info/SOURCES.txt` & `zlogging-0.1.2.post3/zlogging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

