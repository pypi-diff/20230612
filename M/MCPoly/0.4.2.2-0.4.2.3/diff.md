# Comparing `tmp/MCPoly-0.4.2.2.tar.gz` & `tmp/MCPoly-0.4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCPoly-0.4.2.2.tar", last modified: Mon Jun 12 08:45:03 2023, max compression
+gzip compressed data, was "MCPoly-0.4.2.3.tar", last modified: Mon Jun 12 17:24:21 2023, max compression
```

## Comparing `MCPoly-0.4.2.2.tar` & `MCPoly-0.4.2.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.762009 MCPoly-0.4.2.2/
--rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.4.2.2/LICENSE
--rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.4.2.2/MANIFEST.in
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.754461 MCPoly-0.4.2.2/MCPoly/
--rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-06-12 08:44:54.000000 MCPoly-0.4.2.2/MCPoly/.DS_Store
--rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.4.2.2/MCPoly/__init__.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.756330 MCPoly-0.4.2.2/MCPoly/lmpset/
--rw-r--r--   0 cxs454     (503) staff       (20)     5763 2023-06-02 15:38:19.000000 MCPoly-0.4.2.2/MCPoly/lmpset/DATAtoXYZ.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-03 16:09:18.000000 MCPoly-0.4.2.2/MCPoly/lmpset/DATAtomolTXT.py
--rw-r--r--   0 cxs454     (503) staff       (20)      146 2023-06-03 14:29:24.000000 MCPoly-0.4.2.2/MCPoly/lmpset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.4.2.2/MCPoly/lmpset/chain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.4.2.2/MCPoly/lmpset/infchain.py
--rw-r--r--   0 cxs454     (503) staff       (20)    50843 2023-06-05 13:01:56.000000 MCPoly-0.4.2.2/MCPoly/lmpset/mould.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.757417 MCPoly-0.4.2.2/MCPoly/moldraw/
--rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.4.2.2/MCPoly/moldraw/C_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.4.2.2/MCPoly/moldraw/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.4.2.2/MCPoly/moldraw/bind_selection.py
--rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.4.2.2/MCPoly/moldraw/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.4.2.2/MCPoly/moldraw/molecule.py
--rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.4.2.2/MCPoly/moldraw/sub_selection.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.758828 MCPoly-0.4.2.2/MCPoly/orcaset/
--rw-r--r--   0 cxs454     (503) staff       (20)     8635 2023-05-02 16:35:59.000000 MCPoly-0.4.2.2/MCPoly/orcaset/XYZtoINP.py
--rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.4.2.2/MCPoly/orcaset/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    16705 2023-06-07 15:01:10.000000 MCPoly-0.4.2.2/MCPoly/orcaset/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     7592 2023-06-07 15:00:39.000000 MCPoly-0.4.2.2/MCPoly/orcaset/mgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.4.2.2/MCPoly/orcaset/multiorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2072 2023-05-15 15:20:42.000000 MCPoly-0.4.2.2/MCPoly/orcaset/orca.py
--rw-r--r--   0 cxs454     (503) staff       (20)    19705 2023-06-09 15:20:27.000000 MCPoly-0.4.2.2/MCPoly/orcaset/ssgui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     9044 2023-06-09 09:20:04.000000 MCPoly-0.4.2.2/MCPoly/orcaset/ssorca.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.4.2.2/MCPoly/orcaset/view3dchoose.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.759544 MCPoly-0.4.2.2/MCPoly/sscurve/
--rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.4.2.2/MCPoly/sscurve/YModulus.py
--rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.4.2.2/MCPoly/sscurve/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-05-17 15:37:43.000000 MCPoly-0.4.2.2/MCPoly/sscurve/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.4.2.2/MCPoly/sscurve/multiple.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.4.2.2/MCPoly/sscurve/single.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.760087 MCPoly-0.4.2.2/MCPoly/status/
--rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.4.2.2/MCPoly/status/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     6202 2023-05-22 09:10:31.000000 MCPoly-0.4.2.2/MCPoly/status/echart.py
--rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.4.2.2/MCPoly/status/gui.py
--rw-r--r--   0 cxs454     (503) staff       (20)    20682 2023-06-04 14:28:30.000000 MCPoly-0.4.2.2/MCPoly/status/status.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.760378 MCPoly-0.4.2.2/MCPoly/version/
--rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.4.2.2/MCPoly/version/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)       35 2023-06-09 08:40:29.000000 MCPoly-0.4.2.2/MCPoly/version/version.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.760662 MCPoly-0.4.2.2/MCPoly/view3d/
--rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.4.2.2/MCPoly/view3d/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.4.2.2/MCPoly/view3d/view3d.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.760935 MCPoly-0.4.2.2/MCPoly/vis/
--rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.4.2.2/MCPoly/vis/__init__.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2071 2023-05-29 07:04:54.000000 MCPoly-0.4.2.2/MCPoly/vis/vis.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.755323 MCPoly-0.4.2.2/MCPoly.egg-info/
--rw-r--r--   0 cxs454     (503) staff       (20)     3675 2023-06-12 08:45:03.000000 MCPoly-0.4.2.2/MCPoly.egg-info/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     1254 2023-06-12 08:45:03.000000 MCPoly-0.4.2.2/MCPoly.egg-info/SOURCES.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-12 08:45:03.000000 MCPoly-0.4.2.2/MCPoly.egg-info/dependency_links.txt
--rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-12 08:45:03.000000 MCPoly-0.4.2.2/MCPoly.egg-info/requires.txt
--rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-12 08:45:03.000000 MCPoly-0.4.2.2/MCPoly.egg-info/top_level.txt
--rw-r--r--   0 cxs454     (503) staff       (20)     3675 2023-06-12 08:45:03.761847 MCPoly-0.4.2.2/PKG-INFO
--rw-r--r--   0 cxs454     (503) staff       (20)     3311 2023-06-12 08:44:44.000000 MCPoly-0.4.2.2/README.md
--rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-12 08:45:03.762057 MCPoly-0.4.2.2/setup.cfg
--rw-r--r--   0 cxs454     (503) staff       (20)     1033 2023-06-12 08:42:36.000000 MCPoly-0.4.2.2/setup.py
-drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 08:45:03.761634 MCPoly-0.4.2.2/tests/
--rw-r--r--   0 cxs454     (503) staff       (20)     8625 2023-06-05 10:40:35.000000 MCPoly-0.4.2.2/tests/test_lmpset.py
--rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.4.2.2/tests/test_moldraw.py
--rw-r--r--   0 cxs454     (503) staff       (20)     2932 2023-05-02 17:01:47.000000 MCPoly-0.4.2.2/tests/test_orcaset.py
--rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.4.2.2/tests/test_sscurve.py
--rw-r--r--   0 cxs454     (503) staff       (20)     5241 2023-06-05 08:11:04.000000 MCPoly-0.4.2.2/tests/test_status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.129286 MCPoly-0.4.2.3/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1091 2023-05-03 15:22:57.000000 MCPoly-0.4.2.3/LICENSE
+-rw-r--r--   0 cxs454     (503) staff       (20)       17 2023-05-04 08:23:11.000000 MCPoly-0.4.2.3/MANIFEST.in
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.121744 MCPoly-0.4.2.3/MCPoly/
+-rw-r--r--   0 cxs454     (503) staff       (20)    14340 2023-06-12 17:23:57.000000 MCPoly-0.4.2.3/MCPoly/.DS_Store
+-rw-r--r--   0 cxs454     (503) staff       (20)      178 2023-05-15 14:05:30.000000 MCPoly-0.4.2.3/MCPoly/__init__.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.123581 MCPoly-0.4.2.3/MCPoly/lmpset/
+-rw-r--r--   0 cxs454     (503) staff       (20)     5785 2023-06-12 14:51:07.000000 MCPoly-0.4.2.3/MCPoly/lmpset/DATAtoXYZ.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4361 2023-06-12 14:51:59.000000 MCPoly-0.4.2.3/MCPoly/lmpset/DATAtomolTXT.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      146 2023-06-03 14:29:24.000000 MCPoly-0.4.2.3/MCPoly/lmpset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    55548 2023-06-05 13:00:53.000000 MCPoly-0.4.2.3/MCPoly/lmpset/chain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16310 2023-06-03 14:28:50.000000 MCPoly-0.4.2.3/MCPoly/lmpset/infchain.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    50867 2023-06-12 14:57:57.000000 MCPoly-0.4.2.3/MCPoly/lmpset/mould.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.124686 MCPoly-0.4.2.3/MCPoly/moldraw/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8966 2023-05-26 12:59:21.000000 MCPoly-0.4.2.3/MCPoly/moldraw/C_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      128 2023-05-29 06:59:26.000000 MCPoly-0.4.2.3/MCPoly/moldraw/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    64145 2023-05-26 10:41:02.000000 MCPoly-0.4.2.3/MCPoly/moldraw/bind_selection.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    24385 2023-05-29 07:03:41.000000 MCPoly-0.4.2.3/MCPoly/moldraw/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)   181892 2023-05-26 12:59:34.000000 MCPoly-0.4.2.3/MCPoly/moldraw/molecule.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    98156 2023-05-26 10:40:13.000000 MCPoly-0.4.2.3/MCPoly/moldraw/sub_selection.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.126086 MCPoly-0.4.2.3/MCPoly/orcaset/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8635 2023-05-02 16:35:59.000000 MCPoly-0.4.2.3/MCPoly/orcaset/XYZtoINP.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      158 2023-05-11 15:49:25.000000 MCPoly-0.4.2.3/MCPoly/orcaset/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    16723 2023-06-12 17:02:56.000000 MCPoly-0.4.2.3/MCPoly/orcaset/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     7592 2023-06-07 15:00:39.000000 MCPoly-0.4.2.3/MCPoly/orcaset/mgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     4842 2023-05-02 16:29:09.000000 MCPoly-0.4.2.3/MCPoly/orcaset/multiorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2072 2023-05-15 15:20:42.000000 MCPoly-0.4.2.3/MCPoly/orcaset/orca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    19705 2023-06-09 15:20:27.000000 MCPoly-0.4.2.3/MCPoly/orcaset/ssgui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     9044 2023-06-09 09:20:04.000000 MCPoly-0.4.2.3/MCPoly/orcaset/ssorca.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2145 2023-05-09 08:28:02.000000 MCPoly-0.4.2.3/MCPoly/orcaset/view3dchoose.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.126786 MCPoly-0.4.2.3/MCPoly/sscurve/
+-rw-r--r--   0 cxs454     (503) staff       (20)     1193 2023-05-02 16:03:26.000000 MCPoly-0.4.2.3/MCPoly/sscurve/YModulus.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       88 2023-05-09 08:48:45.000000 MCPoly-0.4.2.3/MCPoly/sscurve/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    12770 2023-05-17 15:37:43.000000 MCPoly-0.4.2.3/MCPoly/sscurve/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5843 2023-05-19 09:04:58.000000 MCPoly-0.4.2.3/MCPoly/sscurve/multiple.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6832 2023-05-19 08:52:37.000000 MCPoly-0.4.2.3/MCPoly/sscurve/single.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.127367 MCPoly-0.4.2.3/MCPoly/status/
+-rw-r--r--   0 cxs454     (503) staff       (20)       62 2023-05-18 16:46:40.000000 MCPoly-0.4.2.3/MCPoly/status/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     6202 2023-05-22 09:10:31.000000 MCPoly-0.4.2.3/MCPoly/status/echart.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    15750 2023-05-18 16:45:20.000000 MCPoly-0.4.2.3/MCPoly/status/gui.py
+-rw-r--r--   0 cxs454     (503) staff       (20)    20682 2023-06-04 14:28:30.000000 MCPoly-0.4.2.3/MCPoly/status/status.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.127674 MCPoly-0.4.2.3/MCPoly/version/
+-rw-r--r--   0 cxs454     (503) staff       (20)       23 2023-05-04 08:03:54.000000 MCPoly-0.4.2.3/MCPoly/version/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)       35 2023-06-12 17:24:12.000000 MCPoly-0.4.2.3/MCPoly/version/version.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.127946 MCPoly-0.4.2.3/MCPoly/view3d/
+-rw-r--r--   0 cxs454     (503) staff       (20)       22 2023-04-30 18:16:37.000000 MCPoly-0.4.2.3/MCPoly/view3d/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     1970 2023-05-09 13:30:17.000000 MCPoly-0.4.2.3/MCPoly/view3d/view3d.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.128227 MCPoly-0.4.2.3/MCPoly/vis/
+-rw-r--r--   0 cxs454     (503) staff       (20)       18 2023-05-15 14:05:55.000000 MCPoly-0.4.2.3/MCPoly/vis/__init__.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2071 2023-05-29 07:04:54.000000 MCPoly-0.4.2.3/MCPoly/vis/vis.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.122595 MCPoly-0.4.2.3/MCPoly.egg-info/
+-rw-r--r--   0 cxs454     (503) staff       (20)     3675 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     1254 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/SOURCES.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        1 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/dependency_links.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)      143 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/requires.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)        7 2023-06-12 17:24:21.000000 MCPoly-0.4.2.3/MCPoly.egg-info/top_level.txt
+-rw-r--r--   0 cxs454     (503) staff       (20)     3675 2023-06-12 17:24:21.129119 MCPoly-0.4.2.3/PKG-INFO
+-rw-r--r--   0 cxs454     (503) staff       (20)     3311 2023-06-12 08:44:44.000000 MCPoly-0.4.2.3/README.md
+-rw-r--r--   0 cxs454     (503) staff       (20)       38 2023-06-12 17:24:21.129331 MCPoly-0.4.2.3/setup.cfg
+-rw-r--r--   0 cxs454     (503) staff       (20)     1033 2023-06-12 17:23:45.000000 MCPoly-0.4.2.3/setup.py
+drwxr-xr-x   0 cxs454     (503) staff       (20)        0 2023-06-12 17:24:21.128917 MCPoly-0.4.2.3/tests/
+-rw-r--r--   0 cxs454     (503) staff       (20)     8592 2023-06-12 15:00:22.000000 MCPoly-0.4.2.3/tests/test_lmpset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)      799 2023-05-03 10:12:20.000000 MCPoly-0.4.2.3/tests/test_moldraw.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     2932 2023-05-02 17:01:47.000000 MCPoly-0.4.2.3/tests/test_orcaset.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     3535 2023-05-19 13:19:19.000000 MCPoly-0.4.2.3/tests/test_sscurve.py
+-rw-r--r--   0 cxs454     (503) staff       (20)     5241 2023-06-05 08:11:04.000000 MCPoly-0.4.2.3/tests/test_status.py
```

### Comparing `MCPoly-0.4.2.2/LICENSE` & `MCPoly-0.4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/.DS_Store` & `MCPoly-0.4.2.3/MCPoly/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -262,16 +262,16 @@
 00001050: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
 00001060: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 00001070: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00001080: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00001090: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 000010a0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 000010b0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000010c0: 6261 7208 0908 095f 1018 7b7b 3136 382c  bar...._..{{168,
-000010d0: 2034 3639 7d2c 207b 3932 302c 2034 3336   469}, {920, 436
+000010c0: 6261 7208 0908 095f 1018 7b7b 3131 352c  bar...._..{{115,
+000010d0: 2031 3837 7d2c 207b 3932 302c 2034 3336   187}, {920, 436
 000010e0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 000010f0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001100: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 00001110: 0000 0007 006f 0072 0063 0061 0073 0065  .....o.r.c.a.s.e
 00001120: 0074 6963 7670 626c 6f62 0000 0194 6270  .ticvpblob....bp
 00001130: 6c69 7374 3030 de01 0203 0405 0607 0809  list00..........
 00001140: 0a0b 0c0d 0e0f 1011 0f12 0f13 1314 1516  ................
```

### Comparing `MCPoly-0.4.2.2/MCPoly/lmpset/DATAtoXYZ.py` & `MCPoly-0.4.2.3/MCPoly/lmpset/DATAtoXYZ.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,11 +151,11 @@
             for i4 in range(len(l)):
                 elements.append(elementsort[eval(l[i4][2])-1])
                 XYZs.append([eval(l[i4][-3]),eval(l[i4][-2]),eval(l[i4][-1])])
             w1=0
     f.close()
     molecule = Atoms(elements, positions=XYZs)
     if savename=='':
-        write(file+'.xyz',molecule)
+        write('{0}.xyz'.format(file),molecule)
     else:
-        write(savename+'.xyz',molecule)
+        write('{0}.xyz'.format(savename),molecule)
     os.chdir(opath)
```

### Comparing `MCPoly-0.4.2.2/MCPoly/lmpset/DATAtomolTXT.py` & `MCPoly-0.4.2.3/MCPoly/lmpset/DATAtomolTXT.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/lmpset/chain.py` & `MCPoly-0.4.2.3/MCPoly/lmpset/chain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/lmpset/infchain.py` & `MCPoly-0.4.2.3/MCPoly/lmpset/infchain.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/lmpset/mould.py` & `MCPoly-0.4.2.3/MCPoly/lmpset/mould.py`

 * *Files 1% similar despite different names*

```diff
@@ -968,27 +968,27 @@
         DATAtoXYZ(savename='')
         savename: Name of the saved XYZ File. The default is name of origin LAMMPS Data File.
         Example:
             Input:
                 from MCPoly.lmpset import mould
                 atoms=mould('Poly1')
                 atoms.DATAtoXYZ()
-            Output in Poly1_Chain.xyz:
+            Output in Poly1.xyz:
                 82
                 Properties=species:S:1:pos:R:3 pbc="F F F"
                 H       34.26389000       7.81856000       4.72112000
                 C       33.60940000       7.29160000       5.40582000
                 H       33.81841000       6.25379000       5.63907000
                 C       32.30303000       7.89744000       5.79799000
                 H       31.98877000       7.45674000       6.75085000
                 C       31.23940000       7.64473000       4.74277000
         
                 ...
         """
-        return cxyz(self.file,self.loc,savename)
+        return cxyz(self.atoms,loc=self.loc,savename=savename)
     
     def DATAtomolTXT(self,types={0:0},savename=''):
         """
         The method to change LAMMPS Data File into LAMMPS Molecule Text File.
         DATAtomolTXT(types={0:0, ...},savename='')
         file: Your molecule system name on your .data file.
         types: Change the Atom Type number to suit the main LAMMPS input files.
@@ -1061,15 +1061,15 @@
                 6 3
                 7 2
                 8 4
                 9 5
                 
                     ...
         """
-        return ctxt(self.file,types,self.loc,savename)
+        return ctxt(self.atoms,types,loc=self.loc,savename=savename)
     
     def infchain(self,bondtype):
         """
         The method to create a single molecule for periodical chain, specialised for polymers.
         infchain(bondtype)
         file: Your molecule system name on your .data file.
         bondtype: The bond type between the start and the end of the polymer. 
@@ -1093,15 +1093,15 @@
                 3 improper types
                 
                 ...
                 84 11 79 1
                 
                 ...
         """
-        return inf(self.file,bondtype,self.loc)
+        return inf(self.atoms,bondtype,self.loc)
 
     def chain(self,bondtype,degree):
         """
         The method to create a single molecule for a finite chain, specialised for polymers.
         chain(bondtype,degree)
         degree: Degree of polymerisation.
         bondtype: The bond type between the start and the end of the polymer. 
@@ -1124,8 +1124,8 @@
                 3 improper types
 
                 ...
                 82 1 83 1
 
                 ...
         """
-        return normalchain(self.file,bondtype,degree,self.loc)
+        return normalchain(self.atoms,bondtype,degree,self.loc)
```

### Comparing `MCPoly-0.4.2.2/MCPoly/moldraw/C_selection.py` & `MCPoly-0.4.2.3/MCPoly/moldraw/C_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/moldraw/bind_selection.py` & `MCPoly-0.4.2.3/MCPoly/moldraw/bind_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/moldraw/gui.py` & `MCPoly-0.4.2.3/MCPoly/moldraw/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/moldraw/molecule.py` & `MCPoly-0.4.2.3/MCPoly/moldraw/molecule.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/moldraw/sub_selection.py` & `MCPoly-0.4.2.3/MCPoly/moldraw/sub_selection.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/orcaset/XYZtoINP.py` & `MCPoly-0.4.2.3/MCPoly/orcaset/XYZtoINP.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/orcaset/gui.py` & `MCPoly-0.4.2.3/MCPoly/orcaset/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,19 +193,19 @@
                 aim2.value=num-1
         with output:
             button.description='Processing...'
         if scanox.value==True:
             orca(file.value+'_scan',orcaloc=orcaloc.value)
         elif forceox.value==True:
             if roomox.value==True and coreox.value==True:
-                XYZtoINP(file,inpname='{0}_{1:.3f}'.format(file.value,strain.value),loc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,electron=e.value,state=state.value)
+                XYZtoINP(file.value,inpname='{0}_{1:.3f}'.format(file.value,strain.value),fileloc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,electron=e.value,state=state.value)
             elif roomox.value==False and coreox.value==False:
-                XYZtoINP(file.value,inpname='{0}_{1:.3f}'.format(file.value,strain.value),loc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,maxcore=room.value*1024,corenum=corenum.value,electron=e.value,state=state.value)
+                XYZtoINP(file.value,inpname='{0}_{1:.3f}'.format(file.value,strain.value),fileloc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,maxcore=room.value*1024,corenum=corenum.value,electron=e.value,state=state.value)
             else:
-                XYZtoINP(file.value,inpname='{0}_{1:.3f}'.format(file.value,strain.value),loc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,maxcore=room.value*1024,electron=e.value,state=state.value)
+                XYZtoINP(file.value,inpname='{0}_{1:.3f}'.format(file.value,strain.value),fileloc=loc.value,method=method.value,basis_set=bs.value,opt=opt.value,freq=freq.value,external_force=True,aim=[aim1.value,aim2.value],strain=strain.value,maxcore=room.value*1024,electron=e.value,state=state.value)
             orca('{0}_{1:.3f}'.format(file.value,strain.value),orcaloc=orcaloc.value)
         else:
             orca(file.value,orcaloc=orcaloc.value)
         with output2:
             if scanox.value==True:
                 if status(file.value+'_scan',loc.value).status(figureonly=True,statusonly=True)==2:
                     display(widgets.HBox([widgets.Valid(description=file.value+'_scan',value=True),widgets.Label('  Calculation completed!')]))
```

### Comparing `MCPoly-0.4.2.2/MCPoly/orcaset/mgui.py` & `MCPoly-0.4.2.3/MCPoly/orcaset/mgui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/orcaset/multiorca.py` & `MCPoly-0.4.2.3/MCPoly/orcaset/multiorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/orcaset/orca.py` & `MCPoly-0.4.2.3/MCPoly/orcaset/orca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/orcaset/ssgui.py` & `MCPoly-0.4.2.3/MCPoly/orcaset/ssgui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/orcaset/ssorca.py` & `MCPoly-0.4.2.3/MCPoly/orcaset/ssorca.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/orcaset/view3dchoose.py` & `MCPoly-0.4.2.3/MCPoly/orcaset/view3dchoose.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/sscurve/YModulus.py` & `MCPoly-0.4.2.3/MCPoly/sscurve/YModulus.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/sscurve/gui.py` & `MCPoly-0.4.2.3/MCPoly/sscurve/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/sscurve/multiple.py` & `MCPoly-0.4.2.3/MCPoly/sscurve/multiple.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/sscurve/single.py` & `MCPoly-0.4.2.3/MCPoly/sscurve/single.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/status/echart.py` & `MCPoly-0.4.2.3/MCPoly/status/echart.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/status/gui.py` & `MCPoly-0.4.2.3/MCPoly/status/gui.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/status/status.py` & `MCPoly-0.4.2.3/MCPoly/status/status.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/view3d/view3d.py` & `MCPoly-0.4.2.3/MCPoly/view3d/view3d.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly/vis/vis.py` & `MCPoly-0.4.2.3/MCPoly/vis/vis.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/MCPoly.egg-info/PKG-INFO` & `MCPoly-0.4.2.3/MCPoly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.4.2.2
+Version: 0.4.2.3
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
```

### Comparing `MCPoly-0.4.2.2/MCPoly.egg-info/SOURCES.txt` & `MCPoly-0.4.2.3/MCPoly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/PKG-INFO` & `MCPoly-0.4.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCPoly
-Version: 0.4.2.2
+Version: 0.4.2.3
 Summary: Useful tools for Computational Chemistry for polymers
 Home-page: https://github.com/Omicron-Fluor/MCPoly/
 Author: Omicron Fluor
 Author-email: cxs454@student.bham.ac.uk
 License: MIT
 Keywords: ORCA,Mechanical Property,Computational Chemistry
 Description-Content-Type: text/markdown
```

### Comparing `MCPoly-0.4.2.2/README.md` & `MCPoly-0.4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/setup.py` & `MCPoly-0.4.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='MCPoly',
-    version='0.4.2.2',
+    version='0.4.2.3',
     description='Useful tools for Computational Chemistry for polymers',
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=['MCPoly','MCPoly.lmpset','MCPoly.moldraw','MCPoly.orcaset','MCPoly.sscurve','MCPoly.status','MCPoly.view3d','MCPoly.version','MCPoly.vis'],
     author='Omicron Fluor',
     author_email='cxs454@student.bham.ac.uk',
```

### Comparing `MCPoly-0.4.2.2/tests/test_lmpset.py` & `MCPoly-0.4.2.3/tests/test_lmpset.py`

 * *Files 11% similar despite different names*

```diff
@@ -320,71 +320,71 @@
     return mould('Poly2',loc='./data_lmpset/')
 
 def test_infchain(atoms):
     opath=os.getcwd()
     os.chdir('./MCPoly/tests')
     atoms.infchain(3)
     os.chdir(opath)
-    fl=open('./MCPoly/tests/data_lmpset/Poly2_Chain.txt','r')
+    fl=open('./MCPoly/tests/data_lmpset/Poly2_Chain.data','r')
     i1=0
     i2=0
-    i3=1
+    i3=0
     i4=0
     i5=0
     i6=0
     for line in fl:
         a=re.search('7 atoms',line)
         if a:
             i1=1
         b=re.search('9 angles',line)
         if b:
             i2=1
         c=re.search('2 impropers',line)
         if c:
-            i3=0
+            i3=1
         d=re.search('4 bond types',line)
         if d:
             i4=1
         e=re.search('4 dihedral types',line)
         if e:
             i5=1
         f=re.search('7 3 5 1',line)
         if f:
             i6=1
             break
     fl.close()
     assert i1*i2*i3*i4*i5*i6!=0
 
-#def test_chain(atoms):
-#    opath=os.getcwd()
-#    os.chdir('./MCPoly/tests')
-#    atoms.chain(3,5)
-#    os.chdir(opath)
-#    fl=open('./MCPoly/tests/data_lmpset/Poly2_Chain.txt','r')
-#    i1=0
-#    i2=0
-#    i3=1
-#    i4=0
-#    i5=0
-#    i6=0
-#    for line in fl:
-#        a=re.search('7 atoms',line)
-#        if a:
-#            i1=1
-#        b=re.search('9 angles',line)
-#        if b:
-#            i2=1
-#        c=re.search('2 impropers',line)
-#        if c:
-#            i3=0
-#        d=re.search('4 bond types',line)
-#        if d:
-#            i4=1
-#        e=re.search('4 dihedral types',line)
-#        if e:
-#            i5=1
-#        f=re.search('7 3 5 1',line)
-#        if f:
-#            i6=1
-#            break
-#    fl.close()
-#    assert i1*i2*i3*i4*i5*i6!=0
+def test_chain(atoms):
+    opath=os.getcwd()
+    os.chdir('./MCPoly/tests')
+    atoms.chain(3,5)
+    os.chdir(opath)
+    fl=open('./MCPoly/tests/data_lmpset/Poly2_5x.data','r')
+    i1=0
+    i2=0
+    i3=0
+    i4=0
+    i5=0
+    i6=0
+    for line in fl:
+        a=re.search('37 atoms',line)
+        if a:
+            i1=1
+        b=re.search('36 bonds',line)
+        if b:
+            i2=1
+        c=re.search('49 angles',line)
+        if c:
+            i3=1
+        d=re.search('5 angle types',line)
+        if d:
+            i4=1
+        e=re.search('4 dihedral types',line)
+        if e:
+            i5=1
+        f=re.match('12 2 14 10',line)
+        if f:
+            i6=1
+            break
+    fl.close()
+    assert i1*i2*i3*i4*i5*i6!=0
```

### Comparing `MCPoly-0.4.2.2/tests/test_moldraw.py` & `MCPoly-0.4.2.3/tests/test_moldraw.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/tests/test_orcaset.py` & `MCPoly-0.4.2.3/tests/test_orcaset.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/tests/test_sscurve.py` & `MCPoly-0.4.2.3/tests/test_sscurve.py`

 * *Files identical despite different names*

### Comparing `MCPoly-0.4.2.2/tests/test_status.py` & `MCPoly-0.4.2.3/tests/test_status.py`

 * *Files identical despite different names*

