# Comparing `tmp/giefstat-0.0.7.tar.gz` & `tmp/giefstat-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giefstat-0.0.7.tar", last modified: Tue Jun  6 07:48:00 2023, max compression
+gzip compressed data, was "giefstat-0.0.8.tar", last modified: Mon Jun 12 07:18:37 2023, max compression
```

## Comparing `giefstat-0.0.7.tar` & `giefstat-0.0.8.tar`

### file list

```diff
@@ -1,51 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.843257 giefstat-0.0.7/
--rw-rw-rw-   0        0        0     5790 2023-06-06 07:48:00.841260 giefstat-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4391 2023-06-06 07:47:09.000000 giefstat-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.766462 giefstat-0.0.7/giefstat/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:11:18.000000 giefstat-0.0.7/giefstat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.780423 giefstat-0.0.7/giefstat/estimate/
--rw-rw-rw-   0        0        0     3847 2023-06-06 07:02:39.000000 giefstat-0.0.7/giefstat/estimate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.783415 giefstat-0.0.7/giefstat/estimate/correlation_coeff/
--rw-rw-rw-   0        0        0      147 2023-06-06 06:55:59.000000 giefstat-0.0.7/giefstat/estimate/correlation_coeff/__init__.py
--rw-rw-rw-   0        0        0     1191 2023-06-06 06:56:28.000000 giefstat-0.0.7/giefstat/estimate/correlation_coeff/coefficient.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.787406 giefstat-0.0.7/giefstat/estimate/gief/
--rw-rw-rw-   0        0        0      269 2023-06-06 06:29:37.000000 giefstat-0.0.7/giefstat/estimate/gief/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.793389 giefstat-0.0.7/giefstat/estimate/gief/entropy/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/gief/entropy/__init__.py
--rw-rw-rw-   0        0        0      915 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/gief/entropy/cond_entropy.py
--rw-rw-rw-   0        0        0     2379 2023-06-06 06:30:47.000000 giefstat-0.0.7/giefstat/estimate/gief/entropy/marg_entropy.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.802366 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/__init__.py
--rw-rw-rw-   0        0        0    11403 2023-06-06 06:24:52.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/_kraskov.py
--rw-rw-rw-   0        0        0     2582 2023-06-06 06:26:09.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/_ross.py
--rw-rw-rw-   0        0        0     2506 2023-06-06 06:31:02.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/cmi.py
--rw-rw-rw-   0        0        0     1786 2023-06-06 06:31:06.000000 giefstat-0.0.7/giefstat/estimate/gief/mutual_info/mi.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.809346 giefstat-0.0.7/giefstat/estimate/kde/
--rw-rw-rw-   0        0        0       89 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/kde/__init__.py
--rw-rw-rw-   0        0        0     1630 2023-06-06 06:36:23.000000 giefstat-0.0.7/giefstat/estimate/kde/kde.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.819320 giefstat-0.0.7/giefstat/estimate/mic/
--rw-rw-rw-   0        0        0       58 2023-06-06 06:52:51.000000 giefstat-0.0.7/giefstat/estimate/mic/__init__.py
--rw-rw-rw-   0        0        0     1718 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/estimate/mic/_mic_rmic.py
--rw-rw-rw-   0        0        0     2550 2023-06-06 06:52:23.000000 giefstat-0.0.7/giefstat/estimate/mic/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.825304 giefstat-0.0.7/giefstat/estimate/model_based/
--rw-rw-rw-   0        0        0      112 2023-06-06 06:54:51.000000 giefstat-0.0.7/giefstat/estimate/model_based/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-06 06:54:28.000000 giefstat-0.0.7/giefstat/estimate/model_based/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.832285 giefstat-0.0.7/giefstat/estimate/quant_based/
--rw-rw-rw-   0        0        0      146 2023-06-06 06:59:52.000000 giefstat-0.0.7/giefstat/estimate/quant_based/__init__.py
--rw-rw-rw-   0        0        0     6963 2023-06-06 07:08:24.000000 giefstat-0.0.7/giefstat/estimate/quant_based/_quant_darbellay.py
--rw-rw-rw-   0        0        0     2003 2023-06-06 06:58:36.000000 giefstat-0.0.7/giefstat/estimate/quant_based/mi_classic.py
--rw-rw-rw-   0        0        0     1569 2023-06-06 06:59:21.000000 giefstat-0.0.7/giefstat/estimate/quant_based/mi_darbellay.py
--rw-rw-rw-   0        0        0      238 2023-06-06 06:30:32.000000 giefstat-0.0.7/giefstat/setting.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.839266 giefstat-0.0.7/giefstat/statistical_tools/
--rw-rw-rw-   0        0        0      363 2023-06-06 07:03:27.000000 giefstat-0.0.7/giefstat/statistical_tools/__init__.py
--rw-rw-rw-   0        0        0     3142 2023-06-06 06:07:33.000000 giefstat-0.0.7/giefstat/statistical_tools/surrog_indep_test.py
--rw-rw-rw-   0        0        0     2693 2023-06-06 07:05:47.000000 giefstat-0.0.7/giefstat/statistical_tools/time_delayed_association.py
--rw-rw-rw-   0        0        0     9737 2023-06-06 07:08:36.000000 giefstat-0.0.7/giefstat/util.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:48:00.778428 giefstat-0.0.7/giefstat.egg-info/
--rw-rw-rw-   0        0        0     5790 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1327 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 07:48:00.000000 giefstat-0.0.7/giefstat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 07:48:00.843257 giefstat-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      886 2023-06-06 07:47:31.000000 giefstat-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.125492 giefstat-0.0.8/
+-rw-rw-rw-   0        0        0     6297 2023-06-12 07:18:37.124496 giefstat-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4818 2023-06-09 08:43:33.000000 giefstat-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.034737 giefstat-0.0.8/giefstat/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:11:18.000000 giefstat-0.0.8/giefstat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.049696 giefstat-0.0.8/giefstat/compact_recog/
+-rw-rw-rw-   0        0        0      122 2023-06-10 06:14:28.000000 giefstat-0.0.8/giefstat/compact_recog/__init__.py
+-rw-rw-rw-   0        0        0     5231 2023-06-12 06:48:34.000000 giefstat-0.0.8/giefstat/compact_recog/cmim.py
+-rw-rw-rw-   0        0        0     1922 2023-06-12 06:45:24.000000 giefstat-0.0.8/giefstat/compact_recog/fimt.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.052687 giefstat-0.0.8/giefstat/estimate/
+-rw-rw-rw-   0        0        0     3847 2023-06-06 07:02:39.000000 giefstat-0.0.8/giefstat/estimate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.057673 giefstat-0.0.8/giefstat/estimate/correlation_coeff/
+-rw-rw-rw-   0        0        0      147 2023-06-06 06:55:59.000000 giefstat-0.0.8/giefstat/estimate/correlation_coeff/__init__.py
+-rw-rw-rw-   0        0        0     1191 2023-06-06 06:56:28.000000 giefstat-0.0.8/giefstat/estimate/correlation_coeff/coefficient.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.059668 giefstat-0.0.8/giefstat/estimate/gief/
+-rw-rw-rw-   0        0        0      269 2023-06-06 06:29:37.000000 giefstat-0.0.8/giefstat/estimate/gief/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.066650 giefstat-0.0.8/giefstat/estimate/gief/entropy/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/gief/entropy/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/gief/entropy/cond_entropy.py
+-rw-rw-rw-   0        0        0     2379 2023-06-06 06:30:47.000000 giefstat-0.0.8/giefstat/estimate/gief/entropy/marg_entropy.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.082608 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-06-06 06:24:52.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/_kraskov.py
+-rw-rw-rw-   0        0        0     2582 2023-06-06 06:26:09.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/_ross.py
+-rw-rw-rw-   0        0        0     2506 2023-06-06 06:31:02.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/cmi.py
+-rw-rw-rw-   0        0        0     1786 2023-06-06 06:31:06.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/mi.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.090587 giefstat-0.0.8/giefstat/estimate/kde/
+-rw-rw-rw-   0        0        0       89 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/kde/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-06-06 06:36:23.000000 giefstat-0.0.8/giefstat/estimate/kde/kde.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.095571 giefstat-0.0.8/giefstat/estimate/mic/
+-rw-rw-rw-   0        0        0       58 2023-06-06 06:52:51.000000 giefstat-0.0.8/giefstat/estimate/mic/__init__.py
+-rw-rw-rw-   0        0        0     1718 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/mic/_mic_rmic.py
+-rw-rw-rw-   0        0        0     2502 2023-06-07 06:13:57.000000 giefstat-0.0.8/giefstat/estimate/mic/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.102553 giefstat-0.0.8/giefstat/estimate/model_based/
+-rw-rw-rw-   0        0        0      112 2023-06-06 06:54:51.000000 giefstat-0.0.8/giefstat/estimate/model_based/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-06 06:54:28.000000 giefstat-0.0.8/giefstat/estimate/model_based/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.112528 giefstat-0.0.8/giefstat/estimate/quant_based/
+-rw-rw-rw-   0        0        0      146 2023-06-06 06:59:52.000000 giefstat-0.0.8/giefstat/estimate/quant_based/__init__.py
+-rw-rw-rw-   0        0        0     6963 2023-06-06 07:08:24.000000 giefstat-0.0.8/giefstat/estimate/quant_based/_quant_darbellay.py
+-rw-rw-rw-   0        0        0     2003 2023-06-06 06:58:36.000000 giefstat-0.0.8/giefstat/estimate/quant_based/mi_classic.py
+-rw-rw-rw-   0        0        0     1688 2023-06-07 05:34:37.000000 giefstat-0.0.8/giefstat/estimate/quant_based/mi_darbellay.py
+-rw-rw-rw-   0        0        0      238 2023-06-06 06:30:32.000000 giefstat-0.0.8/giefstat/setting.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.119508 giefstat-0.0.8/giefstat/statistical_tools/
+-rw-rw-rw-   0        0        0      363 2023-06-06 07:03:27.000000 giefstat-0.0.8/giefstat/statistical_tools/__init__.py
+-rw-rw-rw-   0        0        0     3142 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/statistical_tools/surrog_indep_test.py
+-rw-rw-rw-   0        0        0     2711 2023-06-06 08:19:38.000000 giefstat-0.0.8/giefstat/statistical_tools/time_delayed_association.py
+-rw-rw-rw-   0        0        0    11507 2023-06-10 06:10:59.000000 giefstat-0.0.8/giefstat/util.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.044708 giefstat-0.0.8/giefstat.egg-info/
+-rw-rw-rw-   0        0        0     6297 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1424 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:18:37.125492 giefstat-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      886 2023-06-12 07:18:26.000000 giefstat-0.0.8/setup.py
```

### Comparing `giefstat-0.0.7/PKG-INFO` & `giefstat-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
 Description: ### general-information-estimation-framework (GIEF)
         
