# Comparing `tmp/qos_tools-0.0.1.tar.gz` & `tmp/qos_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qos_tools-0.0.1.tar", last modified: Tue Jun  6 05:11:40 2023, max compression
+gzip compressed data, was "qos_tools-0.0.2.tar", last modified: Wed Jun  7 08:14:02 2023, max compression
```

## Comparing `qos_tools-0.0.1.tar` & `qos_tools-0.0.2.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.087004 qos_tools-0.0.1/
--rw-r--r--   0 user       (501) staff       (20)     1064 2023-06-02 09:14:47.000000 qos_tools-0.0.1/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       75 2023-06-06 05:11:40.086877 qos_tools-0.0.1/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1314 2023-06-02 09:14:47.000000 qos_tools-0.0.1/README.md
--rw-r--r--   0 user       (501) staff       (20)       81 2023-06-06 05:11:14.000000 qos_tools-0.0.1/pyproject.toml
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.076785 qos_tools-0.0.1/qos_tools/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.079678 qos_tools-0.0.1/qos_tools/analyzer/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/analyzer/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    11092 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/analyzer/cr.py
--rw-r--r--   0 user       (501) staff       (20)     2457 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/analyzer/gpr.py
--rw-r--r--   0 user       (501) staff       (20)    42431 2023-06-02 09:01:31.000000 qos_tools-0.0.1/qos_tools/analyzer/lib.py
--rw-r--r--   0 user       (501) staff       (20)     3883 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/analyzer/statistics.py
--rw-r--r--   0 user       (501) staff       (20)    21233 2023-06-02 09:01:31.000000 qos_tools-0.0.1/qos_tools/analyzer/tools.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.079875 qos_tools-0.0.1/qos_tools/bigBrother/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/bigBrother/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.081604 qos_tools-0.0.1/qos_tools/core/
--rw-r--r--   0 user       (501) staff       (20)      486 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1375 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/_async_utils.py
--rw-r--r--   0 user       (501) staff       (20)     2144 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/_cfgcontext.py
--rw-r--r--   0 user       (501) staff       (20)     6280 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/_cm.py
--rw-r--r--   0 user       (501) staff       (20)     6921 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/_d2c.py
--rw-r--r--   0 user       (501) staff       (20)     8198 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/_dag_cons_manager.py
--rw-r--r--   0 user       (501) staff       (20)     1242 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/_dict_utils.py
--rw-r--r--   0 user       (501) staff       (20)     1090 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/_equal_utils.py
--rw-r--r--   0 user       (501) staff       (20)     6262 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/_graph_func.py
--rw-r--r--   0 user       (501) staff       (20)     1008 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/core/_iter.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.082058 qos_tools-0.0.1/qos_tools/create/
--rw-r--r--   0 user       (501) staff       (20)      310 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/create/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    12159 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/create/create.py
--rw-r--r--   0 user       (501) staff       (20)     8217 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/create/map.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.083102 qos_tools-0.0.1/qos_tools/experiment/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    79935 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/lib.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.084486 qos_tools-0.0.1/qos_tools/experiment/libs/
--rw-r--r--   0 user       (501) staff       (20)    16109 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/libs/CR.py
--rw-r--r--   0 user       (501) staff       (20)        0 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/libs/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4247 2023-06-05 05:29:33.000000 qos_tools-0.0.1/qos_tools/experiment/libs/coherence.py
--rw-r--r--   0 user       (501) staff       (20)    13047 2023-06-02 09:01:31.000000 qos_tools-0.0.1/qos_tools/experiment/libs/fidelity.py
--rw-r--r--   0 user       (501) staff       (20)    13488 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/libs/readout.py
--rw-r--r--   0 user       (501) staff       (20)    13678 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/libs/rfUnitary.py
--rw-r--r--   0 user       (501) staff       (20)     9900 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/libs/rfUnitary12.py
--rw-r--r--   0 user       (501) staff       (20)     4623 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/libs/tools.py
--rw-r--r--   0 user       (501) staff       (20)      281 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/quark.py
--rw-r--r--   0 user       (501) staff       (20)     9226 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/scanner.py
--rw-r--r--   0 user       (501) staff       (20)    12599 2023-06-02 09:01:31.000000 qos_tools-0.0.1/qos_tools/experiment/scanner2.py
--rw-r--r--   0 user       (501) staff       (20)     7774 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/experiment/transform.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.085079 qos_tools-0.0.1/qos_tools/feedback/
--rw-r--r--   0 user       (501) staff       (20)     3431 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/feedback/BayesOpt.py
--rw-r--r--   0 user       (501) staff       (20)       66 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/feedback/__init__.py
--rw-r--r--   0 user       (501) staff       (20)      703 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/feedback/model.py
--rw-r--r--   0 user       (501) staff       (20)     2236 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/feedback/ngOpt.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.085968 qos_tools-0.0.1/qos_tools/fit/
--rw-r--r--   0 user       (501) staff       (20)      125 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/fit/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     7473 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/fit/fitclass.py
--rw-r--r--   0 user       (501) staff       (20)     2028 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/fit/fitfunc.py
--rw-r--r--   0 user       (501) staff       (20)      620 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/fit/fitindex.py
--rw-r--r--   0 user       (501) staff       (20)     2197 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/fit/function.py
--rw-r--r--   0 user       (501) staff       (20)     3471 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/fit/plotscript.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.086699 qos_tools-0.0.1/qos_tools/gatemap/
--rw-r--r--   0 user       (501) staff       (20)     3759 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/gatemap/__info_extract.py
--rw-r--r--   0 user       (501) staff       (20)      177 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/gatemap/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     4295 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/gatemap/_circuit_convert.py
--rw-r--r--   0 user       (501) staff       (20)     1410 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/gatemap/_cmd_convert.py
--rw-r--r--   0 user       (501) staff       (20)     2899 2023-03-22 02:36:19.000000 qos_tools-0.0.1/qos_tools/gatemap/_index_convert.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-06 05:11:40.078253 qos_tools-0.0.1/qos_tools.egg-info/
--rw-r--r--   0 user       (501) staff       (20)       75 2023-06-06 05:11:40.000000 qos_tools-0.0.1/qos_tools.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1700 2023-06-06 05:11:40.000000 qos_tools-0.0.1/qos_tools.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-06-06 05:11:40.000000 qos_tools-0.0.1/qos_tools.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       10 2023-06-06 05:11:40.000000 qos_tools-0.0.1/qos_tools.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       10 2023-06-06 05:11:40.000000 qos_tools-0.0.1/qos_tools.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2023-06-06 05:11:40.087041 qos_tools-0.0.1/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.588685 qos_tools-0.0.2/
+-rw-r--r--   0 user       (501) staff       (20)     1064 2023-06-02 09:14:47.000000 qos_tools-0.0.2/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      823 2023-06-07 08:14:02.588580 qos_tools-0.0.2/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     1314 2023-06-02 09:14:47.000000 qos_tools-0.0.2/README.md
+-rw-r--r--   0 user       (501) staff       (20)       81 2023-06-07 08:13:57.000000 qos_tools-0.0.2/pyproject.toml
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.582200 qos_tools-0.0.2/qos_tools/
+-rw-r--r--   0 user       (501) staff       (20)       73 2023-06-07 08:03:37.000000 qos_tools-0.0.2/qos_tools/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.583450 qos_tools-0.0.2/qos_tools/analyzer/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/analyzer/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    11092 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/analyzer/cr.py
+-rw-r--r--   0 user       (501) staff       (20)     2457 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/analyzer/gpr.py
+-rw-r--r--   0 user       (501) staff       (20)    42431 2023-06-02 09:01:31.000000 qos_tools-0.0.2/qos_tools/analyzer/lib.py
+-rw-r--r--   0 user       (501) staff       (20)     3883 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/analyzer/statistics.py
+-rw-r--r--   0 user       (501) staff       (20)    21233 2023-06-02 09:01:31.000000 qos_tools-0.0.2/qos_tools/analyzer/tools.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.583583 qos_tools-0.0.2/qos_tools/bigBrother/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/bigBrother/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.584700 qos_tools-0.0.2/qos_tools/core/
+-rw-r--r--   0 user       (501) staff       (20)      486 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1375 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/_async_utils.py
+-rw-r--r--   0 user       (501) staff       (20)     2144 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/_cfgcontext.py
+-rw-r--r--   0 user       (501) staff       (20)     6280 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/_cm.py
+-rw-r--r--   0 user       (501) staff       (20)     6921 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/_d2c.py
+-rw-r--r--   0 user       (501) staff       (20)     8198 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/_dag_cons_manager.py
+-rw-r--r--   0 user       (501) staff       (20)     1242 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/_dict_utils.py
+-rw-r--r--   0 user       (501) staff       (20)     1090 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/_equal_utils.py
+-rw-r--r--   0 user       (501) staff       (20)     6262 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/_graph_func.py
+-rw-r--r--   0 user       (501) staff       (20)     1008 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/core/_iter.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.585026 qos_tools-0.0.2/qos_tools/create/
+-rw-r--r--   0 user       (501) staff       (20)      310 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/create/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    12159 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/create/create.py
+-rw-r--r--   0 user       (501) staff       (20)     8217 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/create/map.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.585756 qos_tools-0.0.2/qos_tools/experiment/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    79935 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/lib.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.586648 qos_tools-0.0.2/qos_tools/experiment/libs/
+-rw-r--r--   0 user       (501) staff       (20)    16109 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/libs/CR.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/libs/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4247 2023-06-05 05:29:33.000000 qos_tools-0.0.2/qos_tools/experiment/libs/coherence.py
+-rw-r--r--   0 user       (501) staff       (20)    13047 2023-06-02 09:01:31.000000 qos_tools-0.0.2/qos_tools/experiment/libs/fidelity.py
+-rw-r--r--   0 user       (501) staff       (20)    13488 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/libs/readout.py
+-rw-r--r--   0 user       (501) staff       (20)    13678 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/libs/rfUnitary.py
+-rw-r--r--   0 user       (501) staff       (20)     9900 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/libs/rfUnitary12.py
+-rw-r--r--   0 user       (501) staff       (20)     4623 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/libs/tools.py
+-rw-r--r--   0 user       (501) staff       (20)      281 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/quark.py
+-rw-r--r--   0 user       (501) staff       (20)     9226 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/scanner.py
+-rw-r--r--   0 user       (501) staff       (20)    12599 2023-06-02 09:01:31.000000 qos_tools-0.0.2/qos_tools/experiment/scanner2.py
+-rw-r--r--   0 user       (501) staff       (20)     7774 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/experiment/transform.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.587099 qos_tools-0.0.2/qos_tools/feedback/
+-rw-r--r--   0 user       (501) staff       (20)     3431 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/feedback/BayesOpt.py
+-rw-r--r--   0 user       (501) staff       (20)       66 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/feedback/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      703 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/feedback/model.py
+-rw-r--r--   0 user       (501) staff       (20)     2236 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/feedback/ngOpt.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.587739 qos_tools-0.0.2/qos_tools/fit/
+-rw-r--r--   0 user       (501) staff       (20)      125 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/fit/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     7473 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/fit/fitclass.py
+-rw-r--r--   0 user       (501) staff       (20)     2028 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/fit/fitfunc.py
+-rw-r--r--   0 user       (501) staff       (20)      620 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/fit/fitindex.py
+-rw-r--r--   0 user       (501) staff       (20)     2197 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/fit/function.py
+-rw-r--r--   0 user       (501) staff       (20)     3471 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/fit/plotscript.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.588385 qos_tools-0.0.2/qos_tools/gatemap/
+-rw-r--r--   0 user       (501) staff       (20)     3759 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/gatemap/__info_extract.py
+-rw-r--r--   0 user       (501) staff       (20)      177 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/gatemap/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4295 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/gatemap/_circuit_convert.py
+-rw-r--r--   0 user       (501) staff       (20)     1410 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/gatemap/_cmd_convert.py
+-rw-r--r--   0 user       (501) staff       (20)     2899 2023-03-22 02:36:19.000000 qos_tools-0.0.2/qos_tools/gatemap/_index_convert.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-06-07 08:14:02.582762 qos_tools-0.0.2/qos_tools.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)      823 2023-06-07 08:14:02.000000 qos_tools-0.0.2/qos_tools.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     1731 2023-06-07 08:14:02.000000 qos_tools-0.0.2/qos_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-06-07 08:14:02.000000 qos_tools-0.0.2/qos_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       17 2023-06-07 08:14:02.000000 qos_tools-0.0.2/qos_tools.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       10 2023-06-07 08:14:02.000000 qos_tools-0.0.2/qos_tools.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-06-07 08:14:02.588718 qos_tools-0.0.2/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     1129 2023-06-07 08:13:54.000000 qos_tools-0.0.2/setup.py
```

### Comparing `qos_tools-0.0.1/LICENSE` & `qos_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/README.md` & `qos_tools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/analyzer/cr.py` & `qos_tools-0.0.2/qos_tools/analyzer/cr.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/analyzer/gpr.py` & `qos_tools-0.0.2/qos_tools/analyzer/gpr.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/analyzer/lib.py` & `qos_tools-0.0.2/qos_tools/analyzer/lib.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/analyzer/statistics.py` & `qos_tools-0.0.2/qos_tools/analyzer/statistics.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/analyzer/tools.py` & `qos_tools-0.0.2/qos_tools/analyzer/tools.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/core/_async_utils.py` & `qos_tools-0.0.2/qos_tools/core/_async_utils.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/core/_cfgcontext.py` & `qos_tools-0.0.2/qos_tools/core/_cfgcontext.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/core/_cm.py` & `qos_tools-0.0.2/qos_tools/core/_cm.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/core/_d2c.py` & `qos_tools-0.0.2/qos_tools/core/_d2c.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/core/_dag_cons_manager.py` & `qos_tools-0.0.2/qos_tools/core/_dag_cons_manager.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/core/_dict_utils.py` & `qos_tools-0.0.2/qos_tools/core/_dict_utils.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/core/_equal_utils.py` & `qos_tools-0.0.2/qos_tools/core/_equal_utils.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/core/_graph_func.py` & `qos_tools-0.0.2/qos_tools/core/_graph_func.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/core/_iter.py` & `qos_tools-0.0.2/qos_tools/core/_iter.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/create/create.py` & `qos_tools-0.0.2/qos_tools/create/create.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/create/map.py` & `qos_tools-0.0.2/qos_tools/create/map.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/lib.py` & `qos_tools-0.0.2/qos_tools/experiment/lib.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/libs/CR.py` & `qos_tools-0.0.2/qos_tools/experiment/libs/CR.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/libs/coherence.py` & `qos_tools-0.0.2/qos_tools/experiment/libs/coherence.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/libs/fidelity.py` & `qos_tools-0.0.2/qos_tools/experiment/libs/fidelity.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/libs/readout.py` & `qos_tools-0.0.2/qos_tools/experiment/libs/readout.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/libs/rfUnitary.py` & `qos_tools-0.0.2/qos_tools/experiment/libs/rfUnitary.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/libs/rfUnitary12.py` & `qos_tools-0.0.2/qos_tools/experiment/libs/rfUnitary12.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/libs/tools.py` & `qos_tools-0.0.2/qos_tools/experiment/libs/tools.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/scanner.py` & `qos_tools-0.0.2/qos_tools/experiment/scanner.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/scanner2.py` & `qos_tools-0.0.2/qos_tools/experiment/scanner2.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/experiment/transform.py` & `qos_tools-0.0.2/qos_tools/experiment/transform.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/feedback/BayesOpt.py` & `qos_tools-0.0.2/qos_tools/feedback/BayesOpt.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/feedback/model.py` & `qos_tools-0.0.2/qos_tools/feedback/model.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/feedback/ngOpt.py` & `qos_tools-0.0.2/qos_tools/feedback/ngOpt.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/fit/fitclass.py` & `qos_tools-0.0.2/qos_tools/fit/fitclass.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/fit/fitfunc.py` & `qos_tools-0.0.2/qos_tools/fit/fitfunc.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/fit/fitindex.py` & `qos_tools-0.0.2/qos_tools/fit/fitindex.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/fit/function.py` & `qos_tools-0.0.2/qos_tools/fit/function.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/fit/plotscript.py` & `qos_tools-0.0.2/qos_tools/fit/plotscript.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/gatemap/__info_extract.py` & `qos_tools-0.0.2/qos_tools/gatemap/__info_extract.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/gatemap/_circuit_convert.py` & `qos_tools-0.0.2/qos_tools/gatemap/_circuit_convert.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/gatemap/_cmd_convert.py` & `qos_tools-0.0.2/qos_tools/gatemap/_cmd_convert.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools/gatemap/_index_convert.py` & `qos_tools-0.0.2/qos_tools/gatemap/_index_convert.py`

 * *Files identical despite different names*

### Comparing `qos_tools-0.0.1/qos_tools.egg-info/SOURCES.txt` & `qos_tools-0.0.2/qos_tools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
+setup.py
+qos_tools/__init__.py
 qos_tools.egg-info/PKG-INFO
 qos_tools.egg-info/SOURCES.txt
 qos_tools.egg-info/dependency_links.txt
 qos_tools.egg-info/requires.txt
 qos_tools.egg-info/top_level.txt
 qos_tools/analyzer/__init__.py
 qos_tools/analyzer/cr.py
```

