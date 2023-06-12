# Comparing `tmp/giefstat-0.0.8.tar.gz` & `tmp/giefstat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giefstat-0.0.8.tar", last modified: Mon Jun 12 07:18:37 2023, max compression
+gzip compressed data, was "giefstat-0.0.9.tar", last modified: Mon Jun 12 07:27:22 2023, max compression
```

## Comparing `giefstat-0.0.8.tar` & `giefstat-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.125492 giefstat-0.0.8/
--rw-rw-rw-   0        0        0     6297 2023-06-12 07:18:37.124496 giefstat-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4818 2023-06-09 08:43:33.000000 giefstat-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.034737 giefstat-0.0.8/giefstat/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:11:18.000000 giefstat-0.0.8/giefstat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.049696 giefstat-0.0.8/giefstat/compact_recog/
--rw-rw-rw-   0        0        0      122 2023-06-10 06:14:28.000000 giefstat-0.0.8/giefstat/compact_recog/__init__.py
--rw-rw-rw-   0        0        0     5231 2023-06-12 06:48:34.000000 giefstat-0.0.8/giefstat/compact_recog/cmim.py
--rw-rw-rw-   0        0        0     1922 2023-06-12 06:45:24.000000 giefstat-0.0.8/giefstat/compact_recog/fimt.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.052687 giefstat-0.0.8/giefstat/estimate/
--rw-rw-rw-   0        0        0     3847 2023-06-06 07:02:39.000000 giefstat-0.0.8/giefstat/estimate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.057673 giefstat-0.0.8/giefstat/estimate/correlation_coeff/
--rw-rw-rw-   0        0        0      147 2023-06-06 06:55:59.000000 giefstat-0.0.8/giefstat/estimate/correlation_coeff/__init__.py
--rw-rw-rw-   0        0        0     1191 2023-06-06 06:56:28.000000 giefstat-0.0.8/giefstat/estimate/correlation_coeff/coefficient.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.059668 giefstat-0.0.8/giefstat/estimate/gief/
--rw-rw-rw-   0        0        0      269 2023-06-06 06:29:37.000000 giefstat-0.0.8/giefstat/estimate/gief/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.066650 giefstat-0.0.8/giefstat/estimate/gief/entropy/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/gief/entropy/__init__.py
--rw-rw-rw-   0        0        0      915 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/gief/entropy/cond_entropy.py
--rw-rw-rw-   0        0        0     2379 2023-06-06 06:30:47.000000 giefstat-0.0.8/giefstat/estimate/gief/entropy/marg_entropy.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.082608 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/__init__.py
--rw-rw-rw-   0        0        0    11403 2023-06-06 06:24:52.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/_kraskov.py
--rw-rw-rw-   0        0        0     2582 2023-06-06 06:26:09.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/_ross.py
--rw-rw-rw-   0        0        0     2506 2023-06-06 06:31:02.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/cmi.py
--rw-rw-rw-   0        0        0     1786 2023-06-06 06:31:06.000000 giefstat-0.0.8/giefstat/estimate/gief/mutual_info/mi.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.090587 giefstat-0.0.8/giefstat/estimate/kde/
--rw-rw-rw-   0        0        0       89 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/kde/__init__.py
--rw-rw-rw-   0        0        0     1630 2023-06-06 06:36:23.000000 giefstat-0.0.8/giefstat/estimate/kde/kde.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.095571 giefstat-0.0.8/giefstat/estimate/mic/
--rw-rw-rw-   0        0        0       58 2023-06-06 06:52:51.000000 giefstat-0.0.8/giefstat/estimate/mic/__init__.py
--rw-rw-rw-   0        0        0     1718 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/estimate/mic/_mic_rmic.py
--rw-rw-rw-   0        0        0     2502 2023-06-07 06:13:57.000000 giefstat-0.0.8/giefstat/estimate/mic/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.102553 giefstat-0.0.8/giefstat/estimate/model_based/
--rw-rw-rw-   0        0        0      112 2023-06-06 06:54:51.000000 giefstat-0.0.8/giefstat/estimate/model_based/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-06 06:54:28.000000 giefstat-0.0.8/giefstat/estimate/model_based/mi_cmi.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.112528 giefstat-0.0.8/giefstat/estimate/quant_based/
--rw-rw-rw-   0        0        0      146 2023-06-06 06:59:52.000000 giefstat-0.0.8/giefstat/estimate/quant_based/__init__.py
--rw-rw-rw-   0        0        0     6963 2023-06-06 07:08:24.000000 giefstat-0.0.8/giefstat/estimate/quant_based/_quant_darbellay.py
--rw-rw-rw-   0        0        0     2003 2023-06-06 06:58:36.000000 giefstat-0.0.8/giefstat/estimate/quant_based/mi_classic.py
--rw-rw-rw-   0        0        0     1688 2023-06-07 05:34:37.000000 giefstat-0.0.8/giefstat/estimate/quant_based/mi_darbellay.py
--rw-rw-rw-   0        0        0      238 2023-06-06 06:30:32.000000 giefstat-0.0.8/giefstat/setting.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.119508 giefstat-0.0.8/giefstat/statistical_tools/
--rw-rw-rw-   0        0        0      363 2023-06-06 07:03:27.000000 giefstat-0.0.8/giefstat/statistical_tools/__init__.py
--rw-rw-rw-   0        0        0     3142 2023-06-06 06:07:33.000000 giefstat-0.0.8/giefstat/statistical_tools/surrog_indep_test.py
--rw-rw-rw-   0        0        0     2711 2023-06-06 08:19:38.000000 giefstat-0.0.8/giefstat/statistical_tools/time_delayed_association.py
--rw-rw-rw-   0        0        0    11507 2023-06-10 06:10:59.000000 giefstat-0.0.8/giefstat/util.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:18:37.044708 giefstat-0.0.8/giefstat.egg-info/
--rw-rw-rw-   0        0        0     6297 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1424 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 07:18:36.000000 giefstat-0.0.8/giefstat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 07:18:37.125492 giefstat-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      886 2023-06-12 07:18:26.000000 giefstat-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.994144 giefstat-0.0.9/
+-rw-rw-rw-   0        0        0     7133 2023-06-12 07:27:22.993146 giefstat-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5526 2023-06-12 07:26:47.000000 giefstat-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.918348 giefstat-0.0.9/giefstat/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:11:18.000000 giefstat-0.0.9/giefstat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.935301 giefstat-0.0.9/giefstat/compact_recog/
+-rw-rw-rw-   0        0        0      122 2023-06-10 06:14:28.000000 giefstat-0.0.9/giefstat/compact_recog/__init__.py
+-rw-rw-rw-   0        0        0     5231 2023-06-12 06:48:34.000000 giefstat-0.0.9/giefstat/compact_recog/cmim.py
+-rw-rw-rw-   0        0        0     1922 2023-06-12 06:45:24.000000 giefstat-0.0.9/giefstat/compact_recog/fimt.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.938294 giefstat-0.0.9/giefstat/estimate/
+-rw-rw-rw-   0        0        0     3847 2023-06-06 07:02:39.000000 giefstat-0.0.9/giefstat/estimate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.944278 giefstat-0.0.9/giefstat/estimate/correlation_coeff/
+-rw-rw-rw-   0        0        0      147 2023-06-06 06:55:59.000000 giefstat-0.0.9/giefstat/estimate/correlation_coeff/__init__.py
+-rw-rw-rw-   0        0        0     1191 2023-06-06 06:56:28.000000 giefstat-0.0.9/giefstat/estimate/correlation_coeff/coefficient.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.946272 giefstat-0.0.9/giefstat/estimate/gief/
+-rw-rw-rw-   0        0        0      269 2023-06-06 06:29:37.000000 giefstat-0.0.9/giefstat/estimate/gief/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.952255 giefstat-0.0.9/giefstat/estimate/gief/entropy/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.9/giefstat/estimate/gief/entropy/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-06-06 06:07:33.000000 giefstat-0.0.9/giefstat/estimate/gief/entropy/cond_entropy.py
+-rw-rw-rw-   0        0        0     2379 2023-06-06 06:30:47.000000 giefstat-0.0.9/giefstat/estimate/gief/entropy/marg_entropy.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.963226 giefstat-0.0.9/giefstat/estimate/gief/mutual_info/
+-rw-rw-rw-   0        0        0        0 2023-06-06 06:07:33.000000 giefstat-0.0.9/giefstat/estimate/gief/mutual_info/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-06-06 06:24:52.000000 giefstat-0.0.9/giefstat/estimate/gief/mutual_info/_kraskov.py
+-rw-rw-rw-   0        0        0     2582 2023-06-06 06:26:09.000000 giefstat-0.0.9/giefstat/estimate/gief/mutual_info/_ross.py
+-rw-rw-rw-   0        0        0     2506 2023-06-06 06:31:02.000000 giefstat-0.0.9/giefstat/estimate/gief/mutual_info/cmi.py
+-rw-rw-rw-   0        0        0     1786 2023-06-06 06:31:06.000000 giefstat-0.0.9/giefstat/estimate/gief/mutual_info/mi.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.967217 giefstat-0.0.9/giefstat/estimate/kde/
+-rw-rw-rw-   0        0        0       89 2023-06-06 06:07:33.000000 giefstat-0.0.9/giefstat/estimate/kde/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-06-06 06:36:23.000000 giefstat-0.0.9/giefstat/estimate/kde/kde.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.973201 giefstat-0.0.9/giefstat/estimate/mic/
+-rw-rw-rw-   0        0        0       58 2023-06-06 06:52:51.000000 giefstat-0.0.9/giefstat/estimate/mic/__init__.py
+-rw-rw-rw-   0        0        0     1718 2023-06-06 06:07:33.000000 giefstat-0.0.9/giefstat/estimate/mic/_mic_rmic.py
+-rw-rw-rw-   0        0        0     2502 2023-06-07 06:13:57.000000 giefstat-0.0.9/giefstat/estimate/mic/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.977190 giefstat-0.0.9/giefstat/estimate/model_based/
+-rw-rw-rw-   0        0        0      112 2023-06-06 06:54:51.000000 giefstat-0.0.9/giefstat/estimate/model_based/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-06 06:54:28.000000 giefstat-0.0.9/giefstat/estimate/model_based/mi_cmi.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.985167 giefstat-0.0.9/giefstat/estimate/quant_based/
+-rw-rw-rw-   0        0        0      146 2023-06-06 06:59:52.000000 giefstat-0.0.9/giefstat/estimate/quant_based/__init__.py
+-rw-rw-rw-   0        0        0     6963 2023-06-06 07:08:24.000000 giefstat-0.0.9/giefstat/estimate/quant_based/_quant_darbellay.py
+-rw-rw-rw-   0        0        0     2003 2023-06-06 06:58:36.000000 giefstat-0.0.9/giefstat/estimate/quant_based/mi_classic.py
+-rw-rw-rw-   0        0        0     1688 2023-06-07 05:34:37.000000 giefstat-0.0.9/giefstat/estimate/quant_based/mi_darbellay.py
+-rw-rw-rw-   0        0        0      238 2023-06-06 06:30:32.000000 giefstat-0.0.9/giefstat/setting.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.991152 giefstat-0.0.9/giefstat/statistical_tools/
+-rw-rw-rw-   0        0        0      363 2023-06-06 07:03:27.000000 giefstat-0.0.9/giefstat/statistical_tools/__init__.py
+-rw-rw-rw-   0        0        0     3142 2023-06-06 06:07:33.000000 giefstat-0.0.9/giefstat/statistical_tools/surrog_indep_test.py
+-rw-rw-rw-   0        0        0     2711 2023-06-06 08:19:38.000000 giefstat-0.0.9/giefstat/statistical_tools/time_delayed_association.py
+-rw-rw-rw-   0        0        0    11507 2023-06-10 06:10:59.000000 giefstat-0.0.9/giefstat/util.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:27:22.930314 giefstat-0.0.9/giefstat.egg-info/
+-rw-rw-rw-   0        0        0     7133 2023-06-12 07:27:22.000000 giefstat-0.0.9/giefstat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1424 2023-06-12 07:27:22.000000 giefstat-0.0.9/giefstat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:27:22.000000 giefstat-0.0.9/giefstat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-12 07:27:22.000000 giefstat-0.0.9/giefstat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 07:27:22.000000 giefstat-0.0.9/giefstat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:27:22.995142 giefstat-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      886 2023-06-12 07:27:02.000000 giefstat-0.0.9/setup.py
```

### Comparing `giefstat-0.0.8/PKG-INFO` & `giefstat-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
 Description: ### general-information-estimation-framework (GIEF)
         
         ### Package Info
         
         https://pypi.org/search/?q=giefstat
         
