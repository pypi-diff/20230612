# Comparing `tmp/stormpy-1.3.0.tar.gz` & `tmp/stormpy-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stormpy-1.3.0.tar", last modified: Thu Jan  3 10:21:48 2019, max compression
+gzip compressed data, was "stormpy-1.8.0.tar", last modified: Mon Jun 12 19:54:27 2023, max compression
```

## Comparing `stormpy-1.3.0.tar` & `stormpy-1.8.0.tar`

### file list

```diff
@@ -1,482 +1,380 @@
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/
--rw-r--r--   0 mvolk      (502) staff       (20)     1784 2018-08-01 15:43:43.000000 stormpy-1.3.0/CMakeLists.txt
--rw-r--r--   0 mvolk      (502) staff       (20)      184 2019-01-03 10:08:46.000000 stormpy-1.3.0/MANIFEST.in
--rw-r--r--   0 mvolk      (502) staff       (20)     1474 2019-01-03 10:21:48.000000 stormpy-1.3.0/PKG-INFO
--rw-r--r--   0 mvolk      (502) staff       (20)      573 2018-03-26 09:50:24.000000 stormpy-1.3.0/README.md
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/cmake/
--rw-r--r--   0 mvolk      (502) staff       (20)     1114 2018-08-01 08:26:27.000000 stormpy-1.3.0/cmake/CMakeLists.txt
--rw-r--r--   0 mvolk      (502) staff       (20)      238 2018-03-26 09:50:24.000000 stormpy-1.3.0/cmake/config.py.in
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/
--rw-r--r--   0 mvolk      (502) staff       (20)    18060 2019-01-02 16:52:56.000000 stormpy-1.3.0/lib/stormpy/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)       22 2019-01-03 09:31:54.000000 stormpy-1.3.0/lib/stormpy/_version.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/dft/
--rw-r--r--   0 mvolk      (502) staff       (20)      172 2018-08-06 13:16:10.000000 stormpy-1.3.0/lib/stormpy/dft/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/
--rw-r--r--   0 mvolk      (502) staff       (20)       27 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/ctmc/
--rw-r--r--   0 mvolk      (502) staff       (20)     3748 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/ctmc/cluster2.sm
--rw-r--r--   0 mvolk      (502) staff       (20)      821 2018-08-01 08:26:27.000000 stormpy-1.3.0/lib/stormpy/examples/files/ctmc/dft.drn
--rw-r--r--   0 mvolk      (502) staff       (20)     4621 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/ctmc/embedded2.sm
--rw-r--r--   0 mvolk      (502) staff       (20)     3753 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/ctmc/fms2.sm
--rw-r--r--   0 mvolk      (502) staff       (20)     1126 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/ctmc/polling2.sm
--rw-r--r--   0 mvolk      (502) staff       (20)      776 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/ctmc/tandem5.sm
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/dft/
--rw-r--r--   0 mvolk      (502) staff       (20)     1734 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dft/and.json
--rw-r--r--   0 mvolk      (502) staff       (20)      678 2018-08-06 11:47:04.000000 stormpy-1.3.0/lib/stormpy/examples/files/dft/hecs.dft
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/
--rw-r--r--   0 mvolk      (502) staff       (20)     2655 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/brp-16-2.pm
--rw-r--r--   0 mvolk      (502) staff       (20)    46875 2018-08-01 08:26:27.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/brp.jani
--rw-r--r--   0 mvolk      (502) staff       (20)     2579 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/crowds-5-5.pm
--rw-r--r--   0 mvolk      (502) staff       (20)     2587 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/crowds5_5.pm
--rw-r--r--   0 mvolk      (502) staff       (20)     6033 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/die.jani
--rw-r--r--   0 mvolk      (502) staff       (20)      145 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/die.lab
--rw-r--r--   0 mvolk      (502) staff       (20)      728 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/die.pm
--rw-r--r--   0 mvolk      (502) staff       (20)      162 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/die.tra
--rw-r--r--   0 mvolk      (502) staff       (20)     2328 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/leader-3-5.pm
--rw-r--r--   0 mvolk      (502) staff       (20)     2328 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/leader3_5.pm
--rw-r--r--   0 mvolk      (502) staff       (20)     2844 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/nand-5-2.pm
--rw-r--r--   0 mvolk      (502) staff       (20)      235 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/dtmc/test_conditional.pm
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/
--rw-r--r--   0 mvolk      (502) staff       (20)      149 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/autoParser.lab
--rw-r--r--   0 mvolk      (502) staff       (20)   162452 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/crowds5_5.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       40 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/declarationMisspell.lab
--rw-r--r--   0 mvolk      (502) staff       (20)      145 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/die.lab
--rw-r--r--   0 mvolk      (502) staff       (20)      110 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/doubledLines.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       76 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/doubledLinesSkipped.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       70 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/dtmc_actionTest.lab
--rw-r--r--   0 mvolk      (502) staff       (20)      127 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/dtmc_general.lab
--rw-r--r--   0 mvolk      (502) staff       (20)      127 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/dtmc_mismatched.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       40 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/endMisspell.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       46 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/labelForNonexistentState.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       99 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/leader4.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       61 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/leader4_8.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       56 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/ma_cslFilterTest.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       52 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/ma_general.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       58 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/ma_mismatched.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       85 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/mdp_general.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       79 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/mdp_mismatched.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       28 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/noDeclarationTag.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       35 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/noEndTag.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       18 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/noLabelsDecNoneGiven.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       53 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/pctl_general.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       40 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/swappedStateAndProposition.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       50 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/tiny1.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       50 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/tiny2.lab
--rw-r--r--   0 mvolk      (502) staff       (20)      615 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/two_dice.lab
--rw-r--r--   0 mvolk      (502) staff       (20)       40 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/undeclaredLabelsGiven.lab
--rw-r--r--   0 mvolk      (502) staff       (20)      160 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/withWhitespaces.lab
--rw-r--r--   0 mvolk      (502) staff       (20)      120 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/lab/withoutWhitespaces.lab
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/ma/
--rw-r--r--   0 mvolk      (502) staff       (20)      350 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/ma/hybrid_states.ma
--rw-r--r--   0 mvolk      (502) staff       (20)      214 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/ma/simple.ma
--rw-r--r--   0 mvolk      (502) staff       (20)      997 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/ma/stream2.ma
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/
--rw-r--r--   0 mvolk      (502) staff       (20)      259 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/SmallPrismTest.nm
--rw-r--r--   0 mvolk      (502) staff       (20)      282 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/SmallPrismTest2.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     1521 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/coin2-2-illegalSynchronizingWrite.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     1502 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/coin2-2.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     1500 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/coin2.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     4711 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/csma2-2.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     4711 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/csma2_2.nm
--rw-r--r--   0 mvolk      (502) staff       (20)      775 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/die_c1.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     1478 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/die_selection.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     5350 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/firewire.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     5361 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/firewire3-0.5.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     3248 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/leader3.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     2914 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/leader4.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     2289 2018-10-09 07:16:56.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/maze_2.nm
--rw-r--r--   0 mvolk      (502) staff       (20)      319 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/multiobjective1.nm
--rw-r--r--   0 mvolk      (502) staff       (20)      244 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/multiobjective2.nm
--rw-r--r--   0 mvolk      (502) staff       (20)      297 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/scheduler_generation.nm
--rw-r--r--   0 mvolk      (502) staff       (20)      408 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/system_composition.nm
--rw-r--r--   0 mvolk      (502) staff       (20)      402 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/system_composition2.nm
--rw-r--r--   0 mvolk      (502) staff       (20)      174 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/tiny_rewards.nm
--rw-r--r--   0 mvolk      (502) staff       (20)      615 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/two_dice.lab
--rw-r--r--   0 mvolk      (502) staff       (20)     1193 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/two_dice.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     5832 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/two_dice.tra
--rw-r--r--   0 mvolk      (502) staff       (20)     7299 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/wlan0-2-2.nm
--rw-r--r--   0 mvolk      (502) staff       (20)     7290 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/mdp/wlan0_collide.nm
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/
--rw-r--r--   0 mvolk      (502) staff       (20)     3105 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/brp16_2.pm
--rw-r--r--   0 mvolk      (502) staff       (20)     3105 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/brp_rewards16_2.pm
--rw-r--r--   0 mvolk      (502) staff       (20)    10983 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/crowds3_5.pm
--rw-r--r--   0 mvolk      (502) staff       (20)      611 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/die.drn
--rw-r--r--   0 mvolk      (502) staff       (20)      761 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/parametric_die.pm
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/pmdp/
--rw-r--r--   0 mvolk      (502) staff       (20)     1335 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/pmdp/coin2_2.pm
--rw-r--r--   0 mvolk      (502) staff       (20)     1295 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/pmdp/two_dice.nm
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/pomdp/
--rw-r--r--   0 mvolk      (502) staff       (20)     2921 2018-10-04 20:41:49.000000 stormpy-1.3.0/lib/stormpy/examples/files/pomdp/maze_2.prism
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/prctl/
--rw-r--r--   0 mvolk      (502) staff       (20)        1 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/prctl/apOnly.prctl
--rw-r--r--   0 mvolk      (502) staff       (20)       70 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/prctl/complexFormula.prctl
--rw-r--r--   0 mvolk      (502) staff       (20)       15 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/prctl/probabilisticFormula.prctl
--rw-r--r--   0 mvolk      (502) staff       (20)       20 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/prctl/probabilisticNoBoundFormula.prctl
--rw-r--r--   0 mvolk      (502) staff       (20)       18 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/prctl/propositionalFormula.prctl
--rw-r--r--   0 mvolk      (502) staff       (20)       18 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/prctl/rewardFormula.prctl
--rw-r--r--   0 mvolk      (502) staff       (20)       27 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/prctl/rewardNoBoundFormula.prctl
--rw-r--r--   0 mvolk      (502) staff       (20)       27 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/prctl/two_dice.prctl
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/
--rw-r--r--   0 mvolk      (502) staff       (20)       56 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/autoParser.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)       87 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/die.coin_flips.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)       40 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/dtmc_general.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      132 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/dtmc_general.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      112 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/dtmc_mismatched.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      132 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/dtmc_mixedStateOrder.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      132 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/dtmc_mixedTransitionOrder.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      139 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/dtmc_rewardForNonExTrans.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      200 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/dtmc_whitespaces.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)     8884 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/leader4.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)    35757 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/leader4_8.pick.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)       53 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/ma_general.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)       58 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/ma_mismatched.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)       30 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/mdp_general.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      160 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/mdp_general.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      176 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/mdp_mismatched.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      160 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/mdp_mixedStateOrder.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      160 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/mdp_mixedTransitionOrder.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      169 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/mdp_rewardForNonExTrans.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      248 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/mdp_whitespaces.trans.rew
--rw-r--r--   0 mvolk      (502) staff       (20)     1084 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/state_reward_parser_basic.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      117 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/state_reward_parser_doubledLines.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      107 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/state_reward_parser_doubledLinesSkipped.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)     1151 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/state_reward_parser_whitespaces.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)      690 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/two_dice.flip.state.rew
--rw-r--r--   0 mvolk      (502) staff       (20)     3808 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/rew/two_dice.flip.trans.rew
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/
--rw-r--r--   0 mvolk      (502) staff       (20)   203313 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/crowds5_5.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      336 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/csl_general.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      264 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/ctmc.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      376 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/ctmdp.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      162 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/die.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      271 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmc.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      276 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmcWhitespaces1.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      275 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmcWhitespaces2.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      163 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmc_actionTest.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      138 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmc_deadlock.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      157 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmc_doubledLines.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      143 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmc_general.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      117 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmc_mismatched.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      143 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmc_mixedStateOrder.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      143 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmc_mixedTransitionOrder.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      200 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/dtmc_whitespaces.tra
--rw-r--r--   0 mvolk      (502) staff       (20)   120734 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/leader4.tra
--rw-r--r--   0 mvolk      (502) staff       (20)   245359 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/leader4_8.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      318 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/ma.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      175 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/ma_cslFilterTest.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      119 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/ma_deadlock.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      119 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/ma_general.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      128 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/ma_whitespaces.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      374 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/mdp.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      220 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/mdp_deadlock.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      240 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/mdp_doubledLines.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      220 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/mdp_general.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      172 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/mdp_mismatched.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      220 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/mdp_mixedStateOrder.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      220 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/mdp_mixedTransitionOrder.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      343 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/mdp_whitespaces.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      266 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/noHint.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      223 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/pctl_general.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      170 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/readme.txt
--rw-r--r--   0 mvolk      (502) staff       (20)      194 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/tiny1.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      194 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/tiny2.tra
--rw-r--r--   0 mvolk      (502) staff       (20)     5832 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/two_dice.tra
--rw-r--r--   0 mvolk      (502) staff       (20)      290 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/wrongHint.tra
--rw-r--r--   0 mvolk      (502) staff       (20)       36 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/wrong_format_header1.tra
--rw-r--r--   0 mvolk      (502) staff       (20)       38 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/wrong_format_header2.tra
--rw-r--r--   0 mvolk      (502) staff       (20)       67 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/tra/wrong_format_transition.tra
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/examples/files/txt/
--rw-r--r--   0 mvolk      (502) staff       (20)       23 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/examples/files/txt/testStringFile.txt
--rw-r--r--   0 mvolk      (502) staff       (20)     1371 2018-12-10 08:34:53.000000 stormpy-1.3.0/lib/stormpy/examples/files.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/exceptions/
--rw-r--r--   0 mvolk      (502) staff       (20)      246 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/exceptions/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/info/
--rw-r--r--   0 mvolk      (502) staff       (20)      537 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/info/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/logic/
--rw-r--r--   0 mvolk      (502) staff       (20)       41 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/logic/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/pars/
--rw-r--r--   0 mvolk      (502) staff       (20)     1978 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/pars/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/storage/
--rw-r--r--   0 mvolk      (502) staff       (20)       46 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/storage/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy/utility/
--rw-r--r--   0 mvolk      (502) staff       (20)       45 2018-04-25 15:01:47.000000 stormpy-1.3.0/lib/stormpy/utility/__init__.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy.egg-info/
--rw-r--r--   0 mvolk      (502) staff       (20)     1474 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy.egg-info/PKG-INFO
--rw-r--r--   0 mvolk      (502) staff       (20)    17653 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy.egg-info/SOURCES.txt
--rw-r--r--   0 mvolk      (502) staff       (20)        1 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy.egg-info/dependency_links.txt
--rw-r--r--   0 mvolk      (502) staff       (20)        1 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy.egg-info/not-zip-safe
--rw-r--r--   0 mvolk      (502) staff       (20)       14 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy.egg-info/requires.txt
--rw-r--r--   0 mvolk      (502) staff       (20)       49 2019-01-03 10:21:48.000000 stormpy-1.3.0/lib/stormpy.egg-info/top_level.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1638 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/.appveyor.yml
--rwxr-xr-x   0 mvolk      (502) staff       (20)      360 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/.gitignore
--rwxr-xr-x   0 mvolk      (502) staff       (20)      100 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/.gitmodules
--rwxr-xr-x   0 mvolk      (502) staff       (20)       62 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/.readthedocs.yml
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7295 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/.travis.yml
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5827 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1896 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/CONTRIBUTING.md
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1271 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/ISSUE_TEMPLATE.md
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2190 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/LICENSE
--rwxr-xr-x   0 mvolk      (502) staff       (20)       71 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/MANIFEST.in
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5896 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/README.md
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/docs/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      535 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/Doxyfile
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/docs/_static/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      254 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/_static/theme_overrides.css
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/cast/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3895 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/cast/chrono.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3189 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/cast/custom.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    14276 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/cast/eigen.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3889 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/cast/functional.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1534 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/cast/index.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11482 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/cast/overview.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7236 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/cast/stl.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     9240 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/cast/strings.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    22719 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/classes.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8052 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/embedding.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7091 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/exceptions.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    22211 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/functions.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     9187 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/pycpp/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      278 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/pycpp/index.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    14118 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/pycpp/numpy.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2922 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/pycpp/object.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2601 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/pycpp/utilities.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     6366 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/advanced/smart_ptrs.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8214 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/basics.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2920 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/benchmark.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3170 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/benchmark.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    27212 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/changelog.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    13014 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/classes.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     9042 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/compiling.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10618 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/conf.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10045 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/faq.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)      693 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/index.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4243 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/intro.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)      879 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/limitations.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)    58510 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/pybind11-logo.png
--rwxr-xr-x   0 mvolk      (502) staff       (20)    44653 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/pybind11_vs_boost_python1.png
--rwxr-xr-x   0 mvolk      (502) staff       (20)    87708 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/pybind11_vs_boost_python1.svg
--rwxr-xr-x   0 mvolk      (502) staff       (20)    41121 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/pybind11_vs_boost_python2.png
--rwxr-xr-x   0 mvolk      (502) staff       (20)    85853 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/pybind11_vs_boost_python2.svg
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1622 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/reference.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1127 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/release.rst
--rwxr-xr-x   0 mvolk      (502) staff       (20)       17 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/docs/requirements.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/include/
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/
--rwxr-xr-x   0 mvolk      (502) staff       (20)    18071 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/attr.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4299 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/buffer_info.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    86469 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/cast.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     6596 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/chrono.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    23813 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/class_support.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    40583 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/common.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1949 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/complex.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7693 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/descr.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    29215 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/eigen.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7425 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/embed.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3845 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/eval.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2934 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/functional.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    65466 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/numpy.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8651 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/operators.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2004 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/options.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    81353 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/pybind11.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    48451 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/pytypes.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    12193 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/stl.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)    20849 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/stl_bind.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1402 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/include/pybind11/typeid.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/pybind11/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      336 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/pybind11/__init__.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)      791 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/pybind11/__main__.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)       77 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/pybind11/_version.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)      238 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/setup.cfg
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3646 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/setup.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tests/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7408 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)     6526 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/conftest.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11150 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/constructor_stats.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5389 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/object.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3626 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/pybind11_tests.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1252 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/pybind11_tests.h
--rwxr-xr-x   0 mvolk      (502) staff       (20)      530 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/pytest.ini
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5830 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_buffers.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2430 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_buffers.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7020 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_builtin_casters.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7948 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_builtin_casters.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3337 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_call_policies.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5118 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_call_policies.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5769 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_callbacks.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4380 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_callbacks.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2100 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_chrono.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3402 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_chrono.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10033 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_class.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4550 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_class.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2042 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)      654 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/installed_embed/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      686 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/installed_function/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      474 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/installed_target/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1056 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)      152 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/subdirectory_embed/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      327 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/subdirectory_function/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      373 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/subdirectory_target/
--rwxr-xr-x   0 mvolk      (502) staff       (20)      695 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)      142 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_cmake_build/test.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3330 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_constants_and_functions.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1100 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_constants_and_functions.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8897 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_copy_move.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5103 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_copy_move.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2284 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_docstring_options.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1705 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_docstring_options.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    16268 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_eigen.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    28676 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tests/test_embed/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1234 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_embed/CMakeLists.txt
--rwxr-xr-x   0 mvolk      (502) staff       (20)      414 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_embed/catch.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7675 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_embed/test_interpreter.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)      195 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_embed/test_interpreter.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1863 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_enum.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4144 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_enum.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2377 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_eval.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)      560 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_eval.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)      119 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_eval_call.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5889 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_exceptions.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2897 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_exceptions.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3026 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_kwargs_and_defaults.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4618 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_kwargs_and_defaults.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    17753 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_methods_and_attributes.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    16018 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_methods_and_attributes.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3283 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_modules.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2208 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_modules.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7853 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_multiple_inheritance.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     9277 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_multiple_inheritance.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    12169 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_numpy_array.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    16119 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_numpy_array.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    15916 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_numpy_dtypes.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11824 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_numpy_dtypes.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3440 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_numpy_vectorize.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8887 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_numpy_vectorize.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2241 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_opaque_types.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1869 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_opaque_types.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5350 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_operator_overloading.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3442 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_operator_overloading.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2945 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_pickling.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)      834 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_pickling.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8189 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_pytypes.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5777 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_pytypes.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11959 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_sequences_and_iterators.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5189 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_sequences_and_iterators.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    12371 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_smart_ptr.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8732 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_smart_ptr.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5883 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_stl.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     5124 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_stl.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3780 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_stl_binders.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)     4850 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_stl_binders.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    16682 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_virtual_functions.cpp
--rwxr-xr-x   0 mvolk      (502) staff       (20)    11020 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tests/test_virtual_functions.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/resources/pybind11/tools/
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2100 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tools/FindCatch.cmake
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2995 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tools/FindEigen3.cmake
--rwxr-xr-x   0 mvolk      (502) staff       (20)     7998 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 mvolk      (502) staff       (20)     2308 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tools/check-style.sh
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1098 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tools/libsize.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10341 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tools/mkdoc.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     3978 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tools/pybind11Config.cmake.in
--rwxr-xr-x   0 mvolk      (502) staff       (20)     8137 2018-03-26 09:50:24.000000 stormpy-1.3.0/resources/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/setup/
--rw-r--r--   0 mvolk      (502) staff       (20)       26 2018-03-26 09:50:24.000000 stormpy-1.3.0/setup/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)     2433 2018-03-26 09:50:24.000000 stormpy-1.3.0/setup/config.py
--rwxr-xr-x   0 mvolk      (502) staff       (20)     1941 2018-03-26 09:50:24.000000 stormpy-1.3.0/setup/helper.py
--rw-r--r--   0 mvolk      (502) staff       (20)      226 2019-01-03 10:21:48.000000 stormpy-1.3.0/setup.cfg
--rwxr-xr-x   0 mvolk      (502) staff       (20)    10919 2019-01-02 16:57:14.000000 stormpy-1.3.0/setup.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/src/
--rw-r--r--   0 mvolk      (502) staff       (20)     1092 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/boost.h
--rw-r--r--   0 mvolk      (502) staff       (20)      486 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/common.h
--rw-r--r--   0 mvolk      (502) staff       (20)       43 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/config.h.in
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/src/core/
--rw-r--r--   0 mvolk      (502) staff       (20)     1148 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/core/analysis.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       80 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/core/analysis.h
--rw-r--r--   0 mvolk      (502) staff       (20)     1875 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/core/bisimulation.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      177 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/core/bisimulation.h
--rw-r--r--   0 mvolk      (502) staff       (20)       79 2018-08-01 15:22:13.000000 stormpy-1.3.0/src/core/common.h
--rw-r--r--   0 mvolk      (502) staff       (20)     8832 2018-08-01 15:22:24.000000 stormpy-1.3.0/src/core/core.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      214 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/core/core.h
--rw-r--r--   0 mvolk      (502) staff       (20)     4409 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/core/counterexample.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       79 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/core/counterexample.h
--rw-r--r--   0 mvolk      (502) staff       (20)     3120 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/core/environment.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      173 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/core/environment.h
--rw-r--r--   0 mvolk      (502) staff       (20)     4021 2018-09-28 11:20:55.000000 stormpy-1.3.0/src/core/input.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      187 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/core/input.h
--rw-r--r--   0 mvolk      (502) staff       (20)     6409 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/core/modelchecking.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      181 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/core/modelchecking.h
--rw-r--r--   0 mvolk      (502) staff       (20)    10167 2018-10-24 15:23:56.000000 stormpy-1.3.0/src/core/result.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      153 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/core/result.h
--rw-r--r--   0 mvolk      (502) staff       (20)     2886 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/core/transformation.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       78 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/core/transformation.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/src/dft/
--rw-r--r--   0 mvolk      (502) staff       (20)     1051 2018-08-01 15:48:03.000000 stormpy-1.3.0/src/dft/analysis.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       72 2018-08-01 14:20:59.000000 stormpy-1.3.0/src/dft/analysis.h
--rw-r--r--   0 mvolk      (502) staff       (20)       60 2018-08-01 08:33:20.000000 stormpy-1.3.0/src/dft/common.h
--rw-r--r--   0 mvolk      (502) staff       (20)     1654 2018-08-06 11:57:52.000000 stormpy-1.3.0/src/dft/dft.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       67 2018-08-01 08:47:18.000000 stormpy-1.3.0/src/dft/dft.h
--rw-r--r--   0 mvolk      (502) staff       (20)      841 2018-08-08 11:36:21.000000 stormpy-1.3.0/src/dft/io.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      104 2018-08-01 08:47:25.000000 stormpy-1.3.0/src/dft/io.h
--rw-r--r--   0 mvolk      (502) staff       (20)      887 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/helpers.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/src/logic/
--rw-r--r--   0 mvolk      (502) staff       (20)     9555 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/logic/formulae.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      168 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/logic/formulae.h
--rw-r--r--   0 mvolk      (502) staff       (20)      808 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/mod_core.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      365 2018-08-01 15:33:23.000000 stormpy-1.3.0/src/mod_dft.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)     1548 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/mod_info.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      258 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/mod_logic.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      375 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/mod_pars.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      972 2018-08-02 07:48:39.000000 stormpy-1.3.0/src/mod_storage.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      247 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/mod_utility.cpp
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/src/pars/
--rw-r--r--   0 mvolk      (502) staff       (20)      207 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/pars/common.h
--rw-r--r--   0 mvolk      (502) staff       (20)     2228 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/pars/model_instantiator.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      201 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/pars/model_instantiator.h
--rw-r--r--   0 mvolk      (502) staff       (20)     2933 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/pars/pars.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      145 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/pars/pars.h
--rw-r--r--   0 mvolk      (502) staff       (20)     7495 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/pars/pla.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      141 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/pars/pla.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/src/storage/
--rw-r--r--   0 mvolk      (502) staff       (20)     1756 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/storage/bitvector.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      174 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/storage/bitvector.h
--rw-r--r--   0 mvolk      (502) staff       (20)     1196 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/storage/choiceorigins.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       71 2018-08-02 07:48:39.000000 stormpy-1.3.0/src/storage/choiceorigins.h
--rw-r--r--   0 mvolk      (502) staff       (20)       24 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/storage/common.h
--rw-r--r--   0 mvolk      (502) staff       (20)      597 2018-04-02 12:23:40.000000 stormpy-1.3.0/src/storage/distribution.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      127 2018-04-02 12:23:40.000000 stormpy-1.3.0/src/storage/distribution.h
--rw-r--r--   0 mvolk      (502) staff       (20)     6606 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/storage/expressions.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      182 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/storage/expressions.h
--rw-r--r--   0 mvolk      (502) staff       (20)    12410 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/storage/jani.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       68 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/storage/jani.h
--rw-r--r--   0 mvolk      (502) staff       (20)     2227 2018-08-02 07:48:39.000000 stormpy-1.3.0/src/storage/labeling.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      170 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/storage/labeling.h
--rw-r--r--   0 mvolk      (502) staff       (20)    11227 2018-10-04 20:41:49.000000 stormpy-1.3.0/src/storage/matrix.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      169 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/storage/matrix.h
--rw-r--r--   0 mvolk      (502) staff       (20)    24199 2018-12-10 08:34:53.000000 stormpy-1.3.0/src/storage/model.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      249 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/storage/model.h
--rw-r--r--   0 mvolk      (502) staff       (20)     4456 2018-09-28 11:23:54.000000 stormpy-1.3.0/src/storage/prism.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       70 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/storage/prism.h
--rw-r--r--   0 mvolk      (502) staff       (20)     2193 2018-11-29 12:15:08.000000 stormpy-1.3.0/src/storage/scheduler.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      126 2018-04-02 12:23:40.000000 stormpy-1.3.0/src/storage/scheduler.h
--rw-r--r--   0 mvolk      (502) staff       (20)     3138 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/storage/state.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)     3806 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/storage/state.h
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-01-03 10:21:48.000000 stormpy-1.3.0/src/utility/
--rw-r--r--   0 mvolk      (502) staff       (20)      365 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/utility/chrono.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       73 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/utility/chrono.h
--rw-r--r--   0 mvolk      (502) staff       (20)     3290 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/utility/shortestPaths.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)      184 2018-03-26 09:50:24.000000 stormpy-1.3.0/src/utility/shortestPaths.h
--rw-r--r--   0 mvolk      (502) staff       (20)     1914 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/utility/smtsolver.cpp
--rw-r--r--   0 mvolk      (502) staff       (20)       70 2018-08-01 08:26:27.000000 stormpy-1.3.0/src/utility/smtsolver.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:27.063070 stormpy-1.8.0/
+-rw-r--r--   0 mvolk      (502) staff       (20)     5086 2023-06-12 19:54:05.000000 stormpy-1.8.0/CMakeLists.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)    35147 2022-02-10 13:02:00.000000 stormpy-1.8.0/LICENSE
+-rw-r--r--   0 mvolk      (502) staff       (20)      184 2022-02-10 13:02:00.000000 stormpy-1.8.0/MANIFEST.in
+-rw-r--r--   0 mvolk      (502) staff       (20)     4236 2023-06-12 19:54:27.063229 stormpy-1.8.0/PKG-INFO
+-rw-r--r--   0 mvolk      (502) staff       (20)     3440 2023-03-23 12:57:24.000000 stormpy-1.8.0/README.md
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.649104 stormpy-1.8.0/cmake/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1023 2023-04-26 14:04:59.000000 stormpy-1.8.0/cmake/CMakeLists.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)      388 2022-08-31 14:40:52.000000 stormpy-1.8.0/cmake/config.py.in
+-rw-r--r--   0 mvolk      (502) staff       (20)      663 2022-09-01 17:23:03.000000 stormpy-1.8.0/cmake/core_config.py.in
+-rw-r--r--   0 mvolk      (502) staff       (20)       67 2022-09-01 17:23:03.000000 stormpy-1.8.0/cmake/dft_config.py.in
+-rw-r--r--   0 mvolk      (502) staff       (20)       69 2022-09-01 17:23:03.000000 stormpy-1.8.0/cmake/gspn_config.py.in
+-rw-r--r--   0 mvolk      (502) staff       (20)      184 2022-09-14 11:04:18.000000 stormpy-1.8.0/cmake/info_config.py.in
+-rw-r--r--   0 mvolk      (502) staff       (20)     1667 2022-09-01 17:23:03.000000 stormpy-1.8.0/cmake/macros.cmake
+-rw-r--r--   0 mvolk      (502) staff       (20)       69 2022-09-01 17:23:03.000000 stormpy-1.8.0/cmake/pars_config.py.in
+-rw-r--r--   0 mvolk      (502) staff       (20)       71 2022-09-01 17:23:03.000000 stormpy-1.8.0/cmake/pomdp_config.py.in
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.619434 stormpy-1.8.0/lib/
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.655234 stormpy-1.8.0/lib/stormpy/
+-rw-r--r--   0 mvolk      (502) staff       (20)    27560 2023-06-07 21:44:52.000000 stormpy-1.8.0/lib/stormpy/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)      490 2023-04-05 12:32:40.000000 stormpy-1.8.0/lib/stormpy/_config.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       22 2023-06-11 18:07:38.000000 stormpy-1.8.0/lib/stormpy/_version.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.662665 stormpy-1.8.0/lib/stormpy/dft/
+-rw-r--r--   0 mvolk      (502) staff       (20)     2613 2022-09-18 20:23:32.000000 stormpy-1.8.0/lib/stormpy/dft/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       50 2023-04-05 12:32:40.000000 stormpy-1.8.0/lib/stormpy/dft/_config.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     1048 2022-09-18 20:23:32.000000 stormpy-1.8.0/lib/stormpy/dft/modules.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.664984 stormpy-1.8.0/lib/stormpy/examples/
+-rw-r--r--   0 mvolk      (502) staff       (20)       27 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/__init__.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.624698 stormpy-1.8.0/lib/stormpy/examples/files/
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.679849 stormpy-1.8.0/lib/stormpy/examples/files/ctmc/
+-rw-r--r--   0 mvolk      (502) staff       (20)     3748 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ctmc/cluster2.sm
+-rw-r--r--   0 mvolk      (502) staff       (20)      821 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ctmc/dft.drn
+-rw-r--r--   0 mvolk      (502) staff       (20)     4621 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ctmc/embedded2.sm
+-rw-r--r--   0 mvolk      (502) staff       (20)     3753 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ctmc/fms2.sm
+-rw-r--r--   0 mvolk      (502) staff       (20)     1126 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ctmc/polling2.sm
+-rw-r--r--   0 mvolk      (502) staff       (20)      776 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ctmc/tandem5.sm
+-rw-r--r--   0 mvolk      (502) staff       (20)      149 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ctmc/tiny.sm
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.688839 stormpy-1.8.0/lib/stormpy/examples/files/dft/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1734 2022-09-14 13:18:43.000000 stormpy-1.8.0/lib/stormpy/examples/files/dft/and.json
+-rw-r--r--   0 mvolk      (502) staff       (20)      182 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dft/fdep.dft
+-rw-r--r--   0 mvolk      (502) staff       (20)      678 2022-10-02 21:33:39.000000 stormpy-1.8.0/lib/stormpy/examples/files/dft/hecs.dft
+-rw-r--r--   0 mvolk      (502) staff       (20)      702 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dft/rc.dft
+-rw-r--r--   0 mvolk      (502) staff       (20)      529 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dft/rc2.dft
+-rw-r--r--   0 mvolk      (502) staff       (20)      173 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dft/symmetry_param.dft
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.707049 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/
+-rw-r--r--   0 mvolk      (502) staff       (20)     2655 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/brp-16-2.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)    46875 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/brp.jani
+-rw-r--r--   0 mvolk      (502) staff       (20)     2579 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/crowds-5-5.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)     2587 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/crowds5_5.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)     6033 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/die.jani
+-rw-r--r--   0 mvolk      (502) staff       (20)      145 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/die.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)      728 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/die.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)      162 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/die.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)     2328 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/leader-3-5.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)     2328 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/leader3_5.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)     2844 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/nand-5-2.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)      113 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/negativevals.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)      235 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/dtmc/test_conditional.pm
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.711166 stormpy-1.8.0/lib/stormpy/examples/files/gspn/
+-rw-r--r--   0 mvolk      (502) staff       (20)     3077 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/gspn/gspn_simple.pnml
+-rw-r--r--   0 mvolk      (502) staff       (20)      735 2023-06-12 08:41:48.000000 stormpy-1.8.0/lib/stormpy/examples/files/gspn/gspn_simple.pnpro
+-rw-r--r--   0 mvolk      (502) staff       (20)     5643 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/gspn/philosophers_4.pnpro
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.745320 stormpy-1.8.0/lib/stormpy/examples/files/lab/
+-rw-r--r--   0 mvolk      (502) staff       (20)      149 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/autoParser.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)   162452 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/crowds5_5.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       40 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/declarationMisspell.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)      145 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/die.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)      110 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/doubledLines.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       76 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/doubledLinesSkipped.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       70 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/dtmc_actionTest.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)      127 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/dtmc_general.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)      127 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/dtmc_mismatched.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       40 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/endMisspell.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       46 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/labelForNonexistentState.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       99 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/leader4.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       61 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/leader4_8.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       56 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/ma_cslFilterTest.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       52 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/ma_general.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       58 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/ma_mismatched.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       85 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/mdp_general.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       79 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/mdp_mismatched.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       28 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/noDeclarationTag.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       35 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/noEndTag.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       18 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/noLabelsDecNoneGiven.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       53 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/pctl_general.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       40 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/swappedStateAndProposition.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       50 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/tiny1.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       50 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/tiny2.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)      615 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/two_dice.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)       40 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/undeclaredLabelsGiven.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)      160 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/withWhitespaces.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)      120 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/lab/withoutWhitespaces.lab
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.749194 stormpy-1.8.0/lib/stormpy/examples/files/ma/
+-rw-r--r--   0 mvolk      (502) staff       (20)      179 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ma/ctmc.ma
+-rw-r--r--   0 mvolk      (502) staff       (20)      350 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ma/hybrid_states.ma
+-rw-r--r--   0 mvolk      (502) staff       (20)      214 2022-10-19 13:24:30.000000 stormpy-1.8.0/lib/stormpy/examples/files/ma/simple.ma
+-rw-r--r--   0 mvolk      (502) staff       (20)      997 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/ma/stream2.ma
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.779869 stormpy-1.8.0/lib/stormpy/examples/files/mdp/
+-rw-r--r--   0 mvolk      (502) staff       (20)      259 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/SmallPrismTest.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      282 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/SmallPrismTest2.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     1521 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/coin2-2-illegalSynchronizingWrite.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     1502 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/coin2-2.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     1500 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/coin2.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     4711 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/csma2-2.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     4711 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/csma2_2.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      775 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/die_c1.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     1478 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/die_selection.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     5350 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/firewire.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     5361 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/firewire3-0.5.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     3248 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/leader3.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     2914 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/leader4.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     2302 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/maze_2.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      319 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/multiobjective1.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      244 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/multiobjective2.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      297 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/scheduler_generation.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      553 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/slipgrid.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      408 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/system_composition.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      402 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/system_composition2.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      174 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/tiny_rewards.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)      615 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/two_dice.lab
+-rw-r--r--   0 mvolk      (502) staff       (20)     1193 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/two_dice.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     5832 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/two_dice.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)     7299 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/wlan0-2-2.nm
+-rw-r--r--   0 mvolk      (502) staff       (20)     7290 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/mdp/wlan0_collide.nm
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.785098 stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/
+-rw-r--r--   0 mvolk      (502) staff       (20)     3105 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/brp16_2.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)     3105 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/brp_rewards16_2.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)    10983 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/crowds3_5.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)      611 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/die.drn
+-rw-r--r--   0 mvolk      (502) staff       (20)     1332 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/herman5.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)      761 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/parametric_die.pm
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.788829 stormpy-1.8.0/lib/stormpy/examples/files/pmdp/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1335 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pmdp/coin2_2.pm
+-rw-r--r--   0 mvolk      (502) staff       (20)     1295 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pmdp/two_dice.nm
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.795452 stormpy-1.8.0/lib/stormpy/examples/files/pomdp/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1555 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pomdp/3x3grid.prism
+-rw-r--r--   0 mvolk      (502) staff       (20)     1764 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pomdp/maze.drn
+-rw-r--r--   0 mvolk      (502) staff       (20)     2943 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pomdp/maze_2.prism
+-rw-r--r--   0 mvolk      (502) staff       (20)     2978 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/pomdp/maze_2_par.prism
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.805209 stormpy-1.8.0/lib/stormpy/examples/files/prctl/
+-rw-r--r--   0 mvolk      (502) staff       (20)        1 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/prctl/apOnly.prctl
+-rw-r--r--   0 mvolk      (502) staff       (20)       70 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/prctl/complexFormula.prctl
+-rw-r--r--   0 mvolk      (502) staff       (20)       15 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/prctl/probabilisticFormula.prctl
+-rw-r--r--   0 mvolk      (502) staff       (20)       20 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/prctl/probabilisticNoBoundFormula.prctl
+-rw-r--r--   0 mvolk      (502) staff       (20)       18 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/prctl/propositionalFormula.prctl
+-rw-r--r--   0 mvolk      (502) staff       (20)       18 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/prctl/rewardFormula.prctl
+-rw-r--r--   0 mvolk      (502) staff       (20)       27 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/prctl/rewardNoBoundFormula.prctl
+-rw-r--r--   0 mvolk      (502) staff       (20)       27 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/prctl/two_dice.prctl
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.839992 stormpy-1.8.0/lib/stormpy/examples/files/rew/
+-rw-r--r--   0 mvolk      (502) staff       (20)       56 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/autoParser.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)       87 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/die.coin_flips.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)       40 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/dtmc_general.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      132 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/dtmc_general.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      112 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/dtmc_mismatched.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      132 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/dtmc_mixedStateOrder.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      132 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/dtmc_mixedTransitionOrder.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      139 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/dtmc_rewardForNonExTrans.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      200 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/dtmc_whitespaces.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)     8884 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/leader4.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)    35757 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/leader4_8.pick.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)       53 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/ma_general.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)       58 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/ma_mismatched.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)       30 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/mdp_general.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      160 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/mdp_general.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      176 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/mdp_mismatched.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      160 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/mdp_mixedStateOrder.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      160 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/mdp_mixedTransitionOrder.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      169 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/mdp_rewardForNonExTrans.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      248 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/mdp_whitespaces.trans.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)     1084 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/state_reward_parser_basic.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      117 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/state_reward_parser_doubledLines.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      107 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/state_reward_parser_doubledLinesSkipped.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)     1151 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/state_reward_parser_whitespaces.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)      690 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/two_dice.flip.state.rew
+-rw-r--r--   0 mvolk      (502) staff       (20)     3808 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/rew/two_dice.flip.trans.rew
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.897477 stormpy-1.8.0/lib/stormpy/examples/files/tra/
+-rw-r--r--   0 mvolk      (502) staff       (20)   203313 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/crowds5_5.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      336 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/csl_general.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      264 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/ctmc.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      376 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/ctmdp.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      162 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/die.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      271 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmc.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      276 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmcWhitespaces1.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      275 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmcWhitespaces2.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      163 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmc_actionTest.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      138 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmc_deadlock.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      157 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmc_doubledLines.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      143 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmc_general.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      117 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmc_mismatched.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      143 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmc_mixedStateOrder.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      143 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmc_mixedTransitionOrder.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      200 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/dtmc_whitespaces.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)   120734 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/leader4.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)   245359 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/leader4_8.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      318 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/ma.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      175 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/ma_cslFilterTest.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      119 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/ma_deadlock.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      119 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/ma_general.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      128 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/ma_whitespaces.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      374 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/mdp.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      220 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/mdp_deadlock.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      240 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/mdp_doubledLines.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      220 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/mdp_general.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      172 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/mdp_mismatched.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      220 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/mdp_mixedStateOrder.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      220 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/mdp_mixedTransitionOrder.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      343 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/mdp_whitespaces.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      266 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/noHint.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      223 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/pctl_general.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      170 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/readme.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)      194 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/tiny1.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      194 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/tiny2.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)     5832 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/two_dice.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)      290 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/wrongHint.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)       36 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/wrong_format_header1.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)       38 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/wrong_format_header2.tra
+-rw-r--r--   0 mvolk      (502) staff       (20)       67 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/tra/wrong_format_transition.tra
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.898095 stormpy-1.8.0/lib/stormpy/examples/files/txt/
+-rw-r--r--   0 mvolk      (502) staff       (20)       23 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files/txt/testStringFile.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)     2088 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/examples/files.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.898727 stormpy-1.8.0/lib/stormpy/exceptions/
+-rw-r--r--   0 mvolk      (502) staff       (20)      246 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/exceptions/__init__.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.901260 stormpy-1.8.0/lib/stormpy/gspn/
+-rw-r--r--   0 mvolk      (502) staff       (20)      161 2022-09-14 13:18:43.000000 stormpy-1.8.0/lib/stormpy/gspn/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       51 2023-04-05 12:32:40.000000 stormpy-1.8.0/lib/stormpy/gspn/_config.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.902960 stormpy-1.8.0/lib/stormpy/info/
+-rw-r--r--   0 mvolk      (502) staff       (20)      537 2022-09-14 13:18:43.000000 stormpy-1.8.0/lib/stormpy/info/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)      127 2023-06-07 08:53:00.000000 stormpy-1.8.0/lib/stormpy/info/_config.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.903949 stormpy-1.8.0/lib/stormpy/logic/
+-rw-r--r--   0 mvolk      (502) staff       (20)       41 2022-09-14 13:18:43.000000 stormpy-1.8.0/lib/stormpy/logic/__init__.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.905828 stormpy-1.8.0/lib/stormpy/pars/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1978 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/pars/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       51 2023-04-05 12:32:40.000000 stormpy-1.8.0/lib/stormpy/pars/_config.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.908960 stormpy-1.8.0/lib/stormpy/pomdp/
+-rw-r--r--   0 mvolk      (502) staff       (20)     2617 2022-09-14 13:18:43.000000 stormpy-1.8.0/lib/stormpy/pomdp/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       52 2023-04-05 12:32:40.000000 stormpy-1.8.0/lib/stormpy/pomdp/_config.py
+-rw-r--r--   0 mvolk      (502) staff       (20)    13543 2022-09-14 13:18:43.000000 stormpy-1.8.0/lib/stormpy/simulator.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.909865 stormpy-1.8.0/lib/stormpy/storage/
+-rw-r--r--   0 mvolk      (502) staff       (20)     2816 2022-09-01 09:24:21.000000 stormpy-1.8.0/lib/stormpy/storage/__init__.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.915322 stormpy-1.8.0/lib/stormpy/utility/
+-rw-r--r--   0 mvolk      (502) staff       (20)      488 2022-09-14 13:18:43.000000 stormpy-1.8.0/lib/stormpy/utility/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     3008 2022-09-14 13:18:43.000000 stormpy-1.8.0/lib/stormpy/utility/multiobjective_plotting.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.660605 stormpy-1.8.0/lib/stormpy.egg-info/
+-rw-r--r--   0 mvolk      (502) staff       (20)     4236 2023-06-12 19:54:26.000000 stormpy-1.8.0/lib/stormpy.egg-info/PKG-INFO
+-rw-r--r--   0 mvolk      (502) staff       (20)    12378 2023-06-12 19:54:26.000000 stormpy-1.8.0/lib/stormpy.egg-info/SOURCES.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)        1 2023-06-12 19:54:26.000000 stormpy-1.8.0/lib/stormpy.egg-info/dependency_links.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)        1 2023-04-05 12:32:39.000000 stormpy-1.8.0/lib/stormpy.egg-info/not-zip-safe
+-rw-r--r--   0 mvolk      (502) staff       (20)      124 2023-06-12 19:54:26.000000 stormpy-1.8.0/lib/stormpy.egg-info/requires.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)       60 2023-06-12 19:54:26.000000 stormpy-1.8.0/lib/stormpy.egg-info/top_level.txt
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.916396 stormpy-1.8.0/resources/
+-rw-r--r--   0 mvolk      (502) staff       (20)      498 2022-09-14 11:04:18.000000 stormpy-1.8.0/resources/include_pybind11.cmake
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.920118 stormpy-1.8.0/setup/
+-rw-r--r--   0 mvolk      (502) staff       (20)       26 2022-09-14 13:20:57.000000 stormpy-1.8.0/setup/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     2537 2022-09-14 13:20:58.000000 stormpy-1.8.0/setup/config.py
+-rwxr-xr-x   0 mvolk      (502) staff       (20)     1941 2022-02-10 13:02:00.000000 stormpy-1.8.0/setup/helper.py
+-rw-r--r--   0 mvolk      (502) staff       (20)      234 2023-06-12 19:54:27.063871 stormpy-1.8.0/setup.cfg
+-rwxr-xr-x   0 mvolk      (502) staff       (20)    10747 2023-06-11 18:07:38.000000 stormpy-1.8.0/setup.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.931860 stormpy-1.8.0/src/
+-rw-r--r--   0 mvolk      (502) staff       (20)      350 2023-03-28 22:13:48.000000 stormpy-1.8.0/src/boost.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      486 2023-03-28 22:13:58.000000 stormpy-1.8.0/src/common.h
+-rw-r--r--   0 mvolk      (502) staff       (20)       43 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/config.h.in
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.960069 stormpy-1.8.0/src/core/
+-rw-r--r--   0 mvolk      (502) staff       (20)      939 2022-02-26 23:54:11.000000 stormpy-1.8.0/src/core/analysis.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       80 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/analysis.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2254 2023-06-07 21:44:52.000000 stormpy-1.8.0/src/core/bisimulation.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      177 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/bisimulation.h
+-rw-r--r--   0 mvolk      (502) staff       (20)       79 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/common.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    14947 2023-03-28 22:14:15.000000 stormpy-1.8.0/src/core/core.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      214 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/core.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     4205 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/counterexample.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       79 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/counterexample.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     4670 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/environment.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      173 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/environment.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     5807 2022-08-31 08:13:17.000000 stormpy-1.8.0/src/core/input.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      187 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/input.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    14323 2023-03-28 22:17:03.000000 stormpy-1.8.0/src/core/modelchecking.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      181 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/modelchecking.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    15313 2022-08-31 08:13:17.000000 stormpy-1.8.0/src/core/result.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      153 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/result.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     4445 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/simulator.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      254 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/simulator.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     8221 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/transformation.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      183 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/core/transformation.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.981440 stormpy-1.8.0/src/dft/
+-rw-r--r--   0 mvolk      (502) staff       (20)     5250 2023-06-12 19:54:05.000000 stormpy-1.8.0/src/dft/analysis.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      175 2022-05-05 11:29:07.000000 stormpy-1.8.0/src/dft/analysis.h
+-rw-r--r--   0 mvolk      (502) staff       (20)       60 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/dft/common.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3689 2023-06-12 19:54:05.000000 stormpy-1.8.0/src/dft/dft.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      205 2022-05-05 11:29:07.000000 stormpy-1.8.0/src/dft/dft.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2459 2022-05-27 15:11:15.000000 stormpy-1.8.0/src/dft/dft_elements.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      183 2022-02-12 20:10:34.000000 stormpy-1.8.0/src/dft/dft_elements.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3689 2022-07-13 13:50:01.000000 stormpy-1.8.0/src/dft/dft_state.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      179 2022-02-12 20:10:33.000000 stormpy-1.8.0/src/dft/dft_state.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     1716 2022-10-07 15:05:05.000000 stormpy-1.8.0/src/dft/io.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      104 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/dft/io.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     1288 2022-10-07 15:07:01.000000 stormpy-1.8.0/src/dft/module.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       69 2022-09-18 20:23:32.000000 stormpy-1.8.0/src/dft/module.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2818 2022-05-27 15:11:15.000000 stormpy-1.8.0/src/dft/simulator.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      177 2022-02-12 20:10:33.000000 stormpy-1.8.0/src/dft/simulator.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      649 2022-05-27 15:11:15.000000 stormpy-1.8.0/src/dft/transformations.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       79 2022-05-05 11:29:07.000000 stormpy-1.8.0/src/dft/transformations.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.989266 stormpy-1.8.0/src/gspn/
+-rw-r--r--   0 mvolk      (502) staff       (20)       62 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/gspn/common.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    15913 2023-03-28 22:17:05.000000 stormpy-1.8.0/src/gspn/gspn.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       70 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/gspn/gspn.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     1113 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/gspn/gspn_io.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       72 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/gspn/gspn_io.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      887 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/helpers.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.990849 stormpy-1.8.0/src/logic/
+-rw-r--r--   0 mvolk      (502) staff       (20)    11717 2023-03-28 13:08:09.000000 stormpy-1.8.0/src/logic/formulae.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      168 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/logic/formulae.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     1212 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/mod_core.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)     1241 2022-09-18 20:23:32.000000 stormpy-1.8.0/src/mod_dft.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      292 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/mod_gspn.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)     1594 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/mod_info.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      258 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/mod_logic.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      418 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/mod_pars.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      826 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/mod_pomdp.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)     2337 2022-08-31 08:13:17.000000 stormpy-1.8.0/src/mod_storage.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      528 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/mod_utility.cpp
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:26.996403 stormpy-1.8.0/src/pars/
+-rw-r--r--   0 mvolk      (502) staff       (20)      207 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pars/common.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    13299 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pars/model_instantiator.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      257 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pars/model_instantiator.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2647 2022-02-27 01:22:58.000000 stormpy-1.8.0/src/pars/pars.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      145 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pars/pars.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     9034 2023-03-28 22:17:05.000000 stormpy-1.8.0/src/pars/pla.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      141 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pars/pla.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:27.010894 stormpy-1.8.0/src/pomdp/
+-rw-r--r--   0 mvolk      (502) staff       (20)       24 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pomdp/common.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     1455 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pomdp/memory.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       69 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pomdp/memory.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     4541 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pomdp/qualitative_analysis.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      195 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pomdp/qualitative_analysis.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     5204 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pomdp/tracker.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      128 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pomdp/tracker.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     5048 2023-06-07 21:42:25.000000 stormpy-1.8.0/src/pomdp/transformations.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      177 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/pomdp/transformations.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:27.053122 stormpy-1.8.0/src/storage/
+-rw-r--r--   0 mvolk      (502) staff       (20)     2128 2023-04-06 14:33:17.000000 stormpy-1.8.0/src/storage/bitvector.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      174 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/bitvector.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2938 2023-04-12 11:30:57.000000 stormpy-1.8.0/src/storage/choiceorigins.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       71 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/choiceorigins.h
+-rw-r--r--   0 mvolk      (502) staff       (20)       24 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/common.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2317 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/dd.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      199 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/dd.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     1921 2022-03-21 12:00:57.000000 stormpy-1.8.0/src/storage/decomposition.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      210 2022-03-21 12:00:57.000000 stormpy-1.8.0/src/storage/decomposition.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      747 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/distribution.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      127 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/distribution.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    11598 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/expressions.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      182 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/expressions.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      730 2022-07-28 15:51:10.000000 stormpy-1.8.0/src/storage/geometry.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      123 2022-07-28 15:51:10.000000 stormpy-1.8.0/src/storage/geometry.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    14163 2023-03-28 22:17:06.000000 stormpy-1.8.0/src/storage/jani.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      113 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/jani.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3195 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/labeling.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      170 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/labeling.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     9435 2023-06-12 19:54:05.000000 stormpy-1.8.0/src/storage/matrix.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      273 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/matrix.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    36399 2023-06-12 19:54:05.000000 stormpy-1.8.0/src/storage/model.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      359 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/model.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     4047 2023-04-12 11:30:57.000000 stormpy-1.8.0/src/storage/model_components.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      278 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/model_components.h
+-rw-r--r--   0 mvolk      (502) staff       (20)    26006 2023-04-12 11:30:57.000000 stormpy-1.8.0/src/storage/prism.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       70 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/prism.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3487 2023-04-12 11:30:57.000000 stormpy-1.8.0/src/storage/scheduler.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      126 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/scheduler.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     1957 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/state.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)     3864 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/state.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3335 2023-04-12 11:30:57.000000 stormpy-1.8.0/src/storage/valuation.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      121 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/storage/valuation.h
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-06-12 19:54:27.061840 stormpy-1.8.0/src/utility/
+-rw-r--r--   0 mvolk      (502) staff       (20)      365 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/utility/chrono.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       73 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/utility/chrono.h
+-rw-r--r--   0 mvolk      (502) staff       (20)      758 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/utility/json.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      137 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/utility/json.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     3236 2023-03-28 22:17:16.000000 stormpy-1.8.0/src/utility/shortestPaths.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)      184 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/utility/shortestPaths.h
+-rw-r--r--   0 mvolk      (502) staff       (20)     2418 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/utility/smtsolver.cpp
+-rw-r--r--   0 mvolk      (502) staff       (20)       70 2022-02-10 13:02:01.000000 stormpy-1.8.0/src/utility/smtsolver.h
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stormpy-1.3.0/lib/stormpy/__init__.py` & `stormpy-1.8.0/lib/stormpy/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import sys
 
 if sys.version_info[0] == 2:
     raise ImportError('Python 2.x is not supported for stormpy.')
 
