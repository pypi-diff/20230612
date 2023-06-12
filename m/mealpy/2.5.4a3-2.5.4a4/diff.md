# Comparing `tmp/mealpy-2.5.4a3.tar.gz` & `tmp/mealpy-2.5.4a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mealpy-2.5.4a3.tar", last modified: Thu May 18 04:30:05 2023, max compression
+gzip compressed data, was "mealpy-2.5.4a4.tar", last modified: Mon Jun 12 03:31:20 2023, max compression
```

## Comparing `mealpy-2.5.4a3.tar` & `mealpy-2.5.4a4.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/
--rw-r--r--   0 runner    (1001) docker     (123)    58092 2023-05-18 04:28:16.000000 mealpy-2.5.4a3/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 04:28:16.000000 mealpy-2.5.4a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 04:28:16.000000 mealpy-2.5.4a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    88069 2023-05-18 04:28:16.000000 mealpy-2.5.4a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.981119 mealpy-2.5.4a3/mealpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.989120 mealpy-2.5.4a3/mealpy/bio_based/
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/BBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/BBOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/BMO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/EOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/IWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/SBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/SMA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/SOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/SOS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/TPO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/TSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/VCS.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/WHO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.993120 mealpy-2.5.4a3/mealpy/evolutionary_based/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/CRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/DE.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/EP.py
--rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/ES.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/FPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    38895 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/GA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/MA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.997120 mealpy-2.5.4a3/mealpy/human_based/
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/BRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/BSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/CA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/CHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/FBIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/GSKA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/HBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/HCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/ICA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/LCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/QSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/SARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/SPBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/SSDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/TLO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/TOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/WarSO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.005120 mealpy-2.5.4a3/mealpy/math_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/AOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/CEM.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/CGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/CircleSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/GBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/HC.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/PSS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/RUN.py
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/SCA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/SHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/multitask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.005120 mealpy-2.5.4a3/mealpy/music_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/music_based/HS.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/music_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33913 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.005120 mealpy-2.5.4a3/mealpy/physics_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/ASO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/ArchOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/CDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/EFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/EO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/EVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/FLA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/HGSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/MVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/NRO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/RIME.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/SA.py
--rw-r--r--   0 runner    (1001) docker     (123)    20830 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/TWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/WDO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.013120 mealpy-2.5.4a3/mealpy/swarm_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ABC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ACOR.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/AGTO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ALO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/AO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/AVOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BES.py
--rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BeesA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/COA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/CSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/CSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/CoatiOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/DMOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/DO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/EHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ESOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FOX.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/GJO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/GOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/GTO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/GWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/HBA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/HGS.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/HHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/JA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MRFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/NGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/NMRA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/OOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/PFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/POA.py
--rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/PSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SCSO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SHO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SLO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SRSR.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SSpiderA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SSpiderO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/STO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SeaHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ServalOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/TDO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/TSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/WOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/WaOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ZOA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.013120 mealpy-2.5.4a3/mealpy/system_based/
--rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/system_based/AEO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/system_based/GCO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/system_based/WCA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/system_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/mealpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/mealpy/utils/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/visualize/linechart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.985120 mealpy-2.5.4a3/mealpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/tests/test_tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.828881 mealpy-2.5.4a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    58140 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    90711 2023-06-12 03:31:20.828881 mealpy-2.5.4a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    88172 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.812881 mealpy-2.5.4a4/mealpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.812881 mealpy-2.5.4a4/mealpy/bio_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/BBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/BBOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/BMO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/EOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/IWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/SBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/SOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/SOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/TPO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/TSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/VCS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/WHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/bio_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.816881 mealpy-2.5.4a4/mealpy/evolutionary_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/evolutionary_based/CRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/evolutionary_based/DE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/evolutionary_based/EP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/evolutionary_based/ES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/evolutionary_based/FPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38895 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/evolutionary_based/GA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/evolutionary_based/MA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/evolutionary_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.816881 mealpy-2.5.4a4/mealpy/human_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/BRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/BSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/CA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/CHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/FBIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/GSKA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/HBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/HCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/ICA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/LCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/QSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/SARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/SPBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/SSDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/TLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/TOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/WarSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/human_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.820881 mealpy-2.5.4a4/mealpy/math_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/AOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/CEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/CGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/CircleSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/GBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/HC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/PSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/RUN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/SCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/SHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/math_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/multitask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.820881 mealpy-2.5.4a4/mealpy/music_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/music_based/HS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/music_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33913 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.820881 mealpy-2.5.4a4/mealpy/physics_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/ASO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/ArchOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/CDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/EFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/EO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/EVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/FLA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/HGSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/MVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/NRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/RIME.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/SA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20830 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/TWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/WDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/physics_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.828881 mealpy-2.5.4a4/mealpy/swarm_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/ABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/ACOR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/AGTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/ALO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/AO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/ARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/AVOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/BA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/BES.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/BFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/BSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/BeesA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/COA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/CSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/CSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/CoatiOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/DMOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/DO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/EHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/ESOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/FA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/FFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/FFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/FOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/FOX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/GJO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/GOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/GTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/GWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/HBA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/HGS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/HHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/JA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/MFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/MGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/MPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/MRFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/MSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/NGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/NMRA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/OOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/PFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/POA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/PSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SCSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SRSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SSpiderA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SSpiderO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/STO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/SeaHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/ServalOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/TDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/TSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/WOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/WaOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/ZOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/swarm_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.828881 mealpy-2.5.4a4/mealpy/system_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/system_based/AEO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/system_based/GCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/system_based/WCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/system_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.828881 mealpy-2.5.4a4/mealpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/utils/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/utils/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/utils/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.828881 mealpy-2.5.4a4/mealpy/utils/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/utils/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/mealpy/utils/visualize/linechart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.812881 mealpy-2.5.4a4/mealpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    90711 2023-06-12 03:31:20.000000 mealpy-2.5.4a4/mealpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-12 03:31:20.000000 mealpy-2.5.4a4/mealpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:31:20.000000 mealpy-2.5.4a4/mealpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 03:31:20.000000 mealpy-2.5.4a4/mealpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 03:31:20.000000 mealpy-2.5.4a4/mealpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:31:20.828881 mealpy-2.5.4a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:31:20.828881 mealpy-2.5.4a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-12 03:29:32.000000 mealpy-2.5.4a4/tests/test_tuner.py
```

### Comparing `mealpy-2.5.4a3/ChangeLog.md` & `mealpy-2.5.4a4/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 + Update the parameter's order in Tuner class  
 + Update the saving's bug when using Termination in Multitask
 + Remove ILA optimizer 
 + Rename "amend_position()" definition in some algorithms to "bounded_position()".
 + Add a "amend_position()" function in Optimizer class. This function will call two functions.
   + bounded_position() from optimizer. This means for optimizer level (get in valid range of position)
   + amend_position() from problem. This means for problem level (transform to the correct solution)
