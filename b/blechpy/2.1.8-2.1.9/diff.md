# Comparing `tmp/blechpy-2.1.8.tar.gz` & `tmp/blechpy-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blechpy-2.1.8.tar", last modified: Thu Aug 19 18:52:24 2021, max compression
+gzip compressed data, was "dist/blechpy-2.1.9.tar", last modified: Thu Aug 19 19:37:38 2021, max compression
```

## Comparing `blechpy-2.1.8.tar` & `blechpy-2.1.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/
--rw-r--r--   0 roshan    (1000) roshan    (1000)      122 2021-02-02 05:13:44.000000 blechpy-2.1.8/MANIFEST.in
--rw-rw-r--   0 roshan    (1000) roshan    (1000)     8160 2021-08-19 18:52:24.000000 blechpy-2.1.8/PKG-INFO
--rw-r--r--   0 roshan    (1000) roshan    (1000)     6272 2021-08-05 17:43:24.000000 blechpy-2.1.8/README.md
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy/
--rw-r--r--   0 roshan    (1000) roshan    (1000)      379 2021-08-12 03:46:25.000000 blechpy-2.1.8/blechpy/__init__.py
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy/analysis/
--rw-r--r--   0 roshan    (1000) roshan    (1000)        0 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/__init__.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    65083 2021-08-07 17:47:58.000000 blechpy-2.1.8/blechpy/analysis/blech_clustering.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    11522 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/circus_interface.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     2734 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/clustering.py
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy/analysis/defaults/
--rw-r--r--   0 roshan    (1000) roshan    (1000)      850 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/defaults/bilateral32.prb
--rw-r--r--   0 roshan    (1000) roshan    (1000)     2797 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/defaults/default_config.params
--rw-r--r--   0 roshan    (1000) roshan    (1000)    12715 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/held_unit_analysis.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    25063 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/palatability_analysis.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    59518 2021-08-19 18:51:38.000000 blechpy-2.1.8/blechpy/analysis/poissonHMM.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    55747 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/poissonHMM_deprecated.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     9486 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/spike_analysis.py
--rw-rw-r--   0 roshan    (1000) roshan    (1000)      516 2021-08-08 16:08:41.000000 blechpy-2.1.8/blechpy/analysis/spike_detection.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    10117 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/spike_sorting.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     1220 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/analysis/stat_tests.py
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy/datastructures/
--rw-r--r--   0 roshan    (1000) roshan    (1000)        0 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/datastructures/__init__.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    53664 2021-08-13 18:52:59.000000 blechpy-2.1.8/blechpy/datastructures/dataset.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    17460 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/datastructures/experiment.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     4967 2021-08-12 03:45:46.000000 blechpy-2.1.8/blechpy/datastructures/objects.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     4567 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/datastructures/project.py
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy/dio/
--rw-r--r--   0 roshan    (1000) roshan    (1000)      118 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/__init__.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    10655 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/blech_params.py
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy/dio/defaults/
--rw-r--r--   0 roshan    (1000) roshan    (1000)      307 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/defaults/CAR_params.json
--rw-r--r--   0 roshan    (1000) roshan    (1000)     1374 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/defaults/clustering_params.json
--rw-r--r--   0 roshan    (1000) roshan    (1000)      205 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/defaults/pal_id_params.json
--rw-r--r--   0 roshan    (1000) roshan    (1000)      100 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/defaults/psth_params.json
--rw-r--r--   0 roshan    (1000) roshan    (1000)      124 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/defaults/spike_array_params.json
--rw-r--r--   0 roshan    (1000) roshan    (1000)    45951 2021-08-12 03:42:52.000000 blechpy-2.1.8/blechpy/dio/h5io.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     9845 2021-04-07 21:10:08.000000 blechpy-2.1.8/blechpy/dio/hmmIO.py
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy/dio/intanutil/
--rwxr--r--   0 roshan    (1000) roshan    (1000)        0 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/intanutil/__init__.py
--rwxr--r--   0 roshan    (1000) roshan    (1000)     2710 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/intanutil/data_to_result.py
--rwxr--r--   0 roshan    (1000) roshan    (1000)     1642 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/intanutil/get_bytes_per_data_block.py
--rwxr--r--   0 roshan    (1000) roshan    (1000)     1467 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/intanutil/notch_filter.py
--rwxr--r--   0 roshan    (1000) roshan    (1000)     1036 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/intanutil/qstring.py
--rwxr--r--   0 roshan    (1000) roshan    (1000)     6858 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/intanutil/read_header.py
--rwxr--r--   0 roshan    (1000) roshan    (1000)     3649 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/intanutil/read_one_data_block.py
--rwxr--r--   0 roshan    (1000) roshan    (1000)    10224 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/dio/load_intan_rhd_format.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     8453 2021-08-12 03:42:23.000000 blechpy-2.1.8/blechpy/dio/rawIO.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     4248 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/environment.yml
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy/plotting/
--rw-r--r--   0 roshan    (1000) roshan    (1000)      149 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/plotting/__init__.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     2822 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/plotting/blech_waveforms_datashader.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    28219 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/plotting/data_plot.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    17029 2021-03-02 21:37:34.000000 blechpy-2.1.8/blechpy/plotting/hmm_plot.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    34279 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/plotting/palatability_plot.py
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy/utils/
--rw-r--r--   0 roshan    (1000) roshan    (1000)      208 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/__init__.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)      736 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/cluster_filters.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)      970 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/data_reset.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     1418 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/decorators.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     1311 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/math_tools.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     1100 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/memory_monitor.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     3547 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/particles.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     3752 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/print_tools.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    20821 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/spike_sorting_GUI.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     5082 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/tk_widgets.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)    19601 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/userIO.py
--rw-r--r--   0 roshan    (1000) roshan    (1000)     1535 2021-02-02 05:13:44.000000 blechpy-2.1.8/blechpy/utils/write_tools.py
-drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy.egg-info/
--rw-r--r--   0 roshan    (1000) roshan    (1000)     8160 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy.egg-info/PKG-INFO
--rw-r--r--   0 roshan    (1000) roshan    (1000)     2068 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy.egg-info/SOURCES.txt
--rw-r--r--   0 roshan    (1000) roshan    (1000)        1 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy.egg-info/dependency_links.txt
--rw-r--r--   0 roshan    (1000) roshan    (1000)      393 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy.egg-info/requires.txt
--rw-r--r--   0 roshan    (1000) roshan    (1000)        8 2021-08-19 18:52:24.000000 blechpy-2.1.8/blechpy.egg-info/top_level.txt
--rw-rw-r--   0 roshan    (1000) roshan    (1000)       38 2021-08-19 18:52:24.000000 blechpy-2.1.8/setup.cfg
--rw-r--r--   0 roshan    (1000) roshan    (1000)     1235 2021-08-19 18:52:01.000000 blechpy-2.1.8/setup.py
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      122 2021-02-02 05:13:44.000000 blechpy-2.1.9/MANIFEST.in
+-rw-rw-r--   0 roshan    (1000) roshan    (1000)     8160 2021-08-19 19:37:38.000000 blechpy-2.1.9/PKG-INFO
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     6272 2021-08-05 17:43:24.000000 blechpy-2.1.9/README.md
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      379 2021-08-12 03:46:25.000000 blechpy-2.1.9/blechpy/__init__.py
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy/analysis/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)        0 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/__init__.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    65083 2021-08-07 17:47:58.000000 blechpy-2.1.9/blechpy/analysis/blech_clustering.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    11522 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/circus_interface.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     2734 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/clustering.py
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy/analysis/defaults/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      850 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/defaults/bilateral32.prb
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     2797 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/defaults/default_config.params
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    12715 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/held_unit_analysis.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    25063 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/palatability_analysis.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    59518 2021-08-19 18:51:38.000000 blechpy-2.1.9/blechpy/analysis/poissonHMM.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    55747 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/poissonHMM_deprecated.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     9486 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/spike_analysis.py
+-rw-rw-r--   0 roshan    (1000) roshan    (1000)      516 2021-08-08 16:08:41.000000 blechpy-2.1.9/blechpy/analysis/spike_detection.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    10117 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/spike_sorting.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     1220 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/analysis/stat_tests.py
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy/datastructures/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)        0 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/datastructures/__init__.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    53664 2021-08-13 18:52:59.000000 blechpy-2.1.9/blechpy/datastructures/dataset.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    17460 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/datastructures/experiment.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     4967 2021-08-12 03:45:46.000000 blechpy-2.1.9/blechpy/datastructures/objects.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     4567 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/datastructures/project.py
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy/dio/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      118 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/__init__.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    10655 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/blech_params.py
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy/dio/defaults/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      844 2021-08-19 19:36:27.000000 blechpy-2.1.9/blechpy/dio/defaults/CAR_params.json
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     1374 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/defaults/clustering_params.json
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      205 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/defaults/pal_id_params.json
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      100 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/defaults/psth_params.json
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      124 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/defaults/spike_array_params.json
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    45951 2021-08-12 03:42:52.000000 blechpy-2.1.9/blechpy/dio/h5io.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     9845 2021-04-07 21:10:08.000000 blechpy-2.1.9/blechpy/dio/hmmIO.py
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy/dio/intanutil/
+-rwxr--r--   0 roshan    (1000) roshan    (1000)        0 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/intanutil/__init__.py
+-rwxr--r--   0 roshan    (1000) roshan    (1000)     2710 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/intanutil/data_to_result.py
+-rwxr--r--   0 roshan    (1000) roshan    (1000)     1642 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/intanutil/get_bytes_per_data_block.py
+-rwxr--r--   0 roshan    (1000) roshan    (1000)     1467 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/intanutil/notch_filter.py
+-rwxr--r--   0 roshan    (1000) roshan    (1000)     1036 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/intanutil/qstring.py
+-rwxr--r--   0 roshan    (1000) roshan    (1000)     6858 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/intanutil/read_header.py
+-rwxr--r--   0 roshan    (1000) roshan    (1000)     3649 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/intanutil/read_one_data_block.py
+-rwxr--r--   0 roshan    (1000) roshan    (1000)    10224 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/dio/load_intan_rhd_format.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     8453 2021-08-12 03:42:23.000000 blechpy-2.1.9/blechpy/dio/rawIO.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     4248 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/environment.yml
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy/plotting/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      149 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/plotting/__init__.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     2822 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/plotting/blech_waveforms_datashader.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    28219 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/plotting/data_plot.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    17029 2021-03-02 21:37:34.000000 blechpy-2.1.9/blechpy/plotting/hmm_plot.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    34279 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/plotting/palatability_plot.py
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy/utils/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      208 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/__init__.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      736 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/cluster_filters.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      970 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/data_reset.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     1418 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/decorators.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     1311 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/math_tools.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     1100 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/memory_monitor.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     3547 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/particles.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     3752 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/print_tools.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    20821 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/spike_sorting_GUI.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     5082 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/tk_widgets.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)    19601 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/userIO.py
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     1535 2021-02-02 05:13:44.000000 blechpy-2.1.9/blechpy/utils/write_tools.py
+drwxrwxr-x   0 roshan    (1000) roshan    (1000)        0 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy.egg-info/
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     8160 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy.egg-info/PKG-INFO
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     2068 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 roshan    (1000) roshan    (1000)        1 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 roshan    (1000) roshan    (1000)      393 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy.egg-info/requires.txt
+-rw-r--r--   0 roshan    (1000) roshan    (1000)        8 2021-08-19 19:37:38.000000 blechpy-2.1.9/blechpy.egg-info/top_level.txt
+-rw-rw-r--   0 roshan    (1000) roshan    (1000)       38 2021-08-19 19:37:38.000000 blechpy-2.1.9/setup.cfg
+-rw-r--r--   0 roshan    (1000) roshan    (1000)     1235 2021-08-19 19:37:16.000000 blechpy-2.1.9/setup.py
```

### Comparing `blechpy-2.1.8/PKG-INFO` & `blechpy-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blechpy
-Version: 2.1.8
+Version: 2.1.9
 Summary: Package for exrtacting, processing and analyzing Intan and OpenEphys data
 Home-page: https://github.com/nubs01/blechpy
 Author: Roshan Nanu
 Author-email: roshan.nanu@gmail.com
 License: UNKNOWN
 Description: See the <a href='https://nubs01.github.io/blechpy'>full documentation</a> here.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blechpy Version: 2.1.8 Summary: Package for