+        ### Package Info
+        
+        https://pypi.org/search/?q=giefstat
+        
+        ### Notes
+        
+        1. <font color="red">根据FGD测试结果, 离散变量可被stdize_values处理后视为连续变量, 代入MI-GIEF中进行计算</font>
+        2. <font color="red">stdize_values在对连续变量处理过程时加入了噪音并归一化</font>
+        
         ### Project Purpose
         
-        This project aims for:
+        This project aims to lay a basis for:
         1. computing higher-order information interactions between different types (discrete & continuous) of variables
         2. uncovering complex associations and causal relationships in high-dimensional data
         
         ### Project Structure
         
         ```
             |-- giefstat
@@ -72,15 +81,16 @@
                 |   |-- indep_test.py               # 独立性检验测试
                 |   |-- statistical_power_test.py   # 统计效能测试
                 |
                 |-- 条件独立性检验
                 |   |-- cond_indep_test.py          # 条件独立性检验测试
                 |
                 |-- 时延关联检测
-                    |-- td_assoc_test.py            # 时延关联检测测试
+                    |-- four_species_test.ipynb     # 四种群时延关联检测测试
+                    |-- four_siso_test.ipynb        # 四SISO系统时延关联检测测试
         
         ```
         
         file dependency plot：
         
         ```mermaid
         flowchart LR
```

