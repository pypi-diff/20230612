# Comparing `tmp/naluconfigs-11.0.1.tar.gz` & `tmp/naluconfigs-11.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-11.0.1.tar", last modified: Fri Jun  2 00:09:28 2023, max compression
+gzip compressed data, was "naluconfigs-11.0.2.tar", last modified: Sun Jun 11 00:41:24 2023, max compression
```

## Comparing `naluconfigs-11.0.1.tar` & `naluconfigs-11.0.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:09:28.171353 naluconfigs-11.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-02 00:09:28.171353 naluconfigs-11.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 00:09:28.171353 naluconfigs-11.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:09:28.163353 naluconfigs-11.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:09:28.163353 naluconfigs-11.0.1/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:09:28.163353 naluconfigs-11.0.1/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:09:28.167353 naluconfigs-11.0.1/src/naluconfigs/data/chips/
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/chips/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/chips/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/chips/aodsv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/chips/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/chips/hdsocv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/chips/udc16.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:09:28.167353 naluconfigs-11.0.1/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:09:28.171353 naluconfigs-11.0.1/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32645 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:09:28.163353 naluconfigs-11.0.1/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-02 00:09:28.000000 naluconfigs-11.0.1/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-02 00:09:28.000000 naluconfigs-11.0.1/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:09:28.000000 naluconfigs-11.0.1/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 00:09:28.000000 naluconfigs-11.0.1/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 00:09:28.000000 naluconfigs-11.0.1/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:09:28.171353 naluconfigs-11.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/tests/test_multichip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-02 00:09:06.000000 naluconfigs-11.0.1/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:41:24.246595 naluconfigs-11.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-11 00:41:24.246595 naluconfigs-11.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 00:41:24.246595 naluconfigs-11.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:41:24.234593 naluconfigs-11.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:41:24.238594 naluconfigs-11.0.2/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:41:24.234593 naluconfigs-11.0.2/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:41:24.238594 naluconfigs-11.0.2/src/naluconfigs/data/chips/
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/chips/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/chips/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/chips/aodsv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/chips/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    51581 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/chips/hdsocv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/chips/udc16.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:41:24.242594 naluconfigs-11.0.2/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:41:24.246595 naluconfigs-11.0.2/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32645 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25224 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:41:24.238594 naluconfigs-11.0.2/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-11 00:41:24.000000 naluconfigs-11.0.2/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-11 00:41:24.000000 naluconfigs-11.0.2/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 00:41:24.000000 naluconfigs-11.0.2/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-11 00:41:24.000000 naluconfigs-11.0.2/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 00:41:24.000000 naluconfigs-11.0.2/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:41:24.246595 naluconfigs-11.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/tests/test_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-11 00:41:02.000000 naluconfigs-11.0.2/tests/test_range_keys.py
```

### Comparing `naluconfigs-11.0.1/PKG-INFO` & `naluconfigs-11.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.0.1
+Version: 11.0.2
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.0.1/README.md` & `naluconfigs-11.0.2/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/pyproject.toml` & `naluconfigs-11.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/setup.py` & `naluconfigs-11.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/__init__.py` & `naluconfigs-11.0.2/src/naluconfigs/__init__.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/_constructors.py` & `naluconfigs-11.0.2/src/naluconfigs/_constructors.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/chips/aardvarcv3.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/chips/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/chips/aodsv1.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/chips/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/chips/aodsv2.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/chips/aodsv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/chips/asocv3.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/chips/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/chips/hdsocv1.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/chips/hdsocv1.yml`

 * *Files 0% similar despite different names*

```diff
@@ -801,15 +801,15 @@
       value: 44
     wrstrb1_te_left:
       address: 0x4D
       bitposition: 0
       bitwidth: 12
       description: 'WRSTRB1_TE'
       readwrite: rw
-      value: 57
+      value: 56
     wrstrb2_le_left:
       address: 0x4E
       bitposition: 0
       bitwidth: 12
       description: 'WRSTRB2_LE'
       readwrite: rw
       value: 8
```

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/chips/udc16.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/chips/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-11.0.2/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/aodsoc_asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/aodsv2_eval.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/asocv2.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/asocv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/asocv3.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/hiper.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/hiper.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/hiper_fmc.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/oleas_box2.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/siread.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/trbhm.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/upac32.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/upac96.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/upaci.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/data/registers/zdigitizer.yml` & `naluconfigs-11.0.2/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/exceptions.py` & `naluconfigs-11.0.2/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/helpers.py` & `naluconfigs-11.0.2/src/naluconfigs/helpers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs/postprocess.py` & `naluconfigs-11.0.2/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-11.0.2/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 11.0.1
+Version: 11.0.2
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-11.0.1/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-11.0.2/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/tests/test_hex_addr_converter.py` & `naluconfigs-11.0.2/tests/test_hex_addr_converter.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/tests/test_i2c_registers.py` & `naluconfigs-11.0.2/tests/test_i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/tests/test_multichip.py` & `naluconfigs-11.0.2/tests/test_multichip.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/tests/test_post_processing.py` & `naluconfigs-11.0.2/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-11.0.1/tests/test_range_keys.py` & `naluconfigs-11.0.2/tests/test_range_keys.py`

 * *Files identical despite different names*