-        ### Notes
-        
-        1. <font color="red">根据FGD测试结果, 离散变量可被stdize_values处理后视为连续变量, 代入MI-GIEF中进行计算</font>
-        2. <font color="red">stdize_values在对连续变量处理过程时加入了噪音并归一化</font>
-        
         ### Project Purpose
         
         This project aims to lay a basis for:
         1. computing higher-order information interactions between different types (discrete & continuous) of variables
         2. uncovering complex associations and causal relationships in high-dimensional data
+           
+        ### Notes
+        
+        1. <font color="red">根据FGD测试结果, 离散变量可被stdize_values处理后视为连续变量, 代入MI-GIEF中进行计算</font>
+        2. <font color="red">stdize_values在对连续变量处理过程时加入了噪音并归一化</font>
         
         ### Project Structure
         
         ```
             |-- giefstat
             |   |-- __init__.py
             |   |-- setting.py          # 项目设置
@@ -68,30 +68,46 @@
             |   |   |-- quant_based
             |   |       |-- __init__.py
             |   |       |-- _quant_darbellay.py # Darbellay数据离散化方法
             |   |       |-- mi_classic.py   # 基于经典等距和等频离散化的互信息估计
             |   |       |-- mi_darbellay.py # 基于Darbellay离散化的互信息估计
             |   |   
             |   |-- statistical_tools
+            |   |   |-- __init__.py
+            |   |   |-- surrog_indep_test.py                # 基于代用数据的关联度量和独立性检验
+            |   |   |-- time_delayed_association.py         # 时延关联检测
+            |   |
+            |   |-- compact_recog
             |       |-- __init__.py
-            |       |-- surrog_indep_test.py                # 基于代用数据的关联度量和独立性检验
-            |       |-- time_delayed_association.py         # 时延关联检测
-            |
+            |       |-- cmim.py     # 基于CMIM-GIEF的紧凑变量排序算法
+            |       |-- fimt.py     # 基于FIMT测试的紧凑变量识别
+            |   
             |-- script
                 |-- 独立性检验
                 |   |-- indep_test.py               # 独立性检验测试
                 |   |-- statistical_power_test.py   # 统计效能测试
                 |
                 |-- 条件独立性检验
                 |   |-- cond_indep_test.py          # 条件独立性检验测试
                 |
                 |-- 时延关联检测
-                    |-- four_species_test.ipynb     # 四种群时延关联检测测试
-                    |-- four_siso_test.ipynb        # 四SISO系统时延关联检测测试
-        
+                |   |-- four_species_test.ipynb     # 四种群时延关联检测测试
+                |   |-- four_siso_test.ipynb        # 四SISO系统时延关联检测测试
+                |
+                |-- 各系数耗时对比
+                |   |-- comparison.ipynb            # 耗时对比测试
+                |   |-- total_tc.csv                # 耗时测试结果
+                |
+                |-- 各相关和关联系数对比
+                |   |-- comparison.ipynb            # 各系数计算效果对比
+                |
+                |-- 一致性测试
+                |-- Darbellay分箱效果展示
+                |-- FGD过程数据关联测试
+                |-- 基于CMIM-GIEF的紧凑关联识别.ipynb
         ```
         
         file dependency plot：
         
         ```mermaid
         flowchart LR
         
@@ -132,14 +148,14 @@
         
         ### TODOs
         
         1. ~~script/独立性检验/statistical_power_test.py~~
         2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
         3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
         4. ~~继续estimate中mic及剩下的部分的封装测试~~
-        5. 一致性测试
-        6. 时效性测试
+        5. ~~一致性测试~~
+        6. ~~时效性测试~~
         
 Keywords: python,information estimation
 Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `giefstat-0.0.8/README.md` & `giefstat-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ### general-information-estimation-framework (GIEF)
 
 ### Package Info
 
 https://pypi.org/search/?q=giefstat
 
