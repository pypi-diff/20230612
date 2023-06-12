# Comparing `tmp/bayes-optim-0.2.5.8.tar.gz` & `tmp/bayes-optim-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayes-optim-0.2.5.8.tar", last modified: Tue Sep 28 11:59:36 2021, max compression
+gzip compressed data, was "bayes-optim-0.2.6.tar", last modified: Mon Nov 15 19:47:02 2021, max compression
```

## Comparing `bayes-optim-0.2.5.8.tar` & `bayes-optim-0.2.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.997809 bayes-optim-0.2.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15314 2021-09-28 11:59:35.997809 bayes-optim-0.2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13507 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.989809 bayes-optim-0.2.5.8/bayes_optim/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7092 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6255 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8291 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/acquisition_fun.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.989809 bayes-optim-0.2.5.8/bayes_optim/acquisition_optim/
--rw-r--r--   0 runner    (1001) docker     (121)     4728 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/acquisition_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13254 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/acquisition_optim/mies.py
--rw-r--r--   0 runner    (1001) docker     (121)    16580 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/acquisition_optim/one_plus_one_cma_es.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/acquisition_optim/option.py
--rw-r--r--   0 runner    (1001) docker     (121)    21071 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7305 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/bayes_opt.py
--rw-r--r--   0 runner    (1001) docker     (121)    13349 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     9420 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/mobo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.989809 bayes-optim-0.2.5.8/bayes_optim/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/multi_objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10653 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/multi_objective/analytic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.989809 bayes-optim-0.2.5.8/bayes_optim/search_space/
--rw-r--r--   0 runner    (1001) docker     (121)      511 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/search_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6389 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/search_space/node.py
--rw-r--r--   0 runner    (1001) docker     (121)    10723 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/search_space/samplers.py
--rw-r--r--   0 runner    (1001) docker     (121)    31705 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/search_space/search_space.py
--rw-r--r--   0 runner    (1001) docker     (121)    11311 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/search_space/variable.py
--rw-r--r--   0 runner    (1001) docker     (121)    15009 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.993809 bayes-optim-0.2.5.8/bayes_optim/surrogate/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/surrogate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.993809 bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/
--rwxr-xr-x   0 runner    (1001) docker     (121)      199 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      997 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/boundary_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23105 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/cma_es.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    48464 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/gpr.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13111 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/kernel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6352 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/trend.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6507 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/surrogate/random_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.993809 bayes-optim-0.2.5.8/bayes_optim/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      585 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6620 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/_daemon.py
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.997809 bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.997809 bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/box_decompositions/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/box_decompositions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11722 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/box_decompositions/box_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (121)    18713 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/box_decompositions/non_dominated.py
--rw-r--r--   0 runner    (1001) docker     (121)    12382 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/box_decompositions/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10328 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/pareto.py
--rw-r--r--   0 runner    (1001) docker     (121)    10187 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/bayes_optim/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 11:59:35.989809 bayes-optim-0.2.5.8/bayes_optim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15314 2021-09-28 11:59:35.000000 bayes-optim-0.2.5.8/bayes_optim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2021-09-28 11:59:35.000000 bayes-optim-0.2.5.8/bayes_optim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-28 11:59:35.000000 bayes-optim-0.2.5.8/bayes_optim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      236 2021-09-28 11:59:35.000000 bayes-optim-0.2.5.8/bayes_optim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-28 11:59:35.000000 bayes-optim-0.2.5.8/bayes_optim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-28 11:59:35.997809 bayes-optim-0.2.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-09-28 11:59:32.000000 bayes-optim-0.2.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    15312 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13507 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.716856 bayes-optim-0.2.6/bayes_optim/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6079 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6255 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8339 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_fun.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/acquisition_optim/
+-rw-r--r--   0 runner    (1001) docker     (121)     4728 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13254 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_optim/mies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16493 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_optim/one_plus_one_cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_optim/option.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20896 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7305 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/bayes_opt.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13034 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/extension.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9311 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/mobo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/multi_objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10653 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/multi_objective/analytic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/search_space/
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6389 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11076 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31705 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11527 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15009 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/surrogate/
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8220 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      997 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/boundary_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    23105 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/cma_es.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    48464 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/gpr.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13111 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/kernel.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6352 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/trend.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6507 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5706 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/random_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/bayes_optim/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6620 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2233 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11722 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/box_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18713 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/non_dominated.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12382 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10328 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3054 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10351 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.716856 bayes-optim-0.2.6/bayes_optim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15312 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/setup.py
```

### Comparing `bayes-optim-0.2.5.8/LICENSE` & `bayes-optim-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/PKG-INFO` & `bayes-optim-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes-optim
-Version: 0.2.5.8
+Version: 0.2.6
 Summary: A Bayesian Optimization Library
 Home-page: https://github.com/wangronin/Bayesian-Optimization
 Author: Hao Wang
 Author-email: wangronin@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/wangronin/Bayesian-Optimization/archive/v0.1.3.tar.gz
 Description: [![Actions Status](https://github.com/wangronin/Bayesian-Optimization/workflows/Build%20and%20Test/badge.svg)](https://github.com/wangronin/Bayesian-Optimization/actions)
```

### Comparing `bayes-optim-0.2.5.8/README.md` & `bayes-optim-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/__init__.py` & `bayes-optim-0.2.6/bayes_optim/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,19 +64,19 @@
     func: Callable,
     lower: Union[float, Vector],
     upper: Union[float, Vector],
     x0: Union[int, Matrix, np.ndarray, None] = None,
     y0: Union[Vector, None] = None,
     n_point: int = 1,
     args: Tuple = (),
-    xtol: float = 1e-4,
-    ftol: float = 1e-4,
+    # xtol: float = 1e-4,
+    # ftol: float = 1e-4,
     max_FEs: Optional[int] = None,
     verbose: Optional[bool] = False,
-    callback: Optional[Callable] = None,
+    # callback: Optional[Callable] = None,
     seed: Optional[int] = None,
     **kwargs,
 ) -> Tuple[Vector, float, int, int, List[np.ndarray]]:
     """Minimize a function using the Bayesian Optimization algorithm, which only uses
     function values, not derivatives or second derivatives. This function maintains an
     interface similar to `scipy.optimize.fmin`. Hereafter, we use the following customized
     types to describe the usage:
@@ -101,27 +101,18 @@
     y0 : Union[Vector, None], optional
         When `x0` is a 2d numpy array, it contains the function values pertaining to `x0`;
         Otherwise, it is ignored. It is by default None.
     n_point : int, optional
         The number of trial points generated in each iteration, by default 1
     args : Tuple, optional
         Extra arguments passed to `func`, i.e., ``func(x, *args)``.
-    xtol : float, optional
-        Absolute error in xopt between iterations that is acceptable for convergence,
-        by default 1e-4.
-    ftol : float, optional
-        Absolute error in func(xopt) between iterations that is acceptable for convergence,
-        by default 1e-4.
     max_FEs : Optional[int], optional
         Maximal number of function evaluations to make, by default None.
     verbose : Optional[bool], optional
         Verbosity of the output, by default False.
-    callback : Optional[Callable], optional
-        Called after each iteration, as `callback(X)`, where `X` is the current parameter
-        vectors, by default None.
     seed : Optional[int], optional
         Seeding the random number generator in `numpy`, by default None.
 
     Returns
     -------
     Tuple[Vector, float, int, int, List[np.ndarray]]
         The return value contains:
@@ -148,39 +139,22 @@
     if seed is not None:
         _state = np.random.get_state()
         np.random.seed(seed)
 
     obj_func = lambda x: func(x, *args)
 
     if isinstance(lower, float) and isinstance(upper, float):
-        dim = 1
         space = RealSpace([lower, upper])
     elif isinstance(lower, list) and isinstance(upper, list):
         assert len(lower) == len(upper)
-        dim = len(lower)
         space = RealSpace(list(zip(lower, upper)))
-        lower, upper = np.array(lower), np.array(upper)
 
-    mean = trend.constant_trend(dim, beta=0)
-    thetaL = 1e-10 * (upper - lower) * np.ones(dim)
-    thetaU = 10 * (upper - lower) * np.ones(dim)
-    theta0 = np.random.rand(dim) * (thetaU - thetaL) + thetaL
     model = GaussianProcess(
-        mean=mean,
-        corr="squared_exponential",
-        theta0=theta0,
-        thetaL=thetaL,
-        thetaU=thetaU,
-        nugget=0,
-        noise_estim=False,
-        optimizer="BFGS",
-        wait_iter=3,
-        random_start=dim,
-        likelihood="concentrated",
-        eval_budget=100 * dim,
+        domain=space,
+        n_restarts_optimizer=space.dim,
     )
 
     # set up the warm-starting and DoE size
     if isinstance(x0, int):
         DoE_size = x0
         warm_data = ()
     elif hasattr(x0, "__iter__"):
@@ -199,30 +173,27 @@
         model=model,
         DoE_size=DoE_size,
         warm_data=warm_data,
         eval_type="list",
         max_FEs=max_FEs,
         verbose=verbose,
         n_point=n_point,
+        **kwargs,
     )
     opt.run()
 
     if seed is not None:
         np.random.set_state(_state)
 
     N, n = opt.DoE_size, opt.n_point
     _data, data = opt.data[:N, :], opt.data[N:, :]
 
     data_per_iteration = [np.asarray(data[:N, :])]
-    data_per_iteration += [
-        np.asarray(data[(i * n) : ((i + 1) * n), :]) for i in range(opt.iter_count - 1)
-    ]
+    data_per_iteration += [np.asarray(data[(i * n) : ((i + 1) * n), :]) for i in range(opt.iter_count - 1)]
 
     print(
         "Optimization terminated successfully.\n"
         "        Current function value: {}\n"
         "        Iterations: {}\n"
-        "        Function evaluations: {}\n".format(
-            opt.xopt.fitness, opt.iter_count, opt.eval_count
-        )
+        "        Function evaluations: {}\n".format(opt.xopt.fitness, opt.iter_count, opt.eval_count)
     )
     return opt.xopt, opt.xopt.fitness, opt.iter_count, opt.eval_count, data_per_iteration
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/_base.py` & `bayes-optim-0.2.6/bayes_optim/_base.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/acquisition_fun.py` & `bayes-optim-0.2.6/bayes_optim/acquisition_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
         if not self.minimize:
             y_hat = -y_hat
         return y_hat, sd
 
     def _gradient(self, X):
         X_ = np.array(X, dtype=float)
         y_dx, sd2_dx = self._model.gradient(X_)
+        y_dx = y_dx.T
+        sd2_dx = sd2_dx.T
         if not self.minimize:
             y_dx = -y_dx
         return y_dx, sd2_dx
 
     def check_X(self, X):
         """Keep input as '2D' object"""
         return np.atleast_2d(X)
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/acquisition_optim/__init__.py` & `bayes-optim-0.2.6/bayes_optim/acquisition_optim/__init__.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/acquisition_optim/mies.py` & `bayes-optim-0.2.6/bayes_optim/acquisition_optim/mies.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/acquisition_optim/one_plus_one_cma_es.py` & `bayes-optim-0.2.6/bayes_optim/acquisition_optim/one_plus_one_cma_es.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,27 +378,23 @@
 
     def _update_covariance(self, z):
         if self.success_rate < self.threshold:
             self.pc = (1 - self.cc) * self.pc + np.sqrt(self._coeff) * z
             self._C = (1 - self.ccov) * self._C + self.ccov * np.outer(self.pc, self.pc)
         else:
             self.pc = (1 - self.cc) * self.pc
-            self._C = (1 - self.ccov * (1 - self._coeff)) * self._C + self.ccov * np.outer(
-                self.pc, self.pc
-            )
+            self._C = (1 - self.ccov * (1 - self._coeff)) * self._C + self.ccov * np.outer(self.pc, self.pc)
 
         self._C = np.triu(self._C) + np.triu(self._C, 1).T
         self._update_A(self._C)
 
     def _update_step_size(self, success):
         prob_target = self.prob_target
         self.success_rate = (1 - self.cp) * self.success_rate + self.cp * success
         self._sigma *= np.exp((self.success_rate - prob_target) / (1 - prob_target) / self.d)
-        if self._sigma is None:
-            breakpoint()
 
     def _update_A(self, C):
         if np.any(np.isinf(C)):
             self._exception = True
         else:
             try:
                 A = np.linalg.cholesky(C)
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/base.py` & `bayes-optim-0.2.6/bayes_optim/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 from sklearn.metrics import mean_absolute_percentage_error, r2_score
 
 from bayes_optim.utils.logger import dump_logger, load_logger
 
 from . import acquisition_fun as AcquisitionFunction
 from ._base import BaseOptimizer
 from .acquisition_optim import argmax_restart
-from .acquisition_optim.option import (
-    default_AQ_max_FEs,
-    default_AQ_n_restart,
-    default_AQ_wait_iter,
-)
+from .acquisition_optim.option import default_AQ_max_FEs, default_AQ_n_restart, default_AQ_wait_iter
 from .search_space import RealSpace
 from .solution import Solution
 from .utils import (
     arg_to_int,
     dynamic_penalty,
     fillin_fixed_value,
     func_with_list_arg,
@@ -188,17 +184,15 @@
                 n_obj=self.n_obj,
                 index=index,
                 n_eval=n_eval,
                 fitness=fitness,
             )
         elif self._eval_type == "dict":
             self._to_pheno = lambda x: x.to_dict().copy()
-            self._to_geno = lambda x, index=None: Solution.from_dict(
-                x, index=index, n_obj=self.n_obj
-            )
+            self._to_geno = lambda x, index=None: Solution.from_dict(x, index=index, n_obj=self.n_obj)
 
     def _set_internal_optimization(self, kwargs):
         if kwargs is None:
             kwargs = {}
 
         # TODO: turn this into an Option Class
         if "optimizer" in kwargs:
@@ -218,17 +212,15 @@
         # NOTE: `AQ` -> acquisition
         if "max_FEs" in kwargs:
             self.AQ_max_FEs = arg_to_int(kwargs["max_FEs"])
         else:
             self.AQ_max_FEs = default_AQ_max_FEs[self._optimizer](self.dim)
 
         self.AQ_n_restart = (
-            default_AQ_n_restart(self.dim)
-            if "n_restart" not in kwargs
-            else arg_to_int(kwargs["n_restart"])
+            default_AQ_n_restart(self.dim) if "n_restart" not in kwargs else arg_to_int(kwargs["n_restart"])
         )
         self.AQ_wait_iter = (
             default_AQ_wait_iter if "wait_iter" not in kwargs else arg_to_int(kwargs["wait_iter"])
         )
 
         # NOTE: `_h` and `_g` are wrappers of `h` and `g`, which always take lists as input
         self._h, self._g = self.h, self.g
@@ -339,17 +331,15 @@
         self.logger.info(f"observing {len(X)} points:")
         for i, _ in enumerate(X):
             X[i].fitness = func_vals[i]
             X[i].n_eval += 1
             if not warm_start:
                 self.eval_count += 1
 
-            self.logger.info(
-                f"#{i + 1} - fitness: {func_vals[i]}, solution: {self._to_pheno(X[i])}"
-            )
+            self.logger.info(f"#{i + 1} - fitness: {func_vals[i]}, solution: {self._to_pheno(X[i])}")
 
         X = self.post_eval_check(X)
         self.data = self.data + X if hasattr(self, "data") else X
         self.update_model()
 
         if self.data_file is not None:
             X.to_csv(self.data_file, header=False, append=True)
@@ -390,33 +380,28 @@
         DoE = []
         while n_point:
             # NOTE: random sampling could generate duplicated points again
             # keep sampling until getting enough points
             X = search_space.sample(
                 n_point,
                 method="LHS" if n_point > 1 else "uniform",
-                h=partial_argument(self._h, self.search_space.var_name, fixed)
-                if self._h
-                else None,
-                g=partial_argument(self._g, self.search_space.var_name, fixed)
-                if self._g
-                else None,
+                h=partial_argument(self._h, self.search_space.var_name, fixed) if self._h else None,
+                g=partial_argument(self._g, self.search_space.var_name, fixed) if self._g else None,
             ).tolist()
             X = fillin_fixed_value(X, fixed, self.search_space)
 
             if len(X) != 0:
                 X = self.search_space.round(X)
                 X = self.pre_eval_check(X)
                 DoE += X
                 n_point -= len(X)
 
             count += 1
             if count > 3:  # maximally 3 iterations
                 break
-
         return DoE
 
     @abstractmethod
     def pre_eval_check(self, X: Solution) -> Solution:
         """This function is meant for checking validaty of the solutions prior to the evaluation
 
         Parameters
@@ -446,21 +431,19 @@
         # appear in the MGF-based acquisition function.
         # Standardization should make it easier to specify the GP prior, compared to
         # rescaling values to the unit interval.
         _std = np.std(fitness)
         if len(fitness) > 5 and np.isclose(_std, 0):
             raise FlatFitnessError()
 
-        fitness_ = (
-            fitness if np.isclose(_std, 0) else (fitness - np.mean(fitness)) / np.std(fitness)
-        )
+        fitness_ = fitness if np.isclose(_std, 0) else (fitness - np.mean(fitness)) / np.std(fitness)
         self.fmin, self.fmax = np.min(fitness_), np.max(fitness_)
         self.frange = self.fmax - self.fmin
 
-        self.model.fit(data, fitness_)
+        self.model.fit(data, fitness_.reshape(-1, 1))
         fitness_hat = self.model.predict(data)
 
         r2 = r2_score(fitness_, fitness_hat)
         MAPE = mean_absolute_percentage_error(fitness_, fitness_hat)
         self.logger.info(f"model r2: {r2}, MAPE: {MAPE}")
 
     @timeit
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/bayes_opt.py` & `bayes-optim-0.2.6/bayes_optim/bayes_opt.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/extension.py` & `bayes-optim-0.2.6/bayes_optim/extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from copy import copy, deepcopy
 from typing import Callable, Dict, List, Union
 
 import numpy as np
 from joblib import Parallel, delayed
 from scipy.stats import rankdata
 from sklearn.decomposition import PCA
+from sklearn.gaussian_process.kernels import ConstantKernel, Matern
 from sklearn.metrics import mean_absolute_percentage_error, r2_score
 
 from . import acquisition_fun as AcquisitionFunction
 from .bayes_opt import BO, ParallelBO
 from .search_space import RealSpace, SearchSpace
 from .solution import Solution
 from .surrogate import GaussianProcess, RandomForest
@@ -104,17 +105,15 @@
         if self.model is not None:
             self.logger.warning(
                 "The surrogate model will be created automatically by PCA-BO. "
                 "The input argument `model` will be ignored"
             )
         assert isinstance(self._search_space, RealSpace)
         self.__search_space = deepcopy(self._search_space)  # the original search space
-        self._pca = LinearTransform(
-            n_components=n_components, svd_solver="full", minimize=self.minimize
-        )
+        self._pca = LinearTransform(n_components=n_components, svd_solver="full", minimize=self.minimize)
 
     @staticmethod
     def _compute_bounds(pca: PCA, search_space: SearchSpace) -> List[float]:
         C = np.array([(l + u) / 2 for l, u in search_space.bounds])
         radius = np.sqrt(np.sum((np.array([l for l, _ in search_space.bounds]) - C) ** 2))
         C = C - pca.mean_ - pca.center
         C_ = C.dot(pca.components_.T)
@@ -177,26 +176,15 @@
         self.update_model(X, self.data.fitness)
         self.logger.info(f"xopt/fopt:\n{self.xopt}\n")
 
     def update_model(self, X: np.ndarray, y: np.ndarray):
         # NOTE: the GPR model will be created since the effective search space (the reduced space
         # is dynamic)
         dim = self._search_space.dim
-        bounds = np.array(self._search_space.bounds)
-        _range = bounds[:, 1] - bounds[:, 0]
-        thetaL, thetaU = 1e-8 * _range, 10 * _range
-        self.model = GaussianProcess(
-            theta0=np.random.rand(dim) * (thetaU - thetaL) + thetaL,
-            thetaL=thetaL,
-            thetaU=thetaU,
-            nugget=1e-8,
-            noise_estim=False,
-            random_start=dim,
-            eval_budget=100 * dim,
-        )
+        self.model = GaussianProcess(domain=self._search_space, n_restarts_optimizer=dim, alpha=1e-8)
 
         _std = np.std(y)
         y_ = y if np.isclose(_std, 0) else (y - np.mean(y)) / _std
 
         self.fmin, self.fmax = np.min(y_), np.max(y_)
         self.frange = self.fmax - self.fmin
 
@@ -242,17 +230,15 @@
 
     def select_subspace(self, n_point: int) -> List[int]:
         if n_point == 0:
             return []
         return np.random.choice(self.n_subspace, n_point).tolist()
 
     @timeit
-    def ask(
-        self, n_point: int = None, fixed: Dict[str, Union[float, int, str]] = None
-    ) -> Union[List[dict]]:
+    def ask(self, n_point: int = None, fixed: Dict[str, Union[float, int, str]] = None) -> List[dict]:
         n_point = self.n_point if n_point is None else n_point
         idx = []
         # initial DoE
         for _ in range(n_point):
             try:
                 idx.append(next(self._init_gen))
             except StopIteration:
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/mobo.py` & `bayes-optim-0.2.6/bayes_optim/mobo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 from joblib import Parallel, delayed
-from sklearn.metrics import mean_absolute_percentage_error, r2_score
+from sklearn.metrics import mean_squared_error, r2_score
 from sklearn.preprocessing import MinMaxScaler
 from torch import Tensor
 
 from .acquisition_optim import argmax_restart
 from .bayes_opt import BO
 from .multi_objective import EHVI
 from .utils import dynamic_penalty, partial_argument, timeit
@@ -39,16 +39,15 @@
         self.n_obj = n_obj
         if self.obj_fun is None:
             return
         assert hasattr(self.obj_fun, "__iter__")
         assert all([hasattr(f, "__call__") for f in self.obj_fun])
         if len(self.obj_fun) != n_obj:
             self.logger.warning(
-                f"len(obj_fun) ({self.obj_fun}) != n_obj ({n_obj})."
-                "Setting n_obj according to the former."
+                f"len(obj_fun) ({self.obj_fun}) != n_obj ({n_obj})." "Setting n_obj according to the former."
             )
             self.n_obj = len(self.obj_fun)
         assert self.n_obj > 1
 
     @property
     def xopt(self):
         """get the non-dominated subset of solutions"""
@@ -135,15 +134,17 @@
         self.update_model()
         # compute the hypervolume indicator value of the incumbent
         # TODO: HV computation is not exactly correct
         xopt = self.xopt
         pf = self._scaler.transform(self.xopt.fitness) * (-1) ** self.minimize
         hv = Hypervolume(ref_point=Tensor(self.ref_point))
         self.logger.info(f"efficient set/Pareto front (xopt/fopt):\n{xopt}")
-        self.logger.info(f"hypervolume of normalized fitness: {hv.compute(Tensor(pf))}")
+        self.logger.info(
+            f"hypervolume of normalized fitness: {hv.compute(Tensor(pf)) / np.prod(self._scaler.scale_)}"
+        )
 
         if self.h is not None or self.g is not None:
             penalty = np.array(
                 [dynamic_penalty(x, 1, self._h, self._g, minimize=False) for x in xopt]
             ).ravel()
             self.logger.info(f"... with corresponding penalty: {penalty}")
 
@@ -153,39 +154,34 @@
 
     def update_model(self):
         # TODO: add model selection to the base class
         X, y = self.data, self.y
         self.model.fit(X, y)
         y_ = self.model.predict(X)
         r2 = r2_score(y, y_, multioutput="raw_values")
-        MAPE = mean_absolute_percentage_error(y, y_, multioutput="raw_values")
-
+        MSE = mean_squared_error(y, y_, multioutput="raw_values")
         for i in range(self.n_obj):
             _r2 = r2[i] if not isinstance(r2, float) else r2
-            _mape = MAPE[i] if not isinstance(MAPE, float) else MAPE
-            self.logger.info(f"model of f{i + 1} r2: {_r2}, MAPE: {_mape}")
+            _mse = MSE[i] if not isinstance(MSE, float) else MSE
+            self.logger.info(f"model of f{i + 1} r2: {_r2}, MSE: {_mse}")
 
 
 class MOBO(BaseMOBO):
     """EHVI with Kriging believer"""
 
     def __init__(self, *args, **kwargv):
         super().__init__(*args, **kwargv)
         if self._acquisition_fun != "EHVI":
             self._acquisition_fun = "EHVI"
-            self.logger.warning(
-                "MOBO only allows using `EHIV` acquisition function. Ignore user's argument."
-            )
+            self.logger.warning("MOBO only allows using `EHIV` acquisition function. Ignore user's argument.")
 
     def _create_acquisition(self, fixed: Dict = None, **kwargv):
         # TODO: implement the Kriging believer strategy
         partitioning = NondominatedPartitioning(ref_point=Tensor(self.ref_point), Y=Tensor(self.y))
-        criterion = EHVI(
-            model=self.model, ref_point=self.ref_point.tolist(), partitioning=partitioning
-        )
+        criterion = EHVI(model=self.model, ref_point=self.ref_point.tolist(), partitioning=partitioning)
         return partial_argument(
             functools.partial(criterion),
             self.search_space.var_name,
             fixed,
             reduce_output=False,
         )
 
@@ -221,19 +217,15 @@
         mask = np.array([v in fixed.keys() for v in self._search_space.var_name])
         values = [fixed[k] for i, k in enumerate(self._search_space.var_name) if mask[i]]
         idx = np.nonzero(~mask)[0]
         _argmax_restart = functools.partial(
             argmax_restart,
             search_space=self._search_space[idx] * n_point,
             h=((self._h, np.repeat(mask, n_point), values * n_point) if self._h else None),
-            g=(
-                partial_argument(self._g, np.repeat(mask, n_point), values * n_point)
-                if self._g
-                else None
-            ),
+            g=(partial_argument(self._g, np.repeat(mask, n_point), values * n_point) if self._g else None),
             eval_budget=self.AQ_max_FEs,
             n_restart=self.AQ_n_restart,
             wait_iter=self.AQ_wait_iter,
             optimizer=self._optimizer,
         )
         candidates, values = _argmax_restart(
             self._create_acquisition(par={"n_point": n_point, "model": self.model}, fixed=fixed),
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/multi_objective/analytic.py` & `bayes-optim-0.2.6/bayes_optim/multi_objective/analytic.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/search_space/node.py` & `bayes-optim-0.2.6/bayes_optim/search_space/node.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/search_space/samplers.py` & `bayes-optim-0.2.6/bayes_optim/search_space/samplers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 from __future__ import annotations
 
-# from abc import ABC
+import warnings
 from typing import Callable
 
 import numpy as np
-
-# import torch
-# from gpytorch.distributions import MultivariateNormal
-
-# from scipy.optimize import root_scalar
 from scipy.stats import norm
 
 from ..utils.exception import ConstraintEvaluationError
 
-# from torch import Tensor
-# from torch.nn import Module
-
-
 __author__ = "Hao Wang"
 
 
 class SCMC:
     r"""Sequential Constrained Monte Carlo sampling
 
     References
@@ -35,14 +26,15 @@
     def __init__(
         self,
         sample_space,
         constraints: Callable,
         target_dist: Callable = lambda _: 1,
         metropolis_hastings_step: int = 17,
         tol: float = 1e-2,
+        sample_out_of_bound: bool = False,
     ):
         """Sequential Constrained Monte Carlo sampling
 
         Parameters
         ----------
         sample_space : SearchSpace
             the sample space
@@ -50,42 +42,47 @@
             constraint functions, which could represent inequalities or equalities
         target_dist : Callable, optional
             the target probability density, by default uniform (lambda x: 1)
         metropolis_hastings_step : int, optional
             the number of MCMC iterations, by default 15
         tol : float, optional
             the tolerance on the constraint
+        sample_out_of_bound: bool, optional
+            if the real- and integer-valued components can go beyond the sample space (`sample_space`). This
+            is intended sometimes, if the sample space does not guarantee to cover the constrained domain.
         """
         if hasattr(constraints, "__call__"):
             constraints = [constraints]
         assert hasattr(target_dist, "__call__")
 
         self.constraints = constraints
         self.target_dist = target_dist
         self.sample_space = sample_space
         self.dim = sample_space.dim
         self.mh_steps = metropolis_hastings_step
         self.nu_target = tol / 8  # 8-sigma CI leads to ~1.24e-15 significance
         self.nu0 = 10
-        self.nu_schedule = np.logspace(
-            np.log10(self.nu0), np.log10(self.nu_target), base=10, num=20
-        )
+        self.nu_schedule = np.logspace(np.log10(self.nu0), np.log10(self.nu_target), base=10, num=20)
 
         # index of each type of variables in the dataframe
         self.id_r = self.sample_space.real_id  # index of continuous variable
         self.id_i = self.sample_space.integer_id  # index of integer variable
         self.id_d = self.sample_space.categorical_id  # index of categorical variable
 
         # the number of variables per each type
         self.N_r = len(self.id_r)
         self.N_i = len(self.id_i)
         self.N_d = len(self.id_d)
 
-        self.bounds_r = np.asarray([self.sample_space.bounds[_] for _ in self.id_r])
-        self.bounds_i = np.asarray([self.sample_space.bounds[_] for _ in self.id_i])
+        if sample_out_of_bound:
+            self.bounds_r = np.asarray([(-np.inf, np.inf) for _ in self.id_r])
+            self.bounds_i = np.asarray([(-np.inf, np.inf) for _ in self.id_i])
+        else:
+            self.bounds_r = np.asarray([self.sample_space.bounds[_] for _ in self.id_r])
+            self.bounds_i = np.asarray([self.sample_space.bounds[_] for _ in self.id_i])
         self.bounds_d = [self.sample_space.bounds[_] for _ in self.id_d]
 
     def _log_posterior(self, x: np.ndarray, nu: float) -> float:
         r"""Log-posterior \log P(x) + \sum_{i=1}^K \log \Phi(-C_i(x) / \nu)
 
         Parameters
         ----------
@@ -102,45 +99,47 @@
             c = np.array([cons(x) for cons in self.constraints])
         except Exception as e:
             raise ConstraintEvaluationError(x, str(e)) from None
         return np.log(self.target_dist(x)) + np.sum(norm.logcdf(-1 * c / nu))
 
     def _rproposal(self, X: np.ndarray, t: int) -> np.ndarray:
         X_ = X.copy()
-        self._rproposal_real(X_, t)
-        self._rproposal_integer(X_, t)
-        self._rproposal_discrete(X_, t)
+        if self.N_r > 0:
+            self._rproposal_real(X_, t)
+        if self.N_i > 0:
+            self._rproposal_integer(X_, t)
+        if self.N_d > 0:
+            self._rproposal_discrete(X_, t)
         return X_
 
     def _rproposal_real(self, X: np.ndarray, t: int):
-        if self.N_r > 0:
-            X_ = X[:, self.id_r].astype(float)
-            q = np.std(X_, axis=0) / (t + 1)
-            X[:, self.id_r] = np.clip(
-                X_ + q * np.random.randn(*X_.shape), self.bounds_r[:, 0], self.bounds_r[:, 1]
-            )
+        X_ = X[:, self.id_r].astype(float)
+        q = np.std(X_, axis=0) / (t + 1)
+        X[:, self.id_r] = np.clip(
+            X_ + q * np.random.randn(*X_.shape),
+            self.bounds_r[:, 0],
+            self.bounds_r[:, 1],
+        )
 
     def _rproposal_integer(self, X: np.ndarray, t: int):
-        if self.N_i > 0:
-            X_ = X[:, self.id_i].astype(int)
-            p = norm.cdf(np.std(X_, axis=0) / (t + 1))
-            X[:, self.id_i] = np.clip(
-                X_ + np.random.geometric(p, X_.shape) - np.random.geometric(p, X_.shape),
-                self.bounds_i[:, 0],
-                self.bounds_i[:, 1],
-            )
+        X_ = X[:, self.id_i].astype(int)
+        p = norm.cdf(np.std(X_, axis=0) / (t + 1))
+        X[:, self.id_i] = np.clip(
+            X_ + np.random.geometric(p, X_.shape) - np.random.geometric(p, X_.shape),
+            self.bounds_i[:, 0],
+            self.bounds_i[:, 1],
+        )
 
     def _rproposal_discrete(self, X: np.ndarray, t: int):
-        if self.N_d > 0:
-            N = len(X)
-            prob = max(0.5 * np.exp(-1 * t), 1 / self.N_d)
-            for i in self.id_d:
-                levels = np.array(self.sample_space.bounds[i])
-                idx = np.random.rand(N) < prob
-                X[idx, i] = levels[np.random.randint(0, len(levels), sum(idx))]
+        N = len(X)
+        prob = max(0.5 * np.exp(-1 * t), 1 / self.N_d)
+        for i in self.id_d:
+            levels = np.array(self.sample_space.bounds[i])
+            idx = np.random.rand(N) < prob
+            X[idx, i] = levels[np.random.randint(0, len(levels), sum(idx))]
 
     def _ess(self, nu: float, nu_ref: float, X: np.ndarray) -> float:
         """effective sample size"""
         w = self.get_weights(nu, nu_ref, X)
         v = 0 if np.any(np.isnan(w)) else 1 / np.sum(w ** 2)
         return v - len(X) / 2
 
@@ -166,22 +165,21 @@
         np.ndarray
             (dependent) sample points from `self._log_posterior`
         """
         N = len(X)  # sample size
         lp = np.array([self._log_posterior(x, nu) for x in X])  # log-probability
         for _ in range(self.mh_steps):
             X_ = self._rproposal(X, t)
-            for i in range(self.dim):
-                X_dim = X.copy()
-                X_dim[:, i] = X_[:, i]
-                lp_ = np.array([self._log_posterior(x_, nu) for x_ in X_dim])
+            lp_ = np.array([self._log_posterior(x_, nu) for x_ in X_])
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
                 prob = np.clip(np.exp(lp_ - lp), 0, 1)
-                mask = np.random.rand(N) <= prob
-                X[mask, i] = X_[mask, i]
-                lp[mask] = lp_[mask]
+            mask = np.random.rand(N) <= prob
+            X[mask, :] = X_[mask, :]
+            lp[mask] = lp_[mask]
         return X
 
     def sample(self, N: int) -> np.ndarray:
         """Draw a sample under constraints
 
         Parameters
         ----------
@@ -189,18 +187,18 @@
             sample size
 
         Returns
         -------
         np.ndarray
             the sample
         """
-        # draw the initial samples u.a.r. from `self.search_space`
+        # draw the initial samples using Latin hypercube sampling from `self.sample_space`
         X = getattr(self.sample_space, "_sample")(N, method="LHS")
         for t, nu in enumerate(self.nu_schedule):
-            nu_ = nu  # `nu_` -> the old `nu`
+            # TODO: will fix those...
             # nu = self.nu_schedule[t]
             # if self._ess(self.nu_target, nu, X) > 0:
             #     nu *= 0.3
             # else:
             #     try:
             #         nu = (
             #             10
@@ -211,24 +209,25 @@
             #                     np.log10(0.001 if t < 2 else self.nu_target),
             #                     np.log10(nu_),
             #                 ),
             #             ).root
             #         )
             #     except ValueError:
             #         return X
-            w = self.get_weights(nu, nu_, X)
-            if any(np.isnan(w)):
-                w = np.ones(N) / N
+
+            # NOTE: this will cause many points being duplicated, hence it is disabled
+            # w = self.get_weights(nu, nu_, X)
+            # if any(np.isnan(w)):
+            # w = np.ones(N) / N
 
             # resampling with replacement to increase the fraction of samples that are
             # more likely distributed from the new probability law, which is controlled by `nu`
-            if N >= 10:
-                idx = np.random.choice(N, N, p=w)
-                X = X[idx, :]
-
+            # if N >= 10:
+            #     idx = np.random.choice(N, N, p=w)
+            #     X = X[idx, :]
             X = self._metropolis_hastings(X, nu, t)
         return X
 
 
 # class MCSampler(Module, ABC):
 #     r"""Abstract base class for Samplers.
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/search_space/search_space.py` & `bayes-optim-0.2.6/bayes_optim/search_space/search_space.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/search_space/variable.py` & `bayes-optim-0.2.6/bayes_optim/search_space/variable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,89 @@
 from __future__ import annotations
 
+import copyreg
 import sys
 import warnings
 from abc import ABC
 from copy import deepcopy
 from itertools import chain, combinations
 from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import scipy as sp
 from numpy.random import randint
 from py_expression_eval import Parser
 
 __authors__ = ["Hao Wang"]
 
+
+def identity(x):
+    return x
+
+
+def bilog(x):
+    return np.sign(x) * np.log(1 + np.abs(x))
+
+
+def logit_inv(x):
+    return 1 / (1 + np.exp(-x))
+
+
+def bilog_inv(x):
+    return np.sign(x) * (np.exp(np.abs(x)) - 1)
+
+
+def log10_inv(x):
+    return np.power(10, x)
+
+
 MAX = sys.float_info.max
 TRANS = {
-    "linear": [lambda x: x, [-MAX, MAX]],
+    "linear": [identity, [-MAX, MAX]],
     "log": [np.log, [1e-300, MAX]],
     "log10": [np.log10, [1e-300, MAX]],
     "logit": [sp.special.logit, [1e-300, 1]],
-    "bilog": [lambda x: np.sign(x) * np.log(1 + np.abs(x)), [-MAX, MAX]],
+    "bilog": [bilog, [-MAX, MAX]],
 }
 INV_TRANS = {
-    "linear": lambda x: x,
+    "linear": identity,
     "log": np.exp,
-    "log10": lambda x: np.power(10, x),
-    "logit": lambda x: 1 / (1 + np.exp(-x)),
-    "bilog": lambda x: np.sign(x) * (np.exp(np.abs(x)) - 1),
+    "log10": log10_inv,
+    "logit": logit_inv,
+    "bilog": bilog_inv,
 }
 
 
+def _gen_action(v):
+    def _action(_):
+        return v
+
+    return _action
+
+
+def _gen_map_func(bounds, step=0):
+    def _map_func(i):
+        if hasattr(bounds, "__iter__"):
+            return bounds[i]
+        else:
+            return bounds + i * step
+
+    return _map_func
+
+
 class Variable(ABC):
     """Base class for decision variables"""
 
     def __init__(
         self,
         bounds: List[int, float, str],
         name: str,
         default_value: Union[int, float, str] = None,
         conditions: str = None,
-        action: Union[callable, int, float, str] = lambda x: x,
+        action: Union[callable, int, float, str] = 0,
     ):
         """Base class for decision variables
 
         Parameters
         ----------
         bounds : List[int, float, str]
             a list/tuple giving the range of the variable.
@@ -96,38 +135,35 @@
 
     def __ne__(self, var: Variable) -> bool:
         return not self.__eq__(var)
 
     def copyfrom(self, var: Variable):
         """copy from another variable of the same type"""
         if not isinstance(var, type(self)):
-            raise TypeError(
-                f"copying from variable {var} which has a type different type than {type(self)}"
-            )
+            raise TypeError(f"copying from variable {var} which has a type different type than {type(self)}")
         self.__dict__.update(**deepcopy(var.__dict__))
 
     def set_default_value(self, value):
         """validate the default value first"""
         if value is not None:
             assert self.__contains__(value)
         self.default_value = value
 
-    def set_conditions(
-        self, conditions: str, action: Union[callable, int, float, str] = lambda x: x
-    ):
+    def set_conditions(self, conditions: str, action: Union[callable, int, float, str] = 0):
         self.conditions = None
         if conditions is not None:
             # TODO: add parsing exceptions here
             expr = Parser().parse(conditions)
             self.conditions = {"string": conditions, "expr": expr, "vars": expr.variables()}
 
-        if isinstance(action, (int, float, str)):
-            self.action = lambda _: action
-        elif hasattr(action, "__call__"):
-            self.action = action
+        self.action = None
+        # if isinstance(action, (int, float, str)):
+        #     self.action = _gen_action(action)
+        # elif hasattr(action, "__call__"):
+        #     self.action = action
 
 
 class Real(Variable):
     """Real-valued variable taking its value in a continuum"""
 
     def __init__(
         self,
@@ -191,18 +227,14 @@
 
         if (bounds[0] < _range[0]) or (bounds[0] > _range[1]):
             bounds[0] = _range[0]
             warnings.warn(
                 f"lower bound {bounds[0]} not in the working "
                 f"range of the given scale {self._scale} is set to the default value {_range[0]}"
             )
-            # raise ValueError(
-            #     f"lower bound {self.bounds[0]} not in the working "
-            #     f"range of the given scale {self._scale}"
-            # )
 
         if (bounds[1] < _range[0]) or (bounds[1] > _range[1]):
             bounds[1] = _range[1]
             warnings.warn(
                 f"upper bound {bounds[1]} not in the working "
                 f"range of the given scale {self._scale} is set to the default value {_range[1]}"
             )
@@ -247,41 +279,39 @@
 
 
 class Discrete(_Discrete):
     """Discrete variable, whose values should come with a linear order"""
 
     def __init__(self, bounds, name: str = "d", default_value: Union[int, str] = None, **kwargs):
         super().__init__(bounds, name, default_value, **kwargs)
-        self._map_func = lambda i: self.bounds[i]
+        self._map_func = _gen_map_func(self.bounds)
         self._size = len(self.bounds)
 
 
 class Subset(Discrete):
     """A discrete variable created by enumerating all subsets of the input `bounds`"""
 
     def __init__(self, bounds, name: str = "s", default_value: Union[int, str] = None, **kwargs):
         self._bounds = bounds
-        bounds = list(
-            chain.from_iterable(map(lambda r: combinations(bounds, r), range(1, len(bounds) + 1)))
-        )
+        bounds = list(chain.from_iterable(map(lambda r: combinations(bounds, r), range(1, len(bounds) + 1))))
         super().__init__(bounds, name, default_value, **kwargs)
 
     def __str__(self):
         msg = f"{self.name} -> {type(self).__name__} | range: 2 ^ {self._bounds}"
         if self.default_value is not None:
             msg += f" | default: {self.default_value}"
         return msg
 
 
 class Ordinal(_Discrete):
     """A generic ordinal variable, whose values should come with a linear order"""
 
     def __init__(self, bounds, name: str = "ordinal", default_value: int = None, **kwargs):
         super().__init__(bounds, name, default_value, **kwargs)
-        self._map_func = lambda i: self.bounds[i]
+        self._map_func = _gen_map_func(self.bounds)
         self._size = len(self.bounds)
 
 
 class Integer(_Discrete):
     """Integer variable"""
 
     def __init__(
@@ -293,15 +323,15 @@
         **kwargs,
     ):
         super().__init__(bounds, name, default_value, **kwargs)
         assert len(self.bounds) == 2
         assert self.bounds[0] < self.bounds[1]
         assert all(map(lambda x: isinstance(x, (int, float)), self.bounds))
         self.step = step
-        self._map_func = lambda i: self.bounds[0] + i * self.step
+        self._map_func = _gen_map_func(self.bounds[0], self.step)
         self._size = int(np.floor((self.bounds[1] - self.bounds[0]) / self.step) + 1)
 
     def __contains__(self, x: int) -> bool:
         return self.bounds[0] <= x <= self.bounds[1]
 
     def __hash__(self):
         return hash((self.name, self.bounds, self.default_value, self.step))
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/solution.py` & `bayes-optim-0.2.6/bayes_optim/solution.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/boundary_handling.py` & `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/boundary_handling.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/cma_es.py` & `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/cma_es.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/gpr.py` & `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/gpr.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/kernel.py` & `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/kernel.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/trend.py` & `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/trend.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/surrogate/gaussian_process/utils.py` & `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/utils.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/surrogate/random_forest.py` & `bayes-optim-0.2.6/bayes_optim/surrogate/random_forest.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     """Linear aggregation of surrogate models used for multi-obvjective optimization"""
 
     def __init__(self, surrogates, aggregation="WS", **kwargs):
         self.surrogates = surrogates
         self.N = len(self.surrogates)
         self.aggregation = aggregation
         self.weights = np.asarray(kwargs["weights"], dtype="float").ravel()
-
         assert self.aggregation in ["WS", "Tchebycheff"]
 
     def fit(self, X, y):
         pass
 
     def predict(self, X, eval_MSE=False):
         if eval_MSE:
@@ -101,23 +100,21 @@
             self._categories = list(self._levels.values())
             # encode categorical variables to binary values
             self._enc = OneHotEncoder(categories=self._categories, sparse=False)
 
     def _check_X(self, X: Union[Solution, List, np.ndarray]) -> Solution:
         X_ = array(X, dtype=object)
         if hasattr(self, "_levels"):
-            X_cat = X_[:, self._cat_idx]
-            try:
-                X_cat = self._enc.transform(X_cat)
-            except Exception:
-                X_cat = self._enc.fit_transform(X_cat)
+            X_cat = self._enc.fit_transform(X_[:, self._cat_idx])
             X = np.c_[np.delete(X_, self._cat_idx, 1).astype(float), X_cat]
         return X
 
     def fit(self, X: Union[Solution, List, np.ndarray], y: np.ndarray):
+        if y.ndim == 2 and y.shape[1] == 1:
+            y = y.ravel()
         self.X = self._check_X(X)
         self.y = y
         self.is_fitted = True
         return super().fit(self.X, self.y)
 
     def predict(self, X: Union[Solution, List, np.ndarray], eval_MSE=False) -> np.ndarray:
         """Predict regression target for `X`.
@@ -144,16 +141,15 @@
         y_hat_all = (
             np.zeros((X.shape[0], self.n_outputs_, self.n_estimators), dtype=np.float64)
             if self.n_outputs_ > 1
             else np.zeros((X.shape[0], self.n_estimators), dtype=np.float64)
         )
         # parallel loop
         Parallel(n_jobs=n_jobs, verbose=self.verbose, backend="threading")(
-            delayed(_save_prediction)(e.predict, X, i, y_hat_all)
-            for i, e in enumerate(self.estimators_)
+            delayed(_save_prediction)(e.predict, X, i, y_hat_all) for i, e in enumerate(self.estimators_)
         )
         y_hat = np.mean(y_hat_all, axis=-1)
 
         if eval_MSE:
             # TODO: implement the jackknife estimate of variance
             MSE_hat = np.std(y_hat_all, axis=-1, ddof=1) ** 2.0
         return (y_hat, MSE_hat) if eval_MSE else y_hat
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/__init__.py` & `bayes-optim-0.2.6/bayes_optim/utils/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     fillin_fixed_value,
     func_with_list_arg,
     handle_box_constraint,
     is_pareto_efficient,
     partial_argument,
     set_bounds,
     timeit,
+    safe_divide,
 )
 
 __all__ = [
     "get_logger",
     "fillin_fixed_value",
     "func_with_list_arg",
     "partial_argument",
@@ -22,8 +23,9 @@
     "arg_to_int",
     "set_bounds",
     "dynamic_penalty",
     "Daemon",
     "handle_box_constraint",
     "load_logger",
     "dump_logger",
+    "safe_divide",
 ]
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/_daemon.py` & `bayes-optim-0.2.6/bayes_optim/utils/_daemon.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/exception.py` & `bayes-optim-0.2.6/bayes_optim/utils/exception.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/logger.py` & `bayes-optim-0.2.6/bayes_optim/utils/logger.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/box_decompositions/box_decomposition.py` & `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/box_decomposition.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/box_decompositions/non_dominated.py` & `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/non_dominated.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/box_decompositions/utils.py` & `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/utils.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/hypervolume.py` & `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/hypervolume.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/multi_objective/pareto.py` & `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/bayes_optim/utils/utils.py` & `bayes-optim-0.2.6/bayes_optim/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,19 @@
     WARNING = "\033[93m"
     FAIL = "\033[91m"
     ENDC = "\033[0m"
     BOLD = "\033[1m"
     UNDERLINE = "\033[4m"
 
 
+def safe_divide(x1, x2):
+    """Divide x1 / x2, return 0 where x2 == 0"""
+    return np.divide(x1, x2, out=np.zeros(np.broadcast(x1, x2).shape), where=(x2 != 0))
+
+
 def random_string(k: int = 15):
     return "".join(random.choices(string.ascii_letters + string.digits, k=k))
 
 
 def expand_replace(s: str):
     m = re.match(r"${.*}", s)
     for _ in m.group():
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim.egg-info/PKG-INFO` & `bayes-optim-0.2.6/bayes_optim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes-optim
-Version: 0.2.5.8
+Version: 0.2.6
 Summary: A Bayesian Optimization Library
 Home-page: https://github.com/wangronin/Bayesian-Optimization
 Author: Hao Wang
 Author-email: wangronin@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/wangronin/Bayesian-Optimization/archive/v0.1.3.tar.gz
 Description: [![Actions Status](https://github.com/wangronin/Bayesian-Optimization/workflows/Build%20and%20Test/badge.svg)](https://github.com/wangronin/Bayesian-Optimization/actions)
```

### Comparing `bayes-optim-0.2.5.8/bayes_optim.egg-info/SOURCES.txt` & `bayes-optim-0.2.6/bayes_optim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.5.8/setup.py` & `bayes-optim-0.2.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bayes-optim",
-    version="0.2.5.8",
+    version="0.2.6",
     author="Hao Wang",
     author_email="wangronin@gmail.com",
     packages=find_packages(),
     description="A Bayesian Optimization Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wangronin/Bayesian-Optimization",
```

