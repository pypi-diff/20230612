# Comparing `tmp/pystoned-0.6.5.tar.gz` & `tmp/pystoned-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystoned-0.6.5.tar", last modified: Fri May  5 11:12:24 2023, max compression
+gzip compressed data, was "pystoned-0.6.6.tar", last modified: Mon Jun 12 18:18:44 2023, max compression
```

## Comparing `pystoned-0.6.5.tar` & `pystoned-0.6.6.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.707428 pystoned-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 11:12:09.000000 pystoned-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-05 11:12:24.707428 pystoned-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-05 11:12:09.000000 pystoned-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.703428 pystoned-0.6.5/pystoned/
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CNLS.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CNLSDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CNLSG.py
--rw-r--r--   0 runner    (1001) docker     (123)    15875 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CQER.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CQERDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)    21684 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CQERG.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/CSVR.py
--rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/DEA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/FDH.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/ICNLS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/ICQER.py
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/StoNED.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.703428 pystoned-0.6.5/pystoned/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/data/41Firm.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/data/abatementCost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/data/electricityFirms.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33693 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/data/riceProduction.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/pCNLS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/pCQER.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/pICQER.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/sCQER.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.707428 pystoned-0.6.5/pystoned/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CNLSG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CNLSG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CNLSZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CNLSZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CQERG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CQERG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CQERZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/CQERZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/sweet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/wCNLS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/wCQER.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-05-05 11:12:10.000000 pystoned-0.6.5/pystoned/weakCNLS.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:24.703428 pystoned-0.6.5/pystoned.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 11:12:24.000000 pystoned-0.6.5/pystoned.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:12:24.707428 pystoned-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-05 11:12:10.000000 pystoned-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:18:44.119720 pystoned-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 18:18:31.000000 pystoned-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-12 18:18:44.119720 pystoned-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-12 18:18:31.000000 pystoned-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:18:44.115720 pystoned-0.6.6/pystoned/
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/CNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/CNLSDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/CNLSG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15875 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/CQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/CQERDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21684 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/CQERG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/CSVR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/DEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/FDH.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/ICNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/ICQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/StoNED.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:18:44.119720 pystoned-0.6.6/pystoned/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/data/41Firm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/data/abatementCost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/data/electricityFirms.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33693 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/data/riceProduction.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/pCNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/pCQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/pICQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/pwCNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/pwCQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/sCQER.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:18:44.119720 pystoned-0.6.6/pystoned/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/CNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/CNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/CNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/CNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/CQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/CQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/CQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/CQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/sweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/wCNLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/wCQER.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-12 18:18:31.000000 pystoned-0.6.6/pystoned/weakCNLS.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:18:44.115720 pystoned-0.6.6/pystoned.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-12 18:18:44.000000 pystoned-0.6.6/pystoned.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-12 18:18:44.000000 pystoned-0.6.6/pystoned.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:18:44.000000 pystoned-0.6.6/pystoned.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:18:43.000000 pystoned-0.6.6/pystoned.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 18:18:44.000000 pystoned-0.6.6/pystoned.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 18:18:44.000000 pystoned-0.6.6/pystoned.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:18:44.119720 pystoned-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-12 18:18:31.000000 pystoned-0.6.6/setup.py
```

### Comparing `pystoned-0.6.5/LICENSE` & `pystoned-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/PKG-INFO` & `pystoned-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystoned
-Version: 0.6.5
+Version: 0.6.6
 Summary: A Python Package for Convex Regression and Frontier Estimation
 Home-page: https://github.com/ds2010/pyStoNED
 Download-URL: https://pypi.org/project/pystoned/
 Author: Sheng Dai, Yu-Hsueh Fang, Chia-Yen Lee, Timo Kuosmanen
 Author-email: sheng.dai@utu.fi
 License: GPLv3
 Keywords: StoNED,CNLS,CER,CQR,Z-variables,CNLSG
```

### Comparing `pystoned-0.6.5/README.md` & `pystoned-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/CNLS.py` & `pystoned-0.6.6/pystoned/CNLS.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/CNLSDDF.py` & `pystoned-0.6.6/pystoned/CNLSDDF.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/CNLSG.py` & `pystoned-0.6.6/pystoned/CNLSG.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/CQER.py` & `pystoned-0.6.6/pystoned/CQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/CQERDDF.py` & `pystoned-0.6.6/pystoned/CQERDDF.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/CQERG.py` & `pystoned-0.6.6/pystoned/CQERG.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/CSVR.py` & `pystoned-0.6.6/pystoned/CSVR.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/DEA.py` & `pystoned-0.6.6/pystoned/DEA.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/FDH.py` & `pystoned-0.6.6/pystoned/FDH.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/ICNLS.py` & `pystoned-0.6.6/pystoned/ICNLS.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/ICQER.py` & `pystoned-0.6.6/pystoned/ICQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/StoNED.py` & `pystoned-0.6.6/pystoned/StoNED.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/__init__.py` & `pystoned-0.6.6/pystoned/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from . import CSVR
 from . import dataset
 from . import DEA
 from . import FDH
 from . import pCNLS
 from . import pCQER
 from . import pICQER
+from . import pwCNLS
+from . import pwCQER
 from . import plot
 from . import ICNLS
 from . import ICQER
 from . import sCQER
 from . import StoNED
 from . import wCNLS
 from . import wCQER