### Comparing `giefstat-0.0.7/README.md` & `giefstat-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 ### general-information-estimation-framework (GIEF)
 
+### Package Info
+
+https://pypi.org/search/?q=giefstat
+
+### Notes
+
+1. <font color="red">根据FGD测试结果, 离散变量可被stdize_values处理后视为连续变量, 代入MI-GIEF中进行计算</font>
+2. <font color="red">stdize_values在对连续变量处理过程时加入了噪音并归一化</font>
+
 ### Project Purpose
 
-This project aims for:
+This project aims to lay a basis for:
 1. computing higher-order information interactions between different types (discrete & continuous) of variables
 2. uncovering complex associations and causal relationships in high-dimensional data
 
 ### Project Structure
 
 ```
     |-- giefstat
@@ -64,15 +73,16 @@
         |   |-- indep_test.py               # 独立性检验测试
         |   |-- statistical_power_test.py   # 统计效能测试
         |
         |-- 条件独立性检验
         |   |-- cond_indep_test.py          # 条件独立性检验测试
         |
         |-- 时延关联检测
-            |-- td_assoc_test.py            # 时延关联检测测试
+            |-- four_species_test.ipynb     # 四种群时延关联检测测试
+            |-- four_siso_test.ipynb        # 四SISO系统时延关联检测测试
 
 ```
 
 file dependency plot：
 
 ```mermaid
 flowchart LR
```