-
++ Fix bugs coefficients in GWO-based optimizers.
 
 
 # Version 2.5.3
 
 ### Update 
 + Fix bug in roulette-wheel-selection in Optimizer
 + Update multitask with input modes and terminations
```

### Comparing `mealpy-2.5.4a3/LICENSE` & `mealpy-2.5.4a4/LICENSE`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/PKG-INFO` & `mealpy-2.5.4a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mealpy
-Version: 2.5.4a3
+Version: 2.5.4a4
 Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
 Home-page: https://github.com/thieu1995/mealpy
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mealpy.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mealpy
@@ -91,22 +91,27 @@
 - Save results in various formats (csv, json, pickle, png, pdf, jpeg)
 - Export and import models can also be done with Mealpy.
 
 
 
 # Installation
 
-### Install with pip
+### Install the stable (latest) version
 Install the [current PyPI release](https://pypi.python.org/pypi/mealpy):
 ```sh 
 $ pip install mealpy==2.5.3
 ```
 
-### Install from source
-In case you want to install directly from the source code, use:
+### Install the alpha/beta version
+```sh 
+$ pip install mealpy==2.5.4a4
+```
+
+### Install the pre-release version
+You can install pre-release directly from the source code:
 ```sh 
 $ git clone https://github.com/thieu1995/mealpy.git
 $ cd mealpy
 $ python setup.py install
 ```
```

### Comparing `mealpy-2.5.4a3/README.md` & `mealpy-2.5.4a4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -48,22 +48,27 @@
 - Save results in various formats (csv, json, pickle, png, pdf, jpeg)
 - Export and import models can also be done with Mealpy.
 
 
 
 # Installation
 