+from ._config import *
+
 from . import core
 from .core import *
 from . import storage
 from .storage import *
-from ._config import *
 from .logic import *
 from .exceptions import *
 
 from pycarl import Variable  # needed for building parametric models
 
 __version__ = "unknown"
 try:
@@ -32,14 +33,16 @@
     """
     if parametric:
         assert model.supports_parameters
         if model.model_type == ModelType.DTMC:
             return model._as_sparse_pdtmc()
         elif model.model_type == ModelType.MDP:
             return model._as_sparse_pmdp()
+        elif model.model_type == ModelType.POMDP:
+            return model._as_sparse_ppomdp()
         elif model.model_type == ModelType.CTMC:
             return model._as_sparse_pctmc()
         elif model.model_type == ModelType.MA:
             return model._as_sparse_pma()
         else:
             raise StormError("Not supported parametric model constructed")
     else:
@@ -185,33 +188,35 @@
         formulae = [(prop.raw_formula if isinstance(prop, Property) else prop) for prop in properties]
         intermediate = core._build_symbolic_parametric_model_from_symbolic_description(symbolic_description, formulae)
     else:
         intermediate = core._build_symbolic_parametric_model_from_symbolic_description(symbolic_description)
     return _convert_symbolic_model(intermediate, parametric=True)
 
 
-def build_model_from_drn(file):
+def build_model_from_drn(file, options=DirectEncodingParserOptions()):
     """
     Build a model in sparse representation from the explicit DRN representation.
 
     :param String file: DRN file containing the model.
+    :param DirectEncodingParserOptions: Options for the parser.
     :return: Model in sparse representation.
     """
-    intermediate = core._build_sparse_model_from_drn(file)
+    intermediate = core._build_sparse_model_from_drn(file, options)
     return _convert_sparse_model(intermediate, parametric=False)
 
 
-def build_parametric_model_from_drn(file):
+def build_parametric_model_from_drn(file, options = DirectEncodingParserOptions()):
     """
     Build a parametric model in sparse representation from the explicit DRN representation.
 
     :param String file: DRN file containing the model.
+    :param DirectEncodingParserOptions: Options for the parser.
     :return: Parametric model in sparse representation.
     """
-    intermediate = core._build_sparse_parametric_model_from_drn(file)
+    intermediate = core._build_sparse_parametric_model_from_drn(file, options)
     return _convert_sparse_model(intermediate, parametric=True)
 
 
 def perform_bisimulation(model, properties, bisimulation_type):
     """
     Perform bisimulation on model.
     :param model: Model.
@@ -233,66 +238,113 @@
     formulae = [(prop.raw_formula if isinstance(prop, Property) else prop) for prop in properties]
     if model.supports_parameters:
         return core._perform_parametric_bisimulation(model, formulae, bisimulation_type)
     else:
         return core._perform_bisimulation(model, formulae, bisimulation_type)
 
 
-def perform_symbolic_bisimulation(model, properties):
+def perform_symbolic_bisimulation(model, properties, quotient_format=stormpy.QuotientFormat.DD):
     """
     Perform bisimulation on model in symbolic representation.
     :param model: Model.
     :param properties: Properties to preserve during bisimulation.
+    :param quotient_format: Return format of quotient.
     :return: Model after bisimulation.
     """
     formulae = [(prop.raw_formula if isinstance(prop, Property) else prop) for prop in properties]
     bisimulation_type = BisimulationType.STRONG
     if model.supports_parameters:
-        return core._perform_symbolic_parametric_bisimulation(model, formulae, bisimulation_type)
+        return core._perform_symbolic_parametric_bisimulation(model, formulae, bisimulation_type, quotient_format)
     else:
-        return core._perform_symbolic_bisimulation(model, formulae, bisimulation_type)
+        return core._perform_symbolic_bisimulation(model, formulae, bisimulation_type, quotient_format)
 
 
-def model_checking(model, property, only_initial_states=False, extract_scheduler=False, environment=Environment()):
+def model_checking(model, property, only_initial_states=False, extract_scheduler=False, force_fully_observable=False, environment=Environment()):
     """
     Perform model checking on model for property.
     :param model: Model.
     :param property: Property to check for.
     :param only_initial_states: If True, only results for initial states are computed, otherwise for all states.
     :param extract_scheduler: If True, try to extract a scheduler
     :return: Model checking result.
     :rtype: CheckResult
     """
-    return check_model_sparse(model, property, only_initial_states=only_initial_states,
-                              extract_scheduler=extract_scheduler, environment=environment)
+    if model.is_sparse_model:
+        return check_model_sparse(model, property, only_initial_states=only_initial_states,
+                                  extract_scheduler=extract_scheduler, force_fully_observable=force_fully_observable, environment=environment)
+    else:
+        assert (model.is_symbolic_model)
+        if extract_scheduler:
+            raise StormError("Model checking based on dd engine does not support extracting schedulers right now.")
+        return check_model_dd(model, property, only_initial_states=only_initial_states,
+                              environment=environment)
 
 
-def check_model_sparse(model, property, only_initial_states=False, extract_scheduler=False, environment=Environment()):
+def check_model_sparse(model, property, only_initial_states=False, extract_scheduler=False, force_fully_observable=False, hint=None, environment=Environment()):
     """
     Perform model checking on model for property.
     :param model: Model.
     :param property: Property to check for.
     :param only_initial_states: If True, only results for initial states are computed, otherwise for all states.
     :param extract_scheduler: If True, try to extract a scheduler
+    :param hint: If not None, this hint is used by the model checker
+    :param force_fully_observable: If True, treat a POMDP as an MDP
     :return: Model checking result.
     :rtype: CheckResult
     """
     if isinstance(property, Property):
         formula = property.raw_formula
     else:
         formula = property
 
+    if model.is_partially_observable:
+        if force_fully_observable:
+            # Note that casting a model to a fully observable model wont work with python/pybind, so we actually have other access points
+            if model.supports_parameters:
+                raise NotImplementedError("")
+            elif model.is_exact:
+                task = core.ExactCheckTask(formula, only_initial_states)
+                task.set_produce_schedulers(extract_scheduler)
+                if hint:
+                    task.set_hint(hint)
+                return core._exact_model_checking_fully_observable(model, task, environment=environment)
+            else:
+                task = core.CheckTask(formula, only_initial_states)
+                task.set_produce_schedulers(extract_scheduler)
+                if hint:
+                    task.set_hint(hint)
+                return core._model_checking_fully_observable(model, task, environment=environment)
+        else:
+            raise RuntimeError("Model checking of partially observable models is handled via dedicated methods, unless the force fully-observable is set.")
+
+
+
     if model.supports_parameters:
         task = core.ParametricCheckTask(formula, only_initial_states)
         task.set_produce_schedulers(extract_scheduler)
+        if hint:
+            task.set_hint(hint)
         return core._parametric_model_checking_sparse_engine(model, task, environment=environment)
     else:
-        task = core.CheckTask(formula, only_initial_states)
-        task.set_produce_schedulers(extract_scheduler)
-        return core._model_checking_sparse_engine(model, task, environment=environment)
+        if model.is_exact:
+            if formula.is_multi_objective_formula:
+                return core._multi_objective_model_checking_exact(model, formula, environment=environment)
+            task = core.ExactCheckTask(formula, only_initial_states)
+            task.set_produce_schedulers(extract_scheduler)
+            if hint:
+                task.set_hint(hint)
+            return core._exact_model_checking_sparse_engine(model, task, environment=environment)
+        else:
+            if formula.is_multi_objective_formula:
+                return core._multi_objective_model_checking_double(model, formula, environment=environment)
+            task = core.CheckTask(formula, only_initial_states)
+            task.set_produce_schedulers(extract_scheduler)
+            if hint:
+                task.set_hint(hint)
+            return core._model_checking_sparse_engine(model, task, environment=environment)
 
 
 def check_model_dd(model, property, only_initial_states=False, environment=Environment()):
     """
     Perform model checking using dd engine.
     :param model: Model.
     :param property: Property to check for.
@@ -330,26 +382,56 @@
     if model.supports_parameters:
         task = core.ParametricCheckTask(formula, only_initial_states)
         return core._parametric_model_checking_hybrid_engine(model, task, environment=environment)
     else:
         task = core.CheckTask(formula, only_initial_states)
         return core._model_checking_hybrid_engine(model, task, environment=environment)
 
+
 def transform_to_sparse_model(model):
     """
     Transform model in symbolic representation into model in sparse representation.
     :param model: Symbolic model.
     :return: Sparse model.
     """
     if model.supports_parameters:
         return core._transform_to_sparse_parametric_model(model)
     else:
         return core._transform_to_sparse_model(model)
 
 
+def transform_to_discrete_time_model(model, properties):
+    """
+    Transform continuous-time model to discrete time model.
+    :param model: Continuous-time model.
+    :param properties: List of properties to transform as well.
+    :return: Tuple (Discrete-time model, converted properties).
+    """
+    formulae = [(prop.raw_formula if isinstance(prop, Property) else prop) for prop in properties]
+    if model.supports_parameters:
+        return core._transform_to_discrete_time_parametric_model(model, formulae)
+    else:
+        return core._transform_to_discrete_time_model(model, formulae)
+
+
+def eliminate_non_markovian_chains(ma, properties, label_behavior):
+    """
+    Eliminate chains of non-Markovian states if possible.
+    :param ma: Markov automaton.
+    :param properties: List of properties to transform as well.
+    :param label_behavior: Behavior of labels while elimination.
+    :return: Tuple (converted MA, converted properties).
+    """
+    formulae = [(prop.raw_formula if isinstance(prop, Property) else prop) for prop in properties]
+    if ma.supports_parameters:
+        return core._eliminate_non_markovian_chains_parametric(ma, formulae, label_behavior)
+    else:
+        return core._eliminate_non_markovian_chains(ma, formulae, label_behavior)
+
+
 def prob01min_states(model, eventually_formula):
     assert type(eventually_formula) == logic.EventuallyFormula
     labelform = eventually_formula.subformula
     labelprop = core.Property("label-prop", labelform)
     phiStates = BitVector(model.nr_states, True)
     psiStates = model_checking(model, labelprop).get_truth_values()
     return compute_prob01min_states(model, phiStates, psiStates)
@@ -394,35 +476,134 @@
     if model.model_type == ModelType.DTMC:
         return compute_prob01_states(model, phi_states, psi_states)
     if model.supports_parameters:
         return core._compute_prob01states_max_rationalfunc(model, phi_states, psi_states)
     else:
         return core._compute_prob01states_max_double(model, phi_states, psi_states)
 
+
 def topological_sort(model, forward=True, initial=[]):
     """
 
-    :param model:
-    :param forward:
-    :return:
+    :param model: A sparse model
+    :param forward: A flag whether the sorting should be forward or backwards
+    :param initial: a list of states
+    :return: A topological sort of the states
     """
     matrix = model.transition_matrix if forward else model.backward_transition_matrix
     if isinstance(model, storage._SparseParametricModel):
         return storage._topological_sort_rf(matrix, initial)
     elif isinstance(model, storage._SparseModel):
         return storage._topological_sort_double(matrix, initial)
     else:
         raise StormError("Unknown kind of model.")
 
-def construct_submodel(model, states, actions, keep_unreachable_states = True, options = SubsystemBuilderOptions()):
+
+def get_reachable_states(model, initial_states, constraint_states, target_states, maximal_steps = None, choice_filter = None ):
+    """
+    Get the states that are reachable in a sparse model
+
+    :param model: A model
+    :param initial_states: Which states should be definitively reachable
+    :param constraint_states:
+    :param target_states: Which states should be considered absorbing
+    :param maximal_steps: The maximal depth to explore
+    :param choice_filter:
+    :return:
+    """
+    if model.supports_parameters:
+        return core._get_reachable_states_rf(model, initial_states, constraint_states, target_states, maximal_steps, choice_filter)
+    if model.is_exact:
+        return core._get_reachable_states_exact(model, initial_states, constraint_states, target_states, maximal_steps, choice_filter)
+    return core._get_reachable_states_double(model, initial_states, constraint_states, target_states, maximal_steps, choice_filter)
+
+
+def compute_expected_number_of_visits(environment, model):
+    """
+    Compute the number of expected visits. Model must be deterministic.
+
+    :param environment: An model checking environment
+    :param model: A DTMC or CTMC
+    :return: A vector with the expected number of visits
+    """
+    if model.supports_parameters:
+        raise NotImplementedError("Expected number of visits is not implemented for parametric models")
+    if model.is_exact:
+        return core._compute_expected_number_of_visits_exact(environment, model)
+    return core._compute_expected_number_of_visits_double(environment, model)
+
+
+def construct_submodel(model, states, actions, keep_unreachable_states=True, options=SubsystemBuilderOptions()):
     """
 
     :param model: The model
     :param states: Which states should be preserved
     :param actions: Which actions should be preserved
     :param keep_unreachable_states: If False, run a reachability analysis.