### Comparing `giefstat-0.0.7/giefstat/estimate/__init__.py` & `giefstat-0.0.8/giefstat/estimate/__init__.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/correlation_coeff/coefficient.py` & `giefstat-0.0.8/giefstat/estimate/correlation_coeff/coefficient.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/gief/entropy/cond_entropy.py` & `giefstat-0.0.8/giefstat/estimate/gief/entropy/cond_entropy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/gief/entropy/marg_entropy.py` & `giefstat-0.0.8/giefstat/estimate/gief/entropy/marg_entropy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/gief/mutual_info/_kraskov.py` & `giefstat-0.0.8/giefstat/estimate/gief/mutual_info/_kraskov.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/gief/mutual_info/_ross.py` & `giefstat-0.0.8/giefstat/estimate/gief/mutual_info/_ross.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/gief/mutual_info/cmi.py` & `giefstat-0.0.8/giefstat/estimate/gief/mutual_info/cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/gief/mutual_info/mi.py` & `giefstat-0.0.8/giefstat/estimate/gief/mutual_info/mi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/kde/kde.py` & `giefstat-0.0.8/giefstat/estimate/kde/kde.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/mic/_mic_rmic.py` & `giefstat-0.0.8/giefstat/estimate/mic/_mic_rmic.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/mic/mi_cmi.py` & `giefstat-0.0.8/giefstat/estimate/mic/mi_cmi.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,21 +48,22 @@
     
     def __init__(self, x, y):
         self.x = x.copy().reshape(len(x), -1)
         self.y = y.copy().reshape(len(y), -1)
     
     def __call__(self, method="rmic", encode=True):
         # 多维数组逐列离散化, 并合并编码压缩为一维数组
-        # todo 优化此处离散化编码处理, 能否确定y顺序?
         y = _reencode(self.y) if self.y.shape[1] > 1 else self.y.copy()
         x = _reencode(self.x) if self.x.shape[1] > 1 else self.x.copy()
         if method != "rmic":
             return MaximalInfoCoeff(x, y).cal_assoc()
+        
         if encode:
             x = SuperCategorEncoding(x, y).encode(method="mhg") # 进行有监督编码, NOTE x值需为int
+            
         return RefinedMaximalInfoCoeff(x, y).cal_assoc()
             
             
 class CMIC(object):
     """条件最大信息系数"""
     
     def __init__(self, x, y, z):
```

### Comparing `giefstat-0.0.7/giefstat/estimate/model_based/mi_cmi.py` & `giefstat-0.0.8/giefstat/estimate/model_based/mi_cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/quant_based/_quant_darbellay.py` & `giefstat-0.0.8/giefstat/estimate/quant_based/_quant_darbellay.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/quant_based/mi_classic.py` & `giefstat-0.0.8/giefstat/estimate/quant_based/mi_classic.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/estimate/quant_based/mi_darbellay.py` & `giefstat-0.0.8/giefstat/estimate/quant_based/mi_darbellay.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ._quant_darbellay import exec_partition, Cell
 
 
 class MutualInfoDarbellay(object):
     """基于Darbellay自适应分箱的互信息计算"""
     
     def __init__(self, x: np.ndarray, y: np.ndarray):
