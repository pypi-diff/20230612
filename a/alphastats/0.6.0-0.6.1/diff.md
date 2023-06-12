# Comparing `tmp/alphastats-0.6.0.tar.gz` & `tmp/alphastats-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphastats-0.6.0.tar", last modified: Wed May 31 13:55:36 2023, max compression
+gzip compressed data, was "alphastats-0.6.1.tar", last modified: Mon Jun 12 17:39:16 2023, max compression
```

## Comparing `alphastats-0.6.0.tar` & `alphastats-0.6.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-31 13:55:10.000000 alphastats-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 13:55:10.000000 alphastats-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-31 13:55:36.877228 alphastats-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-31 13:55:10.000000 alphastats-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet_Plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet_Preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet_Statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/data/contaminations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/gui/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/AlphaPeptStats.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/alphapeptstats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/alphastats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/alphastats_logo_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/02_Import Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/03_Data Overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/03_Preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/04_Analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/06_Results.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/gui/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/sample_data/metadata.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/sample_data/proteinGroups.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/utils/analysis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/utils/software_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/utils/ui_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/loader/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/AlphaPeptLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/BaseLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/DIANNLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/FragPipeLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/MaxQuantLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/SpectronautLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/mzTabLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/multicova/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/multicova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/multicova/multicova.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/ClusterMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/DimensionalityReduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/IntensityPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/PlotUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/SampleHistogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/VolcanoPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/statistics/Anova.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/statistics/DifferentialExpressionAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/statistics/MultiCovaAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/statistics/StatisticUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:55:36.877228 alphastats-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-31 13:55:10.000000 alphastats-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-05-31 13:55:10.000000 alphastats-0.6.0/tests/test_DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-31 13:55:10.000000 alphastats-0.6.0/tests/test_DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-31 13:55:10.000000 alphastats-0.6.0/tests/test_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.418555 alphastats-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-12 17:38:35.000000 alphastats-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 17:38:35.000000 alphastats-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-12 17:39:16.418555 alphastats-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-12 17:38:35.000000 alphastats-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.398555 alphastats-0.6.1/alphastats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet_Plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet_Preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet_Statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/data/contaminations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/gui/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/AlphaPeptStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/alphapeptstats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/alphastats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/alphastats_logo_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/02_Import Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/03_Data Overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/03_Preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/04_Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/06_Results.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/gui/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/sample_data/metadata.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/sample_data/proteinGroups.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/utils/analysis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/utils/software_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/utils/ui_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/AlphaPeptLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/BaseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/DIANNLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/FragPipeLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/MaxQuantLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/SpectronautLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/mzTabLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/multicova/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/multicova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/multicova/multicova.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/ClusterMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/DimensionalityReduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/IntensityPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/PlotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/SampleHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/VolcanoPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/statistics/Anova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/statistics/DifferentialExpressionAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/statistics/MultiCovaAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/statistics/StatisticUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.398555 alphastats-0.6.1/alphastats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:39:16.418555 alphastats-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-12 17:38:36.000000 alphastats-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.418555 alphastats-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-06-12 17:38:36.000000 alphastats-0.6.1/tests/test_DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-12 17:38:36.000000 alphastats-0.6.1/tests/test_DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-12 17:38:36.000000 alphastats-0.6.1/tests/test_loaders.py
```

### Comparing `alphastats-0.6.0/LICENSE.txt` & `alphastats-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/PKG-INFO` & `alphastats-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.0
+Version: 0.6.1
 Summary: An open-source Python package for Mass Spectrometry Analysis
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@hotmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
```

### Comparing `alphastats-0.6.0/README.md` & `alphastats-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/DataSet.py` & `alphastats-0.6.1/alphastats/DataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,15 @@
         # remove Intensity so only sample names remain
         substring_to_remove = regex_find_intensity_columns.replace(".*", "")
         df.columns = df.columns.str.replace(substring_to_remove, "")
         # transpose dataframe
         mat = df.transpose()
         # remove proteins with only zero
         self.mat = mat.loc[:, (mat != 0).any(axis=0)]