+    :param options: An options object of type SubsystemBuilderOptions
     :return: A model with fewer states/actions
     """
-    if isinstance(model, storage._SparseModel):
-        return core._construct_subsystem_double(model, states, actions, keep_unreachable_states, options)
+    if model.supports_parameters:
+        return core._construct_subsystem_RatFunc(model, states, actions, keep_unreachable_states, options)
+    if model.is_exact:
+        return core._construct_subsystem_Exact(model, states, actions, keep_unreachable_states, options)
+    return core._construct_subsystem_Double(model, states, actions, keep_unreachable_states, options)
+
+
+def eliminate_ECs(matrix, subsystem, possible_ecs, add_sink_row_states, add_self_loop_at_sink_states = False):
+    """
+    For each such EC (that is not contained in another EC), we add a new state and redirect all incoming and outgoing
+             transitions of the EC to (and from) this state.
+
+    :param matrix:
+    :param subsystem: BitVector with states many entries. Only states in the given subsystem are kept. Transitions leading to a state outside of the subsystem will be
+             removed (but the corresponding row is kept, possibly yielding empty rows).
+             The ECs are then identified on the subsystem.
+    :param possible_ecs: BitVector with rows many entries. Only ECs for which possible_ecs is true for all choices are considered.
+             Furthermore, the rows that contain a transition leading outside of the subsystem are not considered for an EC.
+    :param add_sink_row_states: BitVector with states many entries. If add_sink_row_states is true for at least one state of an eliminated EC, a row is added to the new state (representing the choice to stay at the EC forever).
+    :param add_self_loop_at_sink_states: if true, such rows get a selfloop (with value 1). Otherwise, the row remains empty.
+    :return: A container with various information.
+    """
+    assert matrix.nr_columns == subsystem.size(), "subsystem vector should have an entry for every state."
+    assert matrix.nr_rows == possible_ecs.size(), "possible_ecs vector should have an entry for every row."
+    assert matrix.nr_columns == add_sink_row_states.size(), "add_sink_row_states vector should have an entry for every state."
+
+    return core._eliminate_end_components_double(matrix, subsystem, possible_ecs, add_sink_row_states, add_self_loop_at_sink_states)
+
+
+def parse_properties(properties, context=None, filters=None):
+    """
+
+    :param properties: A string with the pctl properties
+    :param context: A symbolic model that gives meaning to variables and constants.
+    :param filters: filters, if applicable.
+    :return: A list of properties
+    """
+    if context is None:
+        return core.parse_properties_without_context(properties, filters)
+    elif type(context) == core.SymbolicModelDescription:
+        if context.is_prism_program():
+            return core.parse_properties_for_prism_program(properties, context.as_prism_program(), filters)
+        else:
+            core.parse_properties_for_jani_program(properties, context.as_jani_model(), filters)
+    elif type(context) == storage.PrismProgram:
+        return core.parse_properties_for_prism_program(properties, context, filters)
+    elif type(context) == storage.JaniModel:
+        core.parse_properties_for_jani_model(properties, context, filters)
     else:
-        raise NotImplementedError()
+        raise StormError("Unclear context. Please pass a symbolic model description")
+
+
+def export_to_drn(model, file, options=DirectEncodingOptions()):
+    """
+    Export a model to DRN format
+    :param model: The model
+    :param file: A path
+    :param options: DirectEncodingOptions
+    :return:
+    """
+    if model.supports_parameters:
+        return core._export_parametric_to_drn(model, file, options)
+    if model.is_exact:
+        return core._export_exact_to_drn(model, file, options)
+    return core._export_to_drn(model, file, options)
```

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/ctmc/cluster2.sm` & `stormpy-1.8.0/lib/stormpy/examples/files/ctmc/cluster2.sm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/ctmc/dft.drn` & `stormpy-1.8.0/lib/stormpy/examples/files/ctmc/dft.drn`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/ctmc/embedded2.sm` & `stormpy-1.8.0/lib/stormpy/examples/files/ctmc/embedded2.sm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/ctmc/fms2.sm` & `stormpy-1.8.0/lib/stormpy/examples/files/ctmc/fms2.sm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/ctmc/polling2.sm` & `stormpy-1.8.0/lib/stormpy/examples/files/ctmc/polling2.sm`

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,8 @@
 endrewards
 
 // expected number of times station 1 is served
 rewards "served"
 	[serve1] true : 1;
 endrewards
 
-label "target" = s=1&a=0;
+label "target" = s=1&a=1;
```

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/ctmc/tandem5.sm` & `stormpy-1.8.0/lib/stormpy/examples/files/ctmc/tandem5.sm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dft/and.json` & `stormpy-1.8.0/lib/stormpy/examples/files/dft/and.json`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dft/hecs.dft` & `stormpy-1.8.0/lib/stormpy/examples/files/dft/hecs.dft`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dtmc/brp-16-2.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/dtmc/brp-16-2.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dtmc/brp.jani` & `stormpy-1.8.0/lib/stormpy/examples/files/dtmc/brp.jani`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dtmc/crowds-5-5.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/dtmc/crowds-5-5.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dtmc/crowds5_5.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/dtmc/crowds5_5.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dtmc/die.jani` & `stormpy-1.8.0/lib/stormpy/examples/files/dtmc/die.jani`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dtmc/die.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/dtmc/die.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dtmc/leader-3-5.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/dtmc/leader-3-5.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dtmc/leader3_5.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/dtmc/leader3_5.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/dtmc/nand-5-2.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/dtmc/nand-5-2.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/lab/crowds5_5.lab` & `stormpy-1.8.0/lib/stormpy/examples/files/lab/crowds5_5.lab`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/lab/two_dice.lab` & `stormpy-1.8.0/lib/stormpy/examples/files/lab/two_dice.lab`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/ma/stream2.ma` & `stormpy-1.8.0/lib/stormpy/examples/files/ma/stream2.ma`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/coin2-2-illegalSynchronizingWrite.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/coin2-2-illegalSynchronizingWrite.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/coin2-2.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/coin2-2.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/coin2.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/coin2.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/csma2-2.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/csma2-2.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/csma2_2.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/csma2_2.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/die_c1.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/die_c1.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/die_selection.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/die_selection.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/firewire.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/firewire.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/firewire3-0.5.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/firewire3-0.5.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/leader3.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/leader3.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/leader4.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/leader4.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/maze_2.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/maze_2.nm`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-// maze example (POMDP)
+// maze example (POMDP) as an MDP
 // slightly extends that presented in
 // Littman, Cassandra and Kaelbling
 // Learning policies for partially observable environments: Scaling up
 // Technical Report CS, Brown University
 // gxn 29/01/16
 // Made into a MDP for documentation of stormpy.
 
@@ -87,18 +87,19 @@
 	[south] s=8 -> (s'=11);
 
 	[east] s=9 -> (s'=9);
 	[west] s=9 -> (s'=9);
 	[north] s=9 -> (s'=6);
 	[south] s=9 -> (s'=13);
 
-	[east] s=10 -> (s'=9);
-	[west] s=10 -> (s'=9);
+	[east] s=10 -> (s'=10);
+	[west] s=10 -> (s'=10);
 	[north] s=10 -> (s'=7);
 	[south] s=10 -> (s'=12);
+
 	[east] s=11 -> (s'=11);
 	[west] s=11 -> (s'=11);
 	[north] s=11 -> (s'=8);
 	[south] s=11 -> (s'=11);
 
 	[east] s=12 -> (s'=12);
 	[west] s=12 -> (s'=12);
```

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/two_dice.lab` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/two_dice.lab`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/two_dice.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/two_dice.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/two_dice.tra` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/two_dice.tra`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/wlan0-2-2.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/wlan0-2-2.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/mdp/wlan0_collide.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/mdp/wlan0_collide.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/brp16_2.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/brp16_2.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/brp_rewards16_2.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/brp_rewards16_2.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/crowds3_5.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/crowds3_5.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/die.drn` & `stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/die.drn`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/pdtmc/parametric_die.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/pdtmc/parametric_die.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/pmdp/coin2_2.pm` & `stormpy-1.8.0/lib/stormpy/examples/files/pmdp/coin2_2.pm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/pmdp/two_dice.nm` & `stormpy-1.8.0/lib/stormpy/examples/files/pmdp/two_dice.nm`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/pomdp/maze_2.prism` & `stormpy-1.8.0/lib/stormpy/examples/files/pomdp/maze_2_par.prism`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 
 // can observe the walls and target
 observables
 	o
 endobservables
 // o=0 - observation in initial state
 // o=1 - west and north walls (s0)
-// o=2 - north and south ways (s1 and s3)
+// o=2 - north and south walls (s1 and s3)
 // o=3 - north wall (s2)
 // o=4 - east and north way (s4)
 // o=5 - east and west walls (s5, s6, s7, s8, s9 and s10)
 // o=6 - east, west and south walls (s11 and s12)
 // o=7 - the target (s13)
 
+const double i;
+
 module maze
 
 	s : [-1..13];
 	o : [0..7];
 	
 	// initialisation
 	[] s=-1 -> 1/13 : (s'=0) & (o'=1)
@@ -65,15 +67,15 @@
 
 	[east] s=2 -> (s'=3) & (o'=2);
 	[west] s=2 -> (s'=1) & (o'=2);
 	[north] s=2 -> (s'=2);
 	[south] s=2 -> (s'=6) & (o'=5);
 
 	[east] s=3 -> (s'=4) & (o'=4);
-	[west] s=3 -> (s'=2) & (o'=2);
+	[west] s=3 -> (s'=2) & (o'=3);
 	[north] s=3 -> (s'=3);
 	[south] s=3 -> (s'=3);
 
 	[east] s=4 -> (s'=4);
 	[west] s=4 -> (s'=3) & (o'=2);
 	[north] s=4 -> (s'=4);
 	[south] s=4 -> (s'=7) & (o'=5);
@@ -97,18 +99,18 @@
 	[west] s=8 -> (s'=8);
 	[north] s=8 -> (s'=5);
 	[south] s=8 -> (s'=11) & (o'=6);
 
 	[east] s=9 -> (s'=9);
 	[west] s=9 -> (s'=9);
 	[north] s=9 -> (s'=6);
-	[south] s=9 -> (s'=13) & (o'=7);
+	[south] s=9 -> i: (s'=13) & (o'=7) + (1-i):(s'=9);
 
-	[east] s=10 -> (s'=9);
-	[west] s=10 -> (s'=9);
+	[east] s=10 -> (s'=10);
+	[west] s=10 -> (s'=10);
 	[north] s=10 -> (s'=7);
 	[south] s=10 -> (s'=12) & (o'=6);
 
 	[east] s=11 -> (s'=11);
 	[west] s=11 -> (s'=11);
 	[north] s=11 -> (s'=8) & (o'=5);
 	[south] s=11 -> (s'=11);
@@ -131,9 +133,10 @@
 	[north] true : 1;
 	[south] true : 1;
 
 endrewards
 
 // target observation
 label "goal" = o=7;
+label "bad" = o=6;
```

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/rew/leader4.trans.rew` & `stormpy-1.8.0/lib/stormpy/examples/files/rew/leader4.trans.rew`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/rew/leader4_8.pick.trans.rew` & `stormpy-1.8.0/lib/stormpy/examples/files/rew/leader4_8.pick.trans.rew`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/rew/state_reward_parser_basic.state.rew` & `stormpy-1.8.0/lib/stormpy/examples/files/rew/state_reward_parser_basic.state.rew`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/rew/state_reward_parser_whitespaces.state.rew` & `stormpy-1.8.0/lib/stormpy/examples/files/rew/state_reward_parser_whitespaces.state.rew`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/rew/two_dice.flip.state.rew` & `stormpy-1.8.0/lib/stormpy/examples/files/rew/two_dice.flip.state.rew`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/rew/two_dice.flip.trans.rew` & `stormpy-1.8.0/lib/stormpy/examples/files/rew/two_dice.flip.trans.rew`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/tra/crowds5_5.tra` & `stormpy-1.8.0/lib/stormpy/examples/files/tra/crowds5_5.tra`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/tra/leader4.tra` & `stormpy-1.8.0/lib/stormpy/examples/files/tra/leader4.tra`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/tra/leader4_8.tra` & `stormpy-1.8.0/lib/stormpy/examples/files/tra/leader4_8.tra`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files/tra/two_dice.tra` & `stormpy-1.8.0/lib/stormpy/examples/files/tra/two_dice.tra`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/examples/files.py` & `stormpy-1.8.0/lib/stormpy/examples/files.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,25 +15,41 @@
 
 prism_dtmc_die = _path("dtmc", "die.pm")
 """Knuth Yao Die Example"""
 prism_pdtmc_die = _path("pdtmc", "parametric_die.pm")
 """Knuth Yao Die -- 2 unfair coins Example"""
 prism_dtmc_brp = _path("dtmc", "brp-16-2.pm")
 """Bounded Retransmission Protocol"""
+prism_ma_simple = _path("ma", "simple.ma")
+"""Prism file for a simple Markov automaton"""
 drn_ctmc_dft = _path("ctmc", "dft.drn")
 """DRN format for a CTMC from a DFT"""
 drn_pdtmc_die = _path("pdtmc", "die.drn")
 """DRN format for a pDTMC for the KY-Die"""
 jani_dtmc_die = _path("dtmc", "die.jani")
 """Jani Version of Knuth Yao Die Example"""
+prism_pdtmc_brp = _path("pdtmc", "brp16_2.pm")
+"""Bounded retransmission protocol with parameters"""
 prism_mdp_coin_2_2 = _path("mdp", "coin2-2.nm")
+""""""
+prism_mdp_firewire = _path("mdp", "firewire.nm")
 """Prism example for coin MDP"""
 prism_pmdp_coin_two_dice = _path("pmdp", "two_dice.nm")
 """Prism example for parametric two dice"""
 prism_mdp_maze = _path("mdp", "maze_2.nm")
 """Prism example for the maze MDP"""
+prism_mdp_slipgrid = _path("mdp", "slipgrid.nm")
+"""Prism example for a slippery grid with fixed dimensions"""
+drn_pomdp_maze = _path("pomdp", "maze.drn")
+"""DRN example for the maze POMDP"""
 prism_pomdp_maze = _path("pomdp", "maze_2.prism")
 """Prism example for the maze POMDP"""
+prism_par_pomdp_maze = _path("pomdp", "maze_2_par.prism")
+"""Prism example for the parametric POMDP"""
 dft_galileo_hecs = _path("dft", "hecs.dft")
 """DFT example for HECS (Galileo format)"""
 dft_json_and = _path("dft", "and.json")
 """DFT example for AND gate (JSON format)"""
+gspn_pnpro_simple = _path("gspn", "gspn_simple.pnpro")
+"""GSPN example (PNPRO format)"""
+gspn_pnml_simple = _path("gspn", "gspn_simple.pnml")
+"""GSPN example (PNML format)"""
```

### Comparing `stormpy-1.3.0/lib/stormpy/info/__init__.py` & `stormpy-1.8.0/lib/stormpy/info/__init__.py`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/lib/stormpy/pars/__init__.py` & `stormpy-1.8.0/lib/stormpy/pars/__init__.py`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/setup/config.py` & `stormpy-1.8.0/setup/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,20 @@
         try:
             no_jobs = multiprocessing.cpu_count() if multiprocessing.cpu_count() is not None else 1
         except NotImplementedError:
             no_jobs = 1
         return {
             "storm_dir": "",
             "disable_dft": False,
+            "disable_gspn": False,
             "disable_pars": False,
+            "disable_pomdp": False,
             "debug": False,
             "jobs": str(no_jobs),
+            "pybind_version": ""
         }
 
     def load_from_file(self, path):
         """
         Load config from file.
         :param path Path to config file.
         """
```

### Comparing `stormpy-1.3.0/setup/helper.py` & `stormpy-1.8.0/setup/helper.py`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/setup.py` & `stormpy-1.8.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import os
 import sys
 import subprocess
 import datetime
 
 from setuptools import setup, Extension, find_packages
 from setuptools.command.build_ext import build_ext
-from distutils.version import StrictVersion
 
 import setup.helper as setup_helper
 from setup.config import SetupConfig
 
 if sys.version_info[0] == 2:
     sys.exit('Sorry, Python 2.x is not supported')
 
 # Minimal storm version required
-storm_min_version = "1.3.0"
+storm_min_version = "1.8.0"
 
 # Get the long description from the README file
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 class CMakeExtension(Extension):
-    def __init__(self, name, sourcedir='', subdir=''):
+    def __init__(self, name, sourcedir=''):
         Extension.__init__(self, name, sources=[])
         self.sourcedir = os.path.abspath(sourcedir)
-        self.subdir = subdir
 
 
 class CMakeBuild(build_ext):
     user_options = build_ext.user_options + [
         ('storm-dir=', None, 'Path to storm root (binary) location'),
         ('disable-dft', None, 'Disable support for DFTs'),
+        ('disable-gspn', None, 'Disable support for GSPNs'),
         ('disable-pars', None, 'Disable support for parametric models'),
+        ('disable-pomdp', None, 'Disable support for POMDP analysis'),
         ('debug', None, 'Build in Debug mode'),
-        ('jobs=', 'j', 'Number of jobs to use for compiling')
+        ('jobs=', 'j', 'Number of jobs to use for compiling'),
+        ('pybind-version=', None, 'Pybind11 version to use'),
     ]
 
     config = SetupConfig()
 
     def _extdir(self, extname):
         return os.path.abspath(os.path.dirname(self.get_ext_fullpath(extname)))
 
@@ -65,140 +66,128 @@
         _ = subprocess.check_output(['cmake', os.path.abspath("cmake")] + cmake_args, cwd=build_temp_version)
         cmake_conf = setup_helper.load_cmake_config(os.path.join(build_temp_version, 'generated/config.py'))
 
         # Set storm directory
         if storm_dir == "":
             storm_dir = cmake_conf.STORM_DIR
         if storm_dir != cmake_conf.STORM_DIR:
-            print("Stormpy - Warning: Using different storm directory {} instead of given {}!".format(
+            print("Stormpy - WARNING: Using different storm directory {} instead of given {}!".format(
                 cmake_conf.STORM_DIR,
                 storm_dir))
             storm_dir = cmake_conf.STORM_DIR
 
         # Check version
+        from packaging.version import Version # Need to import here because otherwise packaging cannot be automatically installed as required dependency
         storm_version, storm_commit = setup_helper.parse_storm_version(cmake_conf.STORM_VERSION)
-        if StrictVersion(storm_version) < StrictVersion(storm_min_version):
-            sys.exit(
-                'Stormpy - Error: Storm version {} from \'{}\' is not supported anymore!'.format(storm_version,
-                                                                                                 storm_dir))
+        if Version(storm_version) < Version(storm_min_version):
+            print('Stormpy - Error: Storm version {} from \'{}\' is not supported anymore!'.format(storm_version, storm_dir))
+            print("                 For more information, see https://moves-rwth.github.io/stormpy/installation.html#compatibility-of-stormpy-and-storm")
+            sys.exit(42)  # Custom exit code which can be used for incompatible checks
 
         # Check additional support
         use_dft = cmake_conf.HAVE_STORM_DFT and not self.config.get_as_bool("disable_dft")
+        use_gspn = cmake_conf.HAVE_STORM_GSPN and not self.config.get_as_bool("disable_gspn")
         use_pars = cmake_conf.HAVE_STORM_PARS and not self.config.get_as_bool("disable_pars")
+        use_pomdp = cmake_conf.HAVE_STORM_POMDP and not self.config.get_as_bool("disable_pomdp")
+
+        # Set pybind version
+        from pycarl._config import PYBIND_VERSION as pycarl_pybind_version
+        pybind_version = self.config.get_as_string("pybind_version")
+        if pybind_version == "":
+            pybind_version = pycarl_pybind_version
+        elif Version(pybind_version) != Version(pycarl_pybind_version):
+            print("Stormpy - WARNING: Given pybind11 version {} differs from pycarl pybind11 version {}!".format(pybind_version, pycarl_pybind_version))
 
         # Print build info
         print("Stormpy - Using storm {} from {}".format(storm_version, storm_dir))
+        print("Stormpy - Using pybind11 version {}".format(pybind_version))
         if use_dft:
             print("Stormpy - Support for DFTs found and included.")
         else:
-            print("Stormpy - Warning: No support for DFTs!")
+            print("Stormpy - WARNING: No support for DFTs!")
+        if use_gspn:
+            print("Stormpy - Support for GSPNs found and included.")
+        else:
+            print("Stormpy - WARNING: No support for GSPNs!")
         if use_pars:
             print("Stormpy - Support for parametric models found and included.")
         else:
-            print("Stormpy - Warning: No support for parametric models!")
+            print("Stormpy - WARNING: No support for parametric models!")
+        if use_pomdp:
+            print("Stormpy - Support for POMDP analysis found and included.")
+        else:
+            print("Stormpy - WARNING: No support for POMDP analysis!")
 
-        # Set general cmake build options
         build_type = 'Debug' if self.config.get_as_bool("debug") else 'Release'
-        cmake_args = ['-DPYTHON_EXECUTABLE=' + sys.executable]
+        # Set cmake build options
+        cmake_args = ['-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=' + self._extdir("core")]
+        cmake_args += ['-DPYTHON_EXECUTABLE=' + sys.executable]
         cmake_args += ['-DCMAKE_BUILD_TYPE=' + build_type]
+        cmake_args += ['-DPYBIND_VERSION=' + pybind_version]
         if storm_dir is not None:
             cmake_args += ['-Dstorm_DIR=' + storm_dir]
-        if use_dft:
-            cmake_args += ['-DHAVE_STORM_DFT=ON']
-        if use_pars:
-            cmake_args += ['-DHAVE_STORM_PARS=ON']
+        cmake_args += ['-DUSE_STORM_DFT=' + ('ON' if use_dft else 'OFF')]
+        cmake_args += ['-DUSE_STORM_GSPN=' + ('ON' if use_gspn else 'OFF')]
+        cmake_args += ['-DUSE_STORM_PARS=' + ('ON' if use_pars else 'OFF')]
+        cmake_args += ['-DUSE_STORM_POMDP=' + ('ON' if use_pomdp else 'OFF')]
+        # Configure extensions
+        env = os.environ.copy()
+        env['CXXFLAGS'] = '{} -DVERSION_INFO=\\"{}\\"'.format(env.get('CXXFLAGS', ''), self.distribution.get_version())
+        setup_helper.ensure_dir_exists(self.build_temp)
+        print("Stormpy - CMake args={}".format(cmake_args))
+        # Call cmake
+        subprocess.check_call(['cmake', os.path.abspath("")] + cmake_args, cwd=self.build_temp, env=env)
+
+        # Set build args
         build_args = ['--config', build_type]
         build_args += ['--', '-j{}'.format(self.config.get_as_int("jobs"))]
 
         # Build extensions
         for ext in self.extensions:
-            setup_helper.ensure_dir_exists(os.path.join(self._extdir(ext.name), ext.subdir))
-            if ext.name == "core":
-                with open(os.path.join(self._extdir(ext.name), ext.subdir, "_config.py"), "w") as f:
-                    f.write("# Generated from setup.py at {}\n".format(datetime.datetime.now()))
-
-                    f.write("import pycarl\n")
-                    if cmake_conf.STORM_CLN_EA or cmake_conf.STORM_CLN_RF:
-                        f.write("import pycarl.cln\n")
-                    if not cmake_conf.STORM_CLN_EA or not cmake_conf.STORM_CLN_RF:
-                        f.write("import pycarl.gmp\n")
-
-                    if cmake_conf.STORM_CLN_EA:
-                        f.write("Rational = pycarl.cln.Rational\n")
-                    else:
-                        f.write("Rational = pycarl.gmp.Rational\n")
-
-                    if cmake_conf.STORM_CLN_RF:
-                        rfpackage = "cln"
-                    else:
-                        rfpackage = "gmp"
-                    f.write("RationalRF = pycarl.{}.Rational\n".format(rfpackage))
-                    f.write("Polynomial = pycarl.{}.Polynomial\n".format(rfpackage))
-                    f.write("FactorizedPolynomial = pycarl.{}.FactorizedPolynomial\n".format(rfpackage))
-                    f.write("RationalFunction = pycarl.{}.RationalFunction\n".format(rfpackage))
-                    f.write("FactorizedRationalFunction = pycarl.{}.FactorizedRationalFunction\n".format(rfpackage))
-                    f.write("\n")
-                    f.write("storm_with_dft = {}\n".format(use_dft))
-                    f.write("storm_with_pars = {}\n".format(use_pars))
-
-            elif ext.name == "info":
-                with open(os.path.join(self._extdir(ext.name), ext.subdir, "_config.py"), "w") as f:
-                    f.write("# Generated from setup.py at {}\n".format(datetime.datetime.now()))
-                    f.write("storm_version = \"{}\"\n".format(storm_version))
-                    f.write("storm_cln_ea = {}\n".format(cmake_conf.STORM_CLN_EA))
-                    f.write("storm_cln_rf = {}".format(cmake_conf.STORM_CLN_RF))
-            elif ext.name == "dft":
-                with open(os.path.join(self._extdir(ext.name), ext.subdir, "_config.py"), "w") as f:
-                    f.write("# Generated from setup.py at {}\n".format(datetime.datetime.now()))
-                    f.write("storm_with_dft = {}".format(use_dft))
-                if not use_dft:
-                    print("Stormpy - DFT bindings skipped")
-                    continue
-            elif ext.name == "pars":
-                with open(os.path.join(self._extdir(ext.name), ext.subdir, "_config.py"), "w") as f:
-                    f.write("# Generated from setup.py at {}\n".format(datetime.datetime.now()))
-                    f.write("storm_with_pars = {}".format(use_pars))
-                if not use_pars:
-                    print("Stormpy - Bindings for parametric models skipped")
-                    continue
-            self.build_extension(ext, cmake_args, build_args)
+            if ext.name == "dft" and not use_dft:
+                print("Stormpy - Bindings for DFTs skipped")
+                continue
+            if ext.name == "gspn" and not use_gspn:
+                print("Stormpy - Bindings for GSPNs skipped")
+                continue
+            if ext.name == "pars" and not use_pars:
+                print("Stormpy - Bindings for parametric models skipped")
+                continue
+            if ext.name == "pomdp" and not use_pomdp:
+                print("Stormpy - Bindings for POMDP analysis skipped")
+                continue
+            # Call make
+            subprocess.check_call(['cmake', '--build', '.', '--target', ext.name] + build_args, cwd=self.build_temp)
 
     def initialize_options(self):
         build_ext.initialize_options(self)
-        # Load setup config
-        self.config.load_from_file("build/build_config.cfg")
         # Set default values for custom cmdline flags
         self.storm_dir = None
         self.disable_dft = None
+        self.disable_gspn = None
         self.disable_pars = None
+        self.disable_pomdp = None
         self.debug = None
         self.jobs = None
+        self.pybind_version = None
 
     def finalize_options(self):
         build_ext.finalize_options(self)
+        # Load setup config
+        # This can only be done after the finalization step, because otherwise build_temp is not initialized yet.
+        self.config.load_from_file(os.path.join(self.build_temp, "build_config.cfg"))
         # Update setup config
         self.config.update("storm_dir", self.storm_dir)
         self.config.update("disable_dft", self.disable_dft)
+        self.config.update("disable_gspn", self.disable_gspn)
         self.config.update("disable_pars", self.disable_pars)
+        self.config.update("disable_pomdp", self.disable_pomdp)
         self.config.update("debug", self.debug)
         self.config.update("jobs", self.jobs)
-
-    def build_extension(self, ext, general_cmake_args, general_build_args):
-        extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
-        cmake_args = ['-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=' + os.path.join(extdir, ext.subdir)] + general_cmake_args
-        build_args = general_build_args
-
-        env = os.environ.copy()
-        env['CXXFLAGS'] = '{} -DVERSION_INFO=\\"{}\\"'.format(env.get('CXXFLAGS', ''),
-                                                              self.distribution.get_version())
-        setup_helper.ensure_dir_exists(self.build_temp)
-        print("Stormpy - CMake args={}".format(cmake_args))
-        # Call cmake
-        subprocess.check_call(['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
-        subprocess.check_call(['cmake', '--build', '.', '--target', ext.name] + build_args, cwd=self.build_temp)
+        self.config.update("pybind_version", self.pybind_version)
 
 
 setup(
     name="stormpy",
     version=setup_helper.obtain_version(),
     author="M. Volk",
     author_email="matthias.volk@cs.rwth-aachen.de",
@@ -220,22 +209,32 @@
     ],
 
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     include_package_data=True,
     package_data={'stormpy.examples': ['examples/files/*']},
     ext_package='stormpy',
-    ext_modules=[CMakeExtension('core', subdir=''),
-                 CMakeExtension('info', subdir='info'),
-                 CMakeExtension('logic', subdir='logic'),
-                 CMakeExtension('storage', subdir='storage'),
-                 CMakeExtension('utility', subdir='utility'),
-                 CMakeExtension('dft', subdir='dft'),
-                 CMakeExtension('pars', subdir='pars')],
-
+    ext_modules=[CMakeExtension('core'),
+                 CMakeExtension('info'),
+                 CMakeExtension('logic'),
+                 CMakeExtension('storage'),
+                 CMakeExtension('utility'),
+                 CMakeExtension('dft'),
+                 CMakeExtension('gspn'),
+                 CMakeExtension('pars'),
+                 CMakeExtension('pomdp')
+                 ],
     cmdclass={'build_ext': CMakeBuild},
     zip_safe=False,
-    install_requires=['pycarl>=2.0.3'],
-    setup_requires=['pytest-runner'],
-    tests_require=['pytest'],
-    python_requires='>=3',
+    install_requires=['pycarl>=2.2.0'],
+    setup_requires=['pycarl>=2.2.0', # required to check pybind version used for pycarl
+                   'pytest-runner',
+                   'packaging'
+                   ],
+    tests_require=['pytest', 'nbval', 'numpy'],
+    extras_require={
+        "numpy":  ["numpy"],
+        "plot":  ["matplotlib","numpy","scipy"],
+        "doc": ["Sphinx", "sphinx-bootstrap-theme", "nbsphinx", "ipython", "ipykernel"], # also requires pandoc to be installed
+    },
+    python_requires='>=3.7', # required by packaging
 )
```

### Comparing `stormpy-1.3.0/src/core/analysis.cpp` & `stormpy-1.8.0/src/core/analysis.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,13 @@
 #include "storm/analysis/GraphConditions.h"
 
 // Define python bindings
 void define_graph_constraints(py::module& m) {
 
     // ConstraintCollector
     py::class_<storm::analysis::ConstraintCollector<storm::RationalFunction>, std::shared_ptr<storm::analysis::ConstraintCollector<storm::RationalFunction>>>(m, "ConstraintCollector", "Collector for constraints on parametric Markov chains")
-            .def("__init__", [](storm::analysis::ConstraintCollector<storm::RationalFunction> &instance, storm::models::sparse::Model<storm::RationalFunction> const& model) -> void {
-                new (&instance) storm::analysis::ConstraintCollector<storm::RationalFunction>(model);
-            }, py::arg("model"))
+            .def(py::init<storm::models::sparse::Model<storm::RationalFunction> const&>(), py::arg("model"))
         .def_property_readonly("wellformed_constraints", &storm::analysis::ConstraintCollector<storm::RationalFunction>::getWellformedConstraints, "Get the constraints ensuring a wellformed model")
         .def_property_readonly("graph_preserving_constraints", &storm::analysis::ConstraintCollector<storm::RationalFunction>::getGraphPreservingConstraints, "Get the constraints ensuring the graph is preserved")
     ;
 
 }
```

### Comparing `stormpy-1.3.0/src/core/bisimulation.cpp` & `stormpy-1.8.0/src/core/bisimulation.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 #include "bisimulation.h"
 #include "storm/models/symbolic/StandardRewardModel.h"
 
 
 template <storm::dd::DdType DdType, typename ValueType>
-std::shared_ptr<storm::models::Model<ValueType>> performBisimulationMinimization(std::shared_ptr<storm::models::symbolic::Model<DdType, ValueType>> const& model, std::vector<std::shared_ptr<storm::logic::Formula const>> const& formulas, storm::storage::BisimulationType const& bisimulationType = storm::storage::BisimulationType::Strong) {
-    return storm::api::performBisimulationMinimization<DdType, ValueType, ValueType>(model, formulas, bisimulationType, storm::dd::bisimulation::SignatureMode::Eager);
+std::shared_ptr<storm::models::Model<ValueType>> performBisimulationMinimization(std::shared_ptr<storm::models::symbolic::Model<DdType, ValueType>> const& model, std::vector<std::shared_ptr<storm::logic::Formula const>> const& formulas, storm::storage::BisimulationType const& bisimulationType, storm::dd::bisimulation::QuotientFormat const& quotientFormat) {
+    return storm::api::performBisimulationMinimization<DdType, ValueType, ValueType>(model, formulas, bisimulationType, storm::dd::bisimulation::SignatureMode::Eager, quotientFormat);
 }
 
 // Define python bindings
 void define_bisimulation(py::module& m) {
 
     // Bisimulation
     m.def("_perform_bisimulation", &storm::api::performBisimulationMinimization<double>, "Perform bisimulation", py::arg("model"), py::arg("formulas"), py::arg("bisimulation_type"));
     m.def("_perform_parametric_bisimulation", &storm::api::performBisimulationMinimization<storm::RationalFunction>, "Perform bisimulation on parametric model", py::arg("model"), py::arg("formulas"), py::arg("bisimulation_type"));
-    m.def("_perform_symbolic_bisimulation", &performBisimulationMinimization<storm::dd::DdType::Sylvan, double>, "Perform bisimulation", py::arg("model"), py::arg("formulas"), py::arg("bisimulation_type"));
-    m.def("_perform_symbolic_parametric_bisimulation", &performBisimulationMinimization<storm::dd::DdType::Sylvan, storm::RationalFunction>, "Perform bisimulation on parametric model", py::arg("model"), py::arg("formulas"), py::arg("bisimulation_type"));
+    m.def("_perform_symbolic_bisimulation", &performBisimulationMinimization<storm::dd::DdType::Sylvan, double>, "Perform bisimulation", py::arg("model"), py::arg("formulas"), py::arg("bisimulation_type"), py::arg("quotient_format"));
+    m.def("_perform_symbolic_parametric_bisimulation", &performBisimulationMinimization<storm::dd::DdType::Sylvan, storm::RationalFunction>, "Perform bisimulation on parametric model", py::arg("model"), py::arg("formulas"), py::arg("bisimulation_type"), py::arg("quotient_format"));
 
     // BisimulationType
     py::enum_<storm::storage::BisimulationType>(m, "BisimulationType", "Types of bisimulation")
         .value("STRONG", storm::storage::BisimulationType::Strong)
         .value("WEAK", storm::storage::BisimulationType::Weak)
     ;
 
+    // QuotientFormat
+    py::enum_<storm::dd::bisimulation::QuotientFormat>(m, "QuotientFormat", "Return format of bisimulation quotient")
+        .value("SPARSE", storm::dd::bisimulation::QuotientFormat::Sparse)
+        .value("DD", storm::dd::bisimulation::QuotientFormat::Dd)
+    ;
+
 }
```

### Comparing `stormpy-1.3.0/src/core/core.cpp` & `stormpy-1.8.0/src/core/core.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,52 @@
+#include <pybind11/functional.h>
+
 #include "core.h"
 #include "storm/utility/initialize.h"
-#include "storm/utility/DirectEncodingExporter.h"
+#include "storm/utility/SignalHandler.h"
+#include "storm/io/DirectEncodingExporter.h"
 #include "storm/storage/ModelFormulasPair.h"
 #include "storm/storage/dd/DdType.h"
 #include "storm/storage/jani/Property.h"
 #include "storm/solver/OptimizationDirection.h"
 #include "storm/models/symbolic/StandardRewardModel.h"
+#include "storm/generator/NextStateGenerator.h"
 #include "storm-parsers/api/storm-parsers.h"
 #include "storm-counterexamples/settings/modules/CounterexampleGeneratorSettings.h"
 
 void define_core(py::module& m) {
     // Init
     m.def("_set_up", [](std::string const& args) {
             storm::utility::setUp();
-            storm::settings::initializeAll("StoRM-Py", "stormpy");
+            storm::settings::initializeAll("stormpy", "stormpy");
             storm::settings::addModule<storm::settings::modules::CounterexampleGeneratorSettings>();
-            storm::settings::SettingsManager::manager().setFromString(args);
+            storm::settings::mutableManager().setFromString(args);
         }, "Initialize Storm", py::arg("arguments"));
-
-    m.def("_set_loglevel_debug", []() {
+    m.def("set_settings", [](std::vector<std::string> const& args) {
+            storm::settings::mutableManager().setFromExplodedString(args);
+        }, "Set settings", py::arg("arguments"));
+    m.def("set_loglevel_debug", []() {
         storm::utility::setLogLevel(l3pp::LogLevel::DEBUG);
     }, "set loglevel for storm to debug");
-    m.def("_set_loglevel_trace", []() {
+    m.def("set_loglevel_trace", []() {
         storm::utility::setLogLevel(l3pp::LogLevel::TRACE);
     });
+    m.def("set_loglevel_error", []() {
+        storm::utility::setLogLevel(l3pp::LogLevel::ERR);
+    });
 
+    m.def("set_timeout", &storm::utility::resources::setTimeoutAlarm, py::arg("timeout"), "Set timeout in seconds");
+    m.def("reset_timeout", &storm::utility::resources::resetTimeoutAlarm, "Reset timeout");
+    m.def("install_signal_handlers", &storm::utility::resources::installSignalHandler);
 
 }
 
 void define_parse(py::module& m) {
     // Parse formulas
-    m.def("parse_properties", [](std::string const& inputString, boost::optional<std::set<std::string>> const& propertyFilter = boost::none) {
+    m.def("parse_properties_without_context", [](std::string const& inputString, boost::optional<std::set<std::string>> const& propertyFilter = boost::none) {
                 return storm::api::parseProperties(inputString, propertyFilter);
             }, R"dox(
           
           Parse properties given in the prism format.
           
           :param str formula_str: A string of formulas
           :param str property_filter: A filter
@@ -61,28 +73,33 @@
                 return pair.formulas;
             }, "The formulas")
     ;
 }
 
 // Thin wrapper for model building using sparse representation
 template<typename ValueType>
-std::shared_ptr<storm::models::sparse::Model<ValueType>> buildSparseModel(storm::storage::SymbolicModelDescription const& modelDescription, std::vector<std::shared_ptr<storm::logic::Formula const>> const& formulas, bool jit = false, bool doctor = false) {
+std::shared_ptr<storm::models::sparse::Model<ValueType>> buildSparseModel(storm::storage::SymbolicModelDescription const& modelDescription, std::vector<std::shared_ptr<storm::logic::Formula const>> const& formulas) {
     if (formulas.empty()) {
         // Build all labels and rewards
         storm::builder::BuilderOptions options(true, true);
-        return storm::api::buildSparseModel<ValueType>(modelDescription, options, jit, doctor);
+        return storm::api::buildSparseModel<ValueType>(modelDescription, options);
     } else {
         // Only build labels necessary for formulas
-        return storm::api::buildSparseModel<ValueType>(modelDescription, formulas, jit, doctor);
+        return storm::api::buildSparseModel<ValueType>(modelDescription, formulas);
     }
 }
 
 template<typename ValueType>
-std::shared_ptr<storm::models::ModelBase> buildSparseModelWithOptions(storm::storage::SymbolicModelDescription const& modelDescription, storm::builder::BuilderOptions const& options, bool jit = false, bool doctor = false) {
-    return storm::api::buildSparseModel<ValueType>(modelDescription, options, jit, doctor);
+std::shared_ptr<storm::models::ModelBase> buildSparseModelWithOptions(storm::storage::SymbolicModelDescription const& modelDescription, storm::builder::BuilderOptions const& options) {
+    return storm::api::buildSparseModel<ValueType>(modelDescription, options);
+}
+
+template<typename ValueType>
+storm::builder::ExplicitModelBuilder<double> makeExplicitModelBuilder(storm::storage::SymbolicModelDescription const& model, storm::builder::BuilderOptions const& options) {
+    return storm::api::makeExplicitModelBuilder<double>(model, options, nullptr); // Do not set ActionMask
 }
 
 // Thin wrapper for model building using symbolic representation
 template<storm::dd::DdType DdType, typename ValueType>
 std::shared_ptr<storm::models::symbolic::Model<DdType, ValueType>> buildSymbolicModel(storm::storage::SymbolicModelDescription const& modelDescription, std::vector<std::shared_ptr<storm::logic::Formula const>> const& formulas) {
     if (formulas.empty()) {
         // Build full model
@@ -90,48 +107,91 @@
     } else {
         // Only build labels necessary for formulas
         return storm::api::buildSymbolicModel<DdType, ValueType>(modelDescription, formulas, false);
     }
 }
 
 void define_build(py::module& m) {
+
+    py::class_<storm::parser::DirectEncodingParserOptions>(m, "DirectEncodingParserOptions", "Options for the .drn parser")
+            .def(py::init<>(), "initialise")
+            .def_readwrite("build_choice_labels", &storm::parser::DirectEncodingParserOptions::buildChoiceLabeling, "Build with choice labels");
+
     // Build model
-    m.def("_build_sparse_model_from_symbolic_description", &buildSparseModel<double>, "Build the model in sparse representation", py::arg("model_description"), py::arg("formulas") = std::vector<std::shared_ptr<storm::logic::Formula const>>(), py::arg("use_jit") = false, py::arg("doctor") = false);
-    m.def("_build_sparse_parametric_model_from_symbolic_description", &buildSparseModel<storm::RationalFunction>, "Build the parametric model in sparse representation", py::arg("model_description"), py::arg("formulas") = std::vector<std::shared_ptr<storm::logic::Formula const>>(), py::arg("use_jit") = false, py::arg("doctor") = false);
-    m.def("build_sparse_model_with_options", &buildSparseModelWithOptions<double>, "Build the model in sparse representation", py::arg("model_description"), py::arg("options"), py::arg("use_jit") = false, py::arg("doctor") = false);
+    m.def("_build_sparse_model_from_symbolic_description", &buildSparseModel<double>, "Build the model in sparse representation", py::arg("model_description"), py::arg("formulas") = std::vector<std::shared_ptr<storm::logic::Formula const>>());
+    m.def("_build_sparse_exact_model_from_symbolic_description", &buildSparseModel<storm::RationalNumber>, "Build the model in sparse representation with exact number representation", py::arg("model_description"), py::arg("formulas") = std::vector<std::shared_ptr<storm::logic::Formula const>>());
+    m.def("_build_sparse_parametric_model_from_symbolic_description", &buildSparseModel<storm::RationalFunction>, "Build the parametric model in sparse representation", py::arg("model_description"), py::arg("formulas") = std::vector<std::shared_ptr<storm::logic::Formula const>>());
+    m.def("build_sparse_model_with_options", &buildSparseModelWithOptions<double>, "Build the model in sparse representation", py::arg("model_description"), py::arg("options"));
+    m.def("build_sparse_exact_model_with_options", &buildSparseModelWithOptions<storm::RationalNumber>, "Build the model in sparse representation with exact number representation", py::arg("model_description"), py::arg("options"));
+    m.def("build_sparse_parametric_model_with_options", &buildSparseModelWithOptions<storm::RationalFunction>, "Build the model in sparse representation", py::arg("model_description"), py::arg("options"));
     m.def("_build_symbolic_model_from_symbolic_description", &buildSymbolicModel<storm::dd::DdType::Sylvan, double>, "Build the model in symbolic representation", py::arg("model_description"), py::arg("formulas") = std::vector<std::shared_ptr<storm::logic::Formula const>>());
     m.def("_build_symbolic_parametric_model_from_symbolic_description", &buildSymbolicModel<storm::dd::DdType::Sylvan, storm::RationalFunction>, "Build the parametric model in symbolic representation", py::arg("model_description"), py::arg("formulas") = std::vector<std::shared_ptr<storm::logic::Formula const>>());
-    m.def("_build_sparse_model_from_drn", &storm::api::buildExplicitDRNModel<double>, "Build the model from DRN", py::arg("file"));
-    m.def("_build_sparse_parametric_model_from_drn", &storm::api::buildExplicitDRNModel<storm::RationalFunction>, "Build the parametric model from DRN", py::arg("file"));
+    m.def("_build_sparse_model_from_drn", &storm::api::buildExplicitDRNModel<double>, "Build the model from DRN", py::arg("file"), py::arg("options") = storm::parser::DirectEncodingParserOptions());
+    m.def("_build_sparse_exact_model_from_drn", &storm::api::buildExplicitDRNModel<storm::RationalNumber>, "Build the model from DRN", py::arg("file"), py::arg("options") = storm::parser::DirectEncodingParserOptions());
+    m.def("_build_sparse_parametric_model_from_drn", &storm::api::buildExplicitDRNModel<storm::RationalFunction>, "Build the parametric model from DRN", py::arg("file"), py::arg("options") = storm::parser::DirectEncodingParserOptions());
     m.def("build_sparse_model_from_explicit", &storm::api::buildExplicitModel<double>, "Build the model model from explicit input", py::arg("transition_file"), py::arg("labeling_file"), py::arg("state_reward_file") = "", py::arg("transition_reward_file") = "", py::arg("choice_labeling_file") = "");
 
+    m.def("make_sparse_model_builder", &storm::api::makeExplicitModelBuilder<double>, "Construct a builder instance", py::arg("model_description"), py::arg("options"), py::arg("action_mask") = nullptr);
+    m.def("make_sparse_model_builder_exact", &storm::api::makeExplicitModelBuilder<storm::RationalNumber>, "Construct a builder instance", py::arg("model_description"), py::arg("options"), py::arg("action_mask") = nullptr);
+    m.def("make_sparse_model_builder_parametric", &storm::api::makeExplicitModelBuilder<storm::RationalFunction>, "Construct a builder instance", py::arg("model_description"), py::arg("options"), py::arg("action_mask") = nullptr);
+
+    py::class_<storm::builder::ExplicitModelBuilder<double>>(m, "ExplicitModelBuilder", "Model builder for sparse models")
+        .def("build", &storm::builder::ExplicitModelBuilder<double>::build, "Build the model",  py::call_guard<py::gil_scoped_release>())
+        .def("export_lookup", &storm::builder::ExplicitModelBuilder<double>::exportExplicitStateLookup, "Export a lookup model")
+    ;
+
+    py::class_<storm::builder::ExplicitModelBuilder<storm::RationalFunction>>(m, "ExplicitParametricModelBuilder", "Model builder for sparse models")
+        .def("build", &storm::builder::ExplicitModelBuilder<storm::RationalFunction>::build, "Build the model", py::call_guard<py::gil_scoped_release>())
+        .def("export_lookup", &storm::builder::ExplicitModelBuilder<storm::RationalFunction>::exportExplicitStateLookup, "Export a lookup model")
+    ;
+
+    py::class_<storm::builder::ExplicitStateLookup<uint32_t>>(m, "ExplicitStateLookup", "Lookup model for states")
+        .def("lookup", [](storm::builder::ExplicitStateLookup<uint32_t>const& lookup, std::map<storm::expressions::Variable, storm::expressions::Expression> const& stateDescription) -> py::object
+        { auto res = lookup.lookup(stateDescription); if (res==lookup.size()) {return py::none();} else {return py::cast(res);}} , py::arg("state_description"))
+
+    ;
 
     py::class_<storm::builder::BuilderOptions>(m, "BuilderOptions", "Options for building process")
             .def(py::init<std::vector<std::shared_ptr<storm::logic::Formula const>> const&>(), "Initialise with formulae to preserve", py::arg("formulae"))
-            .def(py::init<bool, bool>(), "Initialise without formulae", py::arg("build_all_reward_models"), py::arg("build_all_labels"))
+            .def(py::init<bool, bool>(), "Initialise without formulae", py::arg("build_all_reward_models")=true, py::arg("build_all_labels")=true)
             .def_property_readonly("preserved_label_names", &storm::builder::BuilderOptions::getLabelNames, "Labels preserved")
+            .def("set_build_state_valuations", &storm::builder::BuilderOptions::setBuildStateValuations, "Build state valuations", py::arg("new_value")=true)
+            .def("set_build_observation_valuations", &storm::builder::BuilderOptions::setBuildObservationValuations, "Build observation valuations", py::arg("new_value")=true)
             .def("set_build_with_choice_origins", &storm::builder::BuilderOptions::setBuildChoiceOrigins, "Build choice origins", py::arg("new_value")=true)
             .def("set_add_out_of_bounds_state", &storm::builder::BuilderOptions::setAddOutOfBoundsState, "Build with out of bounds state", py::arg("new_value")=true)
-            .def("set_add_overlapping_guards_label", &storm::builder::BuilderOptions::setAddOverlappingGuardsLabel, "Build with overlapping guards state labeled", py::arg("new_value")=true);
+            .def("set_add_overlapping_guards_label", &storm::builder::BuilderOptions::setAddOverlappingGuardsLabel, "Build with overlapping guards state labeled", py::arg("new_value")=true)
+            .def("set_build_choice_labels", &storm::builder::BuilderOptions::setBuildChoiceLabels, "Build with choice labels", py::arg("new_value")=true)
+            .def("set_build_all_labels" , &storm::builder::BuilderOptions::setBuildAllLabels, "Build with all state labels", py::arg("new_value")=true)
+            .def("set_build_all_reward_models", &storm::builder::BuilderOptions::setBuildAllRewardModels, "Build with all reward models", py::arg("new_value")=true);
+
+    py::class_<storm::generator::ActionMask<double>, std::shared_ptr<storm::generator::ActionMask<double>>> actionmask(m, "ActionMaskDouble");
+    py::class_<storm::generator::StateValuationFunctionMask<double>, std::shared_ptr<storm::generator::StateValuationFunctionMask<double>>> actfuncmask(m, "StateValuationFunctionActionMaskDouble", actionmask);
+    actfuncmask.def(py::init<std::function<bool (storm::expressions::SimpleValuation const&, uint64_t)>>(), py::arg("f"));
 }
 
 void define_optimality_type(py::module& m) {
     py::enum_<storm::solver::OptimizationDirection>(m, "OptimizationDirection")
         .value("Minimize", storm::solver::OptimizationDirection::Minimize)
         .value("Maximize", storm::solver::OptimizationDirection::Maximize)
     ;
 }
 
 // Thin wrapper for exporting model
 template<typename ValueType>
-void exportDRN(std::shared_ptr<storm::models::sparse::Model<ValueType>> model, std::string const& file) {
+void exportDRN(std::shared_ptr<storm::models::sparse::Model<ValueType>> model, std::string const& file, storm::exporter::DirectEncodingOptions options) {
     std::ofstream stream;
     storm::utility::openFile(file, stream);
-    storm::exporter::explicitExportSparseModel(stream, model, {});
+    storm::exporter::explicitExportSparseModel(stream, model, {}, options);
     storm::utility::closeFile(stream);
 }
 
 void define_export(py::module& m) {
+
+    py::class_<storm::exporter::DirectEncodingOptions> opts(m, "DirectEncodingOptions");
+    opts.def(py::init<>());
+    opts.def_readwrite("allow_placeholders", &storm::exporter::DirectEncodingOptions::allowPlaceholders);
     // Export
-    m.def("export_to_drn", &exportDRN<double>, "Export model in DRN format", py::arg("model"), py::arg("file"));
-    m.def("export_parametric_to_drn", &exportDRN<storm::RationalFunction>, "Export parametric model in DRN format", py::arg("model"), py::arg("file"));
+    // TODO make one export_to_drn that infers which of the folliwng to use.
+    m.def("_export_to_drn", &exportDRN<double>, "Export model in DRN format", py::arg("model"), py::arg("file"), py::arg("options")=storm::exporter::DirectEncodingOptions());
+    m.def("_export_exact_to_drn", &exportDRN<storm::RationalNumber>, "Export model in DRN format", py::arg("model"), py::arg("file"), py::arg("options")=storm::exporter::DirectEncodingOptions());
+    m.def("_export_parametric_to_drn", &exportDRN<storm::RationalFunction>, "Export parametric model in DRN format", py::arg("model"), py::arg("file"), py::arg("options")=storm::exporter::DirectEncodingOptions());
 }
```

### Comparing `stormpy-1.3.0/src/core/counterexample.cpp` & `stormpy-1.8.0/src/core/counterexample.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-#include <algorithm>
 
 #include "counterexample.h"
 #include "storm/environment/Environment.h"
 #include "storm-counterexamples/api/counterexamples.h"
 
 
 using namespace storm::counterexamples;
 
 // Define python bindings
 void define_counterexamples(py::module& m) {
 
+    using FlatSet = boost::container::flat_set<uint64_t, std::less<uint64_t>, boost::container::new_allocator<uint64_t>>;
 
-    py::class_<boost::container::flat_set<uint_fast64_t>>(m, "FlatSet", "Container to pass to program")
+    py::class_<FlatSet>(m, "FlatSet", "Container to pass to program")
             .def(py::init<>())
-            .def(py::init<boost::container::flat_set<uint64_t>>(), "other"_a)
-            .def("insert", [](boost::container::flat_set<uint_fast64_t>& flatset, uint64_t value) {flatset.insert(value);})
-            .def("is_subset_of", [](boost::container::flat_set<uint64_t> const& left, boost::container::flat_set<uint64_t> const& right) {return std::includes(right.begin(), right.end(), left.begin(), left.end()); })
-            .def("insert_set", [](boost::container::flat_set<uint64_t>& left, boost::container::flat_set<uint64_t> const& additional) { for(auto const& i : additional) {left.insert(i);}})
-            .def("__str__", [](boost::container::flat_set<uint64_t> const& set) { std::stringstream str; str << "["; for(auto const& i : set) { str << i << ", ";} str << "]"; return str.str(); })
-            .def("__len__", [](boost::container::flat_set<uint64_t> const& set) { return set.size();})
-            .def("__iter__", [](boost::container::flat_set<uint_fast64_t> &v) {
+            .def(py::init<FlatSet>(), "other"_a)
+            .def("insert", [](FlatSet& flatset, uint64_t value) {flatset.insert(value);})
+            .def("is_subset_of", [](FlatSet const& left, FlatSet const& right) {return std::includes(right.begin(), right.end(), left.begin(), left.end()); })
+            .def("insert_set", [](FlatSet& left, FlatSet const& additional) { for(auto const& i : additional) {left.insert(i);}})
+            .def("__str__", [](FlatSet const& set) { std::stringstream str; str << "["; for(auto const& i : set) { str << i << ", ";} str << "]"; return str.str(); })
+            .def("__len__", [](FlatSet const& set) { return set.size();})
+            .def("__iter__", [](FlatSet &v) {
                 return py::make_iterator(v.begin(), v.end());
             }, py::keep_alive<0, 1>()) /* Keep vector alive while iterator is used */
             ;
 
     using CexGeneratorStats = SMTMinimalLabelSetGenerator<double>::GeneratorStats;
 
     py::class_<CexGeneratorStats>(m, "SMTCounterExampleGeneratorStats", "Stats for highlevel counterexample generation")
```

### Comparing `stormpy-1.3.0/src/core/result.cpp` & `stormpy-1.8.0/src/core/result.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 #include "result.h"
 #include "storm/analysis/GraphConditions.h"
 #include "storm/modelchecker/results/SymbolicQualitativeCheckResult.h"
 #include "storm/modelchecker/results/SymbolicQuantitativeCheckResult.h"
 #include "storm/modelchecker/results/HybridQuantitativeCheckResult.h"
 #include "storm/modelchecker/results/ExplicitQuantitativeCheckResult.h"
 #include "storm/modelchecker/results/ExplicitQualitativeCheckResult.h"
+#include "storm/modelchecker/results/ExplicitParetoCurveCheckResult.h"
 
 #include "storm/models/symbolic/StandardRewardModel.h"
 
 template<typename ValueType>
 std::shared_ptr<storm::modelchecker::QualitativeCheckResult> createFilterInitialStatesSparse(std::shared_ptr<storm::models::sparse::Model<ValueType>> model) {
     return std::make_unique<storm::modelchecker::ExplicitQualitativeCheckResult>(model->getInitialStates());
 }
 
 template<storm::dd::DdType DdType, typename ValueType>
 std::shared_ptr<storm::modelchecker::QualitativeCheckResult> createFilterInitialStatesSymbolic(std::shared_ptr<storm::models::symbolic::Model<DdType, ValueType>> model) {
    return std::make_unique<storm::modelchecker::SymbolicQualitativeCheckResult<DdType>>(model->getReachableStates(), model->getInitialStates());
 }
 
+template<storm::dd::DdType DdType, typename ValueType>
+std::shared_ptr<storm::modelchecker::QualitativeCheckResult> createFilterSymbolic(std::shared_ptr<storm::models::symbolic::Model<DdType, ValueType>> model, storm::expressions::Expression const& expr) {
+    return std::make_unique<storm::modelchecker::SymbolicQualitativeCheckResult<DdType>>(model->getReachableStates(), model->getStates(expr));
+}
 
 // Define python bindings
 void define_result(py::module& m) {
 
     // CheckResult
     py::class_<storm::modelchecker::CheckResult, std::shared_ptr<storm::modelchecker::CheckResult>> checkResult(m, "_CheckResult", "Base class for all modelchecking results");
     checkResult.def_property_readonly("_symbolic", &storm::modelchecker::CheckResult::isSymbolic, "Flag if result is symbolic")
@@ -39,14 +44,17 @@
 
         .def("as_explicit_qualitative", [](storm::modelchecker::CheckResult const& result) {
                 return result.asExplicitQualitativeCheckResult();
             }, "Convert into explicit qualitative result")
         .def("as_explicit_quantitative", [](storm::modelchecker::CheckResult const& result) {
                 return result.asExplicitQuantitativeCheckResult<double>();
             }, "Convert into explicit quantitative result")
+        .def("as_explicit_exact_quantitative", [](storm::modelchecker::CheckResult const& result) {
+                return result.asExplicitQuantitativeCheckResult<storm::RationalNumber>();
+            }, "Convert into explicit quantitative result")
         .def("as_explicit_parametric_quantitative", [](storm::modelchecker::CheckResult const& result) {
                 return result.asExplicitQuantitativeCheckResult<storm::RationalFunction>();
             }, "Convert into explicit quantitative result")
         .def("filter", &storm::modelchecker::CheckResult::filter, py::arg("filter"), "Filter the result")
         .def("__str__",  [](storm::modelchecker::CheckResult const& result) {
                 std::stringstream stream;
                 result.writeToStream(stream);
@@ -59,47 +67,76 @@
     py::class_<storm::modelchecker::ExplicitQualitativeCheckResult, std::shared_ptr<storm::modelchecker::ExplicitQualitativeCheckResult>>(m, "ExplicitQualitativeCheckResult", "Explicit qualitative model checking result", qualitativeCheckResult)
         .def("at", [](storm::modelchecker::ExplicitQualitativeCheckResult const& result, storm::storage::sparse::state_type state) {
                 return result[state];
             }, py::arg("state"), "Get result for given state")
         .def("get_truth_values", &storm::modelchecker::ExplicitQualitativeCheckResult::getTruthValuesVector, "Get BitVector representing the truth values")
     ;
     py::class_<storm::modelchecker::SymbolicQualitativeCheckResult<storm::dd::DdType::Sylvan>, std::shared_ptr<storm::modelchecker::SymbolicQualitativeCheckResult<storm::dd::DdType::Sylvan>>>(m, "SymbolicQualitativeCheckResult", "Symbolic qualitative model checking result", qualitativeCheckResult)
+            .def("get_truth_values", &storm::modelchecker::SymbolicQualitativeCheckResult<storm::dd::DdType::Sylvan>::getTruthValuesVector, "Get Dd representing the truth values")
     ;
 
     // QuantitativeCheckResult
     py::class_<storm::modelchecker::QuantitativeCheckResult<double>, std::shared_ptr<storm::modelchecker::QuantitativeCheckResult<double>>> quantitativeCheckResult(m, "_QuantitativeCheckResult", "Abstract class for quantitative model checking results", checkResult);
     quantitativeCheckResult.def_property_readonly("min", &storm::modelchecker::QuantitativeCheckResult<double>::getMin, "Minimal value")
         .def_property_readonly("max", &storm::modelchecker::QuantitativeCheckResult<double>::getMax, "Maximal value")
     ;
 
     py::class_<storm::modelchecker::ExplicitQuantitativeCheckResult<double>, std::shared_ptr<storm::modelchecker::ExplicitQuantitativeCheckResult<double>>>(m, "ExplicitQuantitativeCheckResult", "Explicit quantitative model checking result", quantitativeCheckResult)
+        .def(py::init<std::vector<double>>(), py::arg("values"))
         .def("at", [](storm::modelchecker::ExplicitQuantitativeCheckResult<double> const& result, storm::storage::sparse::state_type state) {
             return result[state];
         }, py::arg("state"), "Get result for given state")
         .def("get_values", [](storm::modelchecker::ExplicitQuantitativeCheckResult<double> const& res) {return res.getValueVector();}, "Get model checking result values for all states")
         .def_property_readonly("scheduler", [](storm::modelchecker::ExplicitQuantitativeCheckResult<double> const& res) {return res.getScheduler();}, "get scheduler")
     ;
     py::class_<storm::modelchecker::SymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, double>, std::shared_ptr<storm::modelchecker::SymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, double>>>(m, "SymbolicQuantitativeCheckResult", "Symbolic quantitative model checking result", quantitativeCheckResult)
-    ;
+            .def("clone", [](storm::modelchecker::SymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, double> const& dd)  {return dd.clone()->asSymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, double>(); })
+            ;
     py::class_<storm::modelchecker::HybridQuantitativeCheckResult<storm::dd::DdType::Sylvan, double>, std::shared_ptr<storm::modelchecker::HybridQuantitativeCheckResult<storm::dd::DdType::Sylvan, double>>>(m, "HybridQuantitativeCheckResult", "Hybrid quantitative model checking result", quantitativeCheckResult)
         .def("get_values", &storm::modelchecker::HybridQuantitativeCheckResult<storm::dd::DdType::Sylvan, double>::getExplicitValueVector, "Get model checking result values for all states")
     ;
 
+    py::class_<storm::modelchecker::QuantitativeCheckResult<storm::RationalNumber>, std::shared_ptr<storm::modelchecker::QuantitativeCheckResult<storm::RationalNumber>>> exactQuantitativeCheckResult(m, "_ExactQuantitativeCheckResult", "Abstract class for exact quantitative model checking results", checkResult);
+    py::class_<storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalNumber>, std::shared_ptr<storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalNumber>>>(m, "ExplicitExactQuantitativeCheckResult", "Explicit exact quantitative model checking result", exactQuantitativeCheckResult)
+        .def(py::init<std::vector<storm::RationalNumber>>(), py::arg("values"))
+        .def("at", [](storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalNumber> const& result, storm::storage::sparse::state_type state) {
+            return result[state];
+        }, py::arg("state"), "Get result for given state")
+        .def("get_values", [](storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalNumber> const& res) { return res.getValueVector();}, "Get model checking result values for all states")
+        .def_property_readonly("scheduler", [](storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalNumber> const& res) {return res.getScheduler();}, "get scheduler")
+    ;
+    py::class_<storm::modelchecker::SymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalNumber>, std::shared_ptr<storm::modelchecker::SymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalNumber>>>(m, "SymbolicExactQuantitativeCheckResult", "Symbolic exact quantitative model checking result", quantitativeCheckResult)
+       .def("clone", [](storm::modelchecker::SymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalNumber> const& dd)  {return dd.clone()->asSymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalNumber>(); })
+   ;
+    py::class_<storm::modelchecker::HybridQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalNumber>, std::shared_ptr<storm::modelchecker::HybridQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalNumber>>>(m, "HybridExactQuantitativeCheckResult", "Symbolic exact hybrid quantitative model checking result", quantitativeCheckResult)
+        .def("get_values", &storm::modelchecker::HybridQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalNumber>::getExplicitValueVector, "Get model checking result values for all states")
+    ;
+
     py::class_<storm::modelchecker::QuantitativeCheckResult<storm::RationalFunction>, std::shared_ptr<storm::modelchecker::QuantitativeCheckResult<storm::RationalFunction>>> parametricQuantitativeCheckResult(m, "_ParametricQuantitativeCheckResult", "Abstract class for parametric quantitative model checking results", checkResult);
     py::class_<storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalFunction>, std::shared_ptr<storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalFunction>>>(m, "ExplicitParametricQuantitativeCheckResult", "Explicit parametric quantitative model checking result", parametricQuantitativeCheckResult)
         .def("at", [](storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalFunction> const& result, storm::storage::sparse::state_type state) {
             return result[state];
         }, py::arg("state"), "Get result for given state")
         .def("get_values", [](storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalFunction> const& res) { return res.getValueVector();}, "Get model checking result values for all states")
+        .def_property_readonly("scheduler", [](storm::modelchecker::ExplicitQuantitativeCheckResult<storm::RationalFunction> const& res) {return res.getScheduler();}, "get scheduler")
     ;
     py::class_<storm::modelchecker::SymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalFunction>, std::shared_ptr<storm::modelchecker::SymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalFunction>>>(m, "SymbolicParametricQuantitativeCheckResult", "Symbolic parametric quantitative model checking result", quantitativeCheckResult)
+         .def("clone", [](storm::modelchecker::SymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalFunction> const& dd)  {return dd.clone()->asSymbolicQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalFunction>(); })
     ;
     py::class_<storm::modelchecker::HybridQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalFunction>, std::shared_ptr<storm::modelchecker::HybridQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalFunction>>>(m, "HybridParametricQuantitativeCheckResult", "Symbolic parametric hybrid quantitative model checking result", quantitativeCheckResult)
         .def("get_values", &storm::modelchecker::HybridQuantitativeCheckResult<storm::dd::DdType::Sylvan, storm::RationalFunction>::getExplicitValueVector, "Get model checking result values for all states")
     ;
 
+    py::class_<storm::modelchecker::ParetoCurveCheckResult<double>, std::shared_ptr<storm::modelchecker::ParetoCurveCheckResult<double>>> pccheckresult(m, "ParetoCurveCheckResultDouble", "Result for multiobjective model checking", checkResult);
+    pccheckresult.def("get_underapproximation", &storm::modelchecker::ParetoCurveCheckResult<double>::getUnderApproximation);
+    pccheckresult.def("get_overapproximation", &storm::modelchecker::ParetoCurveCheckResult<double>::getOverApproximation);
 
+    py::class_<storm::modelchecker::ExplicitParetoCurveCheckResult<double>, std::shared_ptr<storm::modelchecker::ExplicitParetoCurveCheckResult<double>>> epccheckresult(m, "ExplicitParetoCurveCheckResultDouble", "Result for explicit multiobjective model checking", pccheckresult);
+
+
+    m.def("create_filter_symbolic", &createFilterSymbolic<storm::dd::DdType::Sylvan, double>, "Creates a filter for the given states and a symbolic model", py::arg("model"), py::arg("states"));
     m.def("create_filter_initial_states_sparse", &createFilterInitialStatesSparse<double>, "Create a filter for the initial states on a sparse model", py::arg("model"));
     m.def("create_filter_initial_states_symbolic", &createFilterInitialStatesSymbolic<storm::dd::DdType::Sylvan, double>, "Create a filter for the initial states on a symbolic model", py::arg("model"));
 
+
 }
```

### Comparing `stormpy-1.3.0/src/helpers.h` & `stormpy-1.8.0/src/helpers.h`

 * *Files identical despite different names*

### Comparing `stormpy-1.3.0/src/logic/formulae.cpp` & `stormpy-1.8.0/src/logic/formulae.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,74 @@
 #include "formulae.h"
 #include "storm/logic/Formulas.h"
 #include "storm/logic/CloneVisitor.h"
 #include "storm/logic/LabelSubstitutionVisitor.h"
-
+#include "storm/storage/expressions/Variable.h"
 
 
 void define_formulae(py::module& m) {
- 
+
     py::enum_<storm::logic::ComparisonType>(m, "ComparisonType")
         .value("LESS", storm::logic::ComparisonType::Less)
         .value("LEQ", storm::logic::ComparisonType::LessEqual)
         .value("GREATER", storm::logic::ComparisonType::Greater)
         .value("GEQ", storm::logic::ComparisonType::GreaterEqual)
     ;
 
+
+    py::enum_<storm::logic::BinaryBooleanOperatorType>(m, "BinaryBooleanOperatorType")
+            .value("AND", storm::logic::BinaryBooleanOperatorType::And)
+            .value("OR", storm::logic::BinaryBooleanOperatorType::Or);
+
+
     py::class_<storm::logic::Formula, std::shared_ptr<storm::logic::Formula>> formula(m, "Formula", "Generic Storm Formula");
     formula.def("__str__", &storm::logic::Formula::toString)
         .def("clone", [](storm::logic::Formula const& f) { storm::logic::CloneVisitor cv; return cv.clone(f);})
         .def("substitute", [](storm::logic::Formula const& f, std::map<storm::expressions::Variable, storm::expressions::Expression> const& map) { return f.substitute(map); }, "Substitute variables", py::arg("constants_map"))
         .def("substitute_labels_by_labels", [](storm::logic::Formula const& f, std::map<std::string, std::string> const& labelSubs) {storm::logic::LabelSubstitutionVisitor lsv(labelSubs); return lsv.substitute(f);}, "substitute label occurences", py::arg("replacements"))
         .def_property_readonly("is_probability_operator", &storm::logic::Formula::isProbabilityOperatorFormula, "is it a probability operator")
         .def_property_readonly("is_reward_operator", &storm::logic::Formula::isRewardOperatorFormula, "is it a reward operator")
-
+        .def_property_readonly("is_eventually_formula", &storm::logic::Formula::isEventuallyFormula)
+        .def_property_readonly("is_bounded_until_formula", &storm::logic::Formula::isBoundedUntilFormula)
+        .def_property_readonly("is_until_formula", &storm::logic::Formula::isUntilFormula)
+        .def_property_readonly("is_multi_objective_formula", &storm::logic::Formula::isMultiObjectiveFormula)
             ;
 
     // Path Formulae
     py::class_<storm::logic::PathFormula, std::shared_ptr<storm::logic::PathFormula>> pathFormula(m, "PathFormula", "Formula about the probability of a set of paths in an automaton", formula);
     py::class_<storm::logic::UnaryPathFormula, std::shared_ptr<storm::logic::UnaryPathFormula>> unaryPathFormula(m, "UnaryPathFormula", "Path formula with one operand", pathFormula);
     unaryPathFormula.def_property_readonly("subformula", &storm::logic::UnaryPathFormula::getSubformula, "the subformula");
     py::class_<storm::logic::EventuallyFormula, std::shared_ptr<storm::logic::EventuallyFormula>>(m, "EventuallyFormula", "Formula for eventually", unaryPathFormula);
     py::class_<storm::logic::GloballyFormula, std::shared_ptr<storm::logic::GloballyFormula>>(m, "GloballyFormula", "Formula for globally", unaryPathFormula);
     py::class_<storm::logic::BinaryPathFormula, std::shared_ptr<storm::logic::BinaryPathFormula>> binaryPathFormula(m, "BinaryPathFormula", "Path formula with two operands", pathFormula);
     binaryPathFormula.def_property_readonly("left_subformula", &storm::logic::BinaryPathFormula::getLeftSubformula);
     binaryPathFormula.def_property_readonly("right_subformula", &storm::logic::BinaryPathFormula::getRightSubformula);
-    py::class_<storm::logic::BoundedUntilFormula, std::shared_ptr<storm::logic::BoundedUntilFormula>>(m, "BoundedUntilFormula", "Until Formula with either a step or a time bound.", binaryPathFormula);
+    py::class_<storm::logic::BoundedUntilFormula, std::shared_ptr<storm::logic::BoundedUntilFormula>>(m, "BoundedUntilFormula", "Until Formula with either a step or a time bound.", binaryPathFormula)
+    .def_property_readonly("is_multidimensional", &storm::logic::BoundedUntilFormula::isMultiDimensional, "Is the bound multi-dimensional")
+    .def_property_readonly("has_lower_bound", [](storm::logic::BoundedUntilFormula const& form) { return form.hasLowerBound(); })
+    .def_property_readonly("upper_bound_expression", [](storm::logic::BoundedUntilFormula const& form) { return form.getUpperBound(); } )
+    .def_property_readonly("left_subformula", [](storm::logic::BoundedUntilFormula const& form) -> storm::logic::Formula const& { return form.getLeftSubformula(); }, py::return_value_policy::reference_internal)
+    .def_property_readonly("right_subformula", [](storm::logic::BoundedUntilFormula const& form)-> storm::logic::Formula const& { return form.getRightSubformula(); }, py::return_value_policy::reference_internal);
     py::class_<storm::logic::ConditionalFormula, std::shared_ptr<storm::logic::ConditionalFormula>>(m, "ConditionalFormula", "Formula with the right hand side being a condition.", formula);
     py::class_<storm::logic::UntilFormula, std::shared_ptr<storm::logic::UntilFormula>>(m, "UntilFormula", "Path Formula for unbounded until", binaryPathFormula);
 
     // Reward Path Formulae
     //py::class_<storm::logic::RewardPathFormula, std::shared_ptr<storm::logic::RewardPathFormula>(m, "RewardPathFormula", "Formula about the rewards of a set of paths in an automaton", py::base<storm::logic::Formula>());
     py::class_<storm::logic::CumulativeRewardFormula, std::shared_ptr<storm::logic::CumulativeRewardFormula>>(m, "CumulativeRewardFormula", "Summed rewards over a the paths", pathFormula);
     py::class_<storm::logic::InstantaneousRewardFormula, std::shared_ptr<storm::logic::InstantaneousRewardFormula>>(m ,"InstantaneousRewardFormula", "Instantaneous reward", pathFormula);
     py::class_<storm::logic::LongRunAverageRewardFormula, std::shared_ptr<storm::logic::LongRunAverageRewardFormula>>(m, "LongRunAverageRewardFormula", "Long run average reward", pathFormula);
     //py::class_<storm::logic::ReachabilityRewardFormula, std::shared_ptr<storm::logic::ReachabilityRewardFormula>>(m, "ReachabilityRewardFormula", "Reachability reward", py::base<storm::logic::RewardPathFormula>());
 
 
     // State Formulae
     py::class_<storm::logic::StateFormula, std::shared_ptr<storm::logic::StateFormula>> stateFormula(m, "StateFormula", "Formula about a state of an automaton", formula);
-    py::class_<storm::logic::AtomicExpressionFormula, std::shared_ptr<storm::logic::AtomicExpressionFormula>>(m, "AtomicExpressionFormula", "Formula with an atomic expression", stateFormula);
-    py::class_<storm::logic::AtomicLabelFormula, std::shared_ptr<storm::logic::AtomicLabelFormula>>(m, "AtomicLabelFormula", "Formula with an atomic label", stateFormula);
+    py::class_<storm::logic::AtomicExpressionFormula, std::shared_ptr<storm::logic::AtomicExpressionFormula>>(m, "AtomicExpressionFormula", "Formula with an atomic expression", stateFormula)
+        .def("get_expression", &storm::logic::AtomicExpressionFormula::getExpression);
+    py::class_<storm::logic::AtomicLabelFormula, std::shared_ptr<storm::logic::AtomicLabelFormula>>(m, "AtomicLabelFormula", "Formula with an atomic label", stateFormula)
+        .def_property_readonly("label", &storm::logic::AtomicLabelFormula::getLabel, "label in the formula");
     py::class_<storm::logic::BooleanLiteralFormula, std::shared_ptr<storm::logic::BooleanLiteralFormula>>(m, "BooleanLiteralFormula", "Formula with a boolean literal", stateFormula)
             .def(py::init<bool>(),"truth value"_a);
     py::class_<storm::logic::UnaryStateFormula, std::shared_ptr<storm::logic::UnaryStateFormula>> unaryStateFormula(m, "UnaryStateFormula", "State formula with one operand", stateFormula);
     unaryStateFormula.def_property_readonly("subformula", &storm::logic::UnaryStateFormula::getSubformula, "the subformula");
     py::class_<storm::logic::UnaryBooleanStateFormula, std::shared_ptr<storm::logic::UnaryBooleanStateFormula>>(m, "UnaryBooleanStateFormula", "Unary boolean state formula", unaryStateFormula);
     py::class_<storm::logic::OperatorFormula, std::shared_ptr<storm::logic::OperatorFormula>> operatorFormula(m, "OperatorFormula", "Operator formula", unaryStateFormula);
     operatorFormula.def_property_readonly("has_bound", &storm::logic::OperatorFormula::hasBound, "Flag if formula is bounded")
@@ -83,13 +99,18 @@
 
             ;
     py::class_<storm::logic::TimeOperatorFormula, std::shared_ptr<storm::logic::TimeOperatorFormula>>(m, "TimeOperator", "The time operator", operatorFormula);
     py::class_<storm::logic::LongRunAverageOperatorFormula, std::shared_ptr<storm::logic::LongRunAverageOperatorFormula>>(m, "LongRunAvarageOperator", "Long run average operator", operatorFormula);
     py::class_<storm::logic::ProbabilityOperatorFormula, std::shared_ptr<storm::logic::ProbabilityOperatorFormula>>(m, "ProbabilityOperator", "Probability operator", operatorFormula)
             .def(py::init<std::shared_ptr<storm::logic::Formula>>(), "construct probability operator formula", py::arg("subformula"))
     ;
+
     py::class_<storm::logic::RewardOperatorFormula, std::shared_ptr<storm::logic::RewardOperatorFormula>>(m, "RewardOperator", "Reward operator", operatorFormula)
             .def("has_reward_name", &storm::logic::RewardOperatorFormula::hasRewardModelName)
             .def_property_readonly("reward_name", &storm::logic::RewardOperatorFormula::getRewardModelName);
     py::class_<storm::logic::BinaryStateFormula, std::shared_ptr<storm::logic::BinaryStateFormula>> binaryStateFormula(m, "BinaryStateFormula", "State formula with two operands", stateFormula);
     py::class_<storm::logic::BinaryBooleanStateFormula, std::shared_ptr<storm::logic::BinaryBooleanStateFormula>>(m, "BooleanBinaryStateFormula", "Boolean binary state formula", binaryStateFormula);
+
+    py::class_<storm::logic::MultiObjectiveFormula, std::shared_ptr<storm::logic::MultiObjectiveFormula>>(m, "MultiObjectiveFormula", "Multi objective formula", formula)
+            .def_property_readonly("subformulas", &storm::logic::MultiObjectiveFormula::getSubformulas, "Get vector of subformulas")
+            .def_property_readonly("nr_subformulas", &storm::logic::MultiObjectiveFormula::getNumberOfSubformulas, "Get number of subformulas");
 }
```

### Comparing `stormpy-1.3.0/src/mod_info.cpp` & `stormpy-1.8.0/src/mod_info.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 #include "common.h"
-#include "storm/utility/storm-version.h"
+#include "storm-version-info/storm-version.h"
 
 PYBIND11_MODULE(info, m) {
     m.doc() = "Storm information";
 
-    py::class_<storm::utility::StormVersion>(m, "Version", "Version information for Storm")
+#ifdef STORMPY_DISABLE_SIGNATURE_DOC
+    py::options options;
+    options.disable_function_signatures();
+#endif
+
+    py::class_<storm::StormVersion>(m, "Version", "Version information for Storm")
         // static properties are still called with self as argument (which we ignore), see
         // https://pybind11.readthedocs.io/en/master/advanced/classes.html#static-properties
-        .def_property_readonly_static("major", [](py::object /* self */){ return storm::utility::StormVersion::versionMajor; }, "Storm major version.")
-        .def_property_readonly_static("minor", [](py::object /* self */){ return storm::utility::StormVersion::versionMinor; }, "Storm minor version.")
-        .def_property_readonly_static("patch", [](py::object /* self */){ return storm::utility::StormVersion::versionPatch; }, "Storm patch version.")
-        .def_property_readonly_static("development", [](py::object /* self */){ return storm::utility::StormVersion::versionDev; }, "Flag if Storm is development version.")
-        .def_property_readonly_static("short", [](py::object /* self */){ return storm::utility::StormVersion::shortVersionString(); }, "Storm version in short representation.")
-        .def_property_readonly_static("long", [](py::object /* self */){ return storm::utility::StormVersion::longVersionString(); }, "Storm version in long representation.")
-        .def_property_readonly_static("build_info", [](py::object /* self */){ return storm::utility::StormVersion::buildInfo(); }, "Build info for Storm.")
+        .def_property_readonly_static("major", [](py::object /* self */){ return storm::StormVersion::versionMajor; }, "Storm major version.")
+        .def_property_readonly_static("minor", [](py::object /* self */){ return storm::StormVersion::versionMinor; }, "Storm minor version.")
+        .def_property_readonly_static("patch", [](py::object /* self */){ return storm::StormVersion::versionPatch; }, "Storm patch version.")
+        .def_property_readonly_static("development", [](py::object /* self */){ return storm::StormVersion::versionDev; }, "Flag if Storm is development version.")
+        .def_property_readonly_static("short", [](py::object /* self */){ return storm::StormVersion::shortVersionString(); }, "Storm version in short representation.")
+        .def_property_readonly_static("long", [](py::object /* self */){ return storm::StormVersion::longVersionString(); }, "Storm version in long representation.")
+        .def_property_readonly_static("build_info", [](py::object /* self */){ return storm::StormVersion::buildInfo(); }, "Build info for Storm.")
     ;
 }
```

### Comparing `stormpy-1.3.0/src/pars/pars.cpp` & `stormpy-1.8.0/src/pars/pars.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -13,32 +13,28 @@
 void define_pars(py::module& m) {
     m.def("_set_up", []() {
             storm::settings::addModule<storm::settings::modules::ParametricSettings>();
             storm::settings::addModule<storm::settings::modules::RegionSettings>();
         }, "Initialize Storm-pars");
 
     py::class_<SparseParametricDtmcSimplifier, std::shared_ptr<SparseParametricDtmcSimplifier>>(m, "_SparseParametricDtmcSimplifier", "Model simplifier for parametric DTMCs")
-       .def("__init__", [](SparseParametricDtmcSimplifier &instance, Dtmc const& dtmc) -> void {
-                new (&instance) SparseParametricDtmcSimplifier(dtmc);
-            }, py::arg("dtmc"))
+       .def(py::init<Dtmc const&>(), py::arg("dtmc"))
        .def("simplify", [](SparseParametricDtmcSimplifier &simplifier, storm::logic::Formula const& formula) -> bool {
                 return simplifier.simplify(formula);
             }, "Simplify model", py::arg("formula"))
        .def_property_readonly("simplified_model", [](SparseParametricDtmcSimplifier const& simplifier) {
                 return simplifier.getSimplifiedModel();
             }, "Return simplified model")
        .def_property_readonly("simplified_formula", [](SparseParametricDtmcSimplifier const& simplifier) {
                 return simplifier.getSimplifiedFormula();
             }, "Return simplified formula")
     ;
 
     py::class_<SparseParametricMdpSimplifier, std::shared_ptr<SparseParametricMdpSimplifier>>(m, "_SparseParametricMdpSimplifier", "Model simplifier for parametric MDPs")
-       .def("__init__", [](SparseParametricMdpSimplifier &instance, Mdp const& mdp) -> void {
-                new (&instance) SparseParametricMdpSimplifier(mdp);
-            }, py::arg("mdp"))
+       .def(py::init<Mdp const&>(), py::arg("mdp"))
        .def("simplify", [](SparseParametricMdpSimplifier &simplifier, storm::logic::Formula const& formula) -> bool {
                 return simplifier.simplify(formula);
             }, "Simplify model", py::arg("formula"))
        .def_property_readonly("simplified_model", [](SparseParametricMdpSimplifier const& simplifier) {
                 return simplifier.getSimplifiedModel();
             }, "Return simplified model")
        .def_property_readonly("simplified_formula", [](SparseParametricMdpSimplifier const& simplifier) {
```

### Comparing `stormpy-1.3.0/src/pars/pla.cpp` & `stormpy-1.8.0/src/pars/pla.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 typedef storm::modelchecker::SparseDtmcParameterLiftingModelChecker<storm::models::sparse::Dtmc<storm::RationalFunction>, double> DtmcParameterLiftingModelChecker;
 typedef storm::modelchecker::SparseMdpParameterLiftingModelChecker<storm::models::sparse::Mdp<storm::RationalFunction>, double> MdpParameterLiftingModelChecker;
 
 typedef storm::modelchecker::RegionModelChecker<storm::RationalFunction> RegionModelChecker;
 typedef storm::storage::ParameterRegion<storm::RationalFunction> Region;
 
 // Thin wrappers
-std::shared_ptr<RegionModelChecker> createRegionChecker(storm::Environment const& env, std::shared_ptr<storm::models::sparse::Model<storm::RationalFunction>> const& model, std::shared_ptr<storm::logic::Formula> const& formula, bool generateSplittingEstimate, bool allowModelSimplifications) {
-    return storm::api::initializeParameterLiftingRegionModelChecker<storm::RationalFunction, double>(env, model, storm::api::createTask<storm::RationalFunction>(formula, true), generateSplittingEstimate, allowModelSimplifications);
+std::shared_ptr<RegionModelChecker> createRegionChecker(storm::Environment const& env, std::shared_ptr<storm::models::sparse::Model<storm::RationalFunction>> const& model, std::shared_ptr<storm::logic::Formula> const& formula, bool generateSplittingEstimate, bool allowModelSimplifications, bool preconditionsValidatedManually) {
+    return storm::api::initializeParameterLiftingRegionModelChecker<storm::RationalFunction, double>(env, model, storm::api::createTask<storm::RationalFunction>(formula, true), generateSplittingEstimate, allowModelSimplifications, preconditionsValidatedManually);
 }
 
 void specify(std::shared_ptr<RegionModelChecker>& checker, storm::Environment const& env, std::shared_ptr<storm::models::sparse::Model<storm::RationalFunction>> const& model, std::shared_ptr<storm::logic::Formula> const& formula, bool generateSplittingEstimate, bool allowModelSimplifications) {
     return checker->specify(env, model, storm::api::createTask<storm::RationalFunction>(formula, true), generateSplittingEstimate, allowModelSimplifications);
 }
 
 storm::modelchecker::RegionResult checkRegion(std::shared_ptr<RegionModelChecker>& checker, storm::Environment const& env, Region const& region, storm::modelchecker::RegionResultHypothesis const& hypothesis, storm::modelchecker::RegionResult const& initialResult, bool sampleVertices) {
@@ -56,46 +56,57 @@
         .value("EXISTSVIOLATED", storm::modelchecker::RegionResult::ExistsViolated)
         .value("EXISTSBOTH", storm::modelchecker::RegionResult::ExistsBoth)
         .value("CENTERSAT", storm::modelchecker::RegionResult::CenterSat)
         .value("CENTERVIOLATED", storm::modelchecker::RegionResult::CenterViolated)
         .value("ALLSAT", storm::modelchecker::RegionResult::AllSat)
         .value("ALLVIOLATED", storm::modelchecker::RegionResult::AllViolated)
         .value("UNKNOWN", storm::modelchecker::RegionResult::Unknown)
-        .def("__str__", &streamToString<storm::modelchecker::RegionResult>)
+        .def("__str__", &streamToString<storm::modelchecker::RegionResult>, py::prepend() /* use custom method instead of default enum overload */)
     ;
 
     // RegionResultHypothesis
     py::enum_<storm::modelchecker::RegionResultHypothesis>(m, "RegionResultHypothesis", "Hypothesis for the result of a parameter region")
         .value("UNKNOWN", storm::modelchecker::RegionResultHypothesis::Unknown)
         .value("ALLSAT", storm::modelchecker::RegionResultHypothesis::AllSat)
         .value("ALLVIOLATED", storm::modelchecker::RegionResultHypothesis::AllViolated)
-        .def("__str__", &streamToString<storm::modelchecker::RegionResultHypothesis>)
+        .def("__str__", &streamToString<storm::modelchecker::RegionResultHypothesis>, py::prepend() /* use custom method instead of default enum overload */)
     ;
 
     // Region
     py::class_<Region, std::shared_ptr<Region>>(m, "ParameterRegion", "Parameter region")
-       .def("__init__", [](Region &instance, std::string const& regionString, std::set<Region::VariableType> const& variables) -> void {
-                new (&instance) Region(storm::api::parseRegion<storm::RationalFunction>(regionString, variables));
-            })
+        .def(py::init([](std::map<Region::VariableType, std::pair<Region::CoefficientType, Region::CoefficientType>> valuation) {
+                Region::Valuation lowerValuation;
+                Region::Valuation upperValuation;
+                for (auto const& val : valuation) {
+                    lowerValuation[val.first] = val.second.first;
+                    upperValuation[val.first] = val.second.second;
+                }
+                return Region(lowerValuation, upperValuation);
+            }), "Create region from valuation of var -> (lower_bound, upper_bound)", py::arg("valuation"))
+        .def_static("create_from_string", [](std::string const& regionString, std::set<Region::VariableType> const& variables, boost::optional<int> splittingThreshold = boost::none) -> Region {
+                return storm::api::parseRegion<storm::RationalFunction>(regionString, variables, splittingThreshold);
+            }, "Create region from string", py::arg("region_string"), py::arg("variables"), py::arg("splitting_threshold") = boost::none)
+        .def_property_readonly("area", &Region::area, "Get area")
+        .def("__str__", &streamToString<Region>)
     ;
 
     // RegionModelChecker
-
     py::class_<RegionModelChecker, std::shared_ptr<RegionModelChecker>> regionModelChecker(m, "RegionModelChecker", "Region model checker via paramater lifting");
     regionModelChecker.def("check_region", &checkRegion, "Check region", py::arg("environment"), py::arg("region"), py::arg("hypothesis") = storm::modelchecker::RegionResultHypothesis::Unknown, py::arg("initialResult") = storm::modelchecker::RegionResult::Unknown, py::arg("sampleVertices") = false)
         .def("get_bound", &getBoundAtInit, "Get bound", py::arg("environment"), py::arg("region"), py::arg("maximise")= true)
         .def("get_split_suggestion", &RegionModelChecker::getRegionSplitEstimate, "Get estimate")
-        .def("specify", &specify, "specify arguments",py::arg("environment"), py::arg("model"), py::arg("formula"), py::arg("generate_splitting_estimate") = false, py::arg("allow_model_simplification") = true);
+        .def("specify", &specify, "specify arguments",py::arg("environment"), py::arg("model"), py::arg("formula"), py::arg("generate_splitting_estimate") = false, py::arg("allow_model_simplification") = true)
+        .def("compute_extremum", [] (RegionModelChecker & r, storm::Environment const& env, Region const& region, storm::solver::OptimizationDirection const& dirForParameters, storm::RationalFunctionCoefficient const& precision, bool absolutePrecision) {
+            return r.computeExtremalValue(env, region, dirForParameters, storm::utility::one<storm::RationalFunction>() * precision, absolutePrecision); },
+            py::arg("environment"),  py::arg("region"), py::arg("extremum_direction"), py::arg("precision"), py::arg("precision_absolute") = false);
     ;
 
-
     py::class_<DtmcParameterLiftingModelChecker, std::shared_ptr<DtmcParameterLiftingModelChecker>>(m, "DtmcParameterLiftingModelChecker", "Region model checker for DTMCs", regionModelChecker)
             .def(py::init<>())
             .def("get_bound_all_states", &getBound_dtmc, "Get bound", py::arg("environment"), py::arg("region"), py::arg("maximise")= true);
     py::class_<MdpParameterLiftingModelChecker, std::shared_ptr<MdpParameterLiftingModelChecker>>(m, "MdpParameterLiftingModelChecker", "Region model checker for MPDs", regionModelChecker)
             .def(py::init<>())
             .def("get_bound_all_states", &getBound_mdp, "Get bound", py::arg("environment"), py::arg("region"), py::arg("maximise")= true);
 
-    m.def("create_region_checker", &createRegionChecker, "Create region checker", py::arg("environment"), py::arg("model"), py::arg("formula"), py::arg("generate_splitting_estimate") = false, py::arg("allow_model_simplification") = true);
-    //m.def("is_parameter_lifting_sound", &storm::utility::parameterlifting::validateParameterLiftingSound, "Check if parameter lifting is sound", py::arg("model"), py::arg("formula"));
+    m.def("create_region_checker", &createRegionChecker, "Create region checker", py::arg("environment"), py::arg("model"), py::arg("formula"), py::arg("generate_splitting_estimate") = false, py::arg("allow_model_simplification") = true, py::arg("preconditions_validated_manually") = false );
     m.def("gather_derivatives", &gatherDerivatives, "Gather all derivatives of transition probabilities", py::arg("model"), py::arg("var"));
 }
```

### Comparing `stormpy-1.3.0/src/storage/jani.cpp` & `stormpy-1.8.0/src/storage/jani.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #include "jani.h"
 #include <storm/storage/jani/Model.h>
-#include <storm/storage/jani/JSONExporter.h>
+#include <storm/storage/jani/visitor/JSONExporter.h>
 #include <storm/storage/expressions/ExpressionManager.h>
 #include <storm/logic/RewardAccumulationEliminationVisitor.h>
+#include <storm/storage/jani/traverser/InformationCollector.h>
+#include <storm/storage/jani/JaniLocationExpander.h>
+#include <storm/storage/jani/JaniScopeChanger.h>
 #include "src/helpers.h"
 
 using namespace storm::jani;
 
 std::string janiToString(Model const& m) {
     std::stringstream str;
     JsonExporter::toStream(m, {}, str);
@@ -26,27 +29,30 @@
         .def("get_constant", &Model::getConstant, "name"_a, "get constant by name")
         .def("restrict_edges", &Model::restrictEdges, "restrict model to edges given by set", py::arg("edge_set"))
         .def_property_readonly("expression_manager", &Model::getExpressionManager, "get expression manager", pybind11::return_value_policy::reference_internal)
         .def_property_readonly("has_undefined_constants", &Model::hasUndefinedConstants, "Flag if program has undefined constants")
         .def_property_readonly("undefined_constants_are_graph_preserving", &Model::undefinedConstantsAreGraphPreserving, "Flag if the undefined constants do not change the graph structure")
         .def("__str__", &janiToString)
         .def_property("initial_states_restriction", &Model::getInitialStatesRestriction, &Model::setInitialStatesRestriction, "initial states restriction")
+        .def("add_constant", &Model::addConstant, "adds constant to model", py::arg("constant"))
         .def("define_constants", &Model::defineUndefinedConstants, "define constants with a mapping from the corresponding expression variables to expressions", py::arg("map"))
         .def("substitute_constants", &Model::substituteConstants, "substitute constants")
         .def("remove_constant", &Model::removeConstant, "remove a constant. Make sure the constant does not appear in the model.", "constant_name"_a)
+        .def("get_automaton", [](Model const& model, std::string const& name) {return model.getAutomaton(name);}, "name"_a)
         .def("get_automaton_index", &Model::getAutomatonIndex, "name"_a, "get index for automaton name")
         .def("add_automaton", &Model::addAutomaton, "automaton"_a, "add an automaton (with a unique name)")
         .def("set_standard_system_composition", &Model::setStandardSystemComposition, "sets the composition to the standard composition")
         .def("replace_automaton", &Model::replaceAutomaton, "index"_a, "new_automaton"_a, "replace automaton at index")
         .def("check_valid", &Model::checkValid, "Some basic checks to ensure validity")
         .def("substitute_functions", [](Model& model) {model.substituteFunctions();}, "substitute functions")
         .def_static("encode_automaton_and_edge_index", &Model::encodeAutomatonAndEdgeIndices, "get edge/automaton-index")
         .def_static("decode_automaton_and_edge_index", &Model::decodeAutomatonAndEdgeIndices, "get edge and automaton from edge/automaton index")
         .def("make_standard_compliant", &Model::makeStandardJaniCompliant, "make standard JANI compliant")
         .def("has_standard_composition", &Model::hasStandardComposition, "is the composition the standard composition")
+        .def("flatten_composition", &Model::flattenComposition, py::arg("smt_solver_factory")=std::make_shared<storm::utility::solver::SmtSolverFactory>())
         .def("finalize", &Model::finalize,"finalizes the model. After this action, be careful changing the data structure.")
         .def("to_dot", [](Model& model) {std::stringstream ss; model.writeDotToStream(ss); return ss.str(); })
     ;
 
     py::class_<Automaton, std::shared_ptr<Automaton>> automaton(m, "JaniAutomaton", "A Jani Automation");
     automaton.def(py::init<std::string, storm::expressions::Variable>())
         .def_property_readonly("edges",[](const Automaton& a) -> auto& {
@@ -57,15 +63,15 @@
         .def_property_readonly("variables", [](Automaton& aut) -> VariableSet& {return aut.getVariables();}, py::return_value_policy::reference_internal)
         .def_property_readonly("locations", [](Automaton& aut) -> auto& {return aut.getLocations();})
         .def("add_location", &Automaton::addLocation, "location"_a, "adds a new location, returns the index")
         .def("add_initial_location", [](Automaton& aut, uint64_t index) { aut.addInitialLocation(index); }, "index"_a)
         .def_property_readonly("initial_location_indices", &Automaton::getInitialLocationIndices)
         .def_property("initial_states_restriction", [](Automaton& aut) { aut.getInitialStatesExpression(); }, &Automaton::setInitialStatesRestriction, "initial state restriction")
         .def("add_edge", &Automaton::addEdge, "edge"_a)
-
+        .def("get_location_index", &Automaton::getLocationIndex, "name"_a)
     ;
 
     py::class_<Edge, std::shared_ptr<Edge>> edge(m, "JaniEdge", "A Jani Edge");
     edge.def(py::init<uint64_t, uint64_t, boost::optional<storm::expressions::Expression>, std::shared_ptr<TemplateEdge>, std::vector<std::pair<uint64_t, storm::expressions::Expression>>>(),
             "source_location_index"_a, "action_index"_a, "rate"_a, "template_edge"_a, "destinations_with_probabilities"_a)
         .def_property_readonly("source_location_index", &Edge::getSourceLocationIndex, "index for source location")
         .def_property_readonly("destinations", [](Edge const& e) -> auto&  {
@@ -99,64 +105,83 @@
     templateEdgeDestination.def(py::init<OrderedAssignments>(), "ordered_assignments"_a)
             .def_property_readonly("assignments", [](TemplateEdgeDestination& ted) -> auto& {return ted.getOrderedAssignments();});
 
     py::class_<OrderedAssignments, std::shared_ptr<OrderedAssignments>> orderedAssignments(m, "JaniOrderedAssignments", "Set of assignments");
     orderedAssignments.def("__iter__", [](OrderedAssignments &v) {
                 return py::make_iterator(v.begin(), v.end());
             }, py::keep_alive<0, 1>()) /* Keep vector alive while iterator is used */
+        .def(py::init<std::vector<Assignment> const&>(), "assignments")
         .def("__str__", &streamToString<OrderedAssignments>)
         .def("clone", &OrderedAssignments::clone, "clone assignments (performs a deep copy)")
         .def("substitute", &OrderedAssignments::substitute, "substitute in rhs according to given substitution map", "substitution_map"_a)
         .def("add", [](OrderedAssignments& oa, Assignment const& newAssignment, bool addToExisting) {return oa.add(newAssignment, addToExisting); }, "new_assignment"_a, "add_to_existing"_a = false)
     ;
 
     py::class_<Assignment, std::shared_ptr<Assignment>> assignment(m, "JaniAssignment", "Jani Assignment");
     assignment.def(py::init<Variable const&,storm::expressions::Expression const&,int64_t>(), "lhs"_a, "rhs"_a, "lvl"_a = 0)
         .def("__str__", &streamToString<Assignment>)
         .def_property("expression", &Assignment::getAssignedExpression, &Assignment::setAssignedExpression)
+        .def_property_readonly("variable", &Assignment::getVariable, "variable that is assigned to, if any")
     ;
 
     py::class_<Location, std::shared_ptr<Location>> location(m, "JaniLocation", "A Location in JANI");
-    location.def_property_readonly("name", &Location::getName, "name of the location")
+    location.def(py::init<std::string const&, OrderedAssignments const&>(), "name"_a, "assignments"_a)
+            .def_property_readonly("name", &Location::getName, "name of the location")
             .def_property_readonly("assignments", [](Location& loc) {loc.getAssignments();}, "location assignments")
             ;
 
     py::class_<VariableSet, std::shared_ptr<VariableSet>> variableSet(m, "JaniVariableSet", "Jani Set of Variables");
     variableSet.def(py::init<>())
         .def("__iter__", [](VariableSet &v) {
             return py::make_iterator(v.begin(), v.end());
         }, py::keep_alive<0, 1>())
         .def("add_variable", [](VariableSet& vs, Variable& v) -> void { vs.addVariable(v); })
-        .def("add_bounded_integer_variable", [](VariableSet& vs, BoundedIntegerVariable& v) -> auto& { return vs.addVariable(v); /*return vs.getVariable(v.getExpressionVariable());*/ }, py::return_value_policy::reference_internal, "variable"_a)
         .def("empty", &VariableSet::empty, "is there a variable in the set?")
         .def("get_variable_by_name", [](VariableSet& v, std::string const& name) -> auto& { return v.getVariable(name);})
         .def("get_variable_by_expr_variable", [](VariableSet& v, storm::expressions::Variable const& var) -> auto& { return v.getVariable(var);})
+        .def("erase_variable", &VariableSet::eraseVariable, "variable")
     ;
 
     py::class_<Variable, std::shared_ptr<Variable>> variable(m, "JaniVariable", "A Variable in JANI");
     variable.def_property_readonly("name", &Variable::getName, "name of constant")
             .def_property_readonly("expression_variable", &Variable::getExpressionVariable, "expression variable for this variable")
-            ;
-
-    py::class_<BoundedIntegerVariable, std::shared_ptr<BoundedIntegerVariable>> bivariable(m, "JaniBoundedIntegerVariable", "A Bounded Integer", variable);
-    bivariable.def(py::init<std::string, storm::expressions::Variable, storm::expressions::Expression, storm::expressions::Expression, storm::expressions::Expression>(),
-                "name"_a, "expression_variable"_a, "init_value"_a, "lower_bound"_a, "upper_bound"_a)
-            .def(py::init<std::string, storm::expressions::Variable, storm::expressions::Expression, storm::expressions::Expression>(),
-                 "name"_a, "expression_variable"_a, "lower_bound"_a, "upper_bound"_a);;
+            .def_property_readonly("init_expression", &Variable::getInitExpression);
 
     py::class_<Constant, std::shared_ptr<Constant>> constant(m, "JaniConstant", "A Constant in JANI");
-    constant.def_property_readonly("defined", &Constant::isDefined, "is constant defined by some expression")
+    constant.def(py::init<std::string, storm::expressions::Variable>())
+        .def_property_readonly("defined", &Constant::isDefined, "is constant defined by some expression")
         .def_property_readonly("name", &Constant::getName, "name of constant")
         .def_property_readonly("type", &Constant::getType, "type of constant")
         .def_property_readonly("expression_variable", &Constant::getExpressionVariable, "expression variable for this constant")
     ;
 
 
     m.def("eliminate_reward_accumulations", [](const Model& model, std::vector<Property>& properties) {
             storm::logic::RewardAccumulationEliminationVisitor v(model);
             v.eliminateRewardAccumulations(properties);
             return properties;
         }, "Eliminate reward accumulations", py::arg("model"), py::arg("properties"));
 
 
+    py::class_<InformationObject> informationObject(m, "JaniInformationObject", "An object holding information about a JANI model");
+    informationObject.def_readwrite("model_type", &InformationObject::modelType)
+            .def_readwrite("nr_automata", &InformationObject::nrAutomata)
+            .def_readwrite("nr_edges", &InformationObject::nrEdges)
+            .def_readwrite("nr_variables", &InformationObject::nrVariables)
+    		.def_readwrite("state_domain_size", &InformationObject::stateDomainSize)
+    		.def_readwrite("avg_var_domain_size", &InformationObject::avgVarDomainSize);
+			
+	
+    m.def("collect_information", [](const Model& model) {return storm::jani::collectModelInformation(model);});
 
-}
+}
+
+void define_jani_transformers(py::module& m) {
+    py::class_<JaniLocationExpander>(m, "JaniLocationExpander", "A transformer for Jani expanding variables into locations")
+            .def(py::init<Model const&>(), py::arg("model"))
+            .def("transform", &JaniLocationExpander::transform, py::arg("automaton_name"), py::arg("variable_name"))
+        ;
+
+    py::class_<JaniScopeChanger>(m, "JaniScopeChanger", "A transformer for Jani changing variables from local to global and vice versa")
+            .def(py::init<>())
+            .def("make_variables_local", [](JaniScopeChanger const& sc, Model const& model , std::vector<Property> const& props = {}) { Model newModel(model); sc.makeVariablesLocal(newModel, props); return newModel;}, py::arg("model"), py::arg("properties") = std::vector<Property>());
+}
```

### Comparing `stormpy-1.3.0/src/storage/labeling.cpp` & `stormpy-1.8.0/src/storage/labeling.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -17,20 +17,30 @@
         .def("contains_label", &storm::models::sparse::ItemLabeling::containsLabel, "Check if the given label is contained in the labeling", py::arg("label"))
         .def("__str__", &streamToString<storm::models::sparse::ItemLabeling>)
     ;
 
 
     // StateLabeling
     py::class_<storm::models::sparse::StateLabeling, std::shared_ptr<storm::models::sparse::StateLabeling>>(m, "StateLabeling", "Labeling for states", labeling)
+        .def(py::init<uint_fast64_t>(), "state_count"_a)
         .def("get_labels_of_state", &storm::models::sparse::StateLabeling::getLabelsOfState, "Get labels of given state", py::arg("state"))
         .def("add_label_to_state", &storm::models::sparse::StateLabeling::addLabelToState, "Add label to state", py::arg("label"), py::arg("state"))
         .def("has_state_label", &storm::models::sparse::StateLabeling::getStateHasLabel, "Check if the given state has the given label", py::arg("label"), py::arg("state"))
         .def("get_states", &storm::models::sparse::StateLabeling::getStates, "Get all states which have the given label", py::arg("label"))
         .def("set_states", [](storm::models::sparse::StateLabeling& labeling, std::string const& label, storm::storage::BitVector const& states) {
                 labeling.setStates(label, states);
-            }, "Set all states which have the given label", py::arg("label"), py::arg("states"))
+            }, "Add a label to the given states", py::arg("label"), py::arg("states"))
         .def("__str__", &streamToString<storm::models::sparse::StateLabeling>)
     ;
 
 
-    py::class_<storm::models::sparse::ChoiceLabeling>(m, "ChoiceLabeling", "Labeling for choices", labeling);
+    py::class_<storm::models::sparse::ChoiceLabeling>(m, "ChoiceLabeling", "Labeling for choices", labeling)
+            .def(py::init<uint_fast64_t>(), "choice_count"_a)
+            .def("get_labels_of_choice", &storm::models::sparse::ChoiceLabeling::getLabelsOfChoice, py::arg("choice"),  "Get labels of the given choice")
+            .def("add_label_to_choice", &storm::models::sparse::ChoiceLabeling::addLabelToChoice, "Adds a label to a given choice", py::arg("label"), py::arg("state"))
+            .def("get_choices", &storm::models::sparse::ChoiceLabeling::getChoices, py::arg("label"),  "Get all choices which have the given label")
+            .def("set_choices", [](storm::models::sparse::ChoiceLabeling& labeling, std::string const& label, storm::storage::BitVector const& choices) {
+                labeling.setChoices(label, choices);
+            },  "Add a label to a the given choices", py::arg("label"), py::arg("choices"))
+            .def("__str__", &streamToString<storm::models::sparse::ChoiceLabeling>)
+    ;
 }
```

### Comparing `stormpy-1.3.0/src/storage/model.cpp` & `stormpy-1.8.0/src/storage/model.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -11,26 +11,32 @@
 #include "storm/models/sparse/StandardRewardModel.h"
 #include "storm/models/symbolic/Model.h"
 #include "storm/models/symbolic/Dtmc.h"
 #include "storm/models/symbolic/Mdp.h"
 #include "storm/models/symbolic/Ctmc.h"
 #include "storm/models/symbolic/MarkovAutomaton.h"
 #include "storm/models/symbolic/StandardRewardModel.h"
+#include "storm/utility/dd.h"
+
+#include "storm/storage/dd/DdManager.h"
 
 #include "storm/storage/Scheduler.h"
 
 #include <functional>
 #include <string>
 #include <sstream>
 
 // Typedefs
 using RationalFunction = storm::RationalFunction;
 using ModelBase = storm::models::ModelBase;
 
+template<typename ValueType> using ModelComponents = storm::storage::sparse::ModelComponents<ValueType>;
 template<typename ValueType> using SparseModel = storm::models::sparse::Model<ValueType>;
+template<typename ValueType> using SparseDeterministicModel = storm::models::sparse::DeterministicModel<ValueType>;
+template<typename ValueType> using SparseNondeterministicModel = storm::models::sparse::NondeterministicModel<ValueType>;
 template<typename ValueType> using SparseDtmc = storm::models::sparse::Dtmc<ValueType>;
 template<typename ValueType> using SparseMdp = storm::models::sparse::Mdp<ValueType>;
 template<typename ValueType> using SparsePomdp = storm::models::sparse::Pomdp<ValueType>;
 template<typename ValueType> using SparseCtmc = storm::models::sparse::Ctmc<ValueType>;
 template<typename ValueType> using SparseMarkovAutomaton = storm::models::sparse::MarkovAutomaton<ValueType>;
 template<typename ValueType> using SparseRewardModel = storm::models::sparse::StandardRewardModel<ValueType>;
 
@@ -63,30 +69,36 @@
     return storm::models::sparse::getProbabilityParameters(model);
 }
 
 std::set<storm::RationalFunctionVariable> rewardVariables(SparseModel<RationalFunction> const& model) {
     return storm::models::sparse::getRewardParameters(model);
 }
 
-template<typename ValueType>
-std::function<std::string (storm::models::Model<ValueType> const&)> getModelInfoPrinter(std::string name = "Model") {
-    // look, C++ has lambdas and stuff!
-    return [name](storm::models::Model<ValueType> const& model) {
-        std::stringstream ss;
-        model.printModelInformationToStream(ss);
-
-        // attempting a slightly readable output
-        std::string text = name + " (";
-        std::string line;
-        for (int i = 0; std::getline(ss, line); i++) {
-            if (line != "-------------------------------------------------------------- ")
-                text += line + " ";
+std::set<storm::RationalFunctionVariable> allVariables(SparseModel<RationalFunction> const& model) {
+    return storm::models::sparse::getAllParameters(model);
+}
+
+storm::storage::BitVector statesWithParameter(SparseModel<RationalFunction> const& model, storm::RationalFunctionVariable const& var) {
+    storm::storage::BitVector result(model.getNumberOfStates());
+    for (uint64_t s = 0; s < model.getNumberOfStates(); ++s) {
+        for(auto const& entry : model.getTransitionMatrix().getRowGroup(s)) {
+            if (entry.getValue().gatherVariables().count(var) > 0) {
+                result.set(s);
+                break;
+            }
         }
-        return text + ")";
-    };
+    }
+    return result;
+}
+
+
+std::string getModelInfoPrinter(ModelBase const& model) {
+    std::stringstream ss;
+    model.printModelInformationToStream(ss);
+    return ss.str();
 }
 
 template<typename ValueType>
 storm::models::sparse::StateLabeling& getLabeling(SparseModel<ValueType>& model) {
     return model.getStateLabeling();
 }
 
@@ -108,29 +120,43 @@
     modelBase.def_property_readonly("nr_states", &ModelBase::getNumberOfStates, "Number of states")
         .def_property_readonly("nr_transitions", &ModelBase::getNumberOfTransitions, "Number of transitions")
         .def_property_readonly("nr_choices", &ModelBase::getNumberOfChoices, "Number of choices")
         .def_property_readonly("model_type", &ModelBase::getType, "Model type")
         .def_property_readonly("supports_parameters", &ModelBase::supportsParameters, "Flag whether model supports parameters")
         .def_property_readonly("has_parameters", &ModelBase::hasParameters, "Flag whether model has parameters")
         .def_property_readonly("is_exact", &ModelBase::isExact, "Flag whether model is exact")
+        .def_property_readonly("is_partially_observable", &ModelBase::isPartiallyObservable, "Flag whether the model has observation labels")
+        .def_property_readonly("is_sparse_model", &ModelBase::isSparseModel, "Flag whether the model is stored as a sparse model")
+        .def_property_readonly("is_symbolic_model", &ModelBase::isSymbolicModel, "Flag whether the model is stored using decision diagrams")
+        .def_property_readonly("is_discrete_time_model", &ModelBase::isDiscreteTimeModel, "Flag whether the model is a discrete time model")
+        .def_property_readonly("is_nondeterministic_model", &ModelBase::isNondeterministicModel, "Flag whether the model contains nondeterminism")
         .def("_as_sparse_dtmc", [](ModelBase &modelbase) {
                 return modelbase.as<SparseDtmc<double>>();
             }, "Get model as sparse DTMC")
+        .def("_as_sparse_exact_dtmc", [](ModelBase &modelbase) {
+                return modelbase.as<SparseDtmc<storm::RationalNumber>>();
+            }, "Get model as sparse DTMC")
         .def("_as_sparse_pdtmc", [](ModelBase &modelbase) {
                 return modelbase.as<SparseDtmc<RationalFunction>>();
             }, "Get model as sparse pDTMC")
         .def("_as_sparse_mdp", [](ModelBase &modelbase) {
                 return modelbase.as<SparseMdp<double>>();
             }, "Get model as sparse MDP")
+        .def("_as_sparse_exact_mdp", [](ModelBase &modelbase) {
+                return modelbase.as<SparseMdp<storm::RationalNumber>>();
+            }, "Get model as sparse exact MDP")
         .def("_as_sparse_pmdp", [](ModelBase &modelbase) {
                 return modelbase.as<SparseMdp<RationalFunction>>();
             }, "Get model as sparse pMDP")
         .def("_as_sparse_pomdp", [](ModelBase &modelbase) {
                 return modelbase.as<SparsePomdp<double>>();
             }, "Get model as sparse POMDP")
+        .def("_as_sparse_ppomdp", [](ModelBase &modelbase) {
+            return modelbase.as<SparsePomdp<RationalFunction>>();
+        }, "Get model as sparse pPOMDP")
         .def("_as_sparse_ctmc", [](ModelBase &modelbase) {
                 return modelbase.as<SparseCtmc<double>>();
             }, "Get model as sparse CTMC")
         .def("_as_sparse_pctmc", [](ModelBase &modelbase) {
                 return modelbase.as<SparseCtmc<RationalFunction>>();
             }, "Get model as sparse pCTMC")
         .def("_as_sparse_ma", [](ModelBase &modelbase) {
@@ -164,117 +190,190 @@
                 return modelbase.as<SymbolicMarkovAutomaton<storm::dd::DdType::Sylvan, RationalFunction>>();
             }, "Get model as symbolic pMA")
     ;
 }
 
 
 // Bindings for sparse models
-void define_sparse_model(py::module& m) {
+template<typename ValueType>
+void define_sparse_model(py::module& m, std::string const& vtSuffix) {
 
     // Models with double numbers
-    py::class_<SparseModel<double>, std::shared_ptr<SparseModel<double>>, ModelBase> model(m, "_SparseModel", "A probabilistic model where transitions are represented by doubles and saved in a sparse matrix");
-    model.def_property_readonly("labeling", &getLabeling<double>, "Labels")
-        .def_property_readonly("choice_labeling", [](SparseModel<double> const& model) {return model.getChoiceLabeling();}, "get choice labelling")
-        .def("has_choice_origins", [](SparseModel<double> const& model) {return model.hasChoiceOrigins();}, "has choice origins?")
-        .def_property_readonly("choice_origins", [](SparseModel<double> const& model) {return model.getChoiceOrigins();})
-        .def("labels_state", &SparseModel<double>::getLabelsOfState, py::arg("state"), "Get labels of state")
-        .def_property_readonly("initial_states", &getSparseInitialStates<double>, "Initial states")
-        .def_property_readonly("states", [](SparseModel<double>& model) {
-                return SparseModelStates<double>(model);
+    py::class_<SparseModel<ValueType>, std::shared_ptr<SparseModel<ValueType>>, ModelBase> model(m, ("_Sparse" + vtSuffix + "Model").c_str(),
+                                                                                           "A probabilistic model where transitions are represented by doubles and saved in a sparse matrix");
+    model.def_property_readonly("labeling", &getLabeling<ValueType>, "Labels")
+        .def("has_choice_labeling", [](SparseModel<ValueType> const& model) {return model.hasChoiceLabeling();}, "Does the model have an associated choice labelling?")
+        .def_property_readonly("choice_labeling", [](SparseModel<ValueType> const& model) {return model.getChoiceLabeling();}, "get choice labelling")
+        .def("has_choice_origins", [](SparseModel<ValueType> const& model) {return model.hasChoiceOrigins();}, "has choice origins?")
+        .def_property_readonly("choice_origins", [](SparseModel<ValueType> const& model) {return model.getChoiceOrigins();})
+        .def("labels_state", &SparseModel<ValueType>::getLabelsOfState, py::arg("state"), "Get labels of state")
+        .def_property_readonly("initial_states", &getSparseInitialStates<ValueType>, "Initial states")
+        .def_property_readonly("initial_states_as_bitvector", [](SparseModel<ValueType> const& model) {return model.getInitialStates();})
+        .def_property_readonly("states", [](SparseModel<ValueType>& model) {
+                return SparseModelStates<ValueType>(model);
             }, "Get states")
-        .def_property_readonly("reward_models", [](SparseModel<double>& model) {return model.getRewardModels(); }, "Reward models")
-        .def_property_readonly("transition_matrix", &getTransitionMatrix<double>, py::return_value_policy::reference, py::keep_alive<1, 0>(), "Transition matrix")
-        .def_property_readonly("backward_transition_matrix", &SparseModel<double>::getBackwardTransitions, py::return_value_policy::reference, py::keep_alive<1, 0>(), "Backward transition matrix")
-        .def("reduce_to_state_based_rewards", &SparseModel<double>::reduceToStateBasedRewards)
-        .def("__str__", getModelInfoPrinter<double>())
-        .def("to_dot", [](SparseModel<double>& model) { std::stringstream ss; model.writeDotToStream(ss); return ss.str(); }, "Write dot to a string")
-    ;
-    py::class_<SparseDtmc<double>, std::shared_ptr<SparseDtmc<double>>>(m, "SparseDtmc", "DTMC in sparse representation", model)
-            .def(py::init<SparseDtmc<double>>(), py::arg("other_model"))
-            .def("__str__", getModelInfoPrinter<double>("DTMC"))
-    ;
-    py::class_<SparseMdp<double>, std::shared_ptr<SparseMdp<double>>>(m, "SparseMdp", "MDP in sparse representation", model)
-        .def(py::init<SparseMdp<double>>(), py::arg("other_model"))
-        .def_property_readonly("nondeterministic_choice_indices", [](SparseMdp<double> const& mdp) { return mdp.getNondeterministicChoiceIndices(); })
-        .def("apply_scheduler", [](SparseMdp<double> const& mdp, storm::storage::Scheduler<double> const& scheduler, bool dropUnreachableStates) { return mdp.applyScheduler(scheduler, dropUnreachableStates); } , "apply scheduler", "scheduler"_a, "drop_unreachable_states"_a = true)
-        .def("__str__", getModelInfoPrinter<double>("MDP"))
-    ;
-    py::class_<SparsePomdp<double>, std::shared_ptr<SparsePomdp<double>>>(m, "SparsePomdp", "POMDP in sparse representation", model)
-            .def(py::init<SparsePomdp<double>>(), py::arg("other_model"))
-            .def("__str__", getModelInfoPrinter<double>("POMDP"))
-            .def_property_readonly("observations", &SparsePomdp<double>::getObservations)
-            .def_property_readonly("nr_observations", &SparsePomdp<double>::getNrObservations)
-            ;
-    py::class_<SparseCtmc<double>, std::shared_ptr<SparseCtmc<double>>>(m, "SparseCtmc", "CTMC in sparse representation", model)
-            .def(py::init<SparseCtmc<double>>(), py::arg("other_model"))
-            .def("__str__", getModelInfoPrinter<double>("CTMC"))
-    ;
-    py::class_<SparseMarkovAutomaton<double>, std::shared_ptr<SparseMarkovAutomaton<double>>>(m, "SparseMA", "MA in sparse representation", model)
-            .def(py::init<SparseMarkovAutomaton<double>>(), py::arg("other_model"))
-            .def("__str__", getModelInfoPrinter<double>("MA"))
-    ;
-
-    py::class_<SparseRewardModel<double>>(m, "SparseRewardModel", "Reward structure for sparse models")
-        .def_property_readonly("has_state_rewards", &SparseRewardModel<double>::hasStateRewards)
-        .def_property_readonly("has_state_action_rewards", &SparseRewardModel<double>::hasStateActionRewards)
-        .def_property_readonly("has_transition_rewards", &SparseRewardModel<double>::hasTransitionRewards)
-        .def_property_readonly("transition_rewards", [](SparseRewardModel<double>& rewardModel) {return rewardModel.getTransitionRewardMatrix();})
-        .def_property_readonly("state_rewards", [](SparseRewardModel<double>& rewardModel) {return rewardModel.getStateRewardVector();})
-        .def("get_state_reward", [](SparseRewardModel<double>& rewardModel, uint64_t state) {return rewardModel.getStateReward(state);})
-        .def("get_zero_reward_states", &SparseRewardModel<double>::getStatesWithZeroReward<double>, "get states where all rewards are zero", py::arg("transition_matrix"))
-        .def("get_state_action_reward", [](SparseRewardModel<double>& rewardModel, uint64_t action_index) {return rewardModel.getStateActionReward(action_index);})
-        .def_property_readonly("state_action_rewards", [](SparseRewardModel<double>& rewardModel) {return rewardModel.getStateActionRewardVector();})
-        .def("reduce_to_state_based_rewards", [](SparseRewardModel<double>& rewardModel, storm::storage::SparseMatrix<double> const& transitions, bool onlyStateRewards){return rewardModel.reduceToStateBasedRewards(transitions, onlyStateRewards);},  py::arg("transition_matrix"), py::arg("only_state_rewards"), "Reduce to state-based rewards")
+        .def_property_readonly("reward_models", [](SparseModel<ValueType>& model) {return model.getRewardModels(); }, "Reward models")
+        .def_property_readonly("transition_matrix", &getTransitionMatrix<ValueType>, py::return_value_policy::reference, py::keep_alive<1, 0>(), "Transition matrix")
+        .def_property_readonly("backward_transition_matrix", &SparseModel<ValueType>::getBackwardTransitions, py::return_value_policy::reference, py::keep_alive<1, 0>(), "Backward transition matrix")
+        .def("get_reward_model", [](SparseModel<ValueType>& model, std::string const& name) -> SparseRewardModel<ValueType>& {return model.getRewardModel(name);}, py::return_value_policy::reference, py::keep_alive<1, 0>(), "Reward model")
+        .def("has_reward_model", [](SparseModel<ValueType> const& model, std::string const& name) {return model.hasRewardModel(name);}, py::arg("name"))
+        .def("add_reward_model", [](SparseModel<ValueType>& model, std::string const& name, SparseRewardModel<ValueType> const& rewModel) { model.addRewardModel(name, rewModel);})
+        .def("has_state_valuations", [](SparseModel<ValueType> const& model) {return model.hasStateValuations();}, "has state valuation?")
+        .def_property_readonly("state_valuations",  [](SparseModel<ValueType> const& model) {return model.getStateValuations();}, "state valuations")
+        .def("reduce_to_state_based_rewards", &SparseModel<ValueType>::reduceToStateBasedRewards)
+        .def("is_sink_state", &SparseModel<ValueType>::isSinkState, py::arg("state"))
+        .def("__str__", &getModelInfoPrinter)
+        .def("to_dot", [](SparseModel<ValueType>& model) { std::stringstream ss; model.writeDotToStream(ss); return ss.str(); }, "Write dot to a string")
+    ;
+    py::class_<SparseDeterministicModel<ValueType>, std::shared_ptr<SparseDeterministicModel<ValueType>>> detModel(m, ("_SparseDeterministic" + vtSuffix + "Model").c_str(), "Deterministic sparse model", model)
+    ;
+    py::class_<SparseNondeterministicModel<ValueType>, std::shared_ptr<SparseNondeterministicModel<ValueType>>> nondetModel(m, ("_SparseNondeterministic" + vtSuffix + "Model").c_str(), "Nondeterministic sparse model", model)
+    ;
+
+    py::class_<SparseDtmc<ValueType>, std::shared_ptr<SparseDtmc<ValueType>>>(m, ("Sparse" + vtSuffix + "Dtmc").c_str(), "DTMC in sparse representation", detModel)
+        .def(py::init<SparseDtmc<ValueType>>(), py::arg("other_model"))
+        .def(py::init<ModelComponents<ValueType> const&>(), py::arg("components"))
+        .def("__str__", &getModelInfoPrinter)
+    ;
+    py::class_<SparseMdp<ValueType>, std::shared_ptr<SparseMdp<ValueType>>> mdp(m, ("Sparse" + vtSuffix + "Mdp").c_str(), "MDP in sparse representation", nondetModel);
+    mdp.def(py::init<SparseMdp<ValueType>>(), py::arg("other_model"))
+        .def(py::init<ModelComponents<ValueType> const&, storm::models::ModelType>(), py::arg("components"), py::arg("type")=storm::models::ModelType::Mdp)
+        .def_property_readonly("nondeterministic_choice_indices", [](SparseMdp<ValueType> const& mdp) { return mdp.getNondeterministicChoiceIndices(); })
+        .def("get_nr_available_actions", [](SparseMdp<ValueType> const& mdp, uint64_t stateIndex) { return mdp.getNondeterministicChoiceIndices()[stateIndex+1] - mdp.getNondeterministicChoiceIndices()[stateIndex] ; }, py::arg("state"))
+        .def("get_choice_index", [](SparseMdp<ValueType> const& mdp, uint64_t state, uint64_t actOff) { return mdp.getNondeterministicChoiceIndices()[state]+actOff; }, py::arg("state"), py::arg("action_offset"), "gets the choice index for the offset action from the given state.")
+        .def("apply_scheduler", [](SparseMdp<ValueType> const& mdp, storm::storage::Scheduler<ValueType> const& scheduler, bool dropUnreachableStates) { return mdp.applyScheduler(scheduler, dropUnreachableStates); } , "apply scheduler", "scheduler"_a, "drop_unreachable_states"_a = true)
+        .def("__str__", &getModelInfoPrinter)
+    ;
+    py::class_<SparsePomdp<ValueType>, std::shared_ptr<SparsePomdp<ValueType>>>(m, ("Sparse" + vtSuffix + "Pomdp").c_str(), "POMDP in sparse representation", mdp)
+        .def(py::init<SparsePomdp<ValueType>>(), py::arg("other_model"))
+        .def(py::init<ModelComponents<ValueType> const&, bool>(), py::arg("components"), py::arg("canonic_flag")=false)
+        .def("__str__", &getModelInfoPrinter)
+        .def("get_observation", &SparsePomdp<ValueType>::getObservation, py::arg("state"))
+        .def_property_readonly("observations", &SparsePomdp<ValueType>::getObservations)
+        .def_property_readonly("nr_observations", &SparsePomdp<ValueType>::getNrObservations)
+        .def("has_observation_valuations", &SparsePomdp<ValueType>::hasObservationValuations)
+        .def_property_readonly("observation_valuations", &SparsePomdp<ValueType>::getObservationValuations)
+    ;
+    py::class_<SparseCtmc<ValueType>, std::shared_ptr<SparseCtmc<ValueType>>>(m, ("Sparse" + vtSuffix + "Ctmc").c_str(), "CTMC in sparse representation", detModel)
+        .def(py::init<SparseCtmc<ValueType>>(), py::arg("other_model"))
+        .def(py::init<ModelComponents<ValueType> const&>(), py::arg("components"))
+        .def_property_readonly("exit_rates", [](SparseCtmc<ValueType> const& ctmc) { return ctmc.getExitRateVector(); })
+        .def("__str__", &getModelInfoPrinter)
+    ;
+    py::class_<SparseMarkovAutomaton<ValueType>, std::shared_ptr<SparseMarkovAutomaton<ValueType>>>(m, ("Sparse" + vtSuffix + "MA").c_str(), "MA in sparse representation", nondetModel)
+        .def(py::init<SparseMarkovAutomaton<ValueType>>(), py::arg("other_model"))
+        .def(py::init<ModelComponents<ValueType> const&>(), py::arg("components"))
+        .def_property_readonly("exit_rates", [](SparseMarkovAutomaton<ValueType> const& ma) { return ma.getExitRates(); })
+        .def_property_readonly("markovian_states", [](SparseMarkovAutomaton<ValueType> const& ma) { return ma.getMarkovianStates(); })
+        .def_property_readonly("nondeterministic_choice_indices", [](SparseMarkovAutomaton<ValueType> const& ma) { return ma.getNondeterministicChoiceIndices(); })
+        .def("apply_scheduler", [](SparseMarkovAutomaton<ValueType> const& ma, storm::storage::Scheduler<ValueType> const& scheduler, bool dropUnreachableStates) { return ma.applyScheduler(scheduler, dropUnreachableStates); } , "apply scheduler", "scheduler"_a, "drop_unreachable_states"_a = true)
+        .def("__str__", &getModelInfoPrinter)
+        .def_property_readonly("convertible_to_ctmc", &SparseMarkovAutomaton<ValueType>::isConvertibleToCtmc, "Check whether the MA can be converted into a CTMC.")
+        .def("convert_to_ctmc", &SparseMarkovAutomaton<ValueType>::convertToCtmc, "Convert the MA into a CTMC.")
+    ;
+
+    py::class_<SparseRewardModel<ValueType>>(m, ("Sparse" + vtSuffix + "RewardModel").c_str(), "Reward structure for sparse models")
+        .def(py::init<std::optional<std::vector<ValueType>> const&, std::optional<std::vector<ValueType>> const&,
+                std::optional<storm::storage::SparseMatrix<ValueType>> const&>(), py::arg("optional_state_reward_vector") = std::nullopt,
+                py::arg("optional_state_action_reward_vector") = std::nullopt,  py::arg("optional_transition_reward_matrix") = std::nullopt)
+        .def_property_readonly("has_state_rewards", &SparseRewardModel<ValueType>::hasStateRewards)
+        .def_property_readonly("has_state_action_rewards", &SparseRewardModel<ValueType>::hasStateActionRewards)
+        .def_property_readonly("has_transition_rewards", &SparseRewardModel<ValueType>::hasTransitionRewards)
+        .def_property_readonly("transition_rewards", [](SparseRewardModel<ValueType>& rewardModel) {return rewardModel.getTransitionRewardMatrix();})
+        .def_property_readonly("state_rewards", [](SparseRewardModel<ValueType>& rewardModel) {return rewardModel.getStateRewardVector();})
+        .def("get_state_reward", [](SparseRewardModel<ValueType>& rewardModel, uint64_t state) {return rewardModel.getStateReward(state);})
+        .def("set_state_reward", [](SparseRewardModel<ValueType>& rewardModel, uint64_t state, ValueType const& value) {return rewardModel.setStateReward(state, value);})
+        .def("get_zero_reward_states", &SparseRewardModel<ValueType>::template getStatesWithZeroReward<ValueType>, "get states where all rewards are zero", py::arg("transition_matrix"))
+        .def("get_state_action_reward", [](SparseRewardModel<ValueType>& rewardModel, uint64_t action_index) {return rewardModel.getStateActionReward(action_index);})
+        .def_property_readonly("state_action_rewards", [](SparseRewardModel<ValueType>& rewardModel) {return rewardModel.getStateActionRewardVector();})
+        .def("reduce_to_state_based_rewards", [](SparseRewardModel<ValueType>& rewardModel, storm::storage::SparseMatrix<ValueType> const& transitions, bool onlyStateRewards){return rewardModel.reduceToStateBasedRewards(transitions, onlyStateRewards);},  py::arg("transition_matrix"), py::arg("only_state_rewards"), "Reduce to state-based rewards")
     ;
 
+}
 
+void define_sparse_parametric_model(py::module& m) {
     // Parametric models
     py::class_<SparseModel<RationalFunction>, std::shared_ptr<SparseModel<RationalFunction>>, ModelBase> modelRatFunc(m, "_SparseParametricModel", "A probabilistic model where transitions are represented by rational functions and saved in a sparse matrix");
     modelRatFunc.def("collect_probability_parameters", &probabilityVariables, "Collect parameters")
         .def("collect_reward_parameters", &rewardVariables, "Collect reward parameters")
+        .def("collect_all_parameters", &allVariables, "Collect all parameters")
+        .def("get_states_with_parameter", &statesWithParameter, py::arg("parameter"), "Find states with a particular parameter")
+        .def("has_choice_labeling", [](SparseModel<RationalFunction> const& model) {return model.hasChoiceLabeling();}, "Does the model have an associated choice labelling?")
+        .def_property_readonly("choice_labeling", [](SparseModel<RationalFunction> const& model) {return model.getChoiceLabeling();}, "get choice labelling")
+        .def("has_choice_origins", [](SparseModel<RationalFunction> const& model) {return model.hasChoiceOrigins();}, "has choice origins?")
+        .def_property_readonly("choice_origins", [](SparseModel<RationalFunction> const& model) {return model.getChoiceOrigins();})
+
         .def_property_readonly("labeling", &getLabeling<RationalFunction>, "Labels")
         .def("labels_state", &SparseModel<RationalFunction>::getLabelsOfState, py::arg("state"), "Get labels of state")
         .def_property_readonly("initial_states", &getSparseInitialStates<RationalFunction>, "Initial states")
+        .def_property_readonly("initial_states_as_bitvector", [](SparseModel<RationalFunction> const& model) {return model.getInitialStates();})
         .def_property_readonly("states", [](SparseModel<RationalFunction>& model) {
                 return SparseModelStates<RationalFunction>(model);
             }, "Get states")
         .def_property_readonly("reward_models", [](SparseModel<RationalFunction> const& model) {return model.getRewardModels(); }, "Reward models")
         .def_property_readonly("transition_matrix", &getTransitionMatrix<RationalFunction>, py::return_value_policy::reference, py::keep_alive<1, 0>(), "Transition matrix")
         .def_property_readonly("backward_transition_matrix", &SparseModel<RationalFunction>::getBackwardTransitions, py::return_value_policy::reference, py::keep_alive<1, 0>(), "Backward transition matrix")
+        .def("get_reward_model", [](SparseModel<RationalFunction>& model, std::string const& name) -> SparseRewardModel<RationalFunction>& {return model.getRewardModel(name);}, py::return_value_policy::reference, py::keep_alive<1, 0>(), "Reward model")
+        .def("add_reward_model", [](SparseModel<RationalFunction>& model, std::string const& name, SparseRewardModel<RationalFunction> const& rewModel) { model.addRewardModel(name, rewModel);})
+        .def("has_state_valuations", [](SparseModel<RationalFunction> const& model) {return model.hasStateValuations();}, "has state valuation?")
+        .def_property_readonly("state_valuations",  [](SparseModel<RationalFunction> const& model) {return model.getStateValuations();}, "state valuations")
         .def("reduce_to_state_based_rewards", &SparseModel<RationalFunction>::reduceToStateBasedRewards)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricModel"))
+        .def("is_sink_state", &SparseModel<RationalFunction>::isSinkState, py::arg("state"))
+        .def("__str__", &getModelInfoPrinter)
         .def("to_dot", [](SparseModel<RationalFunction>& model) { std::stringstream ss; model.writeDotToStream(ss); return ss.str(); }, "Write dot to a string")
     ;
+    py::class_<SparseDeterministicModel<RationalFunction>, std::shared_ptr<SparseDeterministicModel<RationalFunction>>> detModelRatFunc(m, "_SparseParametricDeterministicModel", "Parametric deterministic sparse model", modelRatFunc)
+    ;
+    py::class_<SparseNondeterministicModel<RationalFunction>, std::shared_ptr<SparseNondeterministicModel<RationalFunction>>> nondetModelRatFunc(m, "_SparseParametricNondeterministicModel", "Parametric nondeterministic sparse model", modelRatFunc)
+    ;
 
-    py::class_<SparseDtmc<RationalFunction>, std::shared_ptr<SparseDtmc<RationalFunction>>>(m, "SparseParametricDtmc", "pDTMC in sparse representation", modelRatFunc)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricDTMC"))
+    py::class_<SparseDtmc<RationalFunction>, std::shared_ptr<SparseDtmc<RationalFunction>>>(m, "SparseParametricDtmc", "pDTMC in sparse representation", detModelRatFunc)
+        .def(py::init<ModelComponents<RationalFunction> const&>(), py::arg("components"))
+        .def("__str__", &getModelInfoPrinter)
+    ;
+    py::class_<SparseMdp<RationalFunction>, std::shared_ptr<SparseMdp<RationalFunction>>> pmdp(m, "SparseParametricMdp", "pMDP in sparse representation", nondetModelRatFunc);
+    pmdp.def(py::init<ModelComponents<RationalFunction> const&>(), py::arg("components"))
+        .def_property_readonly("nondeterministic_choice_indices", [](SparseMdp<RationalFunction> const& mdp) { return mdp.getNondeterministicChoiceIndices(); })
+        .def("apply_scheduler", [](SparseMdp<RationalFunction> const& mdp, storm::storage::Scheduler<RationalFunction> const& scheduler, bool dropUnreachableStates) { return mdp.applyScheduler(scheduler, dropUnreachableStates); } , "apply scheduler", "scheduler"_a, "drop_unreachable_states"_a = true)
+        .def("get_nr_available_actions", [](SparseMdp<RationalFunction> const& mdp, uint64_t stateIndex) { return mdp.getNondeterministicChoiceIndices()[stateIndex+1] - mdp.getNondeterministicChoiceIndices()[stateIndex] ; }, py::arg("state"))
+        .def("__str__", &getModelInfoPrinter)
     ;
-    py::class_<SparseMdp<RationalFunction>, std::shared_ptr<SparseMdp<RationalFunction>>>(m, "SparseParametricMdp", "pMDP in sparse representation", modelRatFunc)
-        .def_property_readonly("nondeterministic_choice_indices", [](SparseMdp<double> const& mdp) { return mdp.getNondeterministicChoiceIndices(); })
-        .def("apply_scheduler", [](SparseMdp<double> const& mdp, storm::storage::Scheduler<double> const& scheduler, bool dropUnreachableStates) { return mdp.applyScheduler(scheduler, dropUnreachableStates); } , "apply scheduler", "scheduler"_a, "drop_unreachable_states"_a = true)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricMDP"))
+
+    py::class_<SparsePomdp<RationalFunction>, std::shared_ptr<SparsePomdp<RationalFunction>>>(m, "SparseParametricPomdp", "POMDP in sparse representation", pmdp)
+
+        .def(py::init<SparsePomdp<RationalFunction>>(), py::arg("other_model"))
+        .def(py::init<ModelComponents<RationalFunction> const&>(), py::arg("components"))
+        .def("__str__", &getModelInfoPrinter)
+        .def("get_observation", &SparsePomdp<RationalFunction>::getObservation, py::arg("state"))
+        .def_property_readonly("observations", &SparsePomdp<RationalFunction>::getObservations)
+        .def_property_readonly("nr_observations", &SparsePomdp<RationalFunction>::getNrObservations)
     ;
-    py::class_<SparseCtmc<RationalFunction>, std::shared_ptr<SparseCtmc<RationalFunction>>>(m, "SparseParametricCtmc", "pCTMC in sparse representation", modelRatFunc)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricCTMC"))
+
+    py::class_<SparseCtmc<RationalFunction>, std::shared_ptr<SparseCtmc<RationalFunction>>>(m, "SparseParametricCtmc", "pCTMC in sparse representation", detModelRatFunc)
+        .def(py::init<ModelComponents<RationalFunction> const&>(), py::arg("components"))
+        .def("__str__", &getModelInfoPrinter)
     ;
-    py::class_<SparseMarkovAutomaton<RationalFunction>, std::shared_ptr<SparseMarkovAutomaton<RationalFunction>>>(m, "SparseParametricMA", "pMA in sparse representation", modelRatFunc)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricMA"))
+    py::class_<SparseMarkovAutomaton<RationalFunction>, std::shared_ptr<SparseMarkovAutomaton<RationalFunction>>>(m, "SparseParametricMA", "pMA in sparse representation", nondetModelRatFunc)
+        .def(py::init<ModelComponents<RationalFunction> const&>(), py::arg("components"))
+        .def_property_readonly("nondeterministic_choice_indices", [](SparseMarkovAutomaton<RationalFunction> const& ma) { return ma.getNondeterministicChoiceIndices(); })
+        .def("apply_scheduler", [](SparseMarkovAutomaton<RationalFunction> const& ma, storm::storage::Scheduler<RationalFunction> const& scheduler, bool dropUnreachableStates) { return ma.applyScheduler(scheduler, dropUnreachableStates); } , "apply scheduler", "scheduler"_a, "drop_unreachable_states"_a = true)
+        .def("__str__", &getModelInfoPrinter)
     ;
 
     py::class_<SparseRewardModel<RationalFunction>>(m, "SparseParametricRewardModel", "Reward structure for parametric sparse models")
-            .def_property_readonly("has_state_rewards", &SparseRewardModel<RationalFunction>::hasStateRewards)
-            .def_property_readonly("has_state_action_rewards", &SparseRewardModel<RationalFunction>::hasStateActionRewards)
-            .def_property_readonly("has_transition_rewards", &SparseRewardModel<RationalFunction>::hasTransitionRewards)
-            .def_property_readonly("transition_rewards", [](SparseRewardModel<RationalFunction>& rewardModel) {return rewardModel.getTransitionRewardMatrix();})
-            .def_property_readonly("state_rewards", [](SparseRewardModel<RationalFunction>& rewardModel) {return rewardModel.getStateRewardVector();})
-            .def("get_state_reward", [](SparseRewardModel<RationalFunction>& rewardModel, uint64_t state) {return rewardModel.getStateReward(state);})
-            .def("get_state_action_reward", [](SparseRewardModel<RationalFunction>& rewardModel, uint64_t action_index) {return rewardModel.getStateActionReward(action_index);})
+        .def_property_readonly("has_state_rewards", &SparseRewardModel<RationalFunction>::hasStateRewards)
+        .def_property_readonly("has_state_action_rewards", &SparseRewardModel<RationalFunction>::hasStateActionRewards)
+        .def_property_readonly("has_transition_rewards", &SparseRewardModel<RationalFunction>::hasTransitionRewards)
+        .def_property_readonly("transition_rewards", [](SparseRewardModel<RationalFunction>& rewardModel) {return rewardModel.getTransitionRewardMatrix();})
+        .def_property_readonly("state_rewards", [](SparseRewardModel<RationalFunction>& rewardModel) {return rewardModel.getStateRewardVector();})
+        .def("get_state_reward", [](SparseRewardModel<RationalFunction>& rewardModel, uint64_t state) {return rewardModel.getStateReward(state);})
+        .def("get_state_action_reward", [](SparseRewardModel<RationalFunction>& rewardModel, uint64_t action_index) {return rewardModel.getStateActionReward(action_index);})
 
-            .def_property_readonly("state_action_rewards", [](SparseRewardModel<RationalFunction>& rewardModel) {return rewardModel.getStateActionRewardVector();})
-            .def("reduce_to_state_based_rewards", [](SparseRewardModel<RationalFunction>& rewardModel, storm::storage::SparseMatrix<RationalFunction> const& transitions, bool onlyStateRewards){return rewardModel.reduceToStateBasedRewards(transitions, onlyStateRewards);},  py::arg("transition_matrix"), py::arg("only_state_rewards"), "Reduce to state-based rewards")
+        .def_property_readonly("state_action_rewards", [](SparseRewardModel<RationalFunction>& rewardModel) {return rewardModel.getStateActionRewardVector();})
+        .def("reduce_to_state_based_rewards", [](SparseRewardModel<RationalFunction>& rewardModel, storm::storage::SparseMatrix<RationalFunction> const& transitions, bool onlyStateRewards){return rewardModel.reduceToStateBasedRewards(transitions, onlyStateRewards);},  py::arg("transition_matrix"), py::arg("only_state_rewards"), "Reduce to state-based rewards")
     ;
 
 }
 
 
 // Bindings for symbolic models
 template<storm::dd::DdType DdType>
@@ -284,61 +383,70 @@
     std::string prefixClassName = "Symbolic" + vt_suffix;
     std::string prefixParametricClassName = "Symbolic" + vt_suffix + "Parametric";
 
 
     // Models with double numbers
     py::class_<SymbolicModel<DdType, double>, std::shared_ptr<SymbolicModel<DdType, double>>, ModelBase> model(m, ("_"+prefixClassName+"Model").c_str(), "A probabilistic model where transitions are represented by doubles and saved in a symbolic representation");
     model.def_property_readonly("reward_models", [](SymbolicModel<DdType, double>& model) {return model.getRewardModels(); }, "Reward models")
+        .def_property_readonly("dd_manager", &SymbolicModel<DdType, double>::getManager, "dd manager")
+    .def_property_readonly("reachable_states", &SymbolicModel<DdType, double>::getReachableStates, "reachable states as DD")
+        .def_property_readonly("initial_states", &SymbolicModel<DdType, double>::getInitialStates, "initial states as DD")
+        .def("get_states", [](SymbolicModel<DdType, double> const& model, storm::expressions::Expression const& expr) {return model.getStates(expr);}, py::arg("expression"), "Get states that are described by the expression")
+        .def("compute_depth", [](SymbolicModel<DdType, double> const& model) {return storm::utility::dd::computeReachableStates(model.getInitialStates(), model.getQualitativeTransitionMatrix(false), model.getRowVariables(), model.getColumnVariables()).second;}, "Computes the depth of the model, i.e., the distance to the node with the largest minimal distance from the initial states")
         .def("reduce_to_state_based_rewards", &SymbolicModel<DdType, double>::reduceToStateBasedRewards)
-        .def("__str__", getModelInfoPrinter<double>())
+        .def("__str__", &getModelInfoPrinter)
     ;
     py::class_<SymbolicDtmc<DdType, double>, std::shared_ptr<SymbolicDtmc<DdType, double>>>(m, (prefixClassName+"Dtmc").c_str(), "DTMC in symbolic representation", model)
-        .def("__str__", getModelInfoPrinter<double>("DTMC"))
+        .def("__str__", &getModelInfoPrinter)
     ;
     py::class_<SymbolicMdp<DdType, double>, std::shared_ptr<SymbolicMdp<DdType, double>>>(m, (prefixClassName+"Mdp").c_str(), "MDP in symbolic representation", model)
-        .def("__str__", getModelInfoPrinter<double>("MDP"))
+        .def("__str__", &getModelInfoPrinter)
     ;
     py::class_<SymbolicCtmc<DdType, double>, std::shared_ptr<SymbolicCtmc<DdType, double>>>(m, (prefixClassName+"Ctmc").c_str(), "CTMC in symbolic representation", model)
-        .def("__str__", getModelInfoPrinter<double>("CTMC"))
+        .def("__str__", &getModelInfoPrinter)
     ;
     py::class_<SymbolicMarkovAutomaton<DdType, double>, std::shared_ptr<SymbolicMarkovAutomaton<DdType, double>>>(m, (prefixClassName+"MA").c_str(), "MA in symbolic representation", model)
-        .def("__str__", getModelInfoPrinter<double>("MA"))
+        .def("__str__", &getModelInfoPrinter)
     ;
 
     py::class_<SymbolicRewardModel<DdType, double>>(m, (prefixClassName+"RewardModel").c_str(), "Reward structure for symbolic models")
         .def_property_readonly("has_state_rewards", &SymbolicRewardModel<DdType, double>::hasStateRewards)
         .def_property_readonly("has_state_action_rewards", &SymbolicRewardModel<DdType, double>::hasStateActionRewards)
         .def_property_readonly("has_transition_rewards", &SymbolicRewardModel<DdType, double>::hasTransitionRewards)
     ;
 
 
     // Parametric models
     py::class_<SymbolicModel<DdType, RationalFunction>, std::shared_ptr<SymbolicModel<DdType, RationalFunction>>, ModelBase> modelRatFunc(m, ("_"+prefixParametricClassName+"Model").c_str(), "A probabilistic model where transitions are represented by rational functions and saved in a symbolic representation");
-    modelRatFunc.def("collect_probability_parameters", &probabilityVariables, "Collect parameters")
-        .def("collect_reward_parameters", &rewardVariables, "Collect reward parameters")
+    modelRatFunc.def("get_parameters", &SymbolicModel<DdType, RationalFunction>::getParameters, "Get parameters")
         .def_property_readonly("reward_models", [](SymbolicModel<DdType, RationalFunction> const& model) {return model.getRewardModels(); }, "Reward models")
+        .def_property_readonly("reachable_states", &SymbolicModel<DdType, RationalFunction>::getReachableStates, "reachable states as DD")
+        .def_property_readonly("initial_states", &SymbolicModel<DdType, RationalFunction>::getInitialStates, "initial states as DD")
+        .def("get_states", [](SymbolicModel<DdType, RationalFunction> const& model, storm::expressions::Expression const& expr) {return model.getStates(expr);}, py::arg("expression"), "Get states that are described by the expression")
         .def("reduce_to_state_based_rewards", &SymbolicModel<DdType, RationalFunction>::reduceToStateBasedRewards)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricModel"))
+        .def("__str__", &getModelInfoPrinter)
     ;
 
     py::class_<SymbolicDtmc<DdType, RationalFunction>, std::shared_ptr<SymbolicDtmc<DdType, RationalFunction>>>(m, (prefixParametricClassName+"Dtmc").c_str(), "pDTMC in symbolic representation", modelRatFunc)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricDTMC"))
+        .def("__str__", &getModelInfoPrinter)
     ;
     py::class_<SymbolicMdp<DdType, RationalFunction>, std::shared_ptr<SymbolicMdp<DdType, RationalFunction>>>(m, (prefixParametricClassName+"Mdp").c_str(), "pMDP in symbolic representation", modelRatFunc)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricMDP"))
+        .def("__str__", &getModelInfoPrinter)
     ;
     py::class_<SymbolicCtmc<DdType, RationalFunction>, std::shared_ptr<SymbolicCtmc<DdType, RationalFunction>>>(m, (prefixParametricClassName+"Ctmc").c_str(), "pCTMC in symbolic representation", modelRatFunc)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricCTMC"))
+        .def("__str__", &getModelInfoPrinter)
     ;
     py::class_<SymbolicMarkovAutomaton<DdType, RationalFunction>, std::shared_ptr<SymbolicMarkovAutomaton<DdType, RationalFunction>>>(m, (prefixParametricClassName+"MA").c_str(), "pMA in symbolic representation", modelRatFunc)
-        .def("__str__", getModelInfoPrinter<RationalFunction>("ParametricMA"))
+        .def("__str__", &getModelInfoPrinter)
     ;
 
     py::class_<SymbolicRewardModel<DdType, RationalFunction>>(m, (prefixParametricClassName+"RewardModel").c_str(), "Reward structure for parametric symbolic models")
-            .def_property_readonly("has_state_rewards", &SymbolicRewardModel<DdType, RationalFunction>::hasStateRewards)
-            .def_property_readonly("has_state_action_rewards", &SymbolicRewardModel<DdType, RationalFunction>::hasStateActionRewards)
-            .def_property_readonly("has_transition_rewards", &SymbolicRewardModel<DdType, RationalFunction>::hasTransitionRewards)
+        .def_property_readonly("has_state_rewards", &SymbolicRewardModel<DdType, RationalFunction>::hasStateRewards)
+        .def_property_readonly("has_state_action_rewards", &SymbolicRewardModel<DdType, RationalFunction>::hasStateActionRewards)
+        .def_property_readonly("has_transition_rewards", &SymbolicRewardModel<DdType, RationalFunction>::hasTransitionRewards)
     ;
 
 }
 
 template void define_symbolic_model<storm::dd::DdType::Sylvan>(py::module& m, std::string vt_suffix);
+template void define_sparse_model<double>(py::module& m, std::string const& vt_suffix);
+template void define_sparse_model<storm::RationalNumber>(py::module& m, std::string const& vt_suffix);
```

### Comparing `stormpy-1.3.0/src/storage/scheduler.cpp` & `stormpy-1.8.0/src/storage/scheduler.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include "scheduler.h"
 #include "src/helpers.h"
 
+#include "storm/adapters/RationalFunctionAdapter.h"
 #include "storm/storage/Scheduler.h"
 
 template<typename ValueType>
 void define_scheduler(py::module& m, std::string vt_suffix) {
     using Scheduler = storm::storage::Scheduler<ValueType>;
     using SchedulerChoice = storm::storage::SchedulerChoice<ValueType>;
 
@@ -15,24 +16,37 @@
                 std::stringstream str;
                 s.printToStream(str);
                 return str.str();
             })
             .def_property_readonly("memoryless", &Scheduler::isMemorylessScheduler, "Is the scheduler memoryless?")
             .def_property_readonly("memory_size", &Scheduler::getNumberOfMemoryStates, "How much memory does the scheduler take?")
             .def_property_readonly("deterministic", &Scheduler::isDeterministicScheduler, "Is the scheduler deterministic?")
+            .def_property_readonly("partial", &Scheduler::isPartialScheduler, "Is the scheduler partial?")
+            .def("cast_to_double_datatype", &Scheduler::template toValueType<double>, "Construct the scheduler with `double` value type")
+            .def("cast_to_exact_datatype", &Scheduler::template toValueType<storm::RationalNumber>, "Construct the scheduler with `exact` value type")
+            .def("cast_to_parametric_datatype", &Scheduler::template toValueType<storm::RationalFunction>, "Construct the scheduler with `parametric` value type")
             .def("get_choice", &Scheduler::getChoice, py::arg("state_index"), py::arg("memory_index") = 0)
             .def("compute_action_support", &Scheduler::computeActionSupport, "nondeterministic_choice_indices"_a)
+            .def("to_json_str", [](Scheduler const& s, std::shared_ptr<storm::models::sparse::Model<ValueType>> model, bool skipUniqueChoices,
+                               bool skipDontCareStates) {
+                    std::stringstream str;
+                    s.printJsonToStream(str, model, skipUniqueChoices, skipDontCareStates);
+                    return str.str();
+                }, py::arg("model"), py::arg("skip_unique_choices") = false, py::arg("skip_dont_care_states") = false);
+
     ;
 
     std::string schedulerChoiceClassName = std::string("SchedulerChoice") + vt_suffix;
     py::class_<SchedulerChoice> schedulerChoice(m, schedulerChoiceClassName.c_str(), "A choice of a finite memory scheduler");
     schedulerChoice
         .def_property_readonly("defined", &SchedulerChoice::isDefined, "Is the choice defined by the scheduler?")
         .def_property_readonly("deterministic", &SchedulerChoice::isDeterministic, "Is the choice deterministic (given by a Dirac distribution)?")
         .def("get_deterministic_choice", &SchedulerChoice::getDeterministicChoice, "Get the deterministic choice")
         .def("get_choice", &SchedulerChoice::getChoiceAsDistribution, "Get the distribution over the actions")
         .def("__str__", &streamToString<SchedulerChoice>);
 
 }
 
 
-template void define_scheduler<double>(py::module& m, std::string vt_suffix);
+template void define_scheduler<double>(py::module& m, std::string vt_suffix);
+template void define_scheduler<storm::RationalNumber>(py::module& m, std::string vt_suffix);
+template void define_scheduler<storm::RationalFunction>(py::module& m, std::string vt_suffix);
```

### Comparing `stormpy-1.3.0/src/storage/state.cpp` & `stormpy-1.8.0/src/storage/state.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,39 @@
 #include "state.h"
 
-void define_state(py::module& m) {
+template<typename ValueType>
+void define_state(py::module& m, std::string const& vtSuffix) {
     
     // SparseModelStates
-    py::class_<SparseModelStates<double>>(m, "SparseModelStates", "States in sparse model")
-        .def("__getitem__", &SparseModelStates<double>::getState)
-        .def("__len__", &SparseModelStates<double>::getSize)
-    ;
-    py::class_<SparseModelStates<storm::RationalFunction>>(m, "SparseParametricModelStates", "States in sparse parametric model")
-        .def("__getitem__", &SparseModelStates<storm::RationalFunction>::getState)
-        .def("__len__", &SparseModelStates<storm::RationalFunction>::getSize)
+    py::class_<SparseModelStates<ValueType>>(m, ("Sparse" + vtSuffix + "ModelStates").c_str(), "States in sparse model")
+        .def("__getitem__", &SparseModelStates<ValueType>::getState)
+        .def("__len__", &SparseModelStates<ValueType>::getSize)
     ;
+
     // SparseModelState
-    py::class_<SparseModelState<double>>(m, "SparseModelState", "State in sparse model")
-        .def("__str__", &SparseModelState<double>::toString)
-        .def_property_readonly("id", &SparseModelState<double>::getIndex, "Id")
-        .def_property_readonly("labels", &SparseModelState<double>::getLabels, "Labels")
-        .def_property_readonly("actions", &SparseModelState<double>::getActions, "Get actions")
-        .def("__int__",&SparseModelState<double>::getIndex)
-    ;
-    py::class_<SparseModelState<storm::RationalFunction>>(m, "SparseParametricModelState", "State in sparse parametric model")
-        .def("__str__", &SparseModelState<storm::RationalFunction>::toString)
-        .def_property_readonly("id", &SparseModelState<storm::RationalFunction>::getIndex, "Id")
-        .def_property_readonly("labels", &SparseModelState<storm::RationalFunction>::getLabels, "Labels")
-        .def_property_readonly("actions", &SparseModelState<storm::RationalFunction>::getActions, "Get actions")
-        .def("__int__",&SparseModelState<storm::RationalFunction>::getIndex)
+    py::class_<SparseModelState<ValueType>>(m, ("Sparse" + vtSuffix + "ModelState").c_str(), "State in sparse model")
+        .def("__str__", &SparseModelState<ValueType>::toString)
+        .def_property_readonly("id", &SparseModelState<ValueType>::getIndex, "Id")
+        .def_property_readonly("labels", &SparseModelState<ValueType>::getLabels, "Labels")
+        .def_property_readonly("actions", &SparseModelState<ValueType>::getActions, "Get actions")
+        .def("__int__",&SparseModelState<ValueType>::getIndex)
     ;
-    
+
     // SparseModelActions
-    py::class_<SparseModelActions<double>>(m, "SparseModelActions", "Actions for state in sparse model")
-        .def("__getitem__", &SparseModelActions<double>::getAction)
-        .def("__len__", &SparseModelActions<double>::getSize)
-    ;
-    py::class_<SparseModelActions<storm::RationalFunction>>(m, "SparseParametricModelActions", "Actions for state in sparse parametric model")
-        .def("__getitem__", &SparseModelActions<storm::RationalFunction>::getAction)
-        .def("__len__", &SparseModelActions<storm::RationalFunction>::getSize)
+    py::class_<SparseModelActions<ValueType>>(m, ("Sparse" + vtSuffix + "ModelActions").c_str(), "Actions for state in sparse model")
+        .def("__getitem__", &SparseModelActions<ValueType>::getAction)
+        .def("__len__", &SparseModelActions<ValueType>::getSize)
     ;
+
     // SparseModelAction
-    py::class_<SparseModelAction<double>>(m, "SparseModelAction", "Action for state in sparse model")
-        .def("__str__", &SparseModelAction<double>::toString)
-        .def_property_readonly("id", &SparseModelAction<double>::getIndex, "Id")
-        .def_property_readonly("transitions", &SparseModelAction<double>::getTransitions, "Get transitions")
-    ;
-    py::class_<SparseModelAction<storm::RationalFunction>>(m, "SparseParametricModelAction", "Action for state in sparse parametric model")
-        .def("__str__", &SparseModelAction<storm::RationalFunction>::toString)
-        .def_property_readonly("id", &SparseModelAction<storm::RationalFunction>::getIndex, "Id")
-        .def_property_readonly("transitions", &SparseModelAction<storm::RationalFunction>::getTransitions, "Get transitions")
+    py::class_<SparseModelAction<ValueType>>(m, ("Sparse" + vtSuffix + "ModelAction").c_str(), "Action for state in sparse model")
+        .def("__str__", &SparseModelAction<ValueType>::toString)
+        .def_property_readonly("id", &SparseModelAction<ValueType>::getIndex, "Id")
+        .def_property_readonly("transitions", &SparseModelAction<ValueType>::getTransitions, "Get transitions")
     ;
 
 }
+
+template void define_state<double>(py::module& m, std::string const& vtSuffix);
+template void define_state<storm::RationalNumber>(py::module& m, std::string const& vtSuffix);
+template void define_state<storm::RationalFunction>(py::module& m, std::string const& vtSuffix);
+
```

### Comparing `stormpy-1.3.0/src/storage/state.h` & `stormpy-1.8.0/src/storage/state.h`

 * *Files 5% similar despite different names*

```diff
@@ -121,10 +121,11 @@
     
     private:
         s_index stateIndex;
         s_index length;
         storm::models::sparse::Model<ValueType>& model;
 };
 
-void define_state(py::module& m);
+template<typename ValueType>
+void define_state(py::module& m, std::string const& vtSuffix);
 
 #endif /* PYTHON_STORAGE_STATE_H_ */
```

### Comparing `stormpy-1.3.0/src/utility/shortestPaths.cpp` & `stormpy-1.8.0/src/utility/shortestPaths.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     using state_t                = storm::utility::ksp::state_t;
     using Matrix                 = ShortestPathsGenerator::Matrix;
     using Model                  = ShortestPathsGenerator::Model;
     using StateProbMap           = ShortestPathsGenerator::StateProbMap;
 
     py::class_<Path>(m, "Path")
         // overload constructor rather than dealing with boost::optional
-        .def("__init__", [](Path &instance, state_t preNode, unsigned long preK, double distance) {
-                new (&instance) Path { boost::optional<state_t>(preNode), preK, distance };
-            }, "predecessorNode"_a, "predecessorK"_a, "distance"_a)
+        .def(py::init([](state_t preNode, unsigned long preK, double distance) {
+                return Path { boost::optional<state_t>(preNode), preK, distance };
+            }), "predecessorNode"_a, "predecessorK"_a, "distance"_a)
 
-        .def("__init__", [](Path &instance, unsigned long preK, double distance) {
-                new (&instance) Path { boost::none, preK, distance };
-            }, "predecessorK"_a, "distance"_a)
+        .def(py::init([](unsigned long preK, double distance) {
+                return Path { boost::none, preK, distance };
+            }), "predecessorK"_a, "distance"_a)
 
         .def(py::self == py::self, "Compares predecessor node and index, ignoring distance")
 
         //.def("__str__", &streamToString<Path>)
 
         .def_readwrite("predecessorNode", &Path::predecessorNode) // TODO (un-)wrap boost::optional so it's usable
         .def_readwrite("predecessorK", &Path::predecessorK)
```

### Comparing `stormpy-1.3.0/src/utility/smtsolver.cpp` & `stormpy-1.8.0/src/utility/smtsolver.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #include "smtsolver.h"
 #include <storm/solver/Z3SmtSolver.h>
 #include "storm/storage/expressions/ExpressionManager.h"
+#include <storm/solver/SmtSolver.h>
+#include <storm/utility/solver.h>
 
 void define_smt(py::module& m) {
     using SmtSolver              = storm::solver::SmtSolver;
     using Z3SmtSolver            = storm::solver::Z3SmtSolver;
     using ModelReference         = storm::solver::SmtSolver::ModelReference;
 
     py::enum_<SmtSolver::CheckResult>(m, "SmtCheckResult", "Result type")
@@ -25,8 +27,12 @@
             .def("reset", &SmtSolver::reset, "reset")
             .def("add", [](SmtSolver& solver, storm::expressions::Expression const& expr) {solver.add(expr);}, "addconstraint")
             .def("check", &SmtSolver::check, "check")
             .def_property_readonly("model", &SmtSolver::getModel, "get the model");
 
     py::class_<Z3SmtSolver> z3solver(m, "Z3SmtSolver", "z3 API for storm smtsolver wrapper", smtsolver);
     z3solver.def(pybind11::init<storm::expressions::ExpressionManager&>());
+
+    py::class_<storm::utility::solver::SmtSolverFactory, std::shared_ptr<storm::utility::solver::SmtSolverFactory>> smtfactory(m, "SmtSolverFactory", "Factory for creating SMT Solvers");
+    py::class_<storm::utility::solver::Z3SmtSolverFactory, std::shared_ptr<storm::utility::solver::Z3SmtSolverFactory>> z3factory(m, "Z3SmtSolverFactory", "Factory for creating z3 based SMT solvers", smtfactory);
+    z3factory.def(py::init<>());
 }
```