+        # NOTE: 由于本项目中的Darbellay离散化算法设置, 需要对变量数据进行标准化至0-1区间
         self.x_norm = stdize_values(x, "c")
         self.y_norm = stdize_values(y, "c")
         try:
             assert self.x_norm.shape[1] == 1
             assert self.y_norm.shape[1] == 1
         except Exception as e:
             raise ValueError("不支持非一维变量间的MI计算") from e
```

### Comparing `giefstat-0.0.7/giefstat/statistical_tools/surrog_indep_test.py` & `giefstat-0.0.8/giefstat/statistical_tools/surrog_indep_test.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.7/giefstat/statistical_tools/time_delayed_association.py` & `giefstat-0.0.8/giefstat/statistical_tools/time_delayed_association.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,20 @@
             x_td, y_td, method, xtype=xtype, ytype=ytype, size_bt=size_bt, **kwargs)
         
         td_assocs = np.append(td_assocs, assoc)
         td_indeps = np.append(td_indeps, indep)
         
     # 显示结果, 红色点表示显著
     if show:
-        _show_results(taus, td_assocs, td_indeps)
+        _show_results(taus, td_assocs, td_indeps, method)
         
     return td_assocs, td_indeps
         
 
-def _show_results(taus, td_assocs, td_indeps):
+def _show_results(taus, td_assocs, td_indeps, method):
     plt.figure()
     plt.scatter(
         taus, td_assocs, edgecolors=["k" if p==1 else "r" for p in td_indeps], c="w", lw=2, zorder=1)
     plt.plot(taus, td_assocs, c="k", lw=1.5, zorder=0)
     plt.grid(alpha=0.3, zorder=-1)
     plt.xlabel("$\\tau$")
-    plt.ylabel("MI")
+    plt.ylabel(method)
```

### Comparing `giefstat-0.0.7/giefstat/util.py` & `giefstat-0.0.8/giefstat/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import warnings
 
 warnings.filterwarnings("ignore")
 
 from sklearn.neighbors import BallTree, KDTree
 from sklearn.preprocessing import MinMaxScaler
+from sklearn.metrics import mean_squared_error as mse, explained_variance_score as evs,\
+    r2_score as r2
 from scipy.special import gamma
 import category_encoders as ce
 import pandas as pd
 import numpy as np
 import random
 
 
-# #### 数据编码 #####################################################################################
+####################################################################################################
+# 数据编码
+####################################################################################################
 
 UNSUPER_METHODS = ["ordinal", "random", "count"]
 SUPER_METHODS = ["target", "m_estimator", "james_stein", "glmm", "woe", "leave_one_out", "catboost", "mhg"]
 
 
 class UnsuperCategorEncoding(object):
     """无监督一维类别值编码"""
@@ -151,16 +155,17 @@
         elif method == "catboost":
             x_enc = self.catboost_encoding()
         elif method == "mhg":
             x_enc = self.mhg_encoding()
         return x_enc
     
 
-# #### 数据处理 #####################################################################################
-
+####################################################################################################
+# 数据处理 
+####################################################################################################
 
 # ---- 数据标准化 -----------------------------------------------------------------------------------
 
 def normalize(X):
     scaler = MinMaxScaler()
     X = scaler.fit_transform(X.copy())
     return X
@@ -277,8 +282,48 @@
     # 当样本量过高时执行降采样, 降低计算复杂度
     if len(x_td) > max_len:
         idxs = np.arange(len(x_td))
         np.random.shuffle(idxs)
         idxs = idxs[:max_len]
         x_td, y_td = x_td[idxs], y_td[idxs]
 