+        self.mat = self.mat.astype(float)
         # reset preproccessing info
         self.preprocessing_info = self._save_dataset_info()
         self.preprocessed = False
         self.rawmat = mat
 
     def load_metadata(self, file_path):
         """Load metadata either xlsx, txt, csv or txt file
```

### Comparing `alphastats-0.6.0/alphastats/DataSet_Pathway.py` & `alphastats-0.6.1/alphastats/DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/DataSet_Plot.py` & `alphastats-0.6.1/alphastats/DataSet_Plot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/DataSet_Preprocess.py` & `alphastats-0.6.1/alphastats/DataSet_Preprocess.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/DataSet_Statistics.py` & `alphastats-0.6.1/alphastats/DataSet_Statistics.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/__init__.py` & `alphastats-0.6.1/alphastats/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __project__ = "alphastats"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __license__ = "Apache"
 __description__ = "An open-source Python package for Mass Spectrometry Analysis"
 __author__ = "Mann Labs"
 __author_email__ = "elena.krismer@hotmail.com"
 __github__ = "https://github.com/MannLabs/alphapeptstats"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `alphastats-0.6.0/alphastats/data/contaminations.txt` & `alphastats-0.6.1/alphastats/data/contaminations.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/AlphaPeptStats.py` & `alphastats-0.6.1/alphastats/gui/AlphaPeptStats.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/alphapeptstats_logo.png` & `alphastats-0.6.1/alphastats/gui/alphapeptstats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/alphastats_logo.png` & `alphastats-0.6.1/alphastats/gui/alphastats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/alphastats_logo_2.png` & `alphastats-0.6.1/alphastats/gui/alphastats_logo_2.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/gui.py` & `alphastats-0.6.1/alphastats/gui/gui.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/pages/02_Import Data.py` & `alphastats-0.6.1/alphastats/gui/pages/02_Import Data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/pages/03_Data Overview.py` & `alphastats-0.6.1/alphastats/gui/pages/03_Data Overview.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/pages/03_Preprocessing.py` & `alphastats-0.6.1/alphastats/gui/pages/03_Preprocessing.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/pages/04_Analysis.py` & `alphastats-0.6.1/alphastats/gui/pages/04_Analysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/pages/06_Results.py` & `alphastats-0.6.1/alphastats/gui/pages/06_Results.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/sample_data/metadata.xlsx` & `alphastats-0.6.1/alphastats/gui/sample_data/metadata.xlsx`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/sample_data/proteinGroups.txt` & `alphastats-0.6.1/alphastats/gui/sample_data/proteinGroups.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/utils/analysis_helper.py` & `alphastats-0.6.1/alphastats/gui/utils/analysis_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/utils/options.py` & `alphastats-0.6.1/alphastats/gui/utils/options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/utils/software_options.py` & `alphastats-0.6.1/alphastats/gui/utils/software_options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/gui/utils/ui_helper.py` & `alphastats-0.6.1/alphastats/gui/utils/ui_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/load_data.py` & `alphastats-0.6.1/alphastats/load_data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/loader/AlphaPeptLoader.py` & `alphastats-0.6.1/alphastats/loader/AlphaPeptLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/loader/BaseLoader.py` & `alphastats-0.6.1/alphastats/loader/BaseLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/loader/DIANNLoader.py` & `alphastats-0.6.1/alphastats/loader/DIANNLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/loader/FragPipeLoader.py` & `alphastats-0.6.1/alphastats/loader/FragPipeLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/loader/MaxQuantLoader.py` & `alphastats-0.6.1/alphastats/loader/MaxQuantLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/loader/SpectronautLoader.py` & `alphastats-0.6.1/alphastats/loader/SpectronautLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/loader/mzTabLoader.py` & `alphastats-0.6.1/alphastats/loader/mzTabLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/multicova/multicova.py` & `alphastats-0.6.1/alphastats/multicova/multicova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/plots/ClusterMap.py` & `alphastats-0.6.1/alphastats/plots/ClusterMap.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/plots/DimensionalityReduction.py` & `alphastats-0.6.1/alphastats/plots/DimensionalityReduction.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/plots/IntensityPlot.py` & `alphastats-0.6.1/alphastats/plots/IntensityPlot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/plots/PlotUtils.py` & `alphastats-0.6.1/alphastats/plots/PlotUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/plots/SampleHistogram.py` & `alphastats-0.6.1/alphastats/plots/SampleHistogram.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/plots/VolcanoPlot.py` & `alphastats-0.6.1/alphastats/plots/VolcanoPlot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/statistics/Anova.py` & `alphastats-0.6.1/alphastats/statistics/Anova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/statistics/DifferentialExpressionAnalysis.py` & `alphastats-0.6.1/alphastats/statistics/DifferentialExpressionAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/statistics/MultiCovaAnalysis.py` & `alphastats-0.6.1/alphastats/statistics/MultiCovaAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/statistics/StatisticUtils.py` & `alphastats-0.6.1/alphastats/statistics/StatisticUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats/utils.py` & `alphastats-0.6.1/alphastats/utils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/alphastats.egg-info/PKG-INFO` & `alphastats-0.6.1/alphastats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.0
+Version: 0.6.1
 Summary: An open-source Python package for Mass Spectrometry Analysis
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@hotmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
```

### Comparing `alphastats-0.6.0/alphastats.egg-info/SOURCES.txt` & `alphastats-0.6.1/alphastats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/setup.py` & `alphastats-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return required
     
 
 def create_pip_wheel():
     requirements = get_requirements()
     setuptools.setup(
         name="alphastats",
-        version="0.6.0",
+        version="0.6.1",
         license="Apache",
         description="An open-source Python package for Mass Spectrometry Analysis",
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
         author="Mann Labs",
         author_email="elena.krismer@hotmail.com",
         url="https://github.com/MannLabs/alphastats",
```

### Comparing `alphastats-0.6.0/tests/test_DataSet.py` & `alphastats-0.6.1/tests/test_DataSet.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/tests/test_DataSet_Pathway.py` & `alphastats-0.6.1/tests/test_DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.0/tests/test_loaders.py` & `alphastats-0.6.1/tests/test_loaders.py`

 * *Files identical despite different names*

