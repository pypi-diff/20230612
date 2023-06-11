# Comparing `tmp/bayes-optim-0.2.6.tar.gz` & `tmp/bayes-optim-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayes-optim-0.2.6.tar", last modified: Mon Nov 15 19:47:02 2021, max compression
+gzip compressed data, was "bayes-optim-0.2.7.tar", last modified: Sun Jun 11 22:04:20 2023, max compression
```

## Comparing `bayes-optim-0.2.6.tar` & `bayes-optim-0.2.7.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15312 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13507 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.716856 bayes-optim-0.2.6/bayes_optim/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6079 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6255 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8339 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_fun.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/acquisition_optim/
--rw-r--r--   0 runner    (1001) docker     (121)     4728 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13254 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_optim/mies.py
--rw-r--r--   0 runner    (1001) docker     (121)    16493 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_optim/one_plus_one_cma_es.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/acquisition_optim/option.py
--rw-r--r--   0 runner    (1001) docker     (121)    20896 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7305 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/bayes_opt.py
--rw-r--r--   0 runner    (1001) docker     (121)    13034 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     9311 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/mobo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/multi_objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10653 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/multi_objective/analytic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/search_space/
--rw-r--r--   0 runner    (1001) docker     (121)      511 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6389 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/node.py
--rw-r--r--   0 runner    (1001) docker     (121)    11076 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/samplers.py
--rw-r--r--   0 runner    (1001) docker     (121)    31705 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/search_space.py
--rw-r--r--   0 runner    (1001) docker     (121)    11527 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/search_space/variable.py
--rw-r--r--   0 runner    (1001) docker     (121)    15009 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/surrogate/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.720856 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8220 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      997 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/boundary_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23105 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/cma_es.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    48464 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/gpr.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13111 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/kernel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6352 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/trend.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6507 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5706 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/surrogate/random_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/bayes_optim/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      621 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6620 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/_daemon.py
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11722 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/box_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (121)    18713 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/non_dominated.py
--rw-r--r--   0 runner    (1001) docker     (121)    12382 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10328 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/multi_objective/pareto.py
--rw-r--r--   0 runner    (1001) docker     (121)    10351 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/bayes_optim/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:47:02.716856 bayes-optim-0.2.6/bayes_optim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15312 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      236 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-11-15 19:47:02.000000 bayes-optim-0.2.6/bayes_optim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 19:47:02.724856 bayes-optim-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2021-11-15 19:46:58.000000 bayes-optim-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.568402 bayes-optim-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-06-11 22:04:20.568402 bayes-optim-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.564402 bayes-optim-0.2.7/bayes_optim/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6342 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.564402 bayes-optim-0.2.7/bayes_optim/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/acquisition/acquisition_fun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.564402 bayes-optim-0.2.7/bayes_optim/acquisition/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/acquisition/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/acquisition/optim/mies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/acquisition/optim/one_plus_one_cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/acquisition/optim/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20890 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/bayes_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/mobo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.564402 bayes-optim-0.2.7/bayes_optim/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/multi_objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/multi_objective/analytic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.564402 bayes-optim-0.2.7/bayes_optim/search_space/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/search_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/search_space/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/search_space/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31705 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/search_space/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/search_space/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.564402 bayes-optim-0.2.7/bayes_optim/surrogate/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/surrogate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.568402 bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8305 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/boundary_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23105 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/cma_es.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48502 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/gpr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13111 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/kernel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4297 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/trend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6507 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/surrogate/random_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.568402 bayes-optim-0.2.7/bayes_optim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.568402 bayes-optim-0.2.7/bayes_optim/utils/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/multi_objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.568402 bayes-optim-0.2.7/bayes_optim/utils/multi_objective/box_decompositions/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/multi_objective/box_decompositions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/multi_objective/box_decompositions/box_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/multi_objective/box_decompositions/non_dominated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/multi_objective/box_decompositions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/multi_objective/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/multi_objective/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/bayes_optim/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:04:20.564402 bayes-optim-0.2.7/bayes_optim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-06-11 22:04:20.000000 bayes-optim-0.2.7/bayes_optim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-11 22:04:20.000000 bayes-optim-0.2.7/bayes_optim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 22:04:20.000000 bayes-optim-0.2.7/bayes_optim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-11 22:04:20.000000 bayes-optim-0.2.7/bayes_optim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 22:04:20.000000 bayes-optim-0.2.7/bayes_optim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 22:04:20.568402 bayes-optim-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-11 22:04:10.000000 bayes-optim-0.2.7/setup.py
```

### Comparing `bayes-optim-0.2.6/LICENSE` & `bayes-optim-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/PKG-INFO` & `bayes-optim-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes-optim
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Bayesian Optimization Library
 Home-page: https://github.com/wangronin/Bayesian-Optimization
 Author: Hao Wang
 Author-email: wangronin@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/wangronin/Bayesian-Optimization/archive/v0.1.3.tar.gz
 Description: [![Actions Status](https://github.com/wangronin/Bayesian-Optimization/workflows/Build%20and%20Test/badge.svg)](https://github.com/wangronin/Bayesian-Optimization/actions)
```

### Comparing `bayes-optim-0.2.6/README.md` & `bayes-optim-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/__init__.py` & `bayes-optim-0.2.7/bayes_optim/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 from typing import Any, Callable, List, Optional, Tuple, Union
 
 import numpy as np
 
-from .acquisition_fun import EI, MGFI, PI, UCB
+from .acquisition.acquisition_fun import EI, MGFI, PI, UCB
 from .bayes_opt import BO, AnnealingBO, NoisyBO, ParallelBO
 from .mobo import MOBO
 from .search_space import (
     Bool,
     BoolSpace,
     Discrete,
     DiscreteSpace,
@@ -18,24 +18,23 @@
     Real,
     RealSpace,
     SearchSpace,
 )
 from .solution import Solution
 from .surrogate import GaussianProcess, RandomForest, trend
 
-__all__ = [
+__all__: List[str] = [
     "BO",
     "ParallelBO",
     "NoisyBO",
     "AnnealingBO",
     "MOBO",
     "Solution",
     "RandomForest",
     "GaussianProcess",
-    "trend",
     "SearchSpace",
     "IntegerSpace",
     "RealSpace",
     "BoolSpace",
     "DiscreteSpace",
     "EI",
     "UCB",
@@ -44,14 +43,15 @@
     "RandomForest",
     "fmin",
     "Integer",
     "Ordinal",
     "Real",
     "Bool",
     "Discrete",
+    "trend",
 ]
 
 # To use `dill` for the pickling, which works for
 # much more python objects
 os.environ["LOKY_PICKLER"] = "dill"
 
 verbose = {False: logging.NOTSET, "DEBUG": logging.DEBUG, "INFO": logging.INFO}
@@ -64,16 +64,14 @@
     func: Callable,
     lower: Union[float, Vector],
     upper: Union[float, Vector],
     x0: Union[int, Matrix, np.ndarray, None] = None,
     y0: Union[Vector, None] = None,
     n_point: int = 1,
     args: Tuple = (),
-    # xtol: float = 1e-4,
-    # ftol: float = 1e-4,
     max_FEs: Optional[int] = None,
     verbose: Optional[bool] = False,
     # callback: Optional[Callable] = None,
     seed: Optional[int] = None,
     **kwargs,
 ) -> Tuple[Vector, float, int, int, List[np.ndarray]]:
     """Minimize a function using the Bayesian Optimization algorithm, which only uses
@@ -132,29 +130,37 @@
     Optimization terminated successfully.
             Current function value: 0.007165794451494286
             Iterations: 21
             Function evaluations: 30
     >>> minimum[0]
     0.007165794451494286
     """
-    if seed is not None:
-        _state = np.random.get_state()
-        np.random.seed(seed)
-
     obj_func = lambda x: func(x, *args)
 
     if isinstance(lower, float) and isinstance(upper, float):
-        space = RealSpace([lower, upper])
+        search_space = RealSpace([lower, upper])
     elif isinstance(lower, list) and isinstance(upper, list):
         assert len(lower) == len(upper)
-        space = RealSpace(list(zip(lower, upper)))
+        search_space = RealSpace(list(zip(lower, upper)))
 
+    dim = search_space.dim
+    bounds = np.asarray(search_space.bounds)
     model = GaussianProcess(
-        domain=space,
-        n_restarts_optimizer=space.dim,
+        mean=trend.constant_trend(dim),
+        corr="matern",
+        thetaL=1e-3 * (bounds[:, 1] - bounds[:, 0]),
+        thetaU=1e3 * (bounds[:, 1] - bounds[:, 0]),
+        nugget=1e-6,
+        noise_estim=False,
+        optimizer="BFGS",
+        wait_iter=3,
+        random_start=max(10, dim),
+        likelihood="concentrated",
+        eval_budget=100 * dim,
+        random_state=seed,
     )
 
     # set up the warm-starting and DoE size
     if isinstance(x0, int):
         DoE_size = x0
         warm_data = ()
     elif hasattr(x0, "__iter__"):
@@ -164,30 +170,28 @@
         warm_data = (x0, y0)
     else:
         DoE_size = None
         warm_data = ()
 
     _BO = BO if n_point == 1 else ParallelBO
     opt = _BO(
-        search_space=space,
+        search_space=search_space,
         obj_fun=obj_func,
         model=model,
         DoE_size=DoE_size,
         warm_data=warm_data,
         eval_type="list",
         max_FEs=max_FEs,
         verbose=verbose,
         n_point=n_point,
+        random_seed=seed,
         **kwargs,
     )
     opt.run()
 
-    if seed is not None:
-        np.random.set_state(_state)
-
     N, n = opt.DoE_size, opt.n_point
     _data, data = opt.data[:N, :], opt.data[N:, :]
 
     data_per_iteration = [np.asarray(data[:N, :])]
     data_per_iteration += [np.asarray(data[(i * n) : ((i + 1) * n), :]) for i in range(opt.iter_count - 1)]
 
     print(
```

### Comparing `bayes-optim-0.2.6/bayes_optim/_base.py` & `bayes-optim-0.2.7/bayes_optim/_base.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/acquisition_optim/__init__.py` & `bayes-optim-0.2.7/bayes_optim/acquisition/optim/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 import logging
 import time
 from typing import Callable, List, Tuple
 
 import numpy as np
 from scipy.optimize import fmin_l_bfgs_b
 
-from ..search_space import RealSpace
-from ..utils import dynamic_penalty
+from ...search_space import RealSpace
+from ...utils import dynamic_penalty
 from .mies import MIES
 from .one_plus_one_cma_es import OnePlusOne_Cholesky_CMA, OnePlusOne_CMA
+from .option import default_AQ_max_FEs, default_AQ_n_restart, default_AQ_wait_iter
 
-__all__ = ["argmax_restart", "OnePlusOne_CMA", "OnePlusOne_Cholesky_CMA", "MIES"]
+__all__: List[str] = [
+    "argmax_restart",
+    "OnePlusOne_CMA",
+    "OnePlusOne_Cholesky_CMA",
+    "MIES",
+    "default_AQ_max_FEs",
+    "default_AQ_n_restart",
+    "default_AQ_wait_iter",
+]
 
 
 def finite_difference(f: Callable, x: np.ndarray, delta: float = 1e-5, **kwargs):
     N = len(x)
     v = np.eye(N) * delta
     return np.array(
         [(f(x + v[i], **kwargs) - f(x - v[i], **kwargs)) / (2 * delta) for i in range(N)]
@@ -33,17 +42,15 @@
         self.g = g
         self.t = 10
 
     def __call__(self, x: np.ndarray) -> Tuple[float, np.ndarray]:
         f, fg = tuple(map(lambda x: -1.0 * x, self.func(x)))
         if self.h or self.g:
             p = dynamic_penalty(x, t=self.t, equality=self.h, inequality=self.g)
-            pg = finite_difference(
-                dynamic_penalty, x, t=self.t, equality=self.h, inequality=self.g
-            )
+            pg = finite_difference(dynamic_penalty, x, t=self.t, equality=self.h, inequality=self.g)
             self.t += 1
             return f + p, fg + pg
         return f, fg
 
 
 def argmax_restart(
     obj_func: Callable,
```

### Comparing `bayes-optim-0.2.6/bayes_optim/acquisition_optim/mies.py` & `bayes-optim-0.2.7/bayes_optim/acquisition/optim/mies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Callable, List, Union
 
 import numpy as np
 from numpy import argsort, ceil, exp, mod, zeros
 from numpy.random import geometric, rand, randint, randn
 
-from ..search_space import SearchSpace
-from ..solution import Solution
-from ..utils import dynamic_penalty, handle_box_constraint
+from ...search_space import SearchSpace
+from ...solution import Solution
+from ...utils import dynamic_penalty, handle_box_constraint
 
 __author__ = "Hao Wang"
 
 # TODO: improve efficiency, e.g. compile it with cython
 class MIES:
     """Mixed-integer Evolution Strategy"""
 
@@ -97,17 +97,15 @@
             P0 = 1.0 / self.N_d
             par_name += ["P" + str(_) for _ in range(self.N_p)]
 
         # column indices: used for slicing
         self._id_var = np.arange(self.dim)
         self._id_sigma = np.arange(self.N_r) + len(self._id_var)
         self._id_eta = np.arange(self.N_i) + len(self._id_var) + len(self._id_sigma)
-        self._id_p = (
-            np.arange(self.N_p) + len(self._id_var) + len(self._id_sigma) + len(self._id_eta)
-        )
+        self._id_p = np.arange(self.N_p) + len(self._id_var) + len(self._id_sigma) + len(self._id_eta)
         self._id_hyperpar = np.arange(self.dim, self._len)
 
         # initialize the populations
         if x0 is not None:  # given x0
             par = []
             if self.N_r:
                 par += [sigma0]
@@ -175,17 +173,15 @@
             self.tau_p_d = 1 / np.sqrt(2 * np.sqrt(self.N_d))
 
     def recombine(self, id1, id2):
         p1 = self.pop[id1].copy()  # IMPORTANT: make a copy
         if id1 != id2:
             p2 = self.pop[id2]
             # intermediate recombination for the mutation strengths
-            p1[self._id_hyperpar] = (
-                np.array(p1[self._id_hyperpar]) + np.array(p2[self._id_hyperpar])
-            ) / 2
+            p1[self._id_hyperpar] = (np.array(p1[self._id_hyperpar]) + np.array(p2[self._id_hyperpar])) / 2
 
             # dominant recombination for solution parameters
             (_,) = np.nonzero(randn(self.dim) > 0.5)
             p1[_] = p2[_]
         return p1
 
     def select(self):
@@ -204,17 +200,15 @@
         X = self._to_pheno(pop[:, self._id_var])
         if len(pop.shape) == 1:  # one solution
             X = [X]
 
         pop.fitness = np.array(list(map(self.obj_func, X))).ravel()
         self.eval_count += pop.N
         _penalized_fitness = (
-            self._penalty_func(
-                X, self.iter_count + 1, self.eq_func, self.ineq_func, minimize=self.minimize
-            )
+            self._penalty_func(X, self.iter_count + 1, self.eq_func, self.ineq_func, minimize=self.minimize)
             + pop.fitness
         )
         return _penalized_fitness if return_penalized else pop.fitness
 
     def mutate(self, individual):
         if self.N_r:
             self._mutate_r(individual)
@@ -259,17 +253,15 @@
             eta = eta * exp(self.tau_i * randn() + self.tau_p_i * randn(self.N_i))
         eta[eta > 1] = 1
 
         p = 1 - (eta / self.N_i) / (1 + np.sqrt(1 + (eta / self.N_i) ** 2.0))
         x_ = x + geometric(p) - geometric(p)
 
         # Interval Bounds Treatment
-        x_ = np.asarray(
-            handle_box_constraint(x_, self.bounds_i[:, 0], self.bounds_i[:, 1]), dtype="int"
-        )
+        x_ = np.asarray(handle_box_constraint(x_, self.bounds_i[:, 0], self.bounds_i[:, 1]), dtype="int")
         individual[self.id_i] = x_
         individual[self._id_eta] = eta
 
     def _mutate_d(self, individual):
         P = np.asarray(individual[self._id_p], dtype="float")
         #  Unbiased mutation on the mutation probability
         P = 1.0 / (1.0 + (1.0 - P) / P * exp(-self.tau_d * randn()))
```

### Comparing `bayes-optim-0.2.6/bayes_optim/acquisition_optim/one_plus_one_cma_es.py` & `bayes-optim-0.2.7/bayes_optim/acquisition/optim/one_plus_one_cma_es.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from copy import copy
 from typing import Callable, Dict, List, Union
 
 import numpy as np
 from scipy.linalg import solve_triangular
 
-from ..search_space import RealSpace, SearchSpace
-from ..utils import dynamic_penalty, get_logger, handle_box_constraint, set_bounds
+from ...search_space import RealSpace, SearchSpace
+from ...utils import dynamic_penalty, get_logger, handle_box_constraint, set_bounds
 
 Vector = List[float]
 Matrix = List[Vector]
 
 __authors__ = ["Hao Wang"]
 
 
@@ -21,15 +21,15 @@
         self,
         search_space: SearchSpace,
         obj_fun: Callable,
         args: Dict = None,
         h: Callable = None,
         g: Callable = None,
         x0: Union[str, Vector, np.ndarray] = None,
-        sigma0: Union[float] = None,
+        sigma0: float = None,
         C0: Union[Matrix, np.ndarray] = None,
         ftarget: Union[int, float] = None,
         max_FEs: Union[int, str] = np.inf,
         minimize: bool = True,
         n_restart: int = 0,
         xtol: float = 1e-4,
         ftol: float = 1e-4,
@@ -145,15 +145,15 @@
         # set the initial search point
         self.x = x0
 
     def _init_aux_var(self, opts):
         self.prob_target = opts["p_succ_target"] if "p_succ_target" in opts else 2 / 11
         self.threshold = opts["p_threshold"] if "p_threshold" in opts else 0.44
         self.d = opts["d"] if "d" in opts else 1 + self.dim / 2
-        self.ccov = opts["ccov"] if "ccov" in opts else 2 / (self.dim ** 2 + 6)
+        self.ccov = opts["ccov"] if "ccov" in opts else 2 / (self.dim**2 + 6)
         self.cp = opts["cp"] if "cp" in opts else 1 / 12
         self.cc = opts["cc"] if "cc" in opts else 2 / (self.dim + 2)
 
         self.success_rate: float = self.prob_target
         self.pc: np.ndarray = np.zeros(self.dim)
         self._coeff: float = self.cc * (2 - self.cc)
 
@@ -455,14 +455,14 @@
             ca = 1 - self.ccov
         else:
             self.pc = (1 - self.cc) * self.pc
             ca = (1 - self.ccov) + self.ccov * self.cc * (2 - self.cc)
 
         w = self.pc.dot(self._A_inv.T)
         w_ = w.dot(self._A_inv)
-        L = np.sum(w ** 2)
+        L = np.sum(w**2)
 
         self._A += (np.sqrt(1 + L * cb / ca) - 1) / L * np.outer(self.pc, w)
         self._A *= np.sqrt(ca)
 
         self._A_inv -= (1 - 1 / np.sqrt(1 + L * cb / ca)) / L * np.outer(w, w_)
         self._A_inv *= 1 / np.sqrt(ca)
```

### Comparing `bayes-optim-0.2.6/bayes_optim/base.py` & `bayes-optim-0.2.7/bayes_optim/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import functools
-import logging
 import os
 from abc import abstractmethod
 from copy import copy
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import dill
 import numpy as np
 from sklearn.metrics import mean_absolute_percentage_error, r2_score
 
 from bayes_optim.utils.logger import dump_logger, load_logger
 
-from . import acquisition_fun as AcquisitionFunction
 from ._base import BaseOptimizer
-from .acquisition_optim import argmax_restart
-from .acquisition_optim.option import default_AQ_max_FEs, default_AQ_n_restart, default_AQ_wait_iter
+from .acquisition import acquisition_fun as AcquisitionFunction
+from .acquisition.optim import argmax_restart, default_AQ_max_FEs, default_AQ_n_restart, default_AQ_wait_iter
 from .search_space import RealSpace
 from .solution import Solution
 from .utils import (
     arg_to_int,
     dynamic_penalty,
     fillin_fixed_value,
     func_with_list_arg,
@@ -29,14 +27,15 @@
 
 __authors__ = ["Hao Wang"]
 
 
 class BaseBO(BaseOptimizer):
     """Bayesian Optimization base class, which implements the Ask-Evaluate-Tell interface"""
 
+    # TODO: `model` cannot be None
     def __init__(
         self,
         model: Optional[Any] = None,
         eval_type: str = "list",
         DoE_size: Optional[int] = None,
         warm_data: Tuple = None,
         n_point: int = 1,
```

### Comparing `bayes-optim-0.2.6/bayes_optim/bayes_opt.py` & `bayes-optim-0.2.7/bayes_optim/bayes_opt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 from copy import copy
 from typing import Callable, Dict, List
 
 import numpy as np
 from joblib import Parallel, delayed
 
-from . import acquisition_fun as AcquisitionFunction
+from .acquisition import acquisition_fun as AcquisitionFunction
 from .base import BaseBO
 from .solution import Solution
 
 __authors__ = ["Hao Wang"]
 
 
 class BO(BaseBO):
@@ -74,43 +74,40 @@
             n_point=n_point,
             acquisition_fun=acquisition_fun,
             acquisition_par=acquisition_par,
             **kwargs,
         )
         assert self.n_point > 1
 
+        # TODO: this should be moved to the acquisition functions
         if self._acquisition_fun == "MGFI":
             self._par_name = "t"
             # Log-normal distribution for `t` supported on [0, \infty)
             self._sampler = lambda x: np.exp(np.log(x["t"]) + 0.5 * np.random.randn())
         elif self._acquisition_fun == "UCB":
             self._par_name = "alpha"
             # Logit-normal distribution for `alpha` supported on [0, 1]
-            self._sampler = lambda x: 1 / (
-                1 + np.exp((x["alpha"] * 4 - 2) + 0.6 * np.random.randn())
-            )
+            self._sampler = lambda x: 1 / (1 + np.exp((x["alpha"] * 4 - 2) + 0.6 * np.random.randn()))
         elif self._acquisition_fun == "EpsilonPI":
             self._par_name = "epsilon"
             self._sampler = None  # TODO: implement this!
         else:
             raise NotImplementedError
 
-        _criterion = getattr(AcquisitionFunction, self._acquisition_fun)()
+        _criterion = getattr(AcquisitionFunction, self._acquisition_fun)(model=kwargs["model"])
         if self._par_name not in self._acquisition_par:
             self._acquisition_par[self._par_name] = getattr(_criterion, self._par_name)
 
     def _batch_arg_max_acquisition(self, n_point: int, return_dx: bool, fixed: Dict = None):
         criteria = []
         for _ in range(n_point):
             _par = self._sampler(self._acquisition_par)
             _acquisition_par = copy(self._acquisition_par)
             _acquisition_par.update({self._par_name: _par})
-            criteria.append(
-                self._create_acquisition(par=_acquisition_par, return_dx=return_dx, fixed=fixed)
-            )
+            criteria.append(self._create_acquisition(par=_acquisition_par, return_dx=return_dx, fixed=fixed))
 
         if self.n_job > 1:
             __ = Parallel(n_jobs=self.n_job)(
                 delayed(self._argmax_restart)(c, logger=self.logger) for c in criteria
             )
         else:
             __ = [list(self._argmax_restart(_, logger=self.logger)) for _ in criteria]
@@ -158,17 +155,15 @@
         N = int(n_point / 2)
 
         for _ in range(n_point):
             _t = np.exp(self._acquisition_par["t"] * np.random.randn())
             _t_list.append(_t)
             _acquisition_par = copy(self._acquisition_par)
             _acquisition_par.update({"t": _t})
-            criteria.append(
-                self._create_acquisition(par=_acquisition_par, return_dx=return_dx, fixed=fixed)
-            )
+            criteria.append(self._create_acquisition(par=_acquisition_par, return_dx=return_dx, fixed=fixed))
 
         if self.n_job > 1:
             __ = Parallel(n_jobs=self.n_job)(
                 delayed(self._argmax_restart)(c, logger=self.logger) for c in criteria
             )
         else:
             __ = [list(self._argmax_restart(_, logger=self.logger)) for _ in criteria]
```

### Comparing `bayes-optim-0.2.6/bayes_optim/extension.py` & `bayes-optim-0.2.7/bayes_optim/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 from copy import copy, deepcopy
 from typing import Callable, Dict, List, Union
 
 import numpy as np
 from joblib import Parallel, delayed
 from scipy.stats import rankdata
 from sklearn.decomposition import PCA
-from sklearn.gaussian_process.kernels import ConstantKernel, Matern
 from sklearn.metrics import mean_absolute_percentage_error, r2_score
 
-from . import acquisition_fun as AcquisitionFunction
+from .acquisition import acquisition_fun as AcquisitionFunction
 from .bayes_opt import BO, ParallelBO
 from .search_space import RealSpace, SearchSpace
 from .solution import Solution
-from .surrogate import GaussianProcess, RandomForest
+from .surrogate import GaussianProcess, RandomForest, trend
 from .utils import timeit
 
 
 class LinearTransform(PCA):
     def __init__(self, minimize: bool = True, **kwargs):
         super().__init__(**kwargs)
         self.minimize = minimize
@@ -176,15 +175,28 @@
         self.update_model(X, self.data.fitness)
         self.logger.info(f"xopt/fopt:\n{self.xopt}\n")
 
     def update_model(self, X: np.ndarray, y: np.ndarray):
         # NOTE: the GPR model will be created since the effective search space (the reduced space
         # is dynamic)
         dim = self._search_space.dim
-        self.model = GaussianProcess(domain=self._search_space, n_restarts_optimizer=dim, alpha=1e-8)
+        bounds = np.asarray(self._search_space.bounds)
+        self.model = GaussianProcess(
+            mean=trend.constant_trend(dim),
+            corr="matern",
+            thetaL=1e-3 * (bounds[:, 1] - bounds[:, 0]),
+            thetaU=1e3 * (bounds[:, 1] - bounds[:, 0]),
+            nugget=1e-6,
+            noise_estim=False,
+            optimizer="BFGS",
+            wait_iter=3,
+            random_start=max(10, dim),
+            likelihood="concentrated",
+            eval_budget=100 * dim,
+        )
 
         _std = np.std(y)
         y_ = y if np.isclose(_std, 0) else (y - np.mean(y)) / _std
 
         self.fmin, self.fmax = np.min(y_), np.max(y_)
         self.frange = self.fmax - self.fmin
 
@@ -194,15 +206,15 @@
         r2 = r2_score(y_, y_hat)
         MAPE = mean_absolute_percentage_error(y_, y_hat)
         self.logger.info(f"model r2: {r2}, MAPE: {MAPE}")
 
 
 class ConditionalBO(ParallelBO):
     def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+        super().__init__(model=RandomForest(levels={}), **kwargs)
         self._create_optimizer(**kwargs)
         self._ucb = np.zeros(self.n_subspace)
         self._to_pheno = lambda x: x.to_dict()
         self._to_geno = lambda x, **kwargs: Solution.from_dict(x, **kwargs)
         self._bo_idx: List[int] = list()
 
     def _create_optimizer(self, **kwargs):
@@ -308,15 +320,15 @@
             lambda x: 1 / (1 + np.exp((x["alpha"] * 4 - 2) + 0.6 * np.random.randn())),
         ]
         self._par_name_list = ["t", "alpha"]
         self._acquisition_par_list = [{"t": 1}, {"alpha": 0.1}]
         self._N_acquisition = len(self._acquisition_fun_list)
 
         for i, _n in enumerate(self._par_name_list):
-            _criterion = getattr(AcquisitionFunction, self._acquisition_fun_list[i])()
+            _criterion = getattr(AcquisitionFunction, self._acquisition_fun_list[i])(model=kwargs["model"])
             if _n not in self._acquisition_par_list[i]:
                 self._acquisition_par_list[i][_n] = getattr(_criterion, _n)
 
     def _batch_arg_max_acquisition(self, n_point: int, return_dx: bool, fixed: Dict = None):
         criteria = []
         for i in range(n_point):
             k = i % self._N_acquisition
```

### Comparing `bayes-optim-0.2.6/bayes_optim/mobo.py` & `bayes-optim-0.2.7/bayes_optim/mobo.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 from joblib import Parallel, delayed
 from sklearn.metrics import mean_squared_error, r2_score
 from sklearn.preprocessing import MinMaxScaler
 from torch import Tensor
 
-from .acquisition_optim import argmax_restart
+from .acquisition.optim import argmax_restart
 from .bayes_opt import BO
 from .multi_objective import EHVI
 from .utils import dynamic_penalty, partial_argument, timeit
 from .utils.multi_objective import Hypervolume, is_non_dominated
 from .utils.multi_objective.box_decompositions import NondominatedPartitioning
 
 __authors__ = ["Hao Wang"]
@@ -22,23 +22,23 @@
 
     def __init__(self, n_obj: int = 2, minimize: Union[bool, List[bool]] = True, **kwargv):
         # NOTE: setting `minimize=True` to make parent's constructor work
         super().__init__(minimize=True, **kwargv)
         self._check_obj_fun(n_obj)
         self._check_minimize(minimize)
 
-    def _check_minimize(self, minimize):
+    def _check_minimize(self, minimize: bool):
         self.minimize = minimize
         if isinstance(self.minimize, bool):
             self.minimize = [self.minimize] * self.n_obj
         elif hasattr(self.minimize, "__iter__"):
             assert len(self.minimize) == self.n_obj
         self.minimize = np.asarray(self.minimize)
 
-    def _check_obj_fun(self, n_obj):
+    def _check_obj_fun(self, n_obj: int):
         """check the objective functions"""
         self.n_obj = n_obj
         if self.obj_fun is None:
             return
         assert hasattr(self.obj_fun, "__iter__")
         assert all([hasattr(f, "__call__") for f in self.obj_fun])
         if len(self.obj_fun) != n_obj:
```

### Comparing `bayes-optim-0.2.6/bayes_optim/multi_objective/analytic.py` & `bayes-optim-0.2.7/bayes_optim/multi_objective/analytic.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/search_space/node.py` & `bayes-optim-0.2.7/bayes_optim/search_space/node.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/search_space/samplers.py` & `bayes-optim-0.2.7/bayes_optim/search_space/samplers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 from __future__ import annotations
 
 import warnings
+
+# from abc import ABC
 from typing import Callable
 
 import numpy as np
+
+# from scipy.optimize import root_scalar
 from scipy.stats import norm
 
 from ..utils.exception import ConstraintEvaluationError
 
+# import torch
+# from gpytorch.distributions import MultivariateNormal
+
+
+# from torch import Tensor
+# from torch.nn import Module
+
+
 __author__ = "Hao Wang"
 
+warnings.filterwarnings("error")
+
 
 class SCMC:
     r"""Sequential Constrained Monte Carlo sampling
 
     References
 
     .. [GolchiL15]
@@ -136,15 +150,15 @@
             levels = np.array(self.sample_space.bounds[i])
             idx = np.random.rand(N) < prob
             X[idx, i] = levels[np.random.randint(0, len(levels), sum(idx))]
 
     def _ess(self, nu: float, nu_ref: float, X: np.ndarray) -> float:
         """effective sample size"""
         w = self.get_weights(nu, nu_ref, X)
-        v = 0 if np.any(np.isnan(w)) else 1 / np.sum(w ** 2)
+        v = 0 if np.any(np.isnan(w)) else 1 / np.sum(w**2)
         return v - len(X) / 2
 
     def get_weights(self, nu, nu_ref, X):
         w = np.exp([self._log_posterior(x, nu) - self._log_posterior(x, nu_ref) for x in X])
         return w / np.sum(w)
 
     def _metropolis_hastings(self, X: np.ndarray, nu: float, t: int) -> np.ndarray:
@@ -165,21 +179,27 @@
         np.ndarray
             (dependent) sample points from `self._log_posterior`
         """
         N = len(X)  # sample size
         lp = np.array([self._log_posterior(x, nu) for x in X])  # log-probability
         for _ in range(self.mh_steps):
             X_ = self._rproposal(X, t)
-            lp_ = np.array([self._log_posterior(x_, nu) for x_ in X_])
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore")
-                prob = np.clip(np.exp(lp_ - lp), 0, 1)
-            mask = np.random.rand(N) <= prob
-            X[mask, :] = X_[mask, :]
-            lp[mask] = lp_[mask]
+            for i in range(self.dim):
+                X_dim = X.copy()
+                X_dim[:, i] = X_[:, i]
+                lp_ = np.array([self._log_posterior(x_, nu) for x_ in X_dim])
+                with warnings.catch_warnings():
+                    warnings.filterwarnings("error")
+                    try:
+                        prob = np.clip(np.exp(lp_ - lp), 0, 1)
+                    except:
+                        prob = 1
+                mask = np.random.rand(N) <= prob
+                X[mask, i] = X_[mask, i]
+                lp[mask] = lp_[mask]
         return X
 
     def sample(self, N: int) -> np.ndarray:
         """Draw a sample under constraints
 
         Parameters
         ----------
```

### Comparing `bayes-optim-0.2.6/bayes_optim/search_space/search_space.py` & `bayes-optim-0.2.7/bayes_optim/search_space/search_space.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/search_space/variable.py` & `bayes-optim-0.2.7/bayes_optim/search_space/variable.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/solution.py` & `bayes-optim-0.2.7/bayes_optim/solution.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/__init__.py` & `bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 from scipy.linalg import solve_triangular
 from scipy.spatial.distance import cdist
 from sklearn.gaussian_process import GaussianProcessRegressor as sk_gpr
 from sklearn.gaussian_process.kernels import RBF, Matern, WhiteKernel
 
 from ...search_space import RealSpace, SearchSpace
 from ...utils import safe_divide
+from . import trend
+from .gpr import GaussianProcess
 from .utils import MSLL, SMSE
 
 # from sklearn.model_selection import cross_val_score
 
 
 warnings.filterwarnings("ignore")
 
 __author__ = "Hao Wang"
-__all__ = ["SMSE", "MSLL", "GaussianProcess"]
+__all__ = ["SMSE", "MSLL", "GaussianProcess", "trend"]
 
 
-class GaussianProcess:
+class GaussianProcessSklearn:
     """Wrapper for sklearn's GPR model"""
 
     def __init__(
         self,
         domain: SearchSpace,
         codomain: SearchSpace = None,
         n_obj: int = 1,
@@ -132,15 +134,15 @@
             # for k in self._kernel:
             #     scores = cross_val_score(self._gpr_cls(kernel=k), X, y[:, i], cv=cv, scoring="r2", n_jobs=cv)
             #     score_ = np.nanmean(scores)
             #     if score_ > score:
             #         score = score_
             #         kernel = k
 
-            gpr = self._gpr_cls(kernel=self._kernel[0]).fit(X, y[:, i])
+            gpr = self._gpr_cls(kernel=self._kernel[0]).fit(X, y if y.ndim == 1 else y[:, i])
             setattr(gpr, "_K_inv", None)
             self._gprs.append(gpr)
 
         self.is_fitted = True
         return self
 
     def predict(self, X: np.ndarray, eval_MSE: bool = False) -> np.ndarray:
@@ -181,15 +183,15 @@
             k_dx = self.kernel_dx(gp, X)  # shape (n_samples, dim, N_train)
 
             if getattr(gp, "_K_inv") is None:
                 L_inv = solve_triangular(gp.L_.T, np.eye(gp.L_.shape[0]))
                 setattr(gp, "_K_inv", L_inv.dot(L_inv.T))
 
             mean_dx[i, ...] = scale * k_dx @ gp.alpha_
-            var_dx[i, ...] = -2.0 * scale ** 2 * np.squeeze(k_dx @ getattr(gp, "_K_inv") @ k)
+            var_dx[i, ...] = -2.0 * scale**2 * np.squeeze(k_dx @ getattr(gp, "_K_inv") @ k)
         return mean_dx, var_dx
 
     def kernel_dx(self, gp: sk_gpr, X: np.ndarray) -> np.ndarray:
         """compute the gradient of the kernel function w.r.t. the input points
 
         Parameters
         ----------
@@ -209,20 +211,20 @@
 
         d = np.expand_dims(
             cdist(X / length_scale, gp.X_train_ / length_scale), 1
         )  # shape (n_samples, 1, n_train)
         X_ = np.expand_dims(X, 2)  # shape (n_samples, dim, 1)
         X_train_ = np.expand_dims(gp.X_train_.T, 0)  # shape (1, dim, n_train)
         # shape (n_samples, dim, n_train)
-        dd = safe_divide(X_ - X_train_, d * np.expand_dims(length_scale ** 2, 1))
+        dd = safe_divide(X_ - X_train_, d * np.expand_dims(length_scale**2, 1))
 
         if isinstance(kernel, Matern):
             nu = kernel.nu
             if nu == 0.5:
                 g = -sigma2 * np.exp(-d) * dd
             elif nu == 1.5:
                 g = -3 * sigma2 * np.exp(-np.sqrt(3) * d) * d * dd
             elif nu == 2.5:
                 g = -5.0 / 3 * sigma2 * np.exp(-np.sqrt(5) * d) * (1 + np.sqrt(5) * d) * d * dd
         elif isinstance(kernel, RBF):
-            g = -sigma2 * np.exp(-0.5 * d ** 2) * dd
+            g = -sigma2 * np.exp(-0.5 * d**2) * dd
         return g
```

### Comparing `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/boundary_handling.py` & `bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/boundary_handling.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/cma_es.py` & `bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/cma_es.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/gpr.py` & `bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/gpr.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,26 @@
 import numpy as np
 from numpy import array, dot, exp, log, log10, pi, sqrt
 from numpy.random import uniform
 from scipy import linalg
 from scipy.linalg import LinAlgError, cho_solve, cholesky, solve_triangular
 from scipy.optimize import fmin_l_bfgs_b
 from sklearn.base import BaseEstimator, RegressorMixin
-from sklearn.metrics.pairwise import manhattan_distances
 from sklearn.utils import check_array, check_random_state, check_X_y
 
 from .cma_es import cma_es
-from .kernel import (
-    absolute_exponential,
-    cubic,
-    generalized_exponential,
-    matern,
-    squared_exponential,
-)
+from .kernel import absolute_exponential, cubic, generalized_exponential, matern, squared_exponential
 from .trend import BasisExpansionTrend, NonparametricTrend, constant_trend
 
 MACHINE_EPSILON = np.finfo(np.double).eps
 
+warnings.filterwarnings("error")
 
-def l1_cross_distances(X):
+
+def l1_cross_distances(X, Y=None):
     """
     Computes the nonzero componentwise L1 cross-distances between the vectors
     in X.
 
     Parameters
     ----------
 
@@ -40,28 +35,34 @@
     D: array with shape (n_samples * (n_samples - 1) / 2, n_features)
         The array of componentwise L1 cross-distances.
 
     ij: arrays with shape (n_samples * (n_samples - 1) / 2, 2)
         The indices i and j of the vectors in X associated to the cross-
         distances in D: D[k] = np.abs(X[ij[k, 0]] - Y[ij[k, 1]]).
     """
-    X = check_array(X)
-    n_samples, n_features = X.shape
-    n_nonzero_cross_dist = n_samples * (n_samples - 1) // 2
-    ij = np.zeros((n_nonzero_cross_dist, 2), dtype=np.int)
-    D = np.zeros((n_nonzero_cross_dist, n_features))
-    ll_1 = 0
-    for k in range(n_samples - 1):
-        ll_0 = ll_1
-        ll_1 = ll_0 + n_samples - k - 1
-        ij[ll_0:ll_1, 0] = k
-        ij[ll_0:ll_1, 1] = np.arange(k + 1, n_samples)
-        D[ll_0:ll_1] = np.abs(X[k] - X[(k + 1) : n_samples])
-
-    return D, ij
+    if Y is not None:
+        X = check_array(X)
+        Y = check_array(Y)
+        D = X[:, np.newaxis, :] - Y[np.newaxis, :, :]
+        D = np.abs(D, D)
+        return D.reshape((-1, X.shape[1]))
+    else:
+        X = check_array(X)
+        n_samples, n_features = X.shape
+        n_nonzero_cross_dist = n_samples * (n_samples - 1) // 2
+        ij = np.zeros((n_nonzero_cross_dist, 2), dtype=np.int_)
+        D = np.zeros((n_nonzero_cross_dist, n_features))
+        ll_1 = 0
+        for k in range(n_samples - 1):
+            ll_0 = ll_1
+            ll_1 = ll_0 + n_samples - k - 1
+            ij[ll_0:ll_1, 0] = k
+            ij[ll_0:ll_1, 1] = np.arange(k + 1, n_samples)
+            D[ll_0:ll_1] = np.abs(X[k] - X[(k + 1) : n_samples])
+        return D, ij
 
 
 def my_dot(x, y):
     n_row = x.shape[0]
     n_col = y.shape[1]
     res = np.zeros((n_row, n_col))
     for i in range(n_row):
@@ -262,15 +263,15 @@
             self.estimation_mode = "noisy"
 
         assert likelihood in self._likelihood_functions
         self.likelihood = likelihood  # or restricted
         self.is_fitted = False
 
         if self.mean is None:
-            self.mean = constant_trend(len(self.thetaU), beta=0)
+            self.mean = constant_trend(len(self.thetaU), beta=0)  # simple Kriging
 
         # estimation mode for the trend
         if isinstance(self.mean, BasisExpansionTrend):
             self.mean_type = "basis_expansion"
             self.estimate_trend = True if self.mean.beta is None else False
         elif isinstance(self.mean, NonparametricTrend):
             self.mean_type = "nonparametric"
@@ -336,22 +337,22 @@
             )
 
         # remember to normalize the inputs
         # if normalize:
         # X1 = (X1 - self.X_mean) / self.X_std
         # X2 = (X2 - self.X_mean) / self.X_std
 
-        dx_new = manhattan_distances(X1, Y=X2, sum_over_features=False)
+        dx_new = l1_cross_distances(X1, Y=X2)
         R_prior = self.corr(self.theta_, dx_new).reshape(n_eval_X1, n_eval_X2)
 
         if corr:
             return R_prior
         else:
             C_prior = array([self.sigma2[i] * R_prior for i in range(n_targets)])
-            C_prior = sqrt((C_prior ** 2.0).sum(axis=0) / n_targets)
+            C_prior = sqrt((C_prior**2.0).sum(axis=0) / n_targets)
 
             return C_prior
 
     def fit(self, X, y):
         """The Gaussian Process model fitting method.
 
         Parameters
@@ -478,15 +479,15 @@
             # Initialize output
             y = np.zeros(n_eval)
             if eval_MSE:
                 MSE = np.zeros(n_eval)
 
             # Get pairwise componentwise L1-distances to the input training set
             # TODO: remove calculations of distances from here
-            dx = manhattan_distances(X, Y=self.X, sum_over_features=False)
+            dx = l1_cross_distances(X, Y=self.X)
             # Get meanession function and correlation
             r = self.corr(self.theta_, dx).reshape(n_eval, n_samples)
             # Predictor
             y = (self.mean(X) + r.dot(self.gamma)).reshape(n_eval, n_targets)
 
             # Mean Squared Error
             if eval_MSE:
@@ -495,15 +496,15 @@
                 if self.estimate_trend:  # Universal / Ordinary Kriging
                     f = self.mean.F(X)
                     u = solve_triangular(self.G.T, np.dot(self.Ft.T, rt) - f.T, lower=True)
                 else:  # simple Kriging
                     u = np.zeros((1, n_eval))
 
                 MSE = np.dot(
-                    (1.0 - (rt ** 2.0).sum(axis=0) + (u ** 2.0).sum(axis=0)).reshape(n_eval, -1),
+                    (1.0 - (rt**2.0).sum(axis=0) + (u**2.0).sum(axis=0)).reshape(n_eval, -1),
                     self.sigma2.reshape(1, -1),
                 )
                 # MSE = np.sqrt((MSE ** 2.0).sum(axis=0) / n_targets)
 
                 # Mean Squared Error might be slightly negative depending on
                 # machine precision: force to zero!
                 MSE[MSE < 0.0] = 0.0
@@ -548,15 +549,15 @@
             raise Exception("x must be a vector!")
 
         # trend and its Jacobian
         f = self.mean.F(x).reshape(-1, 1)
         f_dx = self.mean.Jacobian(x)
 
         # correlation and its Jacobian
-        d = manhattan_distances(x, Y=self.X, sum_over_features=False)
+        d = l1_cross_distances(x, Y=self.X)
         r = self.corr(self.theta_, d).reshape(n_eval, n_samples)
         r_dx = self.corr_dx(x, X=self.X, r=r).T
 
         # gradient of the posterior mean
         y_dx = dot(self.mean.beta.T, f_dx) + self.gamma.T.dot(r_dx)
 
         # auxiliary variable: rt = C^-1 * r
@@ -586,15 +587,15 @@
         if n_eval != 1:
             raise Exception("x must be a vector!")
 
         # The Hessian tensor of the trend
         f_dx2 = self.mean.Hessian(x)
 
         # The Hessian tensor of the correlation
-        d = manhattan_distances(x, Y=self.X, sum_over_features=False)
+        d = l1_cross_distances(x, Y=self.X)
         r = self.corr(self.theta_, d).reshape(n_eval, n_samples)
         r_dx2 = self.corr_Hessian(x, X=self.X, r=r)
 
         return (f_dx2.dot(self.mean.beta) + r_dx2.dot(self.gamma))[..., 0]
 
     def corr_dx(self, x, X=None, theta=None, r=None, nu=1.5):
         # TODO: move corr_dx, corr_grad_theta the kernel module
@@ -632,15 +633,15 @@
             warnings.filterwarnings("error")
             try:
                 if self.corr_type == "squared_exponential":
                     grad = -2 * r * (theta * diff)
 
                 elif self.corr_type == "matern":
                     c = np.sqrt(3)
-                    D = np.sqrt(np.sum(theta * diff ** 2.0, axis=0))
+                    D = np.sqrt(np.sum(theta * diff**2.0, axis=0))
 
                     if nu == 0.5:
                         grad = -diff * theta / D * r
                     elif nu == 1.5:
                         grad = diff * theta / D
                         grad *= -3.0 * D * exp(-c * D)
                     elif nu == 2.5:
@@ -700,15 +701,15 @@
                     for k in range(n_features):
                         _ = np.zeros((n_features, n_samples))
                         _[k, :] = theta[k]
                         H.append(-2 * (g[k, :] * (theta * diff) + r * _))
                     H = np.atleast_3d(H)
                 elif self.corr_type == "matern":
                     c = np.sqrt(3)
-                    D = np.sqrt(np.sum(theta * diff ** 2.0, axis=0))
+                    D = np.sqrt(np.sum(theta * diff**2.0, axis=0))
 
                     if nu == 0.5:
                         grad = -diff * theta / D * r
                     elif nu == 1.5:
                         grad = diff * theta / D
                         grad *= -3.0 * D * exp(-c * D)
                     elif nu == 2.5:
@@ -883,27 +884,23 @@
             # Covariance: partial derivatives w.r.t. theta
             C_grad_tensor = total_var * self.corr_grad_theta(theta, self.X, R0)
             # Covariance: partial derivatives w.r.t. sigma2
             C_grad_tensor = np.concatenate([C_grad_tensor, R0[..., np.newaxis]], axis=2)
 
             if self.estimation_mode == "noise_estim":
                 # Covariance: partial derivatives w.r.t. noise_var
-                C_grad_tensor = np.concatenate(
-                    [C_grad_tensor, np.eye(n_samples)[..., np.newaxis]], axis=2
-                )
+                C_grad_tensor = np.concatenate([C_grad_tensor, np.eye(n_samples)[..., np.newaxis]], axis=2)
             # partial dderivatives of llf
             gradient = np.zeros((n_par, 1))
             for i in range(n_par):
                 C_grad = C_grad_tensor[:, :, i]
                 # TODO: beta hat is not considered in the partial derivatives
                 if self.estimate_trend:
                     gradient[i] = -0.5 * (
-                        np.sum(Cinv * C_grad)
-                        - gamma_.T.dot(C_grad).dot(gamma_)
-                        - np.sum(term * C_grad)
+                        np.sum(Cinv * C_grad) - gamma_.T.dot(C_grad).dot(gamma_) - np.sum(term * C_grad)
                     )
                 else:  # simple kriging
                     gradient[i] = -0.5 * (np.sum(Cinv * C_grad) - gamma_.T.dot(C_grad).dot(gamma_))
 
         if env is not None:
             env["sigma2"] = sigma2
             env["noise_var"] = noise_var
@@ -932,37 +929,37 @@
         n_samples = self.X.shape[0]
         n_par = len(par)
         n_targets = self.y.shape[1]
         if self.estimation_mode == "noiseless":
             theta = par
             noise_var = 0
             R0 = self.correlation_matrix(theta)
-            try:
-                L, Ft, Yt, Q, G, rho = self._compute_aux_var(R0)
-                # TODO: check experimental correction of the sigma2 estimation
-                k = np.linalg.matrix_rank(Q.dot(Q.T)) if Q is not None else 0
-                sigma2 = (rho ** 2.0).sum(axis=0) / (n_samples - k)
-                log_likelihood = -0.5 * (
-                    n_samples * log(2.0 * pi * sigma2) + 2.0 * np.log(np.diag(L)).sum() + n_samples
-                )
-            except (LinAlgError, ValueError):
-                log_likelihood = None
+            with warnings.catch_warnings():
+                warnings.filterwarnings("error")
+                try:
+                    L, Ft, Yt, Q, G, rho = self._compute_aux_var(R0)
+                    # TODO: check experimental correction of the sigma2 estimation
+                    k = np.linalg.matrix_rank(Q.dot(Q.T)) if Q is not None else 0
+                    sigma2 = (rho**2.0).sum(axis=0) / (n_samples - k)
+                    log_likelihood = -0.5 * (
+                        n_samples * log(2.0 * pi * sigma2) + 2.0 * np.log(np.diag(L)).sum() + n_samples
+                    )
+                except (LinAlgError, ValueError, Warning):
+                    log_likelihood = None
 
         elif self.estimation_mode == "noise_estim":
             theta, alpha = par[:-1], par[-1]
             R0 = self.correlation_matrix(theta)
             R = alpha * R0 + (1 - alpha) * np.eye(n_samples)
             try:
                 L, Ft, Yt, Q, G, rho = self._compute_aux_var(R)
-                sigma2_total = (rho ** 2.0).sum(axis=0) / n_samples
+                sigma2_total = (rho**2.0).sum(axis=0) / n_samples
                 sigma2, noise_var = alpha * sigma2_total, (1 - alpha) * sigma2_total
                 log_likelihood = -0.5 * (
-                    n_samples * log(2.0 * pi * sigma2_total)
-                    + 2.0 * np.log(np.diag(L)).sum()
-                    + n_samples
+                    n_samples * log(2.0 * pi * sigma2_total) + 2.0 * np.log(np.diag(L)).sum() + n_samples
                 )
             except (LinAlgError, ValueError):
                 log_likelihood = None
 
         elif self.estimation_mode == "noisy":
             theta, sigma2 = par[:-1], par[-1]
             noise_var = self.noise_var
@@ -1103,17 +1100,15 @@
                 if self.theta0 is not None
                 else np.random.uniform(log10(self.thetaL), log10(self.thetaU))
             )
 
         if self.estimation_mode == "noiseless" and self.likelihood == "concentrated":
             log10param = log10theta0
         else:
-            log10param = np.r_[
-                log10theta0, uniform(log10bounds[n_theta:, 0], log10bounds[n_theta:, 1])
-            ]
+            log10param = np.r_[log10theta0, uniform(log10bounds[n_theta:, 0], log10bounds[n_theta:, 1])]
 
         n_par = len(log10param)
         eval_budget = 200 * n_par if self.eval_budget is None else self.eval_budget
         llf_opt = np.inf
 
         def _obj_func(eval_grad=False):
             def func(log10param):
@@ -1155,16 +1150,15 @@
                     wait_count += 1
 
                 if self.verbose:
                     print("restart {} takes {} evals".format(iteration + 1, info["funcalls"]))
                     print("best log likekihood value: {}".format(-llf_opt))
                     if info["warnflag"] != 0:
                         warnings.warn(
-                            "fmin_l_bfgs_b terminated abnormally with "
-                            "the state: {}".format(info)
+                            "fmin_l_bfgs_b terminated abnormally with " "the state: {}".format(info)
                         )
 
                 eval_budget -= info["funcalls"]
                 if eval_budget <= 0 or wait_count >= self.wait_iter:
                     break
 
         elif self.optimizer == "CMA":  # IPOP-CMA-ES
@@ -1182,15 +1176,15 @@
             optimizer = cma_es(n_par, log10param, obj_func, opt, is_minimize=False, restart="IPOP")
             param_opt, llf_opt, evalcount, info = optimizer.optimize()
             param_opt = param_opt.flatten()
 
             if self.verbose:
                 print("{} evals, best log likekihood value: {}".format(evalcount, -llf_opt))
 
-        optimal_param = 10.0 ** param_opt
+        optimal_param = 10.0**param_opt
         env = {}
         if self.likelihood == "concentrated":
             optimal_llf_value = self.log_likelihood_concentrated(optimal_param, env)
         elif self.likelihood == "restricted":
             optimal_llf_value = self.log_likelihood_restricted(optimal_param, env)
 
         param = {}
@@ -1223,17 +1217,15 @@
             if self.theta0 is not None and self.theta0.size != self.thetaL.size:
                 raise ValueError("theta0, thetaL, and thetaU must have the same length.")
             if np.any(self.thetaL <= 0) or np.any(self.thetaU < self.thetaL):
                 raise ValueError("The bounds must satisfy O < thetaL <= " "thetaU.")
 
         elif self.thetaL is None and self.thetaU is None:
             if self.theta0 is None:
-                raise ValueError(
-                    "theta0 must be provided when both thetaL and thetaU are not set."
-                )
+                raise ValueError("theta0 must be provided when both thetaL and thetaU are not set.")
             if np.any(self.theta0 <= 0):
                 raise ValueError("theta0 must be strictly positive.")
 
         elif self.thetaL is None or self.thetaU is None:
             raise ValueError("thetaL and thetaU should either be both or " "neither specified.")
 
         # Force verbose type to bool
```

### Comparing `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/kernel.py` & `bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/kernel.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/surrogate/gaussian_process/utils.py` & `bayes-optim-0.2.7/bayes_optim/surrogate/gaussian_process/utils.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/surrogate/random_forest.py` & `bayes-optim-0.2.7/bayes_optim/surrogate/random_forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         # for categorical levels/variable number
         # in the future, maybe implement binary/multi-value split
         if self.levels:
             self._levels = OrderedDict(sorted(levels.items()))
             self._cat_idx = list(self._levels.keys())
             self._categories = list(self._levels.values())
             # encode categorical variables to binary values
-            self._enc = OneHotEncoder(categories=self._categories, sparse=False)
+            self._enc = OneHotEncoder(categories=self._categories, sparse_output=False)
 
     def _check_X(self, X: Union[Solution, List, np.ndarray]) -> Solution:
         X_ = array(X, dtype=object)
         if hasattr(self, "_levels"):
             X_cat = self._enc.fit_transform(X_[:, self._cat_idx])
             X = np.c_[np.delete(X_, self._cat_idx, 1).astype(float), X_cat]
         return X
```

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/__init__.py` & `bayes-optim-0.2.7/bayes_optim/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/_daemon.py` & `bayes-optim-0.2.7/bayes_optim/utils/_daemon.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/exception.py` & `bayes-optim-0.2.7/bayes_optim/utils/exception.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/logger.py` & `bayes-optim-0.2.7/bayes_optim/utils/logger.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/box_decomposition.py` & `bayes-optim-0.2.7/bayes_optim/utils/multi_objective/box_decompositions/box_decomposition.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/non_dominated.py` & `bayes-optim-0.2.7/bayes_optim/utils/multi_objective/box_decompositions/non_dominated.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/box_decompositions/utils.py` & `bayes-optim-0.2.7/bayes_optim/utils/multi_objective/box_decompositions/utils.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/hypervolume.py` & `bayes-optim-0.2.7/bayes_optim/utils/multi_objective/hypervolume.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/multi_objective/pareto.py` & `bayes-optim-0.2.7/bayes_optim/utils/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim/utils/utils.py` & `bayes-optim-0.2.7/bayes_optim/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bayes-optim-0.2.6/bayes_optim.egg-info/PKG-INFO` & `bayes-optim-0.2.7/bayes_optim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayes-optim
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Bayesian Optimization Library
 Home-page: https://github.com/wangronin/Bayesian-Optimization
 Author: Hao Wang
 Author-email: wangronin@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/wangronin/Bayesian-Optimization/archive/v0.1.3.tar.gz
 Description: [![Actions Status](https://github.com/wangronin/Bayesian-Optimization/workflows/Build%20and%20Test/badge.svg)](https://github.com/wangronin/Bayesian-Optimization/actions)
```

### Comparing `bayes-optim-0.2.6/bayes_optim.egg-info/SOURCES.txt` & `bayes-optim-0.2.7/bayes_optim.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 bayes_optim/__init__.py
 bayes_optim/_base.py
-bayes_optim/acquisition_fun.py
 bayes_optim/base.py
 bayes_optim/bayes_opt.py
 bayes_optim/extension.py
 bayes_optim/mobo.py
 bayes_optim/solution.py
 bayes_optim.egg-info/PKG-INFO
 bayes_optim.egg-info/SOURCES.txt
 bayes_optim.egg-info/dependency_links.txt
 bayes_optim.egg-info/requires.txt
 bayes_optim.egg-info/top_level.txt
-bayes_optim/acquisition_optim/__init__.py
-bayes_optim/acquisition_optim/mies.py
-bayes_optim/acquisition_optim/one_plus_one_cma_es.py
-bayes_optim/acquisition_optim/option.py
+bayes_optim/acquisition/__init__.py
+bayes_optim/acquisition/acquisition_fun.py
+bayes_optim/acquisition/optim/__init__.py
+bayes_optim/acquisition/optim/mies.py
+bayes_optim/acquisition/optim/one_plus_one_cma_es.py
+bayes_optim/acquisition/optim/option.py
 bayes_optim/multi_objective/__init__.py
 bayes_optim/multi_objective/analytic.py
 bayes_optim/search_space/__init__.py
 bayes_optim/search_space/node.py
 bayes_optim/search_space/samplers.py
 bayes_optim/search_space/search_space.py
 bayes_optim/search_space/variable.py
```

### Comparing `bayes-optim-0.2.6/setup.py` & `bayes-optim-0.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bayes-optim",
-    version="0.2.6",
+    version="0.2.7",
     author="Hao Wang",
     author_email="wangronin@gmail.com",
     packages=find_packages(),
     description="A Bayesian Optimization Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wangronin/Bayesian-Optimization",
@@ -31,9 +31,10 @@
         "tabulate>=0.8.7",
         "threadpoolctl>=2.1.0",
         "requests>=2.25.0",
         "requests-oauthlib>=1.3.0",
         "sobol-seq>=0.2.0",
         "py-expression-eval>=0.3.13",
         "torch>=1.9.0",
+        "pytest>=6.2.5",
     ],
 )
```