-### Notes
-
-1. <font color="red">根据FGD测试结果, 离散变量可被stdize_values处理后视为连续变量, 代入MI-GIEF中进行计算</font>
-2. <font color="red">stdize_values在对连续变量处理过程时加入了噪音并归一化</font>
-
 ### Project Purpose
 
 This project aims to lay a basis for:
 1. computing higher-order information interactions between different types (discrete & continuous) of variables
 2. uncovering complex associations and causal relationships in high-dimensional data
+   
+### Notes
+
+1. <font color="red">根据FGD测试结果, 离散变量可被stdize_values处理后视为连续变量, 代入MI-GIEF中进行计算</font>
+2. <font color="red">stdize_values在对连续变量处理过程时加入了噪音并归一化</font>
 
 ### Project Structure
 
 ```
     |-- giefstat
     |   |-- __init__.py
     |   |-- setting.py          # 项目设置
@@ -60,30 +60,46 @@
     |   |   |-- quant_based
     |   |       |-- __init__.py
     |   |       |-- _quant_darbellay.py # Darbellay数据离散化方法
     |   |       |-- mi_classic.py   # 基于经典等距和等频离散化的互信息估计
     |   |       |-- mi_darbellay.py # 基于Darbellay离散化的互信息估计
     |   |   
     |   |-- statistical_tools
+    |   |   |-- __init__.py
+    |   |   |-- surrog_indep_test.py                # 基于代用数据的关联度量和独立性检验
+    |   |   |-- time_delayed_association.py         # 时延关联检测
+    |   |
+    |   |-- compact_recog
     |       |-- __init__.py
-    |       |-- surrog_indep_test.py                # 基于代用数据的关联度量和独立性检验
-    |       |-- time_delayed_association.py         # 时延关联检测
-    |
+    |       |-- cmim.py     # 基于CMIM-GIEF的紧凑变量排序算法
+    |       |-- fimt.py     # 基于FIMT测试的紧凑变量识别
+    |   
     |-- script
         |-- 独立性检验
         |   |-- indep_test.py               # 独立性检验测试
         |   |-- statistical_power_test.py   # 统计效能测试
         |
         |-- 条件独立性检验
         |   |-- cond_indep_test.py          # 条件独立性检验测试
         |
         |-- 时延关联检测
-            |-- four_species_test.ipynb     # 四种群时延关联检测测试
-            |-- four_siso_test.ipynb        # 四SISO系统时延关联检测测试
-
+        |   |-- four_species_test.ipynb     # 四种群时延关联检测测试
+        |   |-- four_siso_test.ipynb        # 四SISO系统时延关联检测测试
+        |
+        |-- 各系数耗时对比
+        |   |-- comparison.ipynb            # 耗时对比测试
+        |   |-- total_tc.csv                # 耗时测试结果
+        |
+        |-- 各相关和关联系数对比
+        |   |-- comparison.ipynb            # 各系数计算效果对比
+        |
+        |-- 一致性测试
+        |-- Darbellay分箱效果展示
+        |-- FGD过程数据关联测试
+        |-- 基于CMIM-GIEF的紧凑关联识别.ipynb
 ```
 
 file dependency plot：
 
 ```mermaid
 flowchart LR
 
@@ -124,9 +140,9 @@
 
 ### TODOs
 
 1. ~~script/独立性检验/statistical_power_test.py~~
 2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
 3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
 4. ~~继续estimate中mic及剩下的部分的封装测试~~
-5. 一致性测试
-6. 时效性测试
+5. ~~一致性测试~~
+6. ~~时效性测试~~
```