+Metadata-Version: 2.1 Name: blechpy Version: 2.1.9 Summary: Package for
 exrtacting, processing and analyzing Intan and OpenEphys data Home-page: https:
 //github.com/nubs01/blechpy Author: Roshan Nanu Author-email:
 roshan.nanu@gmail.com License: UNKNOWN Description: See the full_documentation
 here. - [blechpy](#blechpy) - [Installation](#installation) - [Usage](#usage) -
 [Datasets](#datasets) * [Starting wit a raw dataset](#starting-wit-a-raw-
 dataset) + [Create dataset](#create-dataset) + [Initialize Parameters]
 (#initialize-parameters) + [Basic Processing](#basic-processing) + [Viewing a
```

### Comparing `blechpy-2.1.8/README.md` & `blechpy-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/blech_clustering.py` & `blechpy-2.1.9/blechpy/analysis/blech_clustering.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/circus_interface.py` & `blechpy-2.1.9/blechpy/analysis/circus_interface.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/clustering.py` & `blechpy-2.1.9/blechpy/analysis/clustering.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/defaults/bilateral32.prb` & `blechpy-2.1.9/blechpy/analysis/defaults/bilateral32.prb`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/defaults/default_config.params` & `blechpy-2.1.9/blechpy/analysis/defaults/default_config.params`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/held_unit_analysis.py` & `blechpy-2.1.9/blechpy/analysis/held_unit_analysis.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/palatability_analysis.py` & `blechpy-2.1.9/blechpy/analysis/palatability_analysis.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/poissonHMM.py` & `blechpy-2.1.9/blechpy/analysis/poissonHMM.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/poissonHMM_deprecated.py` & `blechpy-2.1.9/blechpy/analysis/poissonHMM_deprecated.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/spike_analysis.py` & `blechpy-2.1.9/blechpy/analysis/spike_analysis.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/spike_detection.py` & `blechpy-2.1.9/blechpy/analysis/spike_detection.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/spike_sorting.py` & `blechpy-2.1.9/blechpy/analysis/spike_sorting.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/analysis/stat_tests.py` & `blechpy-2.1.9/blechpy/analysis/stat_tests.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/datastructures/dataset.py` & `blechpy-2.1.9/blechpy/datastructures/dataset.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/datastructures/experiment.py` & `blechpy-2.1.9/blechpy/datastructures/experiment.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/datastructures/objects.py` & `blechpy-2.1.9/blechpy/datastructures/objects.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/datastructures/project.py` & `blechpy-2.1.9/blechpy/datastructures/project.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/blech_params.py` & `blechpy-2.1.9/blechpy/dio/blech_params.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/defaults/clustering_params.json` & `blechpy-2.1.9/blechpy/dio/defaults/clustering_params.json`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/h5io.py` & `blechpy-2.1.9/blechpy/dio/h5io.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/hmmIO.py` & `blechpy-2.1.9/blechpy/dio/hmmIO.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/intanutil/data_to_result.py` & `blechpy-2.1.9/blechpy/dio/intanutil/data_to_result.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/intanutil/get_bytes_per_data_block.py` & `blechpy-2.1.9/blechpy/dio/intanutil/get_bytes_per_data_block.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/intanutil/notch_filter.py` & `blechpy-2.1.9/blechpy/dio/intanutil/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/intanutil/qstring.py` & `blechpy-2.1.9/blechpy/dio/intanutil/qstring.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/intanutil/read_header.py` & `blechpy-2.1.9/blechpy/dio/intanutil/read_header.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/intanutil/read_one_data_block.py` & `blechpy-2.1.9/blechpy/dio/intanutil/read_one_data_block.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/load_intan_rhd_format.py` & `blechpy-2.1.9/blechpy/dio/load_intan_rhd_format.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/dio/rawIO.py` & `blechpy-2.1.9/blechpy/dio/rawIO.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/environment.yml` & `blechpy-2.1.9/blechpy/environment.yml`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/plotting/blech_waveforms_datashader.py` & `blechpy-2.1.9/blechpy/plotting/blech_waveforms_datashader.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/plotting/data_plot.py` & `blechpy-2.1.9/blechpy/plotting/data_plot.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/plotting/hmm_plot.py` & `blechpy-2.1.9/blechpy/plotting/hmm_plot.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/plotting/palatability_plot.py` & `blechpy-2.1.9/blechpy/plotting/palatability_plot.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/cluster_filters.py` & `blechpy-2.1.9/blechpy/utils/cluster_filters.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/data_reset.py` & `blechpy-2.1.9/blechpy/utils/data_reset.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/decorators.py` & `blechpy-2.1.9/blechpy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/math_tools.py` & `blechpy-2.1.9/blechpy/utils/math_tools.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/memory_monitor.py` & `blechpy-2.1.9/blechpy/utils/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/particles.py` & `blechpy-2.1.9/blechpy/utils/particles.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/print_tools.py` & `blechpy-2.1.9/blechpy/utils/print_tools.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/spike_sorting_GUI.py` & `blechpy-2.1.9/blechpy/utils/spike_sorting_GUI.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/tk_widgets.py` & `blechpy-2.1.9/blechpy/utils/tk_widgets.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/userIO.py` & `blechpy-2.1.9/blechpy/utils/userIO.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy/utils/write_tools.py` & `blechpy-2.1.9/blechpy/utils/write_tools.py`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/blechpy.egg-info/PKG-INFO` & `blechpy-2.1.9/blechpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blechpy
-Version: 2.1.8
+Version: 2.1.9
 Summary: Package for exrtacting, processing and analyzing Intan and OpenEphys data
 Home-page: https://github.com/nubs01/blechpy
 Author: Roshan Nanu
 Author-email: roshan.nanu@gmail.com
 License: UNKNOWN
 Description: See the <a href='https://nubs01.github.io/blechpy'>full documentation</a> here.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blechpy Version: 2.1.8 Summary: Package for
+Metadata-Version: 2.1 Name: blechpy Version: 2.1.9 Summary: Package for
 exrtacting, processing and analyzing Intan and OpenEphys data Home-page: https:
 //github.com/nubs01/blechpy Author: Roshan Nanu Author-email:
 roshan.nanu@gmail.com License: UNKNOWN Description: See the full_documentation
 here. - [blechpy](#blechpy) - [Installation](#installation) - [Usage](#usage) -
 [Datasets](#datasets) * [Starting wit a raw dataset](#starting-wit-a-raw-
 dataset) + [Create dataset](#create-dataset) + [Initialize Parameters]
 (#initialize-parameters) + [Basic Processing](#basic-processing) + [Viewing a
```

### Comparing `blechpy-2.1.8/blechpy.egg-info/SOURCES.txt` & `blechpy-2.1.9/blechpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blechpy-2.1.8/setup.py` & `blechpy-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = [] # Examples: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirementPath):
     with open(requirementPath) as f:
         install_requires = f.read().splitlines()
 
 setuptools.setup(
     name='blechpy',
-    version='2.1.8',
+    version='2.1.9',
     author='Roshan Nanu',
     author_email='roshan.nanu@gmail.com',
     description='Package for exrtacting, processing and analyzing Intan and OpenEphys data',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/nubs01/blechpy',
     packages=setuptools.find_packages(),
```