@@ -32,14 +34,16 @@
     'CSVR',
     'dataset',
     'DEA',
     'FDH',
     'pCNLS',
     'pCQER',
     'pICQER',
+    'pwCNLS',
+    'pwCQER',
     'plot',
     'ICNLS',
     'ICQER',
     'sCQER',
     'StoNED',
     'wCNLS',
     'wCQER',
```

### Comparing `pystoned-0.6.5/pystoned/constant.py` & `pystoned-0.6.6/pystoned/constant.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/data/41Firm.csv` & `pystoned-0.6.6/pystoned/data/41Firm.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/data/abatementCost.csv` & `pystoned-0.6.6/pystoned/data/abatementCost.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/data/electricityFirms.csv` & `pystoned-0.6.6/pystoned/data/electricityFirms.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/data/riceProduction.csv` & `pystoned-0.6.6/pystoned/data/riceProduction.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/dataset.py` & `pystoned-0.6.6/pystoned/dataset.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/pICQER.py` & `pystoned-0.6.6/pystoned/pICQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/plot.py` & `pystoned-0.6.6/pystoned/plot.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/sCQER.py` & `pystoned-0.6.6/pystoned/sCQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/CNLSG1.py` & `pystoned-0.6.6/pystoned/utils/CNLSG1.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/CNLSG2.py` & `pystoned-0.6.6/pystoned/utils/CNLSG2.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/CNLSZG1.py` & `pystoned-0.6.6/pystoned/utils/CNLSZG1.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/CNLSZG2.py` & `pystoned-0.6.6/pystoned/utils/CNLSZG2.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/CQERG1.py` & `pystoned-0.6.6/pystoned/utils/CQERG1.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/CQERG2.py` & `pystoned-0.6.6/pystoned/utils/CQERG2.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/CQERZG1.py` & `pystoned-0.6.6/pystoned/utils/CQERZG1.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/CQERZG2.py` & `pystoned-0.6.6/pystoned/utils/CQERZG2.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/interpolation.py` & `pystoned-0.6.6/pystoned/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/sweet.py` & `pystoned-0.6.6/pystoned/utils/sweet.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/utils/tools.py` & `pystoned-0.6.6/pystoned/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned/wCNLS.py` & `pystoned-0.6.6/pystoned/wCNLS.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # import dependencies
 from pyomo.environ import Objective, minimize
-
 from . import CNLS
 from .constant import CET_ADDI, FUN_PROD, RTS_VRS
 from .utils import tools
 
 
 class wCNLS(CNLS.CNLS):
     """Weighted Convex Nonparametric Least Square (wCNLS)
```

### Comparing `pystoned-0.6.5/pystoned/wCQER.py` & `pystoned-0.6.6/pystoned/wCQER.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # import dependencies
 from pyomo.environ import Objective, minimize
-
 from . import CQER
 from .constant import CET_ADDI, FUN_PROD, RTS_VRS
 from .utils import tools
 
 
 class wCQR(CQER.CQR):
     """Weighted Convex Quantile Regression (wCQR)
```

### Comparing `pystoned-0.6.5/pystoned/weakCNLS.py` & `pystoned-0.6.6/pystoned/weakCNLS.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.5/pystoned.egg-info/PKG-INFO` & `pystoned-0.6.6/pystoned.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystoned
-Version: 0.6.5
+Version: 0.6.6
 Summary: A Python Package for Convex Regression and Frontier Estimation
 Home-page: https://github.com/ds2010/pyStoNED
 Download-URL: https://pypi.org/project/pystoned/
 Author: Sheng Dai, Yu-Hsueh Fang, Chia-Yen Lee, Timo Kuosmanen
 Author-email: sheng.dai@utu.fi
 License: GPLv3
 Keywords: StoNED,CNLS,CER,CQR,Z-variables,CNLSG
```

### Comparing `pystoned-0.6.5/pystoned.egg-info/SOURCES.txt` & `pystoned-0.6.6/pystoned.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 pystoned/__init__.py
 pystoned/constant.py
 pystoned/dataset.py
 pystoned/pCNLS.py
 pystoned/pCQER.py
 pystoned/pICQER.py
 pystoned/plot.py
+pystoned/pwCNLS.py
+pystoned/pwCQER.py
 pystoned/sCQER.py
 pystoned/wCNLS.py
 pystoned/wCQER.py
 pystoned/weakCNLS.py
 pystoned.egg-info/PKG-INFO
 pystoned.egg-info/SOURCES.txt
 pystoned.egg-info/dependency_links.txt
```

### Comparing `pystoned-0.6.5/setup.py` & `pystoned-0.6.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='pystoned',
-    version='0.6.5',
+    version='0.6.6',
     description='A Python Package for Convex Regression and Frontier Estimation',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GPLv3',
     packages=find_packages(),
     author='Sheng Dai, Yu-Hsueh Fang, Chia-Yen Lee, Timo Kuosmanen',
     author_email='sheng.dai@utu.fi',
-    keywords=['StoNED', 'CNLS', 'CER', 'CQR', 'Z-variables','CNLSG'],
+    keywords=['StoNED', 'CNLS', 'CER', 'CQR', 'Z-variables', 'CNLSG'],
     url='https://github.com/ds2010/pyStoNED',
     download_url='https://pypi.org/project/pystoned/',
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
```