### Comparing `giefstat-0.0.8/giefstat/compact_recog/cmim.py` & `giefstat-0.0.9/giefstat/compact_recog/cmim.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/compact_recog/fimt.py` & `giefstat-0.0.9/giefstat/compact_recog/fimt.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/__init__.py` & `giefstat-0.0.9/giefstat/estimate/__init__.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/correlation_coeff/coefficient.py` & `giefstat-0.0.9/giefstat/estimate/correlation_coeff/coefficient.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/gief/entropy/cond_entropy.py` & `giefstat-0.0.9/giefstat/estimate/gief/entropy/cond_entropy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/gief/entropy/marg_entropy.py` & `giefstat-0.0.9/giefstat/estimate/gief/entropy/marg_entropy.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/gief/mutual_info/_kraskov.py` & `giefstat-0.0.9/giefstat/estimate/gief/mutual_info/_kraskov.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/gief/mutual_info/_ross.py` & `giefstat-0.0.9/giefstat/estimate/gief/mutual_info/_ross.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/gief/mutual_info/cmi.py` & `giefstat-0.0.9/giefstat/estimate/gief/mutual_info/cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/gief/mutual_info/mi.py` & `giefstat-0.0.9/giefstat/estimate/gief/mutual_info/mi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/kde/kde.py` & `giefstat-0.0.9/giefstat/estimate/kde/kde.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/mic/_mic_rmic.py` & `giefstat-0.0.9/giefstat/estimate/mic/_mic_rmic.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/mic/mi_cmi.py` & `giefstat-0.0.9/giefstat/estimate/mic/mi_cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/model_based/mi_cmi.py` & `giefstat-0.0.9/giefstat/estimate/model_based/mi_cmi.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/quant_based/_quant_darbellay.py` & `giefstat-0.0.9/giefstat/estimate/quant_based/_quant_darbellay.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/quant_based/mi_classic.py` & `giefstat-0.0.9/giefstat/estimate/quant_based/mi_classic.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/estimate/quant_based/mi_darbellay.py` & `giefstat-0.0.9/giefstat/estimate/quant_based/mi_darbellay.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/statistical_tools/surrog_indep_test.py` & `giefstat-0.0.9/giefstat/statistical_tools/surrog_indep_test.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/statistical_tools/time_delayed_association.py` & `giefstat-0.0.9/giefstat/statistical_tools/time_delayed_association.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat/util.py` & `giefstat-0.0.9/giefstat/util.py`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/giefstat.egg-info/PKG-INFO` & `giefstat-0.0.9/giefstat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: giefstat
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for information estimation, independence test, etc.
 Home-page: https://github.com/Ulti-Dreisteine/general-information-estimation-framework
 Author: Dreisteine
 Author-email: dreisteine@163.com
 License: MIT
 Description: ### general-information-estimation-framework (GIEF)
         
         ### Package Info
         
         https://pypi.org/search/?q=giefstat
         