-    return x_td, y_td
+    return x_td, y_td
+
+
+####################################################################################################
+# 模型评估 
+####################################################################################################
+
+def _cal_metric(y_true, y_pred, metric: str):
+    y_true, y_pred = y_true.flatten(), y_pred.flatten()
+    if metric == "r2":
+        return r2(y_true, y_pred)
+    if metric == "evs":
+        return evs(y_true, y_pred)
+    if metric == "mse":
+        return mse(y_true, y_pred)
+    if metric == "mape":
+        idxs = np.where(y_true != 0)
+        y_true = y_true[idxs]
+        y_pred = y_pred[idxs]
+        return np.sum(np.abs((y_pred - y_true) / y_true)) / len(y_true)
+
+
+# 模型评价
+def exec_model_test(X, y, model, metric: str="r2", test_ratio: float=0.3, rounds: int=10):
+    """执行建模测试"""
+    X, y = X.copy(), y.copy()
+    N = X.shape[0]
+    test_size = int(N * test_ratio)
+    metrics = []
+    for _ in range(rounds):
+        shuffled_indexes = np.random.permutation(range(N))
+        train_idxs = shuffled_indexes[test_size:]
+        test_idxs = shuffled_indexes[:test_size]
+
+        X_train, X_test = X[train_idxs, :], X[test_idxs, :]
+        y_train, y_test = y[train_idxs], y[test_idxs]
+
+        model.fit(X_train, y_train)
+        m = _cal_metric(y_test, model.predict(X_test), metric)
+        metrics.append(m)
+    return np.mean(metrics), metrics
```

### Comparing `giefstat-0.0.7/giefstat.egg-info/PKG-INFO` & `giefstat-0.0.8/giefstat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
 Description: ### general-information-estimation-framework (GIEF)
         
+        ### Package Info
+        
+        https://pypi.org/search/?q=giefstat
+        
+        ### Notes
+        
+        1. <font color="red">根据FGD测试结果, 离散变量可被stdize_values处理后视为连续变量, 代入MI-GIEF中进行计算</font>
+        2. <font color="red">stdize_values在对连续变量处理过程时加入了噪音并归一化</font>
+        
         ### Project Purpose
         
-        This project aims for:
+        This project aims to lay a basis for:
         1. computing higher-order information interactions between different types (discrete & continuous) of variables
         2. uncovering complex associations and causal relationships in high-dimensional data
         
         ### Project Structure
         
         ```
             |-- giefstat
@@ -72,15 +81,16 @@
                 |   |-- indep_test.py               # 独立性检验测试
                 |   |-- statistical_power_test.py   # 统计效能测试
                 |
                 |-- 条件独立性检验
                 |   |-- cond_indep_test.py          # 条件独立性检验测试
                 |
                 |-- 时延关联检测
-                    |-- td_assoc_test.py            # 时延关联检测测试
+                    |-- four_species_test.ipynb     # 四种群时延关联检测测试
+                    |-- four_siso_test.ipynb        # 四SISO系统时延关联检测测试
         
         ```
         
         file dependency plot：
         
         ```mermaid
         flowchart LR
```

### Comparing `giefstat-0.0.7/giefstat.egg-info/SOURCES.txt` & `giefstat-0.0.8/giefstat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 giefstat/setting.py
 giefstat/util.py
 giefstat.egg-info/PKG-INFO
 giefstat.egg-info/SOURCES.txt
 giefstat.egg-info/dependency_links.txt
 giefstat.egg-info/requires.txt
 giefstat.egg-info/top_level.txt
+giefstat/compact_recog/__init__.py
+giefstat/compact_recog/cmim.py
+giefstat/compact_recog/fimt.py
 giefstat/estimate/__init__.py
 giefstat/estimate/correlation_coeff/__init__.py
 giefstat/estimate/correlation_coeff/coefficient.py
 giefstat/estimate/gief/__init__.py
 giefstat/estimate/gief/entropy/__init__.py
 giefstat/estimate/gief/entropy/cond_entropy.py
 giefstat/estimate/gief/entropy/marg_entropy.py
```

### Comparing `giefstat-0.0.7/setup.py` & `giefstat-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 DESCRIPTION = "Package for information estimation, independence test, etc."
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text(encoding="utf-8")
 
 setup(
     name="giefstat",
     version=VERSION,
```

