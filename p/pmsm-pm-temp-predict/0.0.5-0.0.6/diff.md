# Comparing `tmp/pmsm_pm_temp_predict-0.0.5.tar.gz` & `tmp/pmsm_pm_temp_predict-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmsm_pm_temp_predict-0.0.5.tar", last modified: Sun Jun 11 22:25:13 2023, max compression
+gzip compressed data, was "pmsm_pm_temp_predict-0.0.6.tar", last modified: Sun Jun 11 22:36:44 2023, max compression
```

## Comparing `pmsm_pm_temp_predict-0.0.5.tar` & `pmsm_pm_temp_predict-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 22:25:13.239526 pmsm_pm_temp_predict-0.0.5/
--rw-rw-rw-   0        0        0      704 2023-06-11 22:25:13.237525 pmsm_pm_temp_predict-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 22:25:13.224525 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict/
--rw-rw-rw-   0        0        0      119 2023-06-11 20:56:01.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict/__init__.py
--rw-rw-rw-   0        0        0      382 2023-06-11 22:25:10.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict/prediction.py
-drwxrwxrwx   0        0        0        0 2023-06-11 22:25:13.236526 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/
--rw-rw-rw-   0        0        0      704 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 22:25:13.239526 pmsm_pm_temp_predict-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1140 2023-06-11 22:23:58.000000 pmsm_pm_temp_predict-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:36:44.673198 pmsm_pm_temp_predict-0.0.6/
+-rw-rw-rw-   0        0        0     5494 2023-06-11 22:36:44.673198 pmsm_pm_temp_predict-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 22:36:44.648199 pmsm_pm_temp_predict-0.0.6/pmsm_pm_temp_predict/
+-rw-rw-rw-   0        0        0      119 2023-06-11 20:56:01.000000 pmsm_pm_temp_predict-0.0.6/pmsm_pm_temp_predict/__init__.py
+-rw-rw-rw-   0        0        0      382 2023-06-11 22:25:10.000000 pmsm_pm_temp_predict-0.0.6/pmsm_pm_temp_predict/prediction.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:36:44.671199 pmsm_pm_temp_predict-0.0.6/pmsm_pm_temp_predict.egg-info/
+-rw-rw-rw-   0        0        0     5494 2023-06-11 22:36:44.000000 pmsm_pm_temp_predict-0.0.6/pmsm_pm_temp_predict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-11 22:36:44.000000 pmsm_pm_temp_predict-0.0.6/pmsm_pm_temp_predict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 22:36:44.000000 pmsm_pm_temp_predict-0.0.6/pmsm_pm_temp_predict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-11 22:36:44.000000 pmsm_pm_temp_predict-0.0.6/pmsm_pm_temp_predict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-11 22:36:44.000000 pmsm_pm_temp_predict-0.0.6/pmsm_pm_temp_predict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 22:36:44.674201 pmsm_pm_temp_predict-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2023-06-11 22:36:41.000000 pmsm_pm_temp_predict-0.0.6/setup.py
```