-        ### Notes
-        
-        1. <font color="red">根据FGD测试结果, 离散变量可被stdize_values处理后视为连续变量, 代入MI-GIEF中进行计算</font>
-        2. <font color="red">stdize_values在对连续变量处理过程时加入了噪音并归一化</font>
-        
         ### Project Purpose
         
         This project aims to lay a basis for:
         1. computing higher-order information interactions between different types (discrete & continuous) of variables
         2. uncovering complex associations and causal relationships in high-dimensional data
+           
+        ### Notes
+        
+        1. <font color="red">根据FGD测试结果, 离散变量可被stdize_values处理后视为连续变量, 代入MI-GIEF中进行计算</font>
+        2. <font color="red">stdize_values在对连续变量处理过程时加入了噪音并归一化</font>
         
         ### Project Structure
         
         ```
             |-- giefstat
             |   |-- __init__.py
             |   |-- setting.py          # 项目设置
@@ -68,30 +68,46 @@
             |   |   |-- quant_based
             |   |       |-- __init__.py
             |   |       |-- _quant_darbellay.py # Darbellay数据离散化方法
             |   |       |-- mi_classic.py   # 基于经典等距和等频离散化的互信息估计
             |   |       |-- mi_darbellay.py # 基于Darbellay离散化的互信息估计
             |   |   
             |   |-- statistical_tools
+            |   |   |-- __init__.py
+            |   |   |-- surrog_indep_test.py                # 基于代用数据的关联度量和独立性检验
+            |   |   |-- time_delayed_association.py         # 时延关联检测
+            |   |
+            |   |-- compact_recog
             |       |-- __init__.py
-            |       |-- surrog_indep_test.py                # 基于代用数据的关联度量和独立性检验
-            |       |-- time_delayed_association.py         # 时延关联检测
-            |
+            |       |-- cmim.py     # 基于CMIM-GIEF的紧凑变量排序算法
+            |       |-- fimt.py     # 基于FIMT测试的紧凑变量识别
+            |   
             |-- script
                 |-- 独立性检验
                 |   |-- indep_test.py               # 独立性检验测试
                 |   |-- statistical_power_test.py   # 统计效能测试
                 |
                 |-- 条件独立性检验
                 |   |-- cond_indep_test.py          # 条件独立性检验测试
                 |
                 |-- 时延关联检测
-                    |-- four_species_test.ipynb     # 四种群时延关联检测测试
-                    |-- four_siso_test.ipynb        # 四SISO系统时延关联检测测试
-        
+                |   |-- four_species_test.ipynb     # 四种群时延关联检测测试
+                |   |-- four_siso_test.ipynb        # 四SISO系统时延关联检测测试
+                |
+                |-- 各系数耗时对比
+                |   |-- comparison.ipynb            # 耗时对比测试
+                |   |-- total_tc.csv                # 耗时测试结果
+                |
+                |-- 各相关和关联系数对比
+                |   |-- comparison.ipynb            # 各系数计算效果对比
+                |
+                |-- 一致性测试
+                |-- Darbellay分箱效果展示
+                |-- FGD过程数据关联测试
+                |-- 基于CMIM-GIEF的紧凑关联识别.ipynb
         ```
         
         file dependency plot：
         
         ```mermaid
         flowchart LR
         
@@ -132,14 +148,14 @@
         
         ### TODOs
         
         1. ~~script/独立性检验/statistical_power_test.py~~
         2. ~~scipt/时延关联检测/main.py中背景值较高, 与代用数据计算结果不吻合~~
         3. statistital_significance/surrog_indep_test.py中通过随机抽样获得关联值分布
         4. ~~继续estimate中mic及剩下的部分的封装测试~~
-        5. 一致性测试
-        6. 时效性测试
+        5. ~~一致性测试~~
+        6. ~~时效性测试~~
         
 Keywords: python,information estimation
 Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `giefstat-0.0.8/giefstat.egg-info/SOURCES.txt` & `giefstat-0.0.9/giefstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giefstat-0.0.8/setup.py` & `giefstat-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "Package for information estimation, independence test, etc."
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text(encoding="utf-8")
 
 setup(
     name="giefstat",
     version=VERSION,
```