-### Install with pip
+### Install the stable (latest) version
 Install the [current PyPI release](https://pypi.python.org/pypi/mealpy):
 ```sh 
 $ pip install mealpy==2.5.3
 ```
 
-### Install from source
-In case you want to install directly from the source code, use:
+### Install the alpha/beta version
+```sh 
+$ pip install mealpy==2.5.4a4
+```
+
+### Install the pre-release version
+You can install pre-release directly from the source code:
 ```sh 
 $ git clone https://github.com/thieu1995/mealpy.git
 $ cd mealpy
 $ python setup.py install
 ```
```

### Comparing `mealpy-2.5.4a3/mealpy/__init__.py` & `mealpy-2.5.4a4/mealpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # >>>
 # >>> ## Run the algorithm
 # >>> model = PSO.C_PSO(epoch=5, pop_size=50, name="C-PSO")
 # >>> best_position, best_fitness = model.solve(problem)
 # >>> print(f"Best solution: {best_position}, Best fitness: {best_fitness}")
 
 
-__version__ = "2.5.4-alpha.3"
+__version__ = "2.5.4-alpha.4"
 
 from .bio_based import (BBO, BBOA, BMO, EOA, IWO, SBO, SMA, SOA, SOS, TPO, TSA, VCS, WHO)
 from .evolutionary_based import (CRO, DE, EP, ES, FPA, GA, MA)
 from .human_based import (BRO, BSO, CA, CHIO, FBIO, GSKA, HBO, HCO, ICA, LCO, QSA, SARO, SPBO, SSDO, TLO, TOA, WarSO)
 from .math_based import (AOA, CEM, CGO, CircleSA, GBO, HC, INFO, PSS, RUN, SCA, SHIO)
 from .physics_based import (ArchOA, ASO, CDO, EFO, EO, EVO, FLA, HGSO, MVO, NRO, RIME, SA, TWO, WDO)
 from .swarm_based import (ABC, ACOR, AGTO, ALO, AO, ARO, AVOA, BA, BeesA, BES, BFO, BSA, COA, CoatiOA, CSA, CSO,
```

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/BBO.py` & `mealpy-2.5.4a4/mealpy/bio_based/BBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/BBOA.py` & `mealpy-2.5.4a4/mealpy/bio_based/BBOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/BMO.py` & `mealpy-2.5.4a4/mealpy/bio_based/BMO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/EOA.py` & `mealpy-2.5.4a4/mealpy/bio_based/EOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/IWO.py` & `mealpy-2.5.4a4/mealpy/bio_based/IWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/SBO.py` & `mealpy-2.5.4a4/mealpy/bio_based/SBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/SMA.py` & `mealpy-2.5.4a4/mealpy/bio_based/SMA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/SOA.py` & `mealpy-2.5.4a4/mealpy/bio_based/SOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/SOS.py` & `mealpy-2.5.4a4/mealpy/bio_based/SOS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/TPO.py` & `mealpy-2.5.4a4/mealpy/bio_based/TPO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/TSA.py` & `mealpy-2.5.4a4/mealpy/bio_based/TSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/VCS.py` & `mealpy-2.5.4a4/mealpy/bio_based/VCS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/bio_based/WHO.py` & `mealpy-2.5.4a4/mealpy/bio_based/WHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/evolutionary_based/CRO.py` & `mealpy-2.5.4a4/mealpy/evolutionary_based/CRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/evolutionary_based/DE.py` & `mealpy-2.5.4a4/mealpy/evolutionary_based/DE.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/evolutionary_based/EP.py` & `mealpy-2.5.4a4/mealpy/evolutionary_based/EP.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/evolutionary_based/ES.py` & `mealpy-2.5.4a4/mealpy/evolutionary_based/ES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/evolutionary_based/FPA.py` & `mealpy-2.5.4a4/mealpy/evolutionary_based/FPA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/evolutionary_based/GA.py` & `mealpy-2.5.4a4/mealpy/evolutionary_based/GA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/evolutionary_based/MA.py` & `mealpy-2.5.4a4/mealpy/evolutionary_based/MA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/BRO.py` & `mealpy-2.5.4a4/mealpy/human_based/BRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/BSO.py` & `mealpy-2.5.4a4/mealpy/human_based/BSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/CA.py` & `mealpy-2.5.4a4/mealpy/human_based/CA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/CHIO.py` & `mealpy-2.5.4a4/mealpy/human_based/CHIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/FBIO.py` & `mealpy-2.5.4a4/mealpy/human_based/FBIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/GSKA.py` & `mealpy-2.5.4a4/mealpy/human_based/GSKA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/HBO.py` & `mealpy-2.5.4a4/mealpy/human_based/HBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/HCO.py` & `mealpy-2.5.4a4/mealpy/human_based/HCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/ICA.py` & `mealpy-2.5.4a4/mealpy/human_based/ICA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/LCO.py` & `mealpy-2.5.4a4/mealpy/human_based/LCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/QSA.py` & `mealpy-2.5.4a4/mealpy/human_based/QSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/SARO.py` & `mealpy-2.5.4a4/mealpy/human_based/SARO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/SPBO.py` & `mealpy-2.5.4a4/mealpy/human_based/SPBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/SSDO.py` & `mealpy-2.5.4a4/mealpy/human_based/SSDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/TLO.py` & `mealpy-2.5.4a4/mealpy/human_based/TLO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/TOA.py` & `mealpy-2.5.4a4/mealpy/human_based/TOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/human_based/WarSO.py` & `mealpy-2.5.4a4/mealpy/human_based/WarSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/AOA.py` & `mealpy-2.5.4a4/mealpy/math_based/AOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/CEM.py` & `mealpy-2.5.4a4/mealpy/math_based/CEM.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/CGO.py` & `mealpy-2.5.4a4/mealpy/math_based/CGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/CircleSA.py` & `mealpy-2.5.4a4/mealpy/math_based/CircleSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/GBO.py` & `mealpy-2.5.4a4/mealpy/math_based/GBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/HC.py` & `mealpy-2.5.4a4/mealpy/math_based/HC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/INFO.py` & `mealpy-2.5.4a4/mealpy/math_based/INFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/PSS.py` & `mealpy-2.5.4a4/mealpy/math_based/PSS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/RUN.py` & `mealpy-2.5.4a4/mealpy/math_based/RUN.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/SCA.py` & `mealpy-2.5.4a4/mealpy/math_based/SCA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/math_based/SHIO.py` & `mealpy-2.5.4a4/mealpy/math_based/SHIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/multitask.py` & `mealpy-2.5.4a4/mealpy/multitask.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/music_based/HS.py` & `mealpy-2.5.4a4/mealpy/music_based/HS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/optimizer.py` & `mealpy-2.5.4a4/mealpy/optimizer.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/ASO.py` & `mealpy-2.5.4a4/mealpy/physics_based/ASO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/ArchOA.py` & `mealpy-2.5.4a4/mealpy/physics_based/ArchOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/CDO.py` & `mealpy-2.5.4a4/mealpy/physics_based/CDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/EFO.py` & `mealpy-2.5.4a4/mealpy/physics_based/EFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/EO.py` & `mealpy-2.5.4a4/mealpy/physics_based/EO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/EVO.py` & `mealpy-2.5.4a4/mealpy/physics_based/EVO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/FLA.py` & `mealpy-2.5.4a4/mealpy/physics_based/FLA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/HGSO.py` & `mealpy-2.5.4a4/mealpy/physics_based/HGSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/MVO.py` & `mealpy-2.5.4a4/mealpy/physics_based/MVO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/NRO.py` & `mealpy-2.5.4a4/mealpy/physics_based/NRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/RIME.py` & `mealpy-2.5.4a4/mealpy/physics_based/RIME.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/SA.py` & `mealpy-2.5.4a4/mealpy/physics_based/SA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/TWO.py` & `mealpy-2.5.4a4/mealpy/physics_based/TWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/physics_based/WDO.py` & `mealpy-2.5.4a4/mealpy/physics_based/WDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/ABC.py` & `mealpy-2.5.4a4/mealpy/swarm_based/ABC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/ACOR.py` & `mealpy-2.5.4a4/mealpy/swarm_based/ACOR.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/AGTO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/AGTO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/ALO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/ALO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/AO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/AO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/ARO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/ARO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/AVOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/AVOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/BA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/BA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/BES.py` & `mealpy-2.5.4a4/mealpy/swarm_based/BES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/BFO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/BFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/BSA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/BSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/BeesA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/BeesA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/COA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/COA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/CSA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/CSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/CSO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/CSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/CoatiOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/CoatiOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/DMOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/DMOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/DO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/DO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/EHO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/EHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/ESOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/ESOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/FA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/FA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/FFA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/FFA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/FFO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/FFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/FOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/FOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/FOX.py` & `mealpy-2.5.4a4/mealpy/swarm_based/FOX.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/GJO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/GJO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/GOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/GOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/GTO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/GTO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/GWO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/GWO.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,16 +63,20 @@
         """
         # linearly decreased from 2 to 0
         a = 2 - 2 * epoch / (self.epoch - 1)
         _, list_best, _ = self.get_special_solutions(self.pop, best=3)
 
         pop_new = []
         for idx in range(0, self.pop_size):
-            A1, A2, A3 = a * (2 * np.random.uniform() - 1), a * (2 * np.random.uniform() - 1), a * (2 * np.random.uniform() - 1)
-            C1, C2, C3 = 2 * np.random.uniform(), 2 * np.random.uniform(), 2 * np.random.uniform()
+            A1 = a * (2 * np.random.rand(self.problem.n_dims) - 1)
+            A2 = a * (2 * np.random.rand(self.problem.n_dims) - 1)
+            A3 = a * (2 * np.random.rand(self.problem.n_dims) - 1)
+            C1 = 2 * np.random.rand(self.problem.n_dims)
+            C2 = 2 * np.random.rand(self.problem.n_dims)
+            C3 = 2 * np.random.rand(self.problem.n_dims)
             X1 = list_best[0][self.ID_POS] - A1 * np.abs(C1 * list_best[0][self.ID_POS] - self.pop[idx][self.ID_POS])
             X2 = list_best[1][self.ID_POS] - A2 * np.abs(C2 * list_best[1][self.ID_POS] - self.pop[idx][self.ID_POS])
             X3 = list_best[2][self.ID_POS] - A3 * np.abs(C3 * list_best[2][self.ID_POS] - self.pop[idx][self.ID_POS])
             pos_new = (X1 + X2 + X3) / 3.0
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
@@ -150,18 +154,21 @@
         if self.mode in self.AVAILABLE_MODES:
             leaders_new = self.update_target_wrapper_population(leaders_new)
             leaders = self.greedy_selection_population(leaders, leaders_new)
 
         ## Update other wolfs
         pop_new = []
         for idx in range(0, self.pop_size):
-            # Eq. 3
-            miu1, miu2, miu3 = b * (2 * np.random.uniform() - 1), b * (2 * np.random.uniform() - 1), b * (2 * np.random.uniform() - 1)
-            # Eq. 4
-            c1, c2, c3 = 2 * np.random.uniform(), 2 * np.random.uniform(), 2 * np.random.uniform()
+            # Eq. 3 and 4
+            miu1 = a * (2 * np.random.rand(self.problem.n_dims) - 1)
+            miu2 = a * (2 * np.random.rand(self.problem.n_dims) - 1)
+            miu3 = a * (2 * np.random.rand(self.problem.n_dims) - 1)
+            c1 = 2 * np.random.rand(self.problem.n_dims)
+            c2 = 2 * np.random.rand(self.problem.n_dims)
+            c3 = 2 * np.random.rand(self.problem.n_dims)
             X1 = leaders[0][self.ID_POS] - miu1 * np.abs(c1 * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
             X2 = leaders[1][self.ID_POS] - miu2 * np.abs(c2 * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
             X3 = leaders[2][self.ID_POS] - miu3 * np.abs(c3 * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
             pos_new = (X1 + X2 + X3) / 3.0
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
 
@@ -227,16 +234,20 @@
         """
         # linearly decreased from 2 to 0
         a = 2 - (epoch + 1) / self.epoch
         _, list_best, _ = self.get_special_solutions(self.pop, best=3)
 
         pop_new = []
         for idx in range(0, self.pop_size):
-            A1, A2, A3 = a * (2 * np.random.uniform() - 1), a * (2 * np.random.uniform() - 1), a * (2 * np.random.uniform() - 1)
-            C1, C2, C3 = 2 * np.random.uniform(), 2 * np.random.uniform(), 2 * np.random.uniform()
+            A1 = a * (2 * np.random.rand(self.problem.n_dims) - 1)
+            A2 = a * (2 * np.random.rand(self.problem.n_dims) - 1)
+            A3 = a * (2 * np.random.rand(self.problem.n_dims) - 1)
+            C1 = 2 * np.random.rand(self.problem.n_dims)
+            C2 = 2 * np.random.rand(self.problem.n_dims)
+            C3 = 2 * np.random.rand(self.problem.n_dims)
             if np.random.random() < 0.5:
                 da = np.random.random() * np.abs(C1 * list_best[0][self.ID_POS] - self.pop[idx][self.ID_POS])
             else:
                 P, L = np.random.random(), np.random.uniform(-1, 1)
                 da = P * np.exp(self.b * L) * np.cos(2*np.pi*L) * np.abs(C1 * list_best[0][self.ID_POS] - self.pop[idx][self.ID_POS])
             X1 = list_best[0][self.ID_POS] - A1 * da
             X2 = list_best[1][self.ID_POS] - A2 * np.abs(C2 * list_best[1][self.ID_POS] - self.pop[idx][self.ID_POS])
```

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/HBA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/HBA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/HGS.py` & `mealpy-2.5.4a4/mealpy/swarm_based/HGS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/HHO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/HHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/JA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/JA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/MFO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/MFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/MGO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/MGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/MPA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/MPA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/MRFO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/MRFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/MSA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/MSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/NGO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/NGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/NMRA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/NMRA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/OOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/OOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/PFA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/PFA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/POA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/POA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/PSO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/PSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SCSO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SCSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SFO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SHO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SLO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SLO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SRSR.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SRSR.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SSA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SSO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SSpiderA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SSpiderA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SSpiderO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SSpiderO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/STO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/STO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/SeaHO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/SeaHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/ServalOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/ServalOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/TDO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/TDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/TSO.py` & `mealpy-2.5.4a4/mealpy/swarm_based/TSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/WOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/WOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/WaOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/WaOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/swarm_based/ZOA.py` & `mealpy-2.5.4a4/mealpy/swarm_based/ZOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/system_based/AEO.py` & `mealpy-2.5.4a4/mealpy/system_based/AEO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/system_based/GCO.py` & `mealpy-2.5.4a4/mealpy/system_based/GCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/system_based/WCA.py` & `mealpy-2.5.4a4/mealpy/system_based/WCA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/tuner.py` & `mealpy-2.5.4a4/mealpy/tuner.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/utils/history.py` & `mealpy-2.5.4a4/mealpy/utils/history.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/utils/io.py` & `mealpy-2.5.4a4/mealpy/utils/io.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/utils/logger.py` & `mealpy-2.5.4a4/mealpy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/utils/problem.py` & `mealpy-2.5.4a4/mealpy/utils/problem.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/utils/termination.py` & `mealpy-2.5.4a4/mealpy/utils/termination.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/utils/validator.py` & `mealpy-2.5.4a4/mealpy/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy/utils/visualize/linechart.py` & `mealpy-2.5.4a4/mealpy/utils/visualize/linechart.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/mealpy.egg-info/PKG-INFO` & `mealpy-2.5.4a4/mealpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mealpy
-Version: 2.5.4a3
+Version: 2.5.4a4
 Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
 Home-page: https://github.com/thieu1995/mealpy
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mealpy.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mealpy
@@ -91,22 +91,27 @@
 - Save results in various formats (csv, json, pickle, png, pdf, jpeg)
 - Export and import models can also be done with Mealpy.
 
 
 
 # Installation
 
-### Install with pip
+### Install the stable (latest) version
 Install the [current PyPI release](https://pypi.python.org/pypi/mealpy):
 ```sh 
 $ pip install mealpy==2.5.3
 ```
 
-### Install from source
-In case you want to install directly from the source code, use:
+### Install the alpha/beta version
+```sh 
+$ pip install mealpy==2.5.4a4
+```
+
+### Install the pre-release version
+You can install pre-release directly from the source code:
 ```sh 
 $ git clone https://github.com/thieu1995/mealpy.git
 $ cd mealpy
 $ python setup.py install
 ```
```

### Comparing `mealpy-2.5.4a3/mealpy.egg-info/SOURCES.txt` & `mealpy-2.5.4a4/mealpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/setup.py` & `mealpy-2.5.4a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mealpy",
-    version="2.5.4-alpha.3",
+    version="2.5.4-alpha.4",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["optimization", "metaheuristics", "MHA", "mathematical optimization", "nature-inspired algorithms",
               "evolutionary computation", "soft computing", "population-based algorithms",
```

### Comparing `mealpy-2.5.4a3/tests/test_optimizer.py` & `mealpy-2.5.4a4/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a3/tests/test_tuner.py` & `mealpy-2.5.4a4/tests/test_tuner.py`

 * *Files identical despite different names*

